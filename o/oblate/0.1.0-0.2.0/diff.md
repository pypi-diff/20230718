# Comparing `tmp/oblate-0.1.0-py3-none-any.whl.zip` & `tmp/oblate-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15317 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      468 b- defN 23-Jul-15 07:04 oblate/__init__.py
+Zip file size: 17792 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      468 b- defN 23-Jul-18 09:34 oblate/__init__.py
 -rw-rw-rw-  2.0 fat     2377 b- defN 23-Jul-15 07:07 oblate/config.py
--rw-rw-rw-  2.0 fat     5309 b- defN 23-Jul-15 07:07 oblate/exceptions.py
--rw-rw-rw-  2.0 fat    17590 b- defN 23-Jul-15 08:54 oblate/fields.py
--rw-rw-rw-  2.0 fat     5787 b- defN 23-Jul-15 08:51 oblate/schema.py
+-rw-rw-rw-  2.0 fat     6049 b- defN 23-Jul-16 13:39 oblate/exceptions.py
+-rw-rw-rw-  2.0 fat    24162 b- defN 23-Jul-18 09:23 oblate/fields.py
+-rw-rw-rw-  2.0 fat    11169 b- defN 23-Jul-18 08:17 oblate/schema.py
 -rw-rw-rw-  2.0 fat     1515 b- defN 23-Jul-14 06:23 oblate/utils.py
--rw-rw-rw-  2.0 fat     1089 b- defN 23-Jul-15 08:59 oblate-0.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     5366 b- defN 23-Jul-15 08:59 oblate-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-15 08:59 oblate-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-15 08:59 oblate-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      823 b- defN 23-Jul-15 08:59 oblate-0.1.0.dist-info/RECORD
-11 files, 40423 bytes uncompressed, 13949 bytes compressed:  65.5%
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-Jul-18 09:35 oblate-0.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     5366 b- defN 23-Jul-18 09:35 oblate-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-18 09:35 oblate-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-18 09:35 oblate-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      824 b- defN 23-Jul-18 09:35 oblate-0.2.0.dist-info/RECORD
+11 files, 53118 bytes uncompressed, 16424 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: oblate/schema.py
 Comment: 
 
 Filename: oblate/utils.py
 Comment: 
 
-Filename: oblate-0.1.0.dist-info/LICENSE
+Filename: oblate-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: oblate-0.1.0.dist-info/METADATA
+Filename: oblate-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: oblate-0.1.0.dist-info/WHEEL
+Filename: oblate-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: oblate-0.1.0.dist-info/top_level.txt
+Filename: oblate-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: oblate-0.1.0.dist-info/RECORD
+Filename: oblate-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oblate/__init__.py

```diff
@@ -5,15 +5,15 @@
 Oblate is a Python library that provides modern and robust interface
 for data and schema validation.
 
 Licensed under MIT license. Copyright (c) 2023 Izhar Ahmad.
 For more information, see the project's LICENSE.
 """
 
-__version__ = '0.1.0'
+__version__ = '0.2.0'
 __author__  = 'Izhar Ahmad (izxxr) <https://github.com/izxxr>'
 
 from oblate.schema import *
 from oblate.exceptions import *
 from oblate import (
     fields as fields,
     config as config,
```

## oblate/exceptions.py

```diff
@@ -42,20 +42,32 @@
 class ValidationError(OblateException):
     """An error raised when validation fails for a specific field.
 
     Parameters
     ----------
     message:
         The error message.
+    state:
+        Any state data that should be attached to the exception. This
+        is particularly useful when you want to propagate any kind of
+        state data through this exception.
+
+        This can later be accessed, typically from :attr:`SchemaValidationFailed.errors`
+        attribute.
     """
-    def __init__(self, message: Any) -> None:
+    def __init__(self, message: Any, *, state: Any = None) -> None:
         self._field: Optional[Field] = None
         self._message = message
+        self.state = state
         super().__init__(message)
 
+    def is_field_error(self) -> bool:
+        """Indicates whether this is error is related to a field."""
+        return self._field is not None
+
     @property
     def field(self) -> Optional[Field]:
         """The :class:`Field` associated to this error. If None, this error
         is not related to a specific field."""
         return self._field
 
     def _bind(self, field: Field) -> None:
@@ -111,23 +123,30 @@
         return '\n'.join(builder)
 
     def _raw_internal(self) -> Dict[str, Any]:
         out = {
             'errors': [],
             'field_errors': {}
         }
+        from_data = self._schema.is_data_initialized()
 
         for error in self._errors:
-            if error._field is None:
+            field = error._field
+            if field is None:
                 out['errors'].append(error._message)
             else:
+                if from_data:
+                    name = field.load_key if field.load_key else field._name
+                else:
+                    name = field._name
+
                 try:
-                    field_errors = out['field_errors'][error._field._name]
+                    field_errors = out['field_errors'][name]
                 except KeyError:
-                    out['field_errors'][error._field._name] = [error._message]
+                    out['field_errors'][name] = [error._message]
                 else:
                     field_errors.append(error._message)
 
         return out
 
     def raw(self) -> Dict[str, Any]:
         """Converts the error to raw format.
```

