# Comparing `tmp/seamful-0.1.0.tar.gz` & `tmp/seamful-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seamful-0.1.0.tar", max compression
+gzip compressed data, was "seamful-0.2.0.tar", max compression
```

## Comparing `seamful-0.1.0.tar` & `seamful-0.2.0.tar`

### file list

```diff
@@ -1,102 +1,129 @@
--rw-r--r--   0        0        0     6682 2023-07-13 22:29:45.335356 seamful-0.1.0/README.md
--rw-r--r--   0        0        0      404 2023-07-13 22:32:22.609076 seamful-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      187 2023-07-11 00:27:04.110060 seamful-0.1.0/src/seamful/__init__.py
--rw-r--r--   0        0        0       78 2023-07-11 00:27:37.897999 seamful-0.1.0/src/seamful/application/__init__.py
--rw-r--r--   0        0        0    10839 2023-07-13 22:29:45.415357 seamful-0.1.0/src/seamful/application/application.py
--rw-r--r--   0        0        0    15680 2023-07-13 22:28:44.194645 seamful-0.1.0/src/seamful/application/errors.py
--rw-r--r--   0        0        0     3159 2023-07-13 22:28:44.238646 seamful-0.1.0/src/seamful/application/graph_provider.py
--rw-r--r--   0        0        0     4620 2023-07-13 22:28:44.182645 seamful-0.1.0/src/seamful/application/graph_solver.py
--rw-r--r--   0        0        0     2029 2023-07-13 22:28:44.210646 seamful-0.1.0/src/seamful/application/registry.py
--rw-r--r--   0        0        0    45264 2023-07-13 22:28:44.222646 seamful-0.1.0/src/seamful/application/test_container.py
--rw-r--r--   0        0        0      284 2023-07-13 22:29:45.467357 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationCallingProviderMethods_test_provider_method_cannot_access_the_provider_instance.txt
--rw-r--r--   0        0        0      295 2023-07-13 22:29:45.495358 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationImplicitProviders_test_application_fails_on_closing_registration_if_any_implicit_provider_is_unused.txt
--rw-r--r--   0        0        0      553 2023-07-11 02:12:32.105119 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationImplicitProviders_test_cant_install_implicit_provider.txt
--rw-r--r--   0        0        0      159 2023-07-11 02:12:32.105119 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationProvision_test_application_cant_provide_unknown_resource.txt
--rw-r--r--   0        0        0      146 2023-07-11 02:12:32.109120 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationProvision_test_application_refuses_to_provide_before_registrations_are_closed.txt
--rw-r--r--   0        0        0      357 2023-07-13 22:29:45.407357 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationProvision_test_refuses_to_provide_resource_not_defined_on_the_original_provider.txt
--rw-r--r--   0        0        0      111 2023-07-11 02:12:32.109120 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationRegistration_test_application_disallows_installing_a_module_twice.txt
--rw-r--r--   0        0        0      245 2023-07-13 22:29:45.443357 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationRegistration_test_application_install_provider_must_provide_for_module.txt
--rw-r--r--   0        0        0       74 2023-07-11 02:12:32.109120 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationRegistration_test_cannot_install_same_provider_twice.txt
--rw-r--r--   0        0        0      413 2023-07-11 02:12:32.109120 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationRegistration_test_cannot_install_two_providers_for_the_same_module.txt
--rw-r--r--   0        0        0      118 2023-07-11 02:12:32.109120 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationRegistration_test_cant_install_module_after_ready.txt
--rw-r--r--   0        0        0      125 2023-07-11 02:12:32.109120 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationRegistration_test_cant_install_provider_after_ready.txt
--rw-r--r--   0        0        0      181 2023-07-11 02:12:32.113119 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationTampering_test_application_cannot_be_tampered_twice.txt
--rw-r--r--   0        0        0      391 2023-07-11 02:12:32.113119 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationTampering_test_application_must_be_ready_before_tampering_with_it.txt
--rw-r--r--   0        0        0      163 2023-07-11 02:12:32.113119 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationTampering_test_application_refuses_to_restore_if_not_previously_tampered_with.txt
--rw-r--r--   0        0        0      413 2023-07-11 02:12:32.113119 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationTampering_test_cannot_override_provider_on_tampered_application_without_explicit_overrides_allowed.txt
--rw-r--r--   0        0        0      157 2023-07-11 02:12:32.113119 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationTampering_test_cannot_reopen_for_registration_once_a_resource_has_been_provided.txt
--rw-r--r--   0        0        0       77 2023-07-11 02:12:32.113119 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationTampering_test_ready_application_refuses_to_be_made_ready_again.txt
--rw-r--r--   0        0        0      125 2023-07-11 02:12:32.113119 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestApplicationTampering_test_restoring_application_doesn_allow_for_more_registrations.txt
--rw-r--r--   0        0        0      692 2023-07-13 22:29:45.399356 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_catches_circular_dependencies_involving_overriding_resources.txt
--rw-r--r--   0        0        0      250 2023-07-13 22:29:45.367356 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_catches_circular_dependencies_involving_private_resources.txt
--rw-r--r--   0        0        0      588 2023-07-13 22:29:45.315356 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_catches_inner_circular_dependency.txt
--rw-r--r--   0        0        0      801 2023-07-13 22:29:45.435357 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_many_providers_circular_dependency_breaks_on_seal.txt
--rw-r--r--   0        0        0      181 2023-07-13 22:29:45.347356 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_simplest_circular_dependency_breaks_on_seal.txt
--rw-r--r--   0        0        0      389 2023-07-13 22:29:45.471357 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_single_provider_circular_dependency_breaks_on_seal.txt
--rw-r--r--   0        0        0       59 2023-07-11 02:12:32.117119 seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestDefaultProvider_test_application_cant_seal_if_a_module_lacks_a_provider.txt
--rw-r--r--   0        0        0     5119 2023-07-13 22:29:45.379356 seamful-0.1.0/src/seamful/errors.py
--rw-r--r--   0        0        0       55 2023-03-22 00:42:30.896082 seamful-0.1.0/src/seamful/module/__init__.py
--rw-r--r--   0        0        0     9267 2023-07-13 22:28:44.214646 seamful-0.1.0/src/seamful/module/errors.py
--rw-r--r--   0        0        0     4256 2023-07-13 22:28:44.214646 seamful-0.1.0/src/seamful/module/module_type.py
--rw-r--r--   0        0        0      177 2023-07-13 22:29:45.439357 seamful-0.1.0/src/seamful/module/test_fixtures/test_module_TestModuleClassDeclaration_test_module_classes_attributes_must_be_types_or_resources.txt
--rw-r--r--   0        0        0      266 2023-07-13 22:29:45.479357 seamful-0.1.0/src/seamful/module/test_fixtures/test_module_TestModuleClassDeclaration_test_module_classes_cannot_have_an_attribute_named_default_provider.txt
--rw-r--r--   0        0        0      221 2023-07-13 22:29:45.395357 seamful-0.1.0/src/seamful/module/test_fixtures/test_module_TestModuleClassDeclaration_test_module_classes_cannot_have_private_attributes.txt
--rw-r--r--   0        0        0      303 2023-07-11 02:12:32.121119 seamful-0.1.0/src/seamful/module/test_fixtures/test_module_TestModuleClassDeclaration_test_modules_cannot_be_defined_as_a_subclass_of_another_module.txt
--rw-r--r--   0        0        0      165 2023-07-11 02:12:32.121119 seamful-0.1.0/src/seamful/module/test_fixtures/test_module_TestModuleClassDeclaration_test_modules_cannot_be_instantiated.txt
--rw-r--r--   0        0        0      165 2023-07-11 02:12:32.121119 seamful-0.1.0/src/seamful/module/test_fixtures/test_module_TestModuleClassDeclaration_test_modules_cannot_be_instantiated_even_if_defining_constructor.txt
--rw-r--r--   0        0        0      124 2023-07-11 02:12:32.121119 seamful-0.1.0/src/seamful/module/test_fixtures/test_module_TestModuleDefaultProvider_test_cant_set_a_default_provider_to_one_that_provides_to_another_module.txt
--rw-r--r--   0        0        0      261 2023-07-13 22:29:45.431357 seamful-0.1.0/src/seamful/module/test_fixtures/test_module_TestModuleDefaultProvider_test_cant_set_a_default_provider_to_something_not_a_provider.txt
--rw-r--r--   0        0        0       84 2023-07-11 02:12:32.121119 seamful-0.1.0/src/seamful/module/test_fixtures/test_module_TestModuleDefaultProvider_test_cant_use_base_provider_as_default_provider.txt
--rw-r--r--   0        0        0      326 2023-07-13 22:29:45.419357 seamful-0.1.0/src/seamful/module/test_fixtures/test_module_TestModuleResourcesFromResourceInstances_test_module_fails_on_a_resource_defined_as_another_modules_resource.txt
--rw-r--r--   0        0        0      249 2023-07-13 22:29:45.327356 seamful-0.1.0/src/seamful/module/test_fixtures/test_module_TestModuleResourcesFromResourceInstances_test_module_refuses_definition_of_overriding_resource_in_it.txt
--rw-r--r--   0        0        0      241 2023-07-13 22:29:45.487357 seamful-0.1.0/src/seamful/module/test_fixtures/test_module_TestModuleResourcesFromResourceInstances_test_module_refuses_definition_of_private_resource_in_it.txt
--rw-r--r--   0        0        0     8517 2023-07-13 22:28:44.206646 seamful-0.1.0/src/seamful/module/test_module.py
--rw-r--r--   0        0        0       75 2023-03-22 00:42:30.900082 seamful-0.1.0/src/seamful/provider/__init__.py
--rw-r--r--   0        0        0    31490 2023-07-13 22:28:44.234646 seamful-0.1.0/src/seamful/provider/errors.py
--rw-r--r--   0        0        0    13430 2023-07-13 22:28:44.190645 seamful-0.1.0/src/seamful/provider/provider_type.py
--rw-r--r--   0        0        0      199 2023-07-13 22:29:45.519358 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderClassBehavior_test_provider_attributes_can_only_be_resources_or_provider_methods.txt
--rw-r--r--   0        0        0      175 2023-07-11 02:12:32.125119 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderClassBehavior_test_providers_cannot_be_instantiated.txt
--rw-r--r--   0        0        0      175 2023-07-11 02:12:32.125119 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderClassBehavior_test_providers_cannot_be_instantiated_event_if_defining_constructor.txt
--rw-r--r--   0        0        0      228 2023-07-13 22:29:45.503358 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderClassBehavior_test_providers_dont_support_multiple_inheritance.txt
--rw-r--r--   0        0        0      218 2023-07-13 22:29:45.519358 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderClassBehavior_test_providers_module_cannot_be_manually_set.txt
--rw-r--r--   0        0        0      209 2023-07-13 22:29:45.499358 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderClassBehavior_test_providers_must_inherit_from_provider_or_subclass.txt
--rw-r--r--   0        0        0      319 2023-07-13 22:29:45.387356 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderClassBehavior_test_providers_must_state_which_module_it_provides_for_as_class_argument.txt
--rw-r--r--   0        0        0      218 2023-07-11 02:12:32.125119 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderCollectingProviderMethods_test_missing_provider_method.txt
--rw-r--r--   0        0        0      253 2023-07-11 02:12:32.125119 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderCollectingProviderMethods_test_missing_provider_method_for_overriding_provider_resource.txt
--rw-r--r--   0        0        0      242 2023-07-11 02:12:32.125119 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderCollectingProviderMethods_test_missing_provider_method_for_private_provider_resource.txt
--rw-r--r--   0        0        0      259 2023-07-13 22:29:45.355356 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderCollectingProviderMethods_test_provider_method_lookup_module_mismatch.txt
--rw-r--r--   0        0        0      275 2023-07-13 22:29:45.343356 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderCollectingProviderMethods_test_provider_method_lookup_provider_mismatch.txt
--rw-r--r--   0        0        0      217 2023-07-13 22:29:45.423357 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderCollectingProviderMethods_test_provider_method_lookup_unknown_module_resource.txt
--rw-r--r--   0        0        0      245 2023-07-13 22:29:45.451357 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderCollectingProviderMethods_test_provider_method_lookup_unknown_provider_resource.txt
--rw-r--r--   0        0        0      114 2023-07-11 02:12:32.129119 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderCollectingProviderMethods_test_provider_method_not_callable.txt
--rw-r--r--   0        0        0      372 2023-07-13 22:29:45.339356 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_method_for_binding_resource_must_satisfy_more_concrete_type.txt
--rw-r--r--   0        0        0      193 2023-07-13 22:29:45.435357 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_method_must_either_match_by_resource_or_by_name.txt
--rw-r--r--   0        0        0      285 2023-07-13 22:29:45.507358 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_method_must_have_a_compatible_return_type_annotation.txt
--rw-r--r--   0        0        0      342 2023-07-13 22:29:45.455357 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_method_must_have_return_type_annotation.txt
--rw-r--r--   0        0        0      253 2023-07-13 22:29:45.351356 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_method_parameter_annotation_must_be_a_type.txt
--rw-r--r--   0        0        0      170 2023-07-13 22:29:45.359356 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_method_parameters_must_have_type_annotations.txt
--rw-r--r--   0        0        0      289 2023-07-13 22:29:45.511358 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_method_referring_to_module_resource_must_match_type.txt
--rw-r--r--   0        0        0      387 2023-07-13 22:29:45.403357 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_subclass_must_refine_provider_method_if_refining_overriding_resource.txt
--rw-r--r--   0        0        0      366 2023-07-13 22:29:45.427357 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_subclass_must_refine_provider_method_if_refining_private_resource.txt
--rw-r--r--   0        0        0      230 2023-07-13 22:29:45.515358 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderModuleAnnotation_test_cannot_provide_base_module.txt
--rw-r--r--   0        0        0      306 2023-07-13 22:29:45.375356 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderModuleAnnotation_test_invalid_provider_module_annotation.txt
--rw-r--r--   0        0        0      180 2023-07-13 22:29:45.371356 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderModuleAnnotation_test_invalid_provider_module_annotation_not_even_a_class.txt
--rw-r--r--   0        0        0      350 2023-07-13 22:29:45.483358 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderModuleAnnotation_test_provider_method_cannot_depend_on_another_providers_resource.txt
--rw-r--r--   0        0        0      486 2023-07-13 22:29:45.491358 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderModuleAnnotation_test_provider_method_cannot_depend_on_parent_providers_resource.txt
--rw-r--r--   0        0        0      401 2023-07-13 22:29:45.319356 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderResourcesFromResourceInstances_test_provider_fails_on_private_resource_defined_as_another_modules_resource.txt
--rw-r--r--   0        0        0      316 2023-07-13 22:29:45.491358 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderResourcesFromResourceInstances_test_provider_refuses_module_resource.txt
--rw-r--r--   0        0        0      172 2023-07-11 02:12:32.137119 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderResourcesFromResourceInstances_test_provider_refuses_overriding_resource_if_name_doesnt_match_module_resource.txt
--rw-r--r--   0        0        0      290 2023-07-13 22:29:45.475357 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderResourcesFromResourceInstances_test_provider_refuses_private_resource_if_occludes_module_resource.txt
--rw-r--r--   0        0        0      338 2023-07-13 22:29:45.331356 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderResourcesFromResourceInstances_test_provider_refuses_public_resource_looking_like_an_override.txt
--rw-r--r--   0        0        0      434 2023-07-13 22:29:45.391357 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderResourcesFromResourceInstances_test_provider_refuses_resource_declaration_that_uses_another_provider_resource.txt
--rw-r--r--   0        0        0      351 2023-07-13 22:29:45.323356 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderResourcesTypeAliases_test_provider_refuses_overriding_resources_from_type_alias_if_type_not_satisfied.txt
--rw-r--r--   0        0        0      239 2023-07-13 22:29:45.395357 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderSubclasses_test_provider_attribute_cannot_be_named_module.txt
--rw-r--r--   0        0        0      242 2023-07-13 22:29:45.335356 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderSubclasses_test_provider_attribute_cannot_be_named_resources.txt
--rw-r--r--   0        0        0      404 2023-07-13 22:29:45.383356 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderSubclasses_test_provider_subclass_must_provide_for_the_same_module_as_base.txt
--rw-r--r--   0        0        0      505 2023-07-13 22:29:45.463357 seamful-0.1.0/src/seamful/provider/test_fixtures/test_provider_TestProviderSubclasses_test_provider_subclass_overriding_resource_must_be_subtypes_of_base_providers_resource.txt
--rw-r--r--   0        0        0    44102 2023-07-13 22:28:44.178645 seamful-0.1.0/src/seamful/provider/test_provider.py
--rw-r--r--   0        0        0     4822 2023-07-13 22:29:45.411357 seamful-0.1.0/src/seamful/resource/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 00:42:30.904082 seamful-0.1.0/src/seamful/resources/__init__.py
--rw-r--r--   0        0        0       63 2023-03-22 00:42:30.908082 seamful-0.1.0/src/seamful/resources/errors.py
--rw-r--r--   0        0        0     4501 2023-03-22 22:35:52.779594 seamful-0.1.0/src/seamful/utils_for_tests.py
--rw-r--r--   0        0        0     7262 1970-01-01 00:00:00.000000 seamful-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6681 2023-07-17 21:52:34.266366 seamful-0.2.0/README.md
+-rw-r--r--   0        0        0      454 2023-07-17 22:42:31.332881 seamful-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      187 2023-07-11 00:27:04.110060 seamful-0.2.0/src/seamful/__init__.py
+-rw-r--r--   0        0        0       78 2023-07-11 00:27:37.897999 seamful-0.2.0/src/seamful/application/__init__.py
+-rw-r--r--   0        0        0    10501 2023-07-17 21:54:56.323566 seamful-0.2.0/src/seamful/application/application.py
+-rw-r--r--   0        0        0    14002 2023-07-17 22:35:02.127942 seamful-0.2.0/src/seamful/application/errors.py
+-rw-r--r--   0        0        0     3152 2023-07-17 21:56:21.280280 seamful-0.2.0/src/seamful/application/graph_provider.py
+-rw-r--r--   0        0        0     4608 2023-07-17 21:56:39.696944 seamful-0.2.0/src/seamful/application/graph_solver.py
+-rw-r--r--   0        0        0     1896 2023-07-17 22:17:43.423308 seamful-0.2.0/src/seamful/application/registry.py
+-rw-r--r--   0        0        0    48142 2023-07-17 22:35:56.040046 seamful-0.2.0/src/seamful/application/test_application.py
+-rw-r--r--   0        0        0      286 2023-07-17 21:31:20.002010 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationCallingProviderMethods_test_provider_method_cannot_access_the_provider_instance.txt
+-rw-r--r--   0        0        0      295 2023-07-17 21:57:27.786486 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationImplicitProviders_test_application_fails_on_closing_registration_if_any_implicit_provider_is_unused.txt
+-rw-r--r--   0        0        0      157 2023-07-17 21:57:27.786486 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationImplicitProviders_test_can_install_private_provider_if_module_is_used.txt
+-rw-r--r--   0        0        0      295 2023-07-17 21:57:27.786486 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationImplicitProviders_test_cant_install_private_provider_if_module_is_not_used.txt
+-rw-r--r--   0        0        0      157 2023-07-17 21:57:27.790487 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationProvision_test_application_cant_provide_unknown_resource.txt
+-rw-r--r--   0        0        0      146 2023-07-17 21:31:20.010011 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationProvision_test_application_refuses_to_provide_before_registrations_are_closed.txt
+-rw-r--r--   0        0        0      362 2023-07-17 21:57:27.794487 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationProvision_test_refuses_to_provide_resource_not_defined_on_the_original_provider.txt
+-rw-r--r--   0        0        0      109 2023-07-17 21:57:27.794487 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationRegistration_test_application_disallows_installing_a_module_twice.txt
+-rw-r--r--   0        0        0      249 2023-07-17 21:31:20.014011 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationRegistration_test_application_install_provider_must_provide_for_module.txt
+-rw-r--r--   0        0        0      412 2023-07-17 21:57:27.794487 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationRegistration_test_cannot_install_two_providers_for_the_same_module.txt
+-rw-r--r--   0        0        0      118 2023-07-17 21:31:20.014011 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationRegistration_test_cant_install_module_after_ready.txt
+-rw-r--r--   0        0        0      125 2023-07-17 21:31:20.014011 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationRegistration_test_cant_install_provider_after_ready.txt
+-rw-r--r--   0        0        0      181 2023-07-17 21:31:20.018011 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationTampering_test_application_cannot_be_tampered_twice.txt
+-rw-r--r--   0        0        0      391 2023-07-17 21:31:20.018011 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationTampering_test_application_must_be_ready_before_tampering_with_it.txt
+-rw-r--r--   0        0        0      163 2023-07-17 21:31:20.018011 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationTampering_test_application_refuses_to_restore_if_not_previously_tampered_with.txt
+-rw-r--r--   0        0        0      412 2023-07-17 21:57:27.798487 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationTampering_test_cannot_override_provider_on_tampered_application_without_explicit_overrides_allowed.txt
+-rw-r--r--   0        0        0      157 2023-07-17 21:31:20.018011 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationTampering_test_cannot_reopen_for_registration_once_a_resource_has_been_provided.txt
+-rw-r--r--   0        0        0       77 2023-07-17 21:31:20.018011 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationTampering_test_ready_application_refuses_to_be_made_ready_again.txt
+-rw-r--r--   0        0        0      125 2023-07-17 21:31:20.022011 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestApplicationTampering_test_restoring_application_doesn_allow_for_more_registrations.txt
+-rw-r--r--   0        0        0      694 2023-07-17 21:31:20.022011 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestCircularDependencies_test_catches_circular_dependencies_involving_overriding_resources.txt
+-rw-r--r--   0        0        0      252 2023-07-17 21:31:20.022011 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestCircularDependencies_test_catches_circular_dependencies_involving_private_resources.txt
+-rw-r--r--   0        0        0      590 2023-07-17 21:31:20.022011 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestCircularDependencies_test_catches_inner_circular_dependency.txt
+-rw-r--r--   0        0        0      807 2023-07-17 21:31:20.022011 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestCircularDependencies_test_many_providers_circular_dependency_breaks_on_seal.txt
+-rw-r--r--   0        0        0      183 2023-07-17 21:31:20.026011 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestCircularDependencies_test_simplest_circular_dependency_breaks_on_seal.txt
+-rw-r--r--   0        0        0      391 2023-07-17 21:31:20.026011 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestCircularDependencies_test_single_provider_circular_dependency_breaks_on_seal.txt
+-rw-r--r--   0        0        0       58 2023-07-17 21:57:27.806487 seamful-0.2.0/src/seamful/application/test_fixtures/test_application_TestDefaultProvider_test_application_cant_seal_if_a_module_lacks_a_provider.txt
+-rw-r--r--   0        0        0      284 2023-07-13 22:29:45.467357 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationCallingProviderMethods_test_provider_method_cannot_access_the_provider_instance.txt
+-rw-r--r--   0        0        0      295 2023-07-13 22:29:45.495358 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationImplicitProviders_test_application_fails_on_closing_registration_if_any_implicit_provider_is_unused.txt
+-rw-r--r--   0        0        0      159 2023-07-17 21:27:04.279042 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationImplicitProviders_test_can_install_private_provider_if_module_is_used.txt
+-rw-r--r--   0        0        0      295 2023-07-17 21:30:29.297421 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationImplicitProviders_test_cant_install_private_provider_if_module_is_not_used.txt
+-rw-r--r--   0        0        0      159 2023-07-11 02:12:32.105119 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationProvision_test_application_cant_provide_unknown_resource.txt
+-rw-r--r--   0        0        0      146 2023-07-11 02:12:32.109120 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationProvision_test_application_refuses_to_provide_before_registrations_are_closed.txt
+-rw-r--r--   0        0        0      357 2023-07-13 22:29:45.407357 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationProvision_test_refuses_to_provide_resource_not_defined_on_the_original_provider.txt
+-rw-r--r--   0        0        0      111 2023-07-11 02:12:32.109120 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationRegistration_test_application_disallows_installing_a_module_twice.txt
+-rw-r--r--   0        0        0      245 2023-07-13 22:29:45.443357 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationRegistration_test_application_install_provider_must_provide_for_module.txt
+-rw-r--r--   0        0        0       74 2023-07-11 02:12:32.109120 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationRegistration_test_cannot_install_same_provider_twice.txt
+-rw-r--r--   0        0        0      413 2023-07-11 02:12:32.109120 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationRegistration_test_cannot_install_two_providers_for_the_same_module.txt
+-rw-r--r--   0        0        0      118 2023-07-11 02:12:32.109120 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationRegistration_test_cant_install_module_after_ready.txt
+-rw-r--r--   0        0        0      125 2023-07-11 02:12:32.109120 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationRegistration_test_cant_install_provider_after_ready.txt
+-rw-r--r--   0        0        0      181 2023-07-11 02:12:32.113119 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationTampering_test_application_cannot_be_tampered_twice.txt
+-rw-r--r--   0        0        0      391 2023-07-11 02:12:32.113119 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationTampering_test_application_must_be_ready_before_tampering_with_it.txt
+-rw-r--r--   0        0        0      163 2023-07-11 02:12:32.113119 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationTampering_test_application_refuses_to_restore_if_not_previously_tampered_with.txt
+-rw-r--r--   0        0        0      413 2023-07-11 02:12:32.113119 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationTampering_test_cannot_override_provider_on_tampered_application_without_explicit_overrides_allowed.txt
+-rw-r--r--   0        0        0      157 2023-07-11 02:12:32.113119 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationTampering_test_cannot_reopen_for_registration_once_a_resource_has_been_provided.txt
+-rw-r--r--   0        0        0       77 2023-07-11 02:12:32.113119 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationTampering_test_ready_application_refuses_to_be_made_ready_again.txt
+-rw-r--r--   0        0        0      125 2023-07-11 02:12:32.113119 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestApplicationTampering_test_restoring_application_doesn_allow_for_more_registrations.txt
+-rw-r--r--   0        0        0      692 2023-07-13 22:29:45.399356 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_catches_circular_dependencies_involving_overriding_resources.txt
+-rw-r--r--   0        0        0      250 2023-07-13 22:29:45.367356 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_catches_circular_dependencies_involving_private_resources.txt
+-rw-r--r--   0        0        0      588 2023-07-13 22:29:45.315356 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_catches_inner_circular_dependency.txt
+-rw-r--r--   0        0        0      801 2023-07-13 22:29:45.435357 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_many_providers_circular_dependency_breaks_on_seal.txt
+-rw-r--r--   0        0        0      181 2023-07-13 22:29:45.347356 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_simplest_circular_dependency_breaks_on_seal.txt
+-rw-r--r--   0        0        0      389 2023-07-13 22:29:45.471357 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_single_provider_circular_dependency_breaks_on_seal.txt
+-rw-r--r--   0        0        0       59 2023-07-11 02:12:32.117119 seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestDefaultProvider_test_application_cant_seal_if_a_module_lacks_a_provider.txt
+-rw-r--r--   0        0        0     5119 2023-07-13 22:29:45.379356 seamful-0.2.0/src/seamful/errors.py
+-rw-r--r--   0        0        0       55 2023-03-22 00:42:30.896082 seamful-0.2.0/src/seamful/module/__init__.py
+-rw-r--r--   0        0        0     9267 2023-07-13 22:28:44.214646 seamful-0.2.0/src/seamful/module/errors.py
+-rw-r--r--   0        0        0     4256 2023-07-13 22:28:44.214646 seamful-0.2.0/src/seamful/module/module_type.py
+-rw-r--r--   0        0        0      177 2023-07-13 22:29:45.439357 seamful-0.2.0/src/seamful/module/test_fixtures/test_module_TestModuleClassDeclaration_test_module_classes_attributes_must_be_types_or_resources.txt
+-rw-r--r--   0        0        0      266 2023-07-13 22:29:45.479357 seamful-0.2.0/src/seamful/module/test_fixtures/test_module_TestModuleClassDeclaration_test_module_classes_cannot_have_an_attribute_named_default_provider.txt
+-rw-r--r--   0        0        0      221 2023-07-13 22:29:45.395357 seamful-0.2.0/src/seamful/module/test_fixtures/test_module_TestModuleClassDeclaration_test_module_classes_cannot_have_private_attributes.txt
+-rw-r--r--   0        0        0      303 2023-07-11 02:12:32.121119 seamful-0.2.0/src/seamful/module/test_fixtures/test_module_TestModuleClassDeclaration_test_modules_cannot_be_defined_as_a_subclass_of_another_module.txt
+-rw-r--r--   0        0        0      165 2023-07-11 02:12:32.121119 seamful-0.2.0/src/seamful/module/test_fixtures/test_module_TestModuleClassDeclaration_test_modules_cannot_be_instantiated.txt
+-rw-r--r--   0        0        0      165 2023-07-11 02:12:32.121119 seamful-0.2.0/src/seamful/module/test_fixtures/test_module_TestModuleClassDeclaration_test_modules_cannot_be_instantiated_even_if_defining_constructor.txt
+-rw-r--r--   0        0        0      124 2023-07-11 02:12:32.121119 seamful-0.2.0/src/seamful/module/test_fixtures/test_module_TestModuleDefaultProvider_test_cant_set_a_default_provider_to_one_that_provides_to_another_module.txt
+-rw-r--r--   0        0        0      261 2023-07-13 22:29:45.431357 seamful-0.2.0/src/seamful/module/test_fixtures/test_module_TestModuleDefaultProvider_test_cant_set_a_default_provider_to_something_not_a_provider.txt
+-rw-r--r--   0        0        0       84 2023-07-11 02:12:32.121119 seamful-0.2.0/src/seamful/module/test_fixtures/test_module_TestModuleDefaultProvider_test_cant_use_base_provider_as_default_provider.txt
+-rw-r--r--   0        0        0      326 2023-07-13 22:29:45.419357 seamful-0.2.0/src/seamful/module/test_fixtures/test_module_TestModuleResourcesFromResourceInstances_test_module_fails_on_a_resource_defined_as_another_modules_resource.txt
+-rw-r--r--   0        0        0      249 2023-07-13 22:29:45.327356 seamful-0.2.0/src/seamful/module/test_fixtures/test_module_TestModuleResourcesFromResourceInstances_test_module_refuses_definition_of_overriding_resource_in_it.txt
+-rw-r--r--   0        0        0      241 2023-07-13 22:29:45.487357 seamful-0.2.0/src/seamful/module/test_fixtures/test_module_TestModuleResourcesFromResourceInstances_test_module_refuses_definition_of_private_resource_in_it.txt
+-rw-r--r--   0        0        0     8517 2023-07-13 22:28:44.206646 seamful-0.2.0/src/seamful/module/test_module.py
+-rw-r--r--   0        0        0       75 2023-03-22 00:42:30.900082 seamful-0.2.0/src/seamful/provider/__init__.py
+-rw-r--r--   0        0        0    31490 2023-07-13 22:28:44.234646 seamful-0.2.0/src/seamful/provider/errors.py
+-rw-r--r--   0        0        0    13430 2023-07-13 22:28:44.190645 seamful-0.2.0/src/seamful/provider/provider_type.py
+-rw-r--r--   0        0        0      199 2023-07-13 22:29:45.519358 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderClassBehavior_test_provider_attributes_can_only_be_resources_or_provider_methods.txt
+-rw-r--r--   0        0        0      175 2023-07-11 02:12:32.125119 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderClassBehavior_test_providers_cannot_be_instantiated.txt
+-rw-r--r--   0        0        0      175 2023-07-11 02:12:32.125119 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderClassBehavior_test_providers_cannot_be_instantiated_event_if_defining_constructor.txt
+-rw-r--r--   0        0        0      228 2023-07-13 22:29:45.503358 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderClassBehavior_test_providers_dont_support_multiple_inheritance.txt
+-rw-r--r--   0        0        0      218 2023-07-13 22:29:45.519358 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderClassBehavior_test_providers_module_cannot_be_manually_set.txt
+-rw-r--r--   0        0        0      209 2023-07-13 22:29:45.499358 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderClassBehavior_test_providers_must_inherit_from_provider_or_subclass.txt
+-rw-r--r--   0        0        0      319 2023-07-13 22:29:45.387356 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderClassBehavior_test_providers_must_state_which_module_it_provides_for_as_class_argument.txt
+-rw-r--r--   0        0        0      218 2023-07-11 02:12:32.125119 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderCollectingProviderMethods_test_missing_provider_method.txt
+-rw-r--r--   0        0        0      253 2023-07-11 02:12:32.125119 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderCollectingProviderMethods_test_missing_provider_method_for_overriding_provider_resource.txt
+-rw-r--r--   0        0        0      242 2023-07-11 02:12:32.125119 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderCollectingProviderMethods_test_missing_provider_method_for_private_provider_resource.txt
+-rw-r--r--   0        0        0      259 2023-07-13 22:29:45.355356 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderCollectingProviderMethods_test_provider_method_lookup_module_mismatch.txt
+-rw-r--r--   0        0        0      275 2023-07-13 22:29:45.343356 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderCollectingProviderMethods_test_provider_method_lookup_provider_mismatch.txt
+-rw-r--r--   0        0        0      217 2023-07-13 22:29:45.423357 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderCollectingProviderMethods_test_provider_method_lookup_unknown_module_resource.txt
+-rw-r--r--   0        0        0      245 2023-07-13 22:29:45.451357 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderCollectingProviderMethods_test_provider_method_lookup_unknown_provider_resource.txt
+-rw-r--r--   0        0        0      114 2023-07-11 02:12:32.129119 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderCollectingProviderMethods_test_provider_method_not_callable.txt
+-rw-r--r--   0        0        0      372 2023-07-13 22:29:45.339356 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_method_for_binding_resource_must_satisfy_more_concrete_type.txt
+-rw-r--r--   0        0        0      193 2023-07-13 22:29:45.435357 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_method_must_either_match_by_resource_or_by_name.txt
+-rw-r--r--   0        0        0      285 2023-07-13 22:29:45.507358 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_method_must_have_a_compatible_return_type_annotation.txt
+-rw-r--r--   0        0        0      342 2023-07-13 22:29:45.455357 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_method_must_have_return_type_annotation.txt
+-rw-r--r--   0        0        0      253 2023-07-13 22:29:45.351356 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_method_parameter_annotation_must_be_a_type.txt
+-rw-r--r--   0        0        0      170 2023-07-13 22:29:45.359356 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_method_parameters_must_have_type_annotations.txt
+-rw-r--r--   0        0        0      289 2023-07-13 22:29:45.511358 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_method_referring_to_module_resource_must_match_type.txt
+-rw-r--r--   0        0        0      387 2023-07-13 22:29:45.403357 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_subclass_must_refine_provider_method_if_refining_overriding_resource.txt
+-rw-r--r--   0        0        0      366 2023-07-13 22:29:45.427357 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderMethodFromSignature_test_provider_subclass_must_refine_provider_method_if_refining_private_resource.txt
+-rw-r--r--   0        0        0      230 2023-07-13 22:29:45.515358 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderModuleAnnotation_test_cannot_provide_base_module.txt
+-rw-r--r--   0        0        0      306 2023-07-13 22:29:45.375356 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderModuleAnnotation_test_invalid_provider_module_annotation.txt
+-rw-r--r--   0        0        0      180 2023-07-13 22:29:45.371356 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderModuleAnnotation_test_invalid_provider_module_annotation_not_even_a_class.txt
+-rw-r--r--   0        0        0      350 2023-07-13 22:29:45.483358 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderModuleAnnotation_test_provider_method_cannot_depend_on_another_providers_resource.txt
+-rw-r--r--   0        0        0      486 2023-07-13 22:29:45.491358 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderModuleAnnotation_test_provider_method_cannot_depend_on_parent_providers_resource.txt
+-rw-r--r--   0        0        0      401 2023-07-13 22:29:45.319356 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderResourcesFromResourceInstances_test_provider_fails_on_private_resource_defined_as_another_modules_resource.txt
+-rw-r--r--   0        0        0      316 2023-07-13 22:29:45.491358 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderResourcesFromResourceInstances_test_provider_refuses_module_resource.txt
+-rw-r--r--   0        0        0      172 2023-07-11 02:12:32.137119 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderResourcesFromResourceInstances_test_provider_refuses_overriding_resource_if_name_doesnt_match_module_resource.txt
+-rw-r--r--   0        0        0      290 2023-07-13 22:29:45.475357 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderResourcesFromResourceInstances_test_provider_refuses_private_resource_if_occludes_module_resource.txt
+-rw-r--r--   0        0        0      338 2023-07-13 22:29:45.331356 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderResourcesFromResourceInstances_test_provider_refuses_public_resource_looking_like_an_override.txt
+-rw-r--r--   0        0        0      434 2023-07-13 22:29:45.391357 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderResourcesFromResourceInstances_test_provider_refuses_resource_declaration_that_uses_another_provider_resource.txt
+-rw-r--r--   0        0        0      351 2023-07-13 22:29:45.323356 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderResourcesTypeAliases_test_provider_refuses_overriding_resources_from_type_alias_if_type_not_satisfied.txt
+-rw-r--r--   0        0        0      239 2023-07-13 22:29:45.395357 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderSubclasses_test_provider_attribute_cannot_be_named_module.txt
+-rw-r--r--   0        0        0      242 2023-07-13 22:29:45.335356 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderSubclasses_test_provider_attribute_cannot_be_named_resources.txt
+-rw-r--r--   0        0        0      404 2023-07-13 22:29:45.383356 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderSubclasses_test_provider_subclass_must_provide_for_the_same_module_as_base.txt
+-rw-r--r--   0        0        0      505 2023-07-13 22:29:45.463357 seamful-0.2.0/src/seamful/provider/test_fixtures/test_provider_TestProviderSubclasses_test_provider_subclass_overriding_resource_must_be_subtypes_of_base_providers_resource.txt
+-rw-r--r--   0        0        0    44102 2023-07-13 22:28:44.178645 seamful-0.2.0/src/seamful/provider/test_provider.py
+-rw-r--r--   0        0        0     4822 2023-07-13 22:29:45.411357 seamful-0.2.0/src/seamful/resource/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-22 00:42:30.904082 seamful-0.2.0/src/seamful/resources/__init__.py
+-rw-r--r--   0        0        0       63 2023-03-22 00:42:30.908082 seamful-0.2.0/src/seamful/resources/errors.py
+-rw-r--r--   0        0        0     4501 2023-03-22 22:35:52.779594 seamful-0.2.0/src/seamful/utils_for_tests.py
+-rw-r--r--   0        0        0     7367 1970-01-01 00:00:00.000000 seamful-0.2.0/PKG-INFO
```

### Comparing `seamful-0.1.0/README.md` & `seamful-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -64,17 +64,17 @@
 from seamful import Application
 
 application = Application.empty()
 application.install_module(PaymentsModule, PaymentsProvider)
 application.ready()
 ```
 
-Once a application registered some modules and providers, it can become ready for providing resources. `application.ready()` checks that the module resources can be built by following the dependency graphs of the providers, which usually become more complex than the example above.
+Once a application installed some modules and providers, it can become ready for providing resources. `application.ready()` checks that the module resources can be built by following the dependency graphs of the providers, which usually become more complex than the example above.
 
-The application can be built and registered as a pubilc, global variable in your application. Then, in the entry points of your application you can import that application and ask for any of the registered modules resources. For example:
+The application can be built and configured as a pubilc, global variable in your application. Then, in the entry points of your application you can import that application and ask for any of the registered modules resources. For example:
 
 ```python
 
 from .application import application
 
 class Main:
     def __init__(self):
```

### Comparing `seamful-0.1.0/src/seamful/application/application.py` & `seamful-0.2.0/src/seamful/application/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     modules via `provide()`
     Although install/ready/provide is the main workflow of an Application, the value of this
     class (and seamful itself) is the ability to change specific resources with alternative versions
     when testing or running the program in an alternative environment. This is done via `tamper()`
     which is meant to be used solely on these alternative setups (typically in `TestCase.setUp()`)
 
     The methods of an Application have rather strict rules on when they can be called. This is
-    because an Appplicatio is really two different things bundled together:
+    because an Application is really two different things bundled together:
 
      - A registry for modules and providers.
      - A factory for those module resources.
 
     The reason they're bundled under the same class is subtle. With a few cases, it should become
     clearer why this is.
     """
@@ -65,67 +65,65 @@
         For the module to be able to provide resources, the application needs to know which is its
         provider.
 
         The application determines a module's provider through the following rules:
 
         1. If `install_module()` was called with a module _and_ a provider, it uses that one.
         2. If instead the provider was set through `install_provider()`, it uses that one.
-        3. If the provider was not explicitly registered, but it has a default provider
+        3. If the provider was not explicitly installed, but it has a default provider
         (Module.default_provider), it uses that one.
 
-        A module can only be registered once. There's no need to install a module that will not be
+        A module can only be installed once. There's no need to install a module that will not be
         explicitly provided by `provide()`.
 
         The api is rather strict in that it disallows registering modules or providers multiple
         times.
         The intent is to make it very hard to make complex setups.
-        There should be one simple set of modules registered for an application, and a subset of
+        There should be one simple set of modules installed for an application, and a subset of
         those modules having special providers for running in non production scenarios, such as
         testing or local development.
 
         """
         if not self._is_registering:
             raise CantInstallWhenReadyToProvide(module)
         self._registry.register_module(module)
         if provider is not None:
             if provider.module is not module:
                 raise ProviderModuleMismatch(provider, module)
             self._registry.register_provider(
                 provider,
                 allow_override=self._allow_overrides,
-                allow_implicit_module=False,
             )
 
     def install_provider(self, provider: ProviderType) -> None:
         """Instruct the application to use the given provider.
 
-        In most cases, modules are registered alongside their providers via
+        In most cases, modules are installed alongside their providers via
         `install_module(module, provider)`
 
         The two main scenarios where `install_provider()` is useful are:
 
-        - A module was registered through `install_module()` without setting its provider, and it
+        - A module was installed through `install_module()` without setting its provider, and it
         doesn't have a default provider (or it's not appropriate for the given application).
 
-        - A module has a provider already registered, but during tests or other alternative
+        - A module has a provider already installed, but during tests or other alternative
         scenarios, the application is `tamper()`ed to override some of those providers.
 
         See `tamper()` for a more subtle third use case.
 
         """
         if not self._is_registering:
             raise CantInstallWhenReadyToProvide(provider)
         self._registry.register_provider(
             provider,
             allow_override=self._allow_overrides,
-            allow_implicit_module=self._allow_implicit_modules,
         )
 
     def ready(self, allow_provider_resources: bool = False) -> None:
-        """Make the application ready to provide resources for the registered modules.
+        """Make the application ready to provide resources for the installed modules.
 
         Calling `ready()` transitions the application from being registering modules to
         being available to provide resources.
 
         For an application to be ready, all the modules in use must have a provider, either
         their default providers or those manually set. Any used module without a provider will
         make `ready()` to fail with a descriptive message. This happens even if later no resource
@@ -165,15 +163,15 @@
 
         `application.provide(SomeModule.a)` will return an instance of `SomeClass`, built by
         `SomeProvider`.
 
         An application builds resources at most once, meaning that two separate calls to
         `provide()` for the same resource will yield the same object.
 
-        The resource's Module must have been registered explicitly via `install_module()`.
+        The resource's Module must have been installed explicitly via `install_module()`.
         Otherwise, it'll raise an error.
         """
         if self._is_registering:
             raise CannotProvideUntilApplicationIsReady()
         if not self._is_providing:
             self._is_providing = True
             self._registry = None  # type: ignore
@@ -185,15 +183,14 @@
         else:
             raise NotImplementedError()
 
     def tamper(
         self,
         *,
         allow_overrides: bool = False,
-        allow_implicit_modules: bool = False,
     ) -> None:
         """Tamper with a ready application. Useful for changing providers when testing.
 
         An application is typically set up in two phases:
         - Register modules and providers
         - Provide module resources.
 