## oblate/fields.py

```diff
@@ -20,38 +20,42 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import annotations
 
 from typing import (
     Any,
+    List,
+    Set,
     Type,
     TypeVar,
     Generic,
     Optional,
     Union,
     Literal,
     Sequence,
     Callable,
-    List,
     Mapping,
     overload,
     TYPE_CHECKING,
 )
 from typing_extensions import Self
 from oblate import config
 from oblate.utils import MISSING
 from oblate.exceptions import ValidationError, SchemaValidationFailed
 
 import copy
+import collections.abc
 
 if TYPE_CHECKING:
     from oblate.schema import Schema
 
-    ValidatorCallbackT = Callable[['_SchemaT', Any], bool]
+    SerializedValidatorCallbackT = Callable[['_SchemaT', '_SerializedT'], bool]
+    RawValidatorCallbackT = Callable[['_SchemaT', '_RawT'], bool]
+    ValidatorCallbackT = Union[SerializedValidatorCallbackT, RawValidatorCallbackT]
 
 __all__ = (
     'Field',
     'String',
     'Integer',
     'Boolean',
     'Float',
@@ -85,86 +89,150 @@
         optional. Regardless of provided value, if a ``default`` is provided,
         the value for this will automatically be set to True.
     none: :class:`bool`
         Whether this field can have a value of None.
     default:
         The value to assign to this field when it's missing. If this is not provided
         and a field is marked as missing, accessing the field at runtime would result
-        in an AttributeError. 
+        in an AttributeError.
+    load_key: Optional[:class:`str`]
+        The key that refers to this field in the data when loading this field
+        using raw data.
+
+        .. note::
+
+            This parameter is only applicable when loading data with raw data
+            i.e using the ``data`` parameter in the :class:`Schema` object and
+            does not relate to argument name while initializing schema with keyword
+            arguments.
+
+    dump_key: Optional[:class:`str`]
+        The key to which the deserialized value of this field should be set in the
+        data returned by :meth:`Schema.dump`.
     """
     __valid_overrides__ = (
         'missing',
         'none',
         'default',
+        'load_key',
+        'dump_key',
+    )
+
+    __slots__ = (
+        'missing',
+        'none',
+        'default',
+        'load_key',
+        'dump_key',
+        '_validators',
+        '_raw_validators',
+        '_schema',
+        '_name',
     )
 
     def __init__(
             self,
             *,
             missing: bool = False,
             none: bool = False,
             default: Any = MISSING,
+            load_key: Optional[str] = None,
+            dump_key: Optional[str] = None,
         ) -> None:
 
         self.missing = missing or (default is not MISSING)
         self.none = none
         self.default = default
-        self._validators = []
+        self.load_key = load_key
+        self.dump_key = dump_key
+        self._validators: List[SerializedValidatorCallbackT[Any, _SerializedT]] = []
+        self._raw_validators: List[RawValidatorCallbackT[Any, _RawT]] = []
         self._clear_state()
 
     @overload
     def __get__(self, instance: Literal[None], owner: Type[Schema]) -> Self:
         ...
 
     @overload
     def __get__(self, instance: Schema, owner: Type[Schema]) -> _SerializedT:
         ...
 
     def __get__(self, instance: Optional[Schema], owner: Type[Schema]) -> Union[_SerializedT, Self]:
         if instance is None:
             return self
-        if self._value is MISSING:
-            raise AttributeError(f'No value available for field {owner.__qualname__}.{self._name}')
-        return self._value
+        try:
+            return instance._field_values[self._name]
+        except KeyError:
+            raise AttributeError(f'No value available for field {owner.__qualname__}.{self._name}') from None
 
     def __set__(self, instance: Schema, value: Any) -> None:
-        errors = self._run_validators(instance, value)
-        try:
-            self._value = self.value_set(value, False)
-        except ValidationError as err:
+        errors = []
+        name = self._name
+        run_validators = True
+        if instance._partial and name not in instance._partial_included_fields:
+            err = ValidationError('This field cannot be set on this partial object.')
             err._bind(self)
             errors.append(err)
+        else:
+            if value is None:
+                if self.none:
+                    instance._field_values[name] = None
+                else:
+                    run_validators = False
+                    err = ValidationError('Value for this field cannot be None.')
+                    err._bind(self)
+                    errors.append(err)
+        if not errors:
+            values = instance._field_values
+            old_value = values.get(name, MISSING)
+            try:
+                values[name] = assigned_value = self.value_set(value, False)
+            except ValidationError as err:
+                error = config.get_validation_fail_exception()([err], instance)
+                new = ValidationError(error.raw())
+                new._bind(self)
+                errors.append(new)
+            else:
+                if run_validators:
+                    errors.extend(self._run_validators(instance, value, raw=True))
+                    errors.extend(self._run_validators(instance, assigned_value, raw=False))
+                if name in instance._default_fields and not errors:
+                    instance._default_fields.remove(name)
+                if errors and old_value is not MISSING:
+                    # Reset to old value if errors have occured
+                    values[name] = old_value
+
         if errors:
             cls = config.get_validation_fail_exception()
             raise cls(errors, instance)
 
     def _clear_state(self) -> None:
         self._schema: Type[Schema] = MISSING
         self._name: str = MISSING
-        self._value = MISSING
 
-    def _run_validators(self, schema: Schema, value: Any) -> List[ValidationError]:
+    def _run_validators(self, schema: Schema, value: Any, raw: bool = False) -> List[ValidationError]:
         errors = []
+        validators = self._raw_validators if raw else self._validators
 
-        for validator in self._validators:
+        for validator in validators:
             try:
                 validated = validator(schema, value)
                 if not validated:
                     raise ValidationError(f'Validation failed for field {self._name!r}')
             except ValidationError as err:
                 err._bind(self)
                 errors.append(err)
 
         return errors
 
     def _proper_name(self) -> str:
         return f'{self._schema.__qualname__}.{self._name}'
 
     @property
-    def validators(self) -> List[ValidatorCallbackT[_SchemaT]]:
+    def validators(self) -> List[ValidatorCallbackT]:
         """The list of validators for this field."""
         return self._validators.copy()
 
     @property
     def schema(self) -> Type[Schema]:
         """The :class:`Schema` class that this field belongs to."""
         # self._schema should never be MISSING as it is a late-binding
@@ -238,54 +306,62 @@
 
         Returns
         -------
         The deserialized value.
         """
         ...
 
-    def add_validator(self, callback: ValidatorCallbackT[_SchemaT]) -> None:
+    def add_validator(self, callback: ValidatorCallbackT, *, raw: bool = False) -> None:
         """Adds a validator for this field.
 
         Instead of using this method, consider using the :meth:`.validate`
         method for a simpler interface.
 
         Parameters
         ----------
         callback:
             The validator callback function.
+        raw: :class:`bool`
+            Whether this is a raw validator that takes raw value rather than
+            serialized one.
         """
-        self._validators.append(callback)
+        if raw:
+            self._raw_validators.append(callback)
+        else:
+            self._validators.append(callback)
 
-    def validate(self) -> Callable[[ValidatorCallbackT[_SchemaT]], ValidatorCallbackT[_SchemaT]]:
+    def validate(self, *, raw: bool = False) -> Callable[[ValidatorCallbackT], ValidatorCallbackT]:
         """A decorator for registering a validator for this field.
 
         This is a much simpler interface for the :meth:`.add_validator`
         method. The decorated function takes a single parameter apart
         from self and that is the value to validate.
+
+        This decorator takes same keyword arguments as :meth:`.add_validator`.
         """
-        def __decorator(func: ValidatorCallbackT[_SchemaT]) -> ValidatorCallbackT[_SchemaT]:
-            self.add_validator(func)
+        def __decorator(func: ValidatorCallbackT) -> ValidatorCallbackT:
+            self.add_validator(func, raw=raw)
             return func
         return __decorator
 
-    def remove_validator(self, callback: ValidatorCallbackT[_SchemaT]) -> None:
+    def remove_validator(self, callback: ValidatorCallbackT) -> None:
         """Removes a validator.
 
         This method does not raise any error if the given callback
         function does not exist as a validator.
 
         Parameters
         ----------
         callback:
             The validator callback function.
         """
-        try:
+        if callback in self._validators:
             self._validators.remove(callback)
-        except ValueError:
-            pass
+        if callback in self._raw_validators:
+            self._raw_validators.remove(callback)
 
 
     def copy(self: Field[_RawT, _SerializedT], *, validators: bool = True, **overrides: Any) -> Field[_RawT, _SerializedT]:
         """Copies a field.
 
         This method is useful when you want to reuse complex fields from
         another schema without having to redefine the fields.
@@ -318,14 +394,15 @@
             The copied field.
         """
         field = copy.copy(self)
         field._clear_state()
 
         if not validators:
             field._validators.clear()
+            field._raw_validators.clear()
 
         for arg, val in overrides.items():
             if not arg in self.__valid_overrides__:
                 raise TypeError(f'{arg!r} is not a valid override keyword argument.')
 
             setattr(field, arg, val)
 
@@ -339,23 +416,30 @@
 
     Parameters
     ----------
     strict: :class:`bool`
         Whether to only allow string data types. If this is set to False,
         any value is type casted to string. Defaults to True.
     """
+    __slots__ = (
+        'strict',
+    )
+
     def __init__(self, *, strict: bool = True, **kwargs: Any) -> None:
         self.strict = strict
         super().__init__(**kwargs)
 
     def _process_value(self, value: Any) -> str:
-        if not isinstance(value, str) and self.strict:
-            raise ValidationError('Value for this field must be of string data type.')
+        if not isinstance(value, str):
+            if self.strict:
+                raise ValidationError('Value for this field must be of string data type.')
 
-        return str(value)
+            return str(value)
+        else:
+            return value
 
     def value_set(self, value: Any, init: bool) -> str:
         return self._process_value(value)
 
     def value_load(self, value: Any) -> str:
         return self._process_value(value)
 
@@ -368,26 +452,32 @@
 
     Parameters
     ----------
     strict: :class:`bool`
         Whether to only allow integer data types. If this is set to False,
         any integer-castable value is type casted to integer. Defaults to True.
     """
+    __slots__ = (
+        'strict',
+    )
+
     def __init__(self, *, strict: bool = True, **kwargs: Any) -> None:
         self.strict = strict
         super().__init__(**kwargs)
 
     def _process_value(self, value: Any) -> int:
-        if not isinstance(value, int) and self.strict:
-            raise ValidationError('Value for this field must be of integer data type.')
-
-        try:
-            return int(value)
-        except Exception:
-            raise ValidationError('Value for this field must be an integer-convertable value.') from None
+        if not isinstance(value, int):
+            if self.strict:
+                raise ValidationError('Value for this field must be of integer data type.')
+            try:
+                return int(value)
+            except Exception:
+                raise ValidationError('Value for this field must be an integer-convertable value.') from None
+        else:
+            return value 
 
     def value_set(self, value: Any, init: bool) -> int:
         return self._process_value(value)
 
     def value_load(self, value: Any) -> int:
         return self._process_value(value)
 
@@ -424,14 +514,20 @@
     )
 
     FALSE_VALUES: Sequence[str] = (
         'FALSE', 'False', 'false',
         'NO', 'No', 'no', '0'
     )
 
+    __slots__ = (
+        'strict',
+        '_true_values',
+        '_false_values',
+    )
+
     def __init__(
             self,
             *,
             strict: bool = True,
             true_values: Optional[Sequence[str]] = None,
             false_values: Optional[Sequence[str]] = None,
             **kwargs: Any,
@@ -448,24 +544,26 @@
         else:
             self._true_values = []
             self._false_values = []
 
         super().__init__(**kwargs)
 
     def _process_value(self, value: Any) -> bool:
-        if not isinstance(value, bool) and self.strict:
-            raise ValidationError('Value for this field must be of boolean type.')
-
-        value = str(value)
-        if value in self._true_values:
-            return True
-        if value in self._false_values:
-            return False
+        if not isinstance(value, bool):
+            if self.strict:
+                raise ValidationError('Value for this field must be of boolean type.')
+            value = str(value)
+            if value in self._true_values:
+                return True
+            if value in self._false_values:
+                return False
+            else:
+                raise ValidationError('Value for this field must be a boolean-convertable value.')
         else:
-            raise ValidationError('Value for this field must be a boolean-convertable value.')
+            return value
 
     def value_set(self, value: Any, init: bool) -> bool:
         return self._process_value(value)
 
     def value_load(self, value: Any) -> bool:
         return self._process_value(value)
 
@@ -478,26 +576,32 @@
 
     Parameters
     ----------
     strict: :class:`bool`
         Whether to only allow float data types. If this is set to False,
         any float-castable value is type casted to float. Defaults to True.
     """
+    __slots__ = (
+        'strict',
+    )
+
     def __init__(self, *, strict: bool = True, **kwargs: Any) -> None:
         self.strict = strict
         super().__init__(**kwargs)
 
     def _process_value(self, value: Any) -> float:
-        if not isinstance(value, float) and self.strict:
-            raise ValidationError('Value for this field must be a floating point number.')
-
-        try:
-            return float(value)
-        except Exception:
-            raise ValidationError('Value for this field must be an float-convertable value.') from None
+        if not isinstance(value, float):
+            if self.strict:
+                raise ValidationError('Value for this field must be a floating point number.')
+            try:
+                return float(value)
+            except Exception:
+                raise ValidationError('Value for this field must be an float-convertable value.') from None
+        else:
+            return value
 
     def value_set(self, value: Any, init: bool) -> float:
         return self._process_value(value)
 
     def value_load(self, value: Any) -> float:
         return self._process_value(value)
 
@@ -509,25 +613,103 @@
     """Field that allows nesting of schemas.
 
     Parameters
     ----------
     schema_tp: Type[:class:`Schema`]
         The schema to represent in this field.
     """
+    __slots__ = (
+        '_schema_tp',
+    )
+
     def __init__(self, schema_tp: Type[_SchemaT], **kwargs: Any) -> None:
         self._schema_tp = schema_tp
         super().__init__(**kwargs)
 
     def value_set(self, value: Any, init: bool) -> _SchemaT:
-        if not isinstance(value, self._schema_tp):
+        if isinstance(value, collections.abc.Mapping):
+            return self.value_load(value)
+        if isinstance(value, self._schema_tp):
+            return value
+        else:
             raise ValidationError(f'Value for this field must be a {self._schema_tp.__qualname__} object.')
 
-        return value
-
     def value_load(self, value: Mapping[str, Any]) -> _SchemaT:
         try:
             return self._schema_tp._from_nested_object(value)
         except SchemaValidationFailed as err:
             raise ValidationError(err.raw()) from None
 
     def value_dump(self, value: Schema) -> Mapping[str, Any]:
         return value.dump()
+
+
+class Partial(Field[Mapping[str, Any], _SchemaT]):
+    """Field that allows nesting of partial schemas.
+
+    Partial schemas are schemas with a subset of fields of the
+    original schema.
+
+    Parameters
+    ----------
+    schema_tp: Type[:class:`Schema`]
+        The schema to represent in this field.
+    include: Sequence[:class:`str`]
+        The list of fields to include in partial schema.
+    exclude: Sequence[:class:`str`]
+        The list of fields to exclude from partial schema.
+    """
+    __slots__ = (
+        '_schema_tp',
+        'include',
+        'exclude',
+    )
+
+    def __init__(
+            self,
+            schema_tp: Type[_SchemaT],
+            include: Sequence[str] = MISSING,
+            exclude: Sequence[str] = MISSING,
+            **kwargs: Any,
+        ) -> None:
+
+        if include is not MISSING and exclude is not MISSING:
+            raise TypeError('include and exclude are mutually exclusive')
+        if not include and not exclude:
+            raise TypeError('one of include or exclude must be provided')
+
+        self._schema_tp = schema_tp
+        self.include = set() if include is MISSING else set(include)
+        self.exclude = set() if exclude is MISSING else set(exclude)
+        super().__init__(**kwargs)
+
+    @property
+    def fields(self) -> Set[str]:
+        """The set of field names to include in partial schema.
+
+        This attribute is resolved using :attr:`.include` or :attr:`.exclude`.
+        """
+        total = set(self._schema_tp.__fields__.keys())
+        if self.exclude:
+            return total.difference(self.exclude)
+        if self.include:
+            return total.intersection(self.include)
+
+        raise RuntimeError('This should never be reached')
+
+    def value_set(self, value: Any, init: bool) -> _SchemaT:
+        if isinstance(value, collections.abc.Mapping):
+            return self.value_load(value)
+        if isinstance(value, self._schema_tp):
+            value._transform_to_partial(include=self.fields)
+            return value
+        else:
+            raise ValidationError(f'Value for this field must be a {self._schema_tp.__qualname__} object.')
+
+    def value_load(self, value: Mapping[str, Any]) -> _SchemaT:
+        try:
+            return self._schema_tp._from_partial(value, include=self.fields, from_data=True)
+        except SchemaValidationFailed as err:
+            raise ValidationError(err.raw()) from None
+
+    def value_dump(self, value: Schema) -> Mapping[str, Any]:
+        return value.dump()
```

## oblate/schema.py

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import annotations
 
-from typing import Optional, Mapping, Dict, Any
+from typing import Optional, Mapping, Dict, Set, Any, Sequence
 from typing_extensions import Self
 from oblate import config
 from oblate.fields import Field
 from oblate.utils import maybe_callable, MISSING
 from oblate.exceptions import ValidationError, SchemaValidationFailed
 
 import collections.abc
@@ -47,119 +47,258 @@
         arguments.
     **kwargs:
         The keyword arguments to initialize the schema with. Cannot be
         mixed with ``data``.
     """
 
     __fields__: Dict[str, Field]
+    __load_key_fields__: Dict[str, Field]
+
+    __slots__ = (
+        '_initialized',
+        '_field_values',
+        '_default_fields',
+        '_from_data',
+        '_partial',
+        '_partial_included_fields',
+    )
 
     def __init__(self, data: Optional[Mapping[str, Any]] = None, **kwargs: Any) -> None:
-        self._initialized = False
         if data is not None:
             if kwargs:
                 raise TypeError('Cannot mix data argument with keyword arguments')
-            self._prepare(data, from_data=True)
+            from_data = True
         else:
-            self._prepare(kwargs)
+            data = kwargs
+            from_data = False
+
+        self._init(data, from_data=from_data)
 
     def __init_subclass__(cls) -> None:
         cls.__fields__ = {}
+        cls.__load_key_fields__ = {}
+
         for name, field in inspect.getmembers(cls):
             if not isinstance(field, Field):
                 continue
             
             field._schema = cls
             field._name = name
             cls.__fields__[name] = field
 
+            if field.load_key:
+                cls.__load_key_fields__[field.load_key] = field
+
     @classmethod
     def _from_nested_object(cls, data: Mapping[str, Any]) -> Self:
         if not isinstance(data, collections.abc.Mapping):
             raise ValidationError(f'Value for this field must be a {cls.__qualname__} object.')
-        
+
         return cls(data)
+    
+    @classmethod
+    def _from_partial(cls, data: Mapping[str, Any], include: Set[str], from_data: bool = False) -> Self:
+        if not isinstance(data, collections.abc.Mapping):
+            raise ValidationError(f'Value for this field must be a partial {cls.__qualname__} object.')
+
+        self = cls.__new__(cls)  # Bypass Schema.__init__()
+        self._init(
+            data,
+            from_data=from_data,
+            partial=True,
+            partial_included_fields=include,
+        )
+
+        return self
+
+    def _init(
+            self, 
+            data: Mapping[str, Any],
+            from_data: bool = False,
+            partial: bool = False,
+            partial_included_fields: Set[str] = MISSING,
+        ) -> None:
+
+        self._field_values: Dict[str, Any] = {}
+        self._default_fields: Set[str] = set()
+        self._initialized = False
+        self._from_data = from_data
+        self._partial = partial
+        self._partial_included_fields = partial_included_fields
+        self._prepare(data, include=partial_included_fields, from_data=from_data)
+        self._initialized = True
+        self.after_init_hook(data, from_data)
 
-    def _assign_field_value(self, value: Any, field: Field[Any, Any], from_data: bool = False) -> None:
+    def _assign_field_value(self, value: Any, field: Field[Any, Any], from_data: bool = False) -> Any:
         if value is None:
             if not field.none:
                 raise ValidationError('Value for this field cannot be None')
             else:
-                field._value = None
+                self._field_values[field._name] = None
             return
 
         if from_data:
-            field._value = field.value_load(value)
+            self._field_values[field._name] = final_value = field.value_load(value)
         else:
-            field._value = field.value_set(value, True)
+            self._field_values[field._name] = final_value = field.value_set(value, True)
+        
+        return final_value
+
+    def _transform_to_partial(self, include: Set[str]) -> None:
+        if self._partial:
+            return
+
+        for name, field in self.__fields__.items():
+            if name in include:
+                continue
+            try:
+                self._field_values[field._name]
+            except KeyError:
+                continue
+            else:
+                if field._name in self._default_fields:
+                    continue
+
+                err = ValidationError('This field cannot be set in this partial object.')
+                err._bind(field)
+                raise err
+
+        self._partial = True
+        self._partial_included_fields = include
 
-    def _prepare(self, data: Mapping[str, Any], from_data: bool = False) -> None:
+    def _prepare(self, data: Mapping[str, Any], include: Set[str] = MISSING, from_data: bool = False) -> None:
         fields = self.__fields__.copy()
-        validators = []
+        to_validate = []  # List of three element tuple: (field_instance, value_to_validate, is_value_raw)
         errors = []
 
         for arg, value in data.items():
             try:
                 field = fields.pop(arg)
             except KeyError:
-                errors.append(ValidationError(f'Unknown or invalid field {arg!r} provided.'))
+                if from_data and arg in self.__load_key_fields__:
+                    field = self.__load_key_fields__[arg]
+                    fields.pop(field._name, None)
+                else:
+                    errors.append(ValidationError(f'Unknown or invalid field {arg!r} provided.'))
+                    continue
+
+            if include and field._name not in include:
+                err = ValidationError(f'This field cannot be set in this partial object.')
+                err._bind(field)
+                errors.append(err)
+
+            try:
+                assigned_value = self._assign_field_value(value, field, from_data=True)
+            except ValidationError as exc:
+                exc._bind(field)
+                errors.append(exc)
             else:
-                try:
-                    self._assign_field_value(value, field, from_data=True)
-                except ValidationError as exc:
-                    exc._bind(field)
-                    errors.append(exc)
+                if field._raw_validators:
+                    to_validate.append((field, value, True))
+                if field._validators:
+                    to_validate.append((field, assigned_value, False))
 
-                if field.validators:
-                    validators.append((field, value))
+        for _, field in fields.items():
+            if include and field._name not in include:
+                continue
 
-        for name, field in fields.items():
             if field.missing:
-                field._value = maybe_callable(field.default)
-            else:
-                err = ValidationError('This field is required.')
-                err._bind(field)
-                errors.append(err)
+                if field.default is not MISSING:
+                    self._field_values[field._name] = maybe_callable(field.default)
+                    self._default_fields.add(field._name)
+                continue
+
+            err = ValidationError('This field is required.')
+            err._bind(field)
+            errors.append(err)
 
-        for field, value in validators:
-            validator_errors = field._run_validators(self, value)
+        for field, value, raw in to_validate:
+            validator_errors = field._run_validators(self, value, raw)
             errors.extend(validator_errors)
- 
+
         if errors:
             cls = config.get_validation_fail_exception()
             raise cls(errors, self)
 
-        self._initialized = True
+    def after_init_hook(self, data: Mapping[str, Any], is_data: bool, /):
+        """A hook called when the schema has successfully initialized.
+
+        This is meant to be overriden in subclasses and does nothing
+        by default.        
+
+        Parameters
+        ----------
+        data: Mapping[:class:`str`, Any]
+            The data used to initialize the model. This either corresponds
+            to the value of data argument in ``Schema.__init__()`` or the
+            keyword arguments passed.
+        is_data: :class:`bool`
+            Whether the ``data`` parameter value corresponds to the ``data``
+            argument in ``Schema.__init__()``.
+        """
+
+    def is_data_initialized(self) -> bool:
+        """Indicates whether the schema was initialized using raw data."""
+        return self._from_data
 
     def is_initialized(self) -> bool:
         """Indicates whether the schema has been initialized.
 
         This only returns True when all fields have been set
         and validated.
         """
         return self._initialized
 
-    def dump(self) -> Dict[str, Any]:
+    def is_partial(self) -> bool:
+        """Indicates whether the schema is a partial schema (see :class:`fields.Partial` for more info)."""
+        return self._partial
+
+    def dump(self, *, include: Optional[Sequence[str]] = None, exclude: Optional[Sequence[str]] = None) -> Dict[str, Any]:
         """Deserializes the schema.
 