@@ -203,39 +200,36 @@
         development), `tamper()`'ing with a ready application allows some providers to be changed
         with alternative ones.
         In essence, `tamper()` puts an application back into installing mode with slight changes
         in its behavior:
 
         - An explicitly set provider can be overriden by using install_provider() when
         allow_overrides=True. (Default providers can always be overriden when tampering.)
-        - A provider can be set for a non explicitly registered module when
-        allow_implicit_modules=True
 
         After tampering with an application, calling `ready()` again is needed for it to be
         ready for providing resources.
 
         Note that an application cannot be tampered many times in sequence. Once tampered (and
-        possibly having used module reources), an application can go back to it's original state
+        possibly having used module resources), an application can go back to its original state
         via restore().
         """
         if self._is_providing:
             raise CannotTamperAfterHavingProvidedResources(self)
         if self._is_registering:
             raise CannotTamperUntilApplicationIsReady(self)
         if self._checkpoint is not None:
             raise CannotTamperWithApplicationTwice(self)
         self._checkpoint = (self._registry, cast(ModuleGraphProvider, self._provider))
         self._registry = self._registry.copy()
         self._provider = None
         self._is_registering = True
         self._allow_overrides = allow_overrides
-        self._allow_implicit_modules = allow_implicit_modules
 
     def restore(self) -> None:
-        """Restores the state of an application that was tampered with to it's previous state.
+        """Restores the state of an application that was tampered with to its previous state.
 
         This effectively undoes all the module and provider registrations and overrides that
         happened after calling tamper().
 
         Once restored, the application is ready to provide resources.
         """
         if self._checkpoint is None:
```

### Comparing `seamful-0.1.0/src/seamful/application/errors.py` & `seamful-0.2.0/src/seamful/application/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,53 +8,53 @@
 from seamful.resource import ModuleResource, ProviderResource, BoundResource
 from seamful.provider.provider_type import ProviderType, ProviderMethod
 
 if TYPE_CHECKING:
     from seamful.application import Application
 
 
-class ModuleNotRegisteredForResource(HelpfulException):
+class ModuleNotInstalledForResource(HelpfulException):
     def __init__(
         self,
         resource: BoundResource[Any],
-        registered_modules: set[ModuleType],
+        installed_modules: set[ModuleType],
         known_modules: set[ModuleType],
     ):
         self.resource = resource
-        self.registered_modules = registered_modules
+        self.installed_modules = installed_modules
         self.known_modules = known_modules
 
     def explanation(self) -> str:
         t = Text("Attempted to provide for resource:")
         t.indented_line(rdef(self.resource))
-        t.newline("Which doesn't belong to any registered module. Registered modules are:")
+        t.newline("Which doesn't belong to any installed module. Installed modules are:")
         with t.indented_block(blank_before=False):
-            for module in self.registered_modules:
+            for module in self.installed_modules:
                 t.newline(f"- {sname(module)}")
         return str(t)
 
     def failsafe_explanation(self) -> str:
-        return "Attempted to provide for resource that does not belong to any registered module."
+        return "Attempted to provide for resource that does not belong to any installed module."
 
 
-class ModuleAlreadyRegistered(HelpfulException):
-    def __init__(self, module: ModuleType, registered_modules: set[ModuleType]):
+class ModuleAlreadyInstalled(HelpfulException):
+    def __init__(self, module: ModuleType, instaled_modules: set[ModuleType]):
         self.module = module
-        self.registered_modules = registered_modules
+        self.installed_modules = instaled_modules
 
     def explanation(self) -> str:
         t = Text(f"Attempted to install module {qname(self.module)}")
-        t.sentence("which is already registered. Registered modules are:")
+        t.sentence("which is already installed. Installed modules are:")
         with t.indented_block(blank_before=False):
-            for module in self.registered_modules:
+            for module in self.installed_modules:
                 t.newline(f"- {sname(module)}")
         return str(t)
 
     def failsafe_explanation(self) -> str:
-        return "Attempted to install module that is already registered."
+        return "Attempted to install module that is already installed."
 
 
 class ProviderModuleMismatch(HelpfulException):
     def __init__(self, provider: ProviderType, module: ModuleType):
         self.provider = provider
         self.module = module
 
@@ -72,94 +72,57 @@
     def failsafe_explanation(self) -> str:
         return (
             "Attempted to install a provider alongside a module, "
             "but the provider provides for a different module."
         )
 
 
-class CannotRegisterProviderToNotRegisteredModule(HelpfulException):
-    def __init__(self, provider: ProviderType, registered_modules: set[ModuleType]):
-        self.provider = provider
-        self.registered_modules = registered_modules
+class CannotOverrideInstalledProvider(HelpfulException):
+    def __init__(self, module: ModuleType, *, installed: ProviderType, registering: ProviderType):
+        self.module = module
+        self.installed = installed
+        self.registering = registering
 
     def explanation(self) -> str:
-        t = Text(f"Attempted to install provider {qname(self.provider)}")
+        t = Text(f"Attempted to install provider {qname(self.registering)}")
         t.sentence(
-            f"which provides for {qname(self.provider.module)}, "
-            f"which is not registered. Registered modules are:"
+            f"which provides for {qname(self.module)}, "
+            f"but {qname(self.installed)} was already installed as its provider."
         )
-        with t.indented_block(blank_before=False):
-            for module in self.registered_modules:
-                t.newline(f"- {sname(module)}")
+
+        t.blank()
+
         t.newline(
-            "Registering providers for implicit modules is only meant to be used for "
-            "testing and secondary scenarios, and can be enabled by tampering with the application:"
+            "Overriding providers is not allowed. You can enable overriding a provider "
+            "after the application is ready tampering with it:"
         )