-        The returned value is deserialized data in dictionary form.
+        The returned value is deserialized data in dictionary form. The
+        ``include`` and ``exclude`` parameters are mutually exclusive.
+
+        Parameters
+        ----------
+        include: Optional[Sequence[:class:`str`]]
+            The fields to include in the returned data.
+        exclude: Optional[Sequence[:class:`str`]]
+            The fields to exclude from the returned data.
 
         Returns
         -------
         Dict[:class:`str`, Any]
             The deserialized data.
         """
+        fields = set(self.__fields__.keys())
+        if include is not None and exclude is not None:
+            raise TypeError('include and exclude are mutually exclusive parameters.')
+        if include is not None:
+            fields = fields.intersection(set(include))
+        if exclude is not None:
+            fields = fields.difference(set(exclude))
+
         out = {}
         errors = []
-        for name, field in self.__fields__.items():
-            if field._value is MISSING:
+        partial_included = self._partial_included_fields
+
+        for name in fields:
+            field = self.__fields__[name]
+            if partial_included and name not in partial_included:
+                continue
+            key = field.dump_key if field.dump_key else field._name
+            try:
+                value = self._field_values[name]
+            except KeyError:
                 if field.default is not MISSING:
-                    value = maybe_callable(field.default)
+                    out[key] = maybe_callable(field.default)
                 continue
             try:
-                field._value = field.value_dump(field._value)
+                out[key] = field.value_dump(value)
             except ValidationError as err:
                 err._bind(field)
                 errors.append(err)
 
         if errors:
             cls = config.get_validation_fail_exception()
             raise cls(errors, self)
```

## Comparing `oblate-0.1.0.dist-info/LICENSE` & `oblate-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `oblate-0.1.0.dist-info/METADATA` & `oblate-0.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oblate
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python library for data validation
 Home-page: https://github.com/izxxr/oblate
 Author: izxxr
 License: MIT
 Project-URL: Documentation, https://oblate.readthedocs.io
 Project-URL: Issue tracker, https://github.com/izxxr/oblate/issues
 Classifier: Development Status :: 2 - Pre-Alpha
```

## Comparing `oblate-0.1.0.dist-info/RECORD` & `oblate-0.2.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-oblate/__init__.py,sha256=knE4ioydls7VqI6oNfekPuyCxK37WBU9GBK_V8bypNQ,468
+oblate/__init__.py,sha256=_G2Sk02gyIYV4FMjTaNt42pmaqVy_-pR_LfoDLcFxL4,468
 oblate/config.py,sha256=_YG-fkQsui47UzZ3jaGDOvnmnqW-SqkeZLaJ5HeZ9G8,2377
-oblate/exceptions.py,sha256=_X-OVoqqKvUIXb4o07_nTa-No-CzXHdGfCRzO9dinLs,5309
-oblate/fields.py,sha256=AJzhkHUtMMVkl1ehUPxJG0fcYMIZlvWqtWB05BAYcs0,17590
-oblate/schema.py,sha256=ccdYLhrwfrc4OAK7S6hopna9EFx5IKp-NiZYdaRFRbA,5787
+oblate/exceptions.py,sha256=OdXQJAhz1VNyq0NhjWqOexkQjnKLIStYLUalbqg7jxg,6049
+oblate/fields.py,sha256=Wq9sESJF5p6xDIvx4FTkaD4jcgB-ULPCoKlbi5NXAlc,24162
+oblate/schema.py,sha256=omuUKjrt3XxSrer2TnMJq0UuY-1PQAHVqf0lHHgrl0M,11169
 oblate/utils.py,sha256=REakgRbxgRr4lR71d0QEyI54H14EQB-JjcKlZptw8D0,1515
-oblate-0.1.0.dist-info/LICENSE,sha256=mKXNxzGtJSFJR9bJO6qD0eHfjXAkzcYpaQDpGBfSnTQ,1089
-oblate-0.1.0.dist-info/METADATA,sha256=Uj9uWx2x06ttyfVXWQzJHpOm_623ybjF8WX0oz2oqgg,5366
-oblate-0.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-oblate-0.1.0.dist-info/top_level.txt,sha256=qaLuhl_5_njDgbVh2b6hw4kLVy3p1i2QRiAULmZYGzM,7
-oblate-0.1.0.dist-info/RECORD,,
+oblate-0.2.0.dist-info/LICENSE,sha256=mKXNxzGtJSFJR9bJO6qD0eHfjXAkzcYpaQDpGBfSnTQ,1089
+oblate-0.2.0.dist-info/METADATA,sha256=LFUWWt0sQRas9Kw5IEB6uFHbtTOA-ovMM2XOXWdPUD0,5366
+oblate-0.2.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+oblate-0.2.0.dist-info/top_level.txt,sha256=qaLuhl_5_njDgbVh2b6hw4kLVy3p1i2QRiAULmZYGzM,7
+oblate-0.2.0.dist-info/RECORD,,
```