-        t.indented_line("application.tamper(allow_implicit_modules=True)")
+        t.indented_line("application.tamper(allow_overrides=True)")
         t.blank()
         t.newline(
-            "If instead, the application is expected to provide resources for "
-            f"{qname(self.provider.module)}, you can register both at once by calling:"
+            "Keep in mind that overriding providers is mostly meant for testing "
+            "and alternative running scenarios."
         )
-        t.indented_line(
-            f"application.register({sname(self.provider.module)}, provider={sname(self.provider)})"
-        )
-        return str(t)
-
-    def failsafe_explanation(self) -> str:
-        return "Attempted to install a provider for a module that is not registered."
-
-
-class CannotOverrideRegisteredProvider(HelpfulException):
-    def __init__(self, module: ModuleType, *, registered: ProviderType, registering: ProviderType):
-        self.module = module
-        self.registered = registered
-        self.registering = registering
-
-    def explanation(self) -> str:
-        t = Text(f"Attempted to install provider {qname(self.registering)}")
-        if self.registered is self.registering:
-            t.sentence("which is already registered.")
-        else:
-            t.sentence(
-                f"which provides for {qname(self.module)}, "
-                f"but {qname(self.registered)} was already registered as its provider."
-            )
-
-            t.blank()
-
-            t.newline(
-                "Overriding providers is not allowed. You can enable overriding a provider "
-                "after the application is ready tampering with it:"
-            )
-            t.indented_line("application.tamper(allow_overrides=True)")
-            t.blank()
-            t.newline(
-                "Keep in mind that overriding providers is mostly meant for testing "
-                "and alternative running scenarios."
-            )
         return str(t)
 
     def failsafe_explanation(self) -> str:
         return (
-            "Attempted to install a provider for a module that already "
-            "has a registered provider."
+            "Attempted to install a provider for a module that already " "has a installed provider."
         )
 
 
-class ModuleWithoutRegisteredOrDefaultProvider(HelpfulException):
+class ModuleWithoutInstalledOrDefaultProvider(HelpfulException):
     def __init__(self, module: ModuleType):
         self.module = module
 
     def explanation(self) -> str:
-        t = Text(f"Module {qname(self.module)} has no registered or default provider.")
+        t = Text(f"Module {qname(self.module)} has no installed or default provider.")
         return str(t)
 
     def failsafe_explanation(self) -> str:
-        return "A registered module has no registered or default provider."
+        return "A installed module has no installed or default provider."
 
 
 class CannotProvideUntilApplicationIsReady(HelpfulException):
     def explanation(self) -> str:
         t = Text(
             "Attempted to provide a resource before application is ready for providing. "
             "You can make the application ready by calling:"
@@ -342,59 +305,59 @@
         t.newline("A application can only be tampered with before it has provided any resources.")
         return str(t)
 
     def failsafe_explanation(self) -> str:
         return "Attempted tamper with a application, but it has already provided resources."
 
 
-class RegisteredProvidersNotUsed(HelpfulException):
+class InstalledProvidersNotUsed(HelpfulException):
     def __init__(self, providers: set[ProviderType]):
         self.providers = providers
 
     def explanation(self) -> str:
-        t = Text("The following providers were registered, but not used:")
+        t = Text("The following providers were installed, but not used:")
         with t.indented_block():
             for provider in self.providers:
                 t.newline(f"- {point_to_definition(provider)}")
 
         t.newline(
-            "Those providers were explicitly registered, "
+            "Those providers were explicitly installed, "
             "but the modules they provide for were not, "
             "and those modules are also not part "
             "of the dependency graph of any other used provider"
         )
         return str(t)
 
     def failsafe_explanation(self) -> str:
-        return "Some registered providers were not used."
+        return "Some installed providers were not used."
 
 
-class ProviderResourceOfUnregisteredProvider(HelpfulException):
+class ProviderResourceOfNotInstalledProvider(HelpfulException):
     def __init__(self, resource: ProviderResource[Any], provider_in_use: ProviderType):
         self.resource = resource
         self.provider_in_use = provider_in_use
 
     def explanation(self) -> str:
         provider = self.resource.provider
         t = Text(
             f"Requested to provide {rname(self.resource)}, "
-            f"but {qname(provider)} was not registered."
+            f"but {qname(provider)} was not installed."
         )
 
         t.blank()
         t.newline(f"{qname(provider)} provides for {qname(provider.module)},")
         t.sentence(f"but that module is being provided by {qname(self.provider_in_use)}.")
         t.blank()
         t.newline(point_to_definition(provider))
         t.newline(point_to_definition(provider.module))
         t.newline(point_to_definition(self.provider_in_use))
         return str(t)
 
     def failsafe_explanation(self) -> str:
-        return "Requested to provide a resource of an unregistered provider."
+        return "Requested to provide a resource of a non installed provider."
 
 
 class CannotTamperWithApplicationTwice(HelpfulException):
     def __init__(self, application: Application):
         self.application = application
 
     def explanation(self) -> str:
```

### Comparing `seamful-0.1.0/src/seamful/application/graph_provider.py` & `seamful-0.2.0/src/seamful/application/graph_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, cast, TypeVar, Set, Dict
 
 from seamful.application.errors import (
-    ModuleNotRegisteredForResource,
+    ModuleNotInstalledForResource,
     InvalidProviderInstanceAccess,
     ProviderMethodsCantAccessProviderInstance,
-    ProviderResourceOfUnregisteredProvider,
+    ProviderResourceOfNotInstalledProvider,
 )
 from seamful.module.module_type import ModuleType
 from seamful.provider.provider_type import ProviderType
 from seamful.resource import (
     ModuleResource,
     OverridingResource,
     ProviderResource,
@@ -22,44 +22,44 @@
     def __init__(self, resource: ProviderResource[Any]):
         self.resource = resource
 
 
 class ModuleGraphProvider:
     def __init__(
         self,
-        registered_modules: Set[ModuleType],
+        installed_modules: Set[ModuleType],
         providers_by_module: Dict[ModuleType, ProviderType],
         allow_provider_resources: bool,
     ):
-        self._registered_modules = registered_modules
+        self._installed_modules = installed_modules
         self._providers = providers_by_module
         self._instances_by_resource: Dict[BoundResource[Any], Any] = {}
         self._fake_provider_instance = UnusableProviderInstance()
         self._allow_provider_resources = allow_provider_resources
 
     def provide(self, resource: BoundResource[T]) -> T:
         self._ensure_known_module(resource)
         if isinstance(resource, ModuleResource):
             return self._provide(cast(ModuleResource[T], resource))
         elif isinstance(resource, ProviderResource):
             if not self._allow_provider_resources:
                 raise ProviderResourcesNotAllowed(resource)
             if resource.provider is not self._providers[resource.provider.module]:
-                raise ProviderResourceOfUnregisteredProvider(
+                raise ProviderResourceOfNotInstalledProvider(
                     resource, self._providers[resource.provider.module]
                 )
             return self._provide(cast(ProviderResource[T], resource))
         else:
             raise TypeError()
 
     def _ensure_known_module(self, resource: BoundResource[Any]) -> None:
-        if resource.module not in self._registered_modules:
-            raise ModuleNotRegisteredForResource(
+        if resource.module not in self._installed_modules:
+            raise ModuleNotInstalledForResource(
                 resource,
-                self._registered_modules,
+                self._installed_modules,
                 set(self._providers.keys()),
             )
 
     def _provide(self, resource: BoundResource[T]) -> T:
         if resource in self._instances_by_resource:
             return cast(T, self._instances_by_resource[resource])
         if isinstance(resource, OverridingResource):
```

### Comparing `seamful-0.1.0/src/seamful/application/graph_solver.py` & `seamful-0.2.0/src/seamful/application/graph_solver.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Optional, cast, Dict, Set, List
 
 from seamful.application.errors import (
-    ModuleWithoutRegisteredOrDefaultProvider,
+    ModuleWithoutInstalledOrDefaultProvider,
     CircularDependency,
     ResolutionStep,
-    RegisteredProvidersNotUsed,
+    InstalledProvidersNotUsed,
 )
 from seamful.application.graph_provider import ModuleGraphProvider
 from seamful.module.module_type import ModuleType
 from seamful.provider.provider_type import ProviderType
 from seamful.resource import (
     ModuleResource,
     PrivateResource,
@@ -16,57 +16,57 @@
     BoundResource,
 )
 
 
 class ModuleGraphSolver:
     def __init__(
         self,
-        registered_modules: Set[ModuleType],
-        registered_providers: Dict[ModuleType, ProviderType],
+        installed_modules: Set[ModuleType],
+        installed_providers: Dict[ModuleType, ProviderType],
     ):
-        self._registered_modules = registered_modules
+        self._installed_modules = installed_modules
 
         self._providers_by_module: Dict[ModuleType, ProviderType] = {}
-        self._needed_modules_without_providers: Set[ModuleType] = registered_modules.copy()
-        self._unused_providers_by_module = registered_providers.copy()
+        self._needed_modules_without_providers: Set[ModuleType] = installed_modules.copy()
+        self._unused_providers_by_module = installed_providers.copy()
 
     def solve(self, allow_provider_resources: bool) -> ModuleGraphProvider:
         while len(self._needed_modules_without_providers) > 0:
             for module in self._needed_modules_without_providers.copy():
                 provider = self._install_provider_for_module(module)
                 self._providers_by_module[module] = provider
                 self._needed_modules_without_providers.remove(module)
                 self._add_modules_needed_by_provider(provider)
 
         self._fail_on_circular_dependencies()
         self._fail_on_unused_implicit_modules()
         return ModuleGraphProvider(
-            self._registered_modules,
+            self._installed_modules,
             self._providers_by_module,
             allow_provider_resources,
         )
 
     def _install_provider_for_module(self, module: ModuleType) -> ProviderType:
         if module in self._unused_providers_by_module:
             return self._unused_providers_by_module.pop(module)
         elif module.default_provider is not None:
             return module.default_provider
         else:
-            raise ModuleWithoutRegisteredOrDefaultProvider(module)
+            raise ModuleWithoutInstalledOrDefaultProvider(module)
 
     def _add_modules_needed_by_provider(self, provider: ProviderType) -> None:
         for provider_method in provider:
             for parameter_name, dependency in provider_method.dependencies:
                 if dependency.module not in self._providers_by_module:
                     self._needed_modules_without_providers.add(dependency.module)
 
     def _fail_on_circular_dependencies(self) -> None:
         solved: set[BoundResource[Any]] = set()
         loops: list[list[ResolutionStep]] = []
-        for module in self._registered_modules:
+        for module in self._installed_modules:
             for resource in module:
                 stack: set[BoundResource[Any]] = set()
                 loop = self._find_circular_dependency(resource, in_stack=stack, solved=solved)
                 if loop is not None:
                     loops.append(loop)
         if len(loops) > 0:
             raise CircularDependency(loops)
@@ -104,8 +104,8 @@
         elif isinstance(resource, ModuleResource):
             return self._providers_by_module[resource.module]
         else:
             raise TypeError()
 
     def _fail_on_unused_implicit_modules(self) -> None:
         if len(self._unused_providers_by_module) > 0:
-            raise RegisteredProvidersNotUsed(set(self._unused_providers_by_module.values()))
+            raise InstalledProvidersNotUsed(set(self._unused_providers_by_module.values()))
```

### Comparing `seamful-0.1.0/src/seamful/application/registry.py` & `seamful-0.2.0/src/seamful/application/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 from typing import TypeVar
 
 from seamful.application.errors import (
-    ModuleAlreadyRegistered,
-    CannotRegisterProviderToNotRegisteredModule,
-    CannotOverrideRegisteredProvider,
+    ModuleAlreadyInstalled,
+    CannotOverrideInstalledProvider,
 )
 from seamful.application.graph_provider import ModuleGraphProvider
 from seamful.application.graph_solver import ModuleGraphSolver
 from seamful.module.module_type import ModuleType
 from seamful.provider.provider_type import ProviderType
 
 T = TypeVar("T")
@@ -19,28 +18,26 @@
         self, explicit_modules: set[ModuleType], explicit_providers: dict[ModuleType, ProviderType]
     ) -> None:
         self._explicit_modules = explicit_modules
         self._explicit_providers = explicit_providers
 
     def register_module(self, module: ModuleType) -> None:
         if module in self._explicit_modules:
-            raise ModuleAlreadyRegistered(module, self._explicit_modules)
+            raise ModuleAlreadyInstalled(module, self._explicit_modules)
 
         self._explicit_modules.add(module)
 
-    def register_provider(
-        self, provider: ProviderType, allow_override: bool, allow_implicit_module: bool
-    ) -> None:
+    def register_provider(self, provider: ProviderType, allow_override: bool) -> None:
         module = provider.module
-        if module not in self._explicit_modules and not allow_implicit_module:
-            raise CannotRegisterProviderToNotRegisteredModule(provider, self._explicit_modules)
-        if module in self._explicit_providers and not allow_override:
-            raise CannotOverrideRegisteredProvider(
+        installed_provider = self._explicit_providers.get(module)
+        is_overriding = installed_provider is not None and installed_provider is not provider
+        if is_overriding and not allow_override:
+            raise CannotOverrideInstalledProvider(
                 module,
-                registered=self._explicit_providers[module],
+                installed=self._explicit_providers[module],
                 registering=provider,
             )
         self._explicit_providers[module] = provider
 
     def solve_graph(self, allow_provider_resources: bool) -> ModuleGraphProvider:
         return ModuleGraphSolver(self._explicit_modules, self._explicit_providers).solve(
             allow_provider_resources
```

### Comparing `seamful-0.1.0/src/seamful/application/test_container.py` & `seamful-0.2.0/src/seamful/application/test_application.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
+import sys
 from typing import Sequence, Type, cast, TypeVar, List
+from unittest import skipIf
 
 from seamful.errors import HelpfulException
 from seamful.module import Module
 from seamful.application import Application
 from seamful.application.errors import (
-    ModuleNotRegisteredForResource,
-    ModuleAlreadyRegistered,
+    ModuleNotInstalledForResource,
+    ModuleAlreadyInstalled,
     ProviderModuleMismatch,
-    CannotRegisterProviderToNotRegisteredModule,
-    CannotOverrideRegisteredProvider,
-    ModuleWithoutRegisteredOrDefaultProvider,
+    CannotOverrideInstalledProvider,
+    ModuleWithoutInstalledOrDefaultProvider,
     CannotProvideUntilApplicationIsReady,
     CantInstallWhenReadyToProvide,
     CannotProvideRawType,
     CircularDependency,
     ResolutionStep,
     ProviderMethodsCantAccessProviderInstance,
     CannotTamperAfterHavingProvidedResources,
-    RegisteredProvidersNotUsed,
+    InstalledProvidersNotUsed,
     CannotTamperUntilApplicationIsReady,
     ApplicationAlreadyReady,
-    ProviderResourceOfUnregisteredProvider,
+    ProviderResourceOfNotInstalledProvider,
     CannotTamperWithApplicationTwice,
     ApplicationWasNotTamperedWith,
 )
 from seamful.provider.provider_type import Provider, ProviderType, ProviderMethod
 from seamful.resource import Resource, ModuleResource
 from seamful.utils_for_tests import (
     validate_output,
@@ -106,19 +107,19 @@
 
         class AnotherModule(Module):
             a = int
 
         application = Application.empty()
         application.install_module(SomeModule, SomeProvider)
         application.ready()
-        with self.assertRaises(ModuleNotRegisteredForResource) as ctx:
+        with self.assertRaises(ModuleNotInstalledForResource) as ctx:
             application.provide(AnotherModule.a)
 
         self.assertEqual(ctx.exception.resource, AnotherModule.a)
-        self.assertEqual(ctx.exception.registered_modules, {SomeModule})
+        self.assertEqual(ctx.exception.installed_modules, {SomeModule})
         self.assertEqual(ctx.exception.known_modules, {SomeModule})
         return ctx.exception
 
     @validate_output
     def test_application_refuses_to_provide_before_registrations_are_closed(
         self,
     ) -> HelpfulException:
@@ -163,15 +164,15 @@
             def provide_b(self) -> int:
                 return 11
 
         application = Application()
         application.install_module(SomeModule, SomeProvider)
         application.ready(allow_provider_resources=True)
 
-        with self.assertRaises(ProviderResourceOfUnregisteredProvider) as ctx:
+        with self.assertRaises(ProviderResourceOfNotInstalledProvider) as ctx:
             application.provide(AnotherProvider.b)
         self.assertEqual(ctx.exception.resource.provider, AnotherProvider)
         self.assertEqual(ctx.exception.provider_in_use, SomeProvider)
         return ctx.exception
 
 
 class TestApplicationProvidesPrivateResources(TestCaseWithOutputFixtures):
@@ -401,18 +402,18 @@
 
         class SomeProvider(Provider, module=SomeModule):
             def provide_a(self) -> int:
                 return 10
 
         application = Application.empty()
         application.install_module(SomeModule, SomeProvider)
-        with self.assertRaises(ModuleAlreadyRegistered) as ctx:
+        with self.assertRaises(ModuleAlreadyInstalled) as ctx:
             application.install_module(SomeModule, SomeProvider)
         self.assertEqual(ctx.exception.module, SomeModule)
-        self.assertEqual(ctx.exception.registered_modules, {SomeModule})
+        self.assertEqual(ctx.exception.installed_modules, {SomeModule})
         return ctx.exception
 
     @validate_output
     def test_application_install_provider_must_provide_for_module(self) -> HelpfulException:
         class SomeModule(Module):
             a = int
 
@@ -456,41 +457,23 @@
             pass
 
         class AnotherProvider(Provider, module=SomeModule):
             pass
 
         application = Application.empty()
         application.install_module(SomeModule, SomeProvider)
-        with self.assertRaises(CannotOverrideRegisteredProvider) as ctx:
+        with self.assertRaises(CannotOverrideInstalledProvider) as ctx:
             application.install_provider(AnotherProvider)
 
         self.assertEqual(ctx.exception.module, SomeModule)
-        self.assertEqual(ctx.exception.registered, SomeProvider)
+        self.assertEqual(ctx.exception.installed, SomeProvider)
         self.assertEqual(ctx.exception.registering, AnotherProvider)
         return ctx.exception
 
     @validate_output
-    def test_cannot_install_same_provider_twice(self) -> HelpfulException:
-        class SomeModule(Module):
-            pass
-
-        class SomeProvider(Provider, module=SomeModule):
-            pass
-
-        application = Application.empty()
-        application.install_module(SomeModule, SomeProvider)
-        with self.assertRaises(CannotOverrideRegisteredProvider) as ctx:
-            application.install_provider(SomeProvider)
-
-        self.assertEqual(ctx.exception.module, SomeModule)
-        self.assertEqual(ctx.exception.registered, SomeProvider)
-        self.assertEqual(ctx.exception.registering, SomeProvider)
-        return ctx.exception
-
-    @validate_output
     def test_cant_install_module_after_ready(self) -> HelpfulException:
         class SomeModule(Module):
             pass
 
         application = Application.empty()
         application.ready()
         with self.assertRaises(CantInstallWhenReadyToProvide) as ctx:
@@ -621,18 +604,18 @@
         application.ready()
         application.tamper()
 
         class AnotherProvider(Provider, module=SomeModule):
             def provide_a(self) -> int:
                 return 11
 
-        with self.assertRaises(CannotOverrideRegisteredProvider) as ctx:
+        with self.assertRaises(CannotOverrideInstalledProvider) as ctx:
             application.install_provider(AnotherProvider)
 
-        self.assertEqual(ctx.exception.registered, SomeProvider)
+        self.assertEqual(ctx.exception.installed, SomeProvider)
         self.assertEqual(ctx.exception.module, SomeModule)
         self.assertEqual(ctx.exception.registering, AnotherProvider)
         return ctx.exception
 
     @validate_output
     def test_application_cannot_be_tampered_twice(self) -> HelpfulException:
         application = Application.empty()
@@ -737,15 +720,23 @@
             application.restore()
         self.assertEqual(ctx.exception.application, application)
         return ctx.exception
 
 
 class TestApplicationImplicitProviders(TestCaseWithOutputFixtures):
     @validate_output
-    def test_cant_install_implicit_provider(self) -> HelpfulException:
+    def test_can_install_private_provider_if_module_is_used(self) -> HelpfulException:
+        """An application that doesn't install a module may transitively depend on it.
+
+        In those cases, one should be able to install a provider for that module without
+        installing the module. This results on the resources of the module being available
+        for the provider that depends on it, but application.provide() will refuse to
+        provide that resource.
+        """
+
         class SomeModule(Module):
             a = Resource(int)
 
         class AnotherModule(Module):
             b = Resource(int)
 
         class SomeProvider(Provider, module=SomeModule):
@@ -754,19 +745,104 @@
 
         class AnotherProvider(Provider, module=AnotherModule):
             def provide_b(self) -> int:
                 return 10
 
         application = Application.empty()
         application.install_module(SomeModule, SomeProvider)
-        with self.assertRaises(CannotRegisterProviderToNotRegisteredModule) as ctx:
-            application.install_provider(AnotherProvider)
+        application.install_provider(AnotherProvider)
+        application.ready()
+
+        self.assertEqual(application.provide(SomeModule.a), 11)
+
+        with self.assertRaises(ModuleNotInstalledForResource) as ctx:
+            application.provide(AnotherModule.b)
+        return ctx.exception
+
+    @skipIf(sys.version_info < (3, 10), "Type aliases are not supported")
+    def test_can_install_private_provider_twice(self) -> None:
+        """Private provider installs can happen in different, isolated places, thus repeated.
+
+        A common use case is to have a library or third party module that has an "install_x"
+        function that installs the providers for the exposed modules, so one can depend on those
+        modules. Different libraries may depend on a common one that itself exposes an install_x
+        function, that would be called more than once when setting up each of the depending
+        libraries. It makes sense to allow each library to provide its self-contained setup
+        and not raise an error when the same provider is registered more than once, as long as
+        it's used by any of the installed modules.
+        """
+
+        from typing import TypeAlias
+
+        class CoreModule(Module):
+            a: TypeAlias = int
+
+        class CoreProvider(Provider, module=CoreModule):
+            def provide_a(self) -> int:
+                return 10
+
+        def use_core(app: Application) -> None:
+            app.install_provider(CoreProvider)
+
+        class SomeLibraryModule(Module):
+            b: TypeAlias = int
+
+        class SomeLibraryProvider(Provider, module=SomeLibraryModule):
+            def provide_b(self, base: CoreModule.a) -> int:
+                return base + 1
+
+        def use_some_library(app: Application) -> None:
+            app.install_provider(SomeLibraryProvider)
+            use_core(app)
+
+        class AnotherLibraryModule(Module):
+            c: TypeAlias = int
+
+        class AnotherLibraryProvider(Provider, module=AnotherLibraryModule):
+            def provide_c(self, base: CoreModule.a) -> int:
+                return base + 2
+
+        def use_another_library(app: Application) -> None:
+            app.install_provider(AnotherLibraryProvider)
+            use_core(app)
+
+        class AppModule(Module):
+            d: TypeAlias = int
+
+        class AppProvider(Provider, module=AppModule):
+            def provide_d(self, some: SomeLibraryModule.b, another: AnotherLibraryModule.c) -> int:
+                return some + another + 1
+
+        app = Application.empty()
+        app.install_module(AppModule, AppProvider)
+        use_some_library(app)
+        use_another_library(app)
+        app.ready()
+        self.assertEqual(app.provide(AppModule.d), 24)
+
+    @validate_output
+    def test_cant_install_private_provider_if_module_is_not_used(self) -> HelpfulException:
+        """When installing a provider without its module must transitively depend on the module.
+
+        An application may install a provider for a non installed module, but the application will
+        refuse to become ready unless the module is transitively used by another provider.
+        """
+
+        class SomeModule(Module):
+            a = Resource(int)
+
+        class SomeProvider(Provider, module=SomeModule):
+            def provide_a(self) -> int:
+                return 10
+
+        app = Application.empty()
+        app.install_provider(SomeProvider)
+        with self.assertRaises(InstalledProvidersNotUsed) as ctx:
+            app.ready()
 
-        self.assertEqual(ctx.exception.provider, AnotherProvider)
-        self.assertEqual(ctx.exception.registered_modules, {SomeModule})
         return ctx.exception
 
     def test_can_install_implicit_provider_if_reopened_explicitly_and_module_is_used(
         self,
     ) -> None:
         class Module1(Module):
             a = Resource(int)
@@ -787,15 +863,15 @@
         class AnotherProvider2(Provider, module=Module2):
             def provide_b(self) -> int:
                 return 11
 
         application = Application.empty()
         application.install_module(Module1, Provider1)
         application.ready()
-        application.tamper(allow_overrides=True, allow_implicit_modules=True)
+        application.tamper(allow_overrides=True)
         application.install_provider(AnotherProvider2)
         application.ready()
         self.assertEqual(application.provide(Module1.a), 12)
 
     @validate_output
     def test_application_fails_on_closing_registration_if_any_implicit_provider_is_unused(
         self,
@@ -805,31 +881,31 @@
 
         class SomeProvider(Provider, module=SomeModule):
             def provide_a(self) -> int:
                 return 10
 
         application = Application.empty()
         application.ready()
-        application.tamper(allow_overrides=True, allow_implicit_modules=True)
+        application.tamper(allow_overrides=True)
         application.install_provider(SomeProvider)
-        with self.assertRaises(RegisteredProvidersNotUsed) as ctx:
+        with self.assertRaises(InstalledProvidersNotUsed) as ctx:
             application.ready()
         self.assertEqual(ctx.exception.providers, {SomeProvider})
         return ctx.exception
 
 
 class TestDefaultProvider(TestCaseWithOutputFixtures):
     @validate_output
     def test_application_cant_seal_if_a_module_lacks_a_provider(self) -> HelpfulException:
         class SomeModule(Module):
             pass
 
         application = Application.empty()
         application.install_module(SomeModule)
-        with self.assertRaises(ModuleWithoutRegisteredOrDefaultProvider) as ctx:
+        with self.assertRaises(ModuleWithoutInstalledOrDefaultProvider) as ctx:
             application.ready()
 
         self.assertEqual(ctx.exception.module, SomeModule)
         return ctx.exception
 
     def test_application_uses_default_provider_if_none_installed(self) -> None:
         class SomeModule(Module):
```

### Comparing `seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_catches_circular_dependencies_involving_overriding_resources.txt` & `seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_catches_circular_dependencies_involving_overriding_resources.txt`

 * *Files identical despite different names*

### Comparing `seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_catches_inner_circular_dependency.txt` & `seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_catches_inner_circular_dependency.txt`

 * *Files identical despite different names*

### Comparing `seamful-0.1.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_many_providers_circular_dependency_breaks_on_seal.txt` & `seamful-0.2.0/src/seamful/application/test_fixtures/test_container_TestCircularDependencies_test_many_providers_circular_dependency_breaks_on_seal.txt`

 * *Files identical despite different names*

### Comparing `seamful-0.1.0/src/seamful/errors.py` & `seamful-0.2.0/src/seamful/errors.py`

 * *Files identical despite different names*

### Comparing `seamful-0.1.0/src/seamful/module/errors.py` & `seamful-0.2.0/src/seamful/module/errors.py`

 * *Files identical despite different names*

### Comparing `seamful-0.1.0/src/seamful/module/module_type.py` & `seamful-0.2.0/src/seamful/module/module_type.py`

 * *Files identical despite different names*

### Comparing `seamful-0.1.0/src/seamful/module/test_module.py` & `seamful-0.2.0/src/seamful/module/test_module.py`

 * *Files identical despite different names*

### Comparing `seamful-0.1.0/src/seamful/provider/errors.py` & `seamful-0.2.0/src/seamful/provider/errors.py`

 * *Files identical despite different names*

### Comparing `seamful-0.1.0/src/seamful/provider/provider_type.py` & `seamful-0.2.0/src/seamful/provider/provider_type.py`

 * *Files identical despite different names*

### Comparing `seamful-0.1.0/src/seamful/provider/test_provider.py` & `seamful-0.2.0/src/seamful/provider/test_provider.py`

 * *Files identical despite different names*

### Comparing `seamful-0.1.0/src/seamful/resource/__init__.py` & `seamful-0.2.0/src/seamful/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `seamful-0.1.0/src/seamful/utils_for_tests.py` & `seamful-0.2.0/src/seamful/utils_for_tests.py`

 * *Files identical despite different names*

### Comparing `seamful-0.1.0/PKG-INFO` & `seamful-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: seamful
-Version: 0.1.0
+Version: 0.2.0
 Summary: Dependency management for python
+Home-page: https://github.com/rdarder/seamful
 License: MIT
 Author: Rafael Darder
 Author-email: darder@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/rdarder/seamful
 Description-Content-Type: text/markdown
 
 Seamful is a dependency injection library for Python.
 
 It aims to facilitate writing integration tests that replace the minimum amount of dependencies with test doubles. It incentivizes using _working_ test doubles as opposed inspectable mocks.
 
 Seamful intervenes by instantiating the objects and their dependencies. While typically one would manually instantiate these:
@@ -81,17 +83,17 @@
 from seamful import Application
 
 application = Application.empty()
 application.install_module(PaymentsModule, PaymentsProvider)
 application.ready()
 ```
 
-Once a application registered some modules and providers, it can become ready for providing resources. `application.ready()` checks that the module resources can be built by following the dependency graphs of the providers, which usually become more complex than the example above.
+Once a application installed some modules and providers, it can become ready for providing resources. `application.ready()` checks that the module resources can be built by following the dependency graphs of the providers, which usually become more complex than the example above.
 
-The application can be built and registered as a pubilc, global variable in your application. Then, in the entry points of your application you can import that application and ask for any of the registered modules resources. For example:
+The application can be built and configured as a pubilc, global variable in your application. Then, in the entry points of your application you can import that application and ask for any of the registered modules resources. For example:
 
 ```python
 
 from .application import application
 
 class Main:
     def __init__(self):
```

