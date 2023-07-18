# Comparing `tmp/LolzteamApi-1.0.19.tar.gz` & `tmp/LolzteamApi-1.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LolzteamApi-1.0.19.tar", last modified: Sat Jul 15 08:25:01 2023, max compression
+gzip compressed data, was "LolzteamApi-1.0.20.tar", last modified: Tue Jul 18 11:40:17 2023, max compression
```

## Comparing `LolzteamApi-1.0.19.tar` & `LolzteamApi-1.0.20.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 08:25:01.957109 LolzteamApi-1.0.19/
--rw-rw-rw-   0        0        0     1089 2023-07-08 18:11:39.000000 LolzteamApi-1.0.19/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-15 08:25:01.950106 LolzteamApi-1.0.19/LolzteamApi/
--rw-rw-rw-   0        0        0   175980 2023-07-15 08:15:04.000000 LolzteamApi-1.0.19/LolzteamApi/LolzteamApi.py
--rw-rw-rw-   0        0        0       43 2023-07-15 08:07:56.000000 LolzteamApi-1.0.19/LolzteamApi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 08:25:01.955105 LolzteamApi-1.0.19/LolzteamApi.egg-info/
--rw-rw-rw-   0        0        0     2262 2023-07-15 08:25:01.000000 LolzteamApi-1.0.19/LolzteamApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-15 08:25:01.000000 LolzteamApi-1.0.19/LolzteamApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 08:25:01.000000 LolzteamApi-1.0.19/LolzteamApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-15 08:25:01.000000 LolzteamApi-1.0.19/LolzteamApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-15 08:25:01.000000 LolzteamApi-1.0.19/LolzteamApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2262 2023-07-15 08:25:01.956106 LolzteamApi-1.0.19/PKG-INFO
--rw-rw-rw-   0        0        0     1860 2023-07-10 01:19:44.000000 LolzteamApi-1.0.19/README.md
--rw-rw-rw-   0        0        0       42 2023-07-15 08:25:01.958106 LolzteamApi-1.0.19/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-07-15 08:10:04.000000 LolzteamApi-1.0.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:40:17.042615 LolzteamApi-1.0.20/
+-rw-rw-rw-   0        0        0     1089 2023-07-08 18:11:39.000000 LolzteamApi-1.0.20/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-18 11:40:17.034616 LolzteamApi-1.0.20/LolzteamApi/
+-rw-rw-rw-   0        0        0   179761 2023-07-18 11:32:30.000000 LolzteamApi-1.0.20/LolzteamApi/LolzteamApi.py
+-rw-rw-rw-   0        0        0       43 2023-07-15 08:07:56.000000 LolzteamApi-1.0.20/LolzteamApi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:40:17.040615 LolzteamApi-1.0.20/LolzteamApi.egg-info/
+-rw-rw-rw-   0        0        0     2262 2023-07-18 11:40:16.000000 LolzteamApi-1.0.20/LolzteamApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-18 11:40:16.000000 LolzteamApi-1.0.20/LolzteamApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 11:40:16.000000 LolzteamApi-1.0.20/LolzteamApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-18 11:40:16.000000 LolzteamApi-1.0.20/LolzteamApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-18 11:40:16.000000 LolzteamApi-1.0.20/LolzteamApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2262 2023-07-18 11:40:17.041616 LolzteamApi-1.0.20/PKG-INFO
+-rw-rw-rw-   0        0        0     1860 2023-07-10 01:19:44.000000 LolzteamApi-1.0.20/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 11:40:17.042615 LolzteamApi-1.0.20/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-07-18 11:32:42.000000 LolzteamApi-1.0.20/setup.py
```

### Comparing `LolzteamApi-1.0.19/LICENSE` & `LolzteamApi-1.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.19/LolzteamApi/LolzteamApi.py` & `LolzteamApi-1.0.20/LolzteamApi/LolzteamApi.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             paid_item = "paid_item"
             sold_item = "sold_item"
             money_transfer = "money_transfer"
             receiving_money = "receiving_money"
             internal_purchase = "internal_purchase"
             claim_hold = "claim_hold"
 
-        class Length:
+        class Hold_Options:
             hour = "hour"
             day = "day"
             week = "week"
             month = "month"
             year = "year"
 
         class Currency:
@@ -70,15 +70,15 @@
                 antipublic = 12
                 uniq = 14
                 photo_leaks = 17
                 auto_participation = 19
 
 
 class LolzteamApi:
-    def __init__(self, token: str, bypass_429: bool = True, language: str = "RU", disable_update_check: bool = False,
+    def __init__(self, token: str, bypass_429: bool = True, language: str = None, disable_update_check: bool = False,
                  proxy_type: str = None, proxy: str = None):
         """
         :param token: Your token. You can get in there -> https://zelenka.guru/account/api
         :param bypass_429: Bypass status code 429 by sleep
         :param language: Language for your api responses. Pass "en" if you want to get responses in english or pass "ru" if you want to get responses in russian.
         :param disable_update_check: Pass True if you don't want to see annoying update message
         :param proxy_type: Your proxy type. You can use types ( Types.Proxy.socks5 or socks4,https,http )
@@ -109,15 +109,14 @@
 
         self.market = self.__Market(self, self.__token_user_id)
         self.forum = self.__Forum(self)
 
     def send_request(self, method: str, url: str, params: dict = None, data=None, files=None):
         method = method.upper()
         LolzteamApi.__auto_delay(self)
-
         if params is None:
             params = {}
         params["locale"] = self.__locale
         proxies = {}
         if self.__proxy_type is not None:
             match self.__proxy_type:
                 case "HTTP":
@@ -389,15 +388,15 @@
                 Required scopes: read
 
                 :param total: If included in the request, only the forum count is returned as forums_total.
 
                 :return: json server response
                 """
                 url = f"https://api.zelenka.guru/forums/followed"
-                if True:  # Костыль, пока не пофиксят недочет #43
+                if True:  # Tweak 0
                     if total:
                         total = 1
                     else:
                         total = 0
                 params = {
                     "total": total
                 }
@@ -925,15 +924,15 @@
                 :param thread_tag_id: Filter to get only threads with the specified tag.
                 :param page: Page number of threads.
                 :param limit: Number of threads in a page.
                 :param order: Can be [natural, thread_create_date, thread_create_date_reverse, thread_update_date, thread_update_date_reverse, thread_view_count, thread_view_count_reverse, thread_post_count, thread_post_count_reverse]
                 :return: json server response
                 """
                 url = f"https://api.zelenka.guru/threads"
-                if sticky:  # Костыль, пока не пофиксят недочет #43
+                if sticky:  # Tweak 0
                     sticky = 1
                 else:
                     sticky = 0
                 params = {
                     "forum_id": forum_id,
                     "thread_ids": thread_ids,
                     "creator_user_id": creator_user_id,
@@ -1031,15 +1030,15 @@
                 Required scopes: read
 
                 :param total: If included in the request, only the forum count is returned as forums_total.
 
                 :return: json server response
                 """
                 url = f"https://api.zelenka.guru/forums/followed"
-                if True:  # Костыль, пока не пофиксят недочет #43
+                if True:  # Tweak 0
                     if total:
                         total = 1
                     else:
                         total = 0
                 params = {
                     "total": total
                 }
@@ -1556,15 +1555,15 @@
                 Required scopes: read
 
                 :param total: If included in the request, only the user count is returned as users_total.
 
                 :return: json server response
                 """
                 url = f"https://api.zelenka.guru/users/ignored"
-                if True:  # Костыль, пока не пофиксят недочет #43
+                if True:  # Tweak 0
                     if total:
                         total = 1
                     else:
                         total = 0
                 params = {
                     "total": total
                 }
@@ -2263,14 +2262,102 @@
                 :param conversation_id: ID of conversation.
 
                 :return: json server response
                 """
                 url = f"https://api.zelenka.guru/conversations/{conversation_id}"
                 return LolzteamApi.send_request(self=self.__api, method="DELETE", url=url)
 
+            def create(self, recipient_id: int, message: str, open_invite: bool = False,
+                       conversation_locked: bool = False, allow_edit_messages: bool = True):
+                """
+                POST https://api.zelenka.guru/conversations
+
+                Create a new conversation.
+
+                Required scopes: conversate, post
+
+                :param recipient_id: ID of recipient.
+                :param message: First message in conversation.
+                :param open_invite: Allow invites in conversation.
+                :param conversation_locked: Is conversation locked.
+                :param allow_edit_messages: Allow edit messages.
+
+                :return: json server response
+                """
+                if True:  # Tweak 0
+                    if open_invite:
+                        open_invite = 1
+                    else:
+                        open_invite = 0
+
+                    if conversation_locked:
+                        conversation_locked = 1
+                    else:
+                        conversation_locked = 0
+
+                    if allow_edit_messages:
+                        allow_edit_messages = 1
+                    else:
+                        allow_edit_messages = 0
+                params = {
+                    "recipient_id": recipient_id,
+                    "message_body": message,
+                    "is_group": 0,
+                    "open_invite": open_invite,
+                    "conversation_locked": conversation_locked,
+                    "allow_edit_messages": allow_edit_messages
+                }
+                url = f"https://api.zelenka.guru/conversations"
+                return LolzteamApi.send_request(self=self.__api, method="POST", url=url, params=params)
+
+            def create_group(self, recipients: str, title: str, message: str, open_invite: bool = True,
+                             conversation_locked: bool = False, allow_edit_messages: bool = True):
+                """
+                POST https://api.zelenka.guru/conversations
+
+                Create a new group conversation.
+
+                Required scopes: conversate, post
+
+                :param recipients: List of usernames (Separated by comma. Example -> "RaysMorgan,Thomas,Requeste")
+                :param title: The title of new conversation.
+                :param message: First message in conversation.
+                :param open_invite: Allow invites in conversation.
+                :param conversation_locked: Is conversation locked.
+                :param allow_edit_messages: Allow edit messages.
+
+                :return: json server response
+                """
+                if True:  # Tweak 0
+                    if open_invite:
+                        open_invite = 1
+                    else:
+                        open_invite = 0
+
+                    if conversation_locked:
+                        conversation_locked = 1
+                    else:
+                        conversation_locked = 0
+
+                    if allow_edit_messages:
+                        allow_edit_messages = 1
+                    else:
+                        allow_edit_messages = 0
+                params = {
+                    "recipients": recipients,
+                    "title": title,
+                    "message_body": message,
+                    "is_group": 1,
+                    "open_invite": open_invite,
+                    "conversation_locked": conversation_locked,
+                    "allow_edit_messages": allow_edit_messages
+                }
+                url = f"https://api.zelenka.guru/conversations"
+                return LolzteamApi.send_request(self=self.__api, method="POST", url=url, params=params)
+
         class __Oauth:
             def __init__(self, api_self):
                 self.__api = api_self
 
             def facebook(self, client_id: int, client_secret: str, facebook_token: str):
                 """
                 GET https://api.zelenka.guru/oauth/token/facebook
@@ -2579,15 +2666,15 @@
                 :param title: The word or words contained in the account title
                 :param search_params: Search params for your request. Example {"category_id":19} will return only VPN accounts
 
                 :return: json server response
 
                 """
 
-                if user_id is None:  # Tweak
+                if user_id is None:  # Tweak 1
                     if type(self.__token_user_id) is not int:
                         self.__token_user_id = self.__token_user_id()
                     user_id = self.__token_user_id
                 params = {
                     "user_id": user_id,
                     "category_id": category_id,
                     "pmin": pmin,
@@ -2669,15 +2756,15 @@
                 :param title: The word or words contained in the account title
                 :param search_params: Search params for your request. Example {"category_id":19} will return only VPN accounts
 
                 :return: json server response
 
                 """
 
-                if user_id is None:  # Tweak
+                if user_id is None:  # Tweak 1
                     if type(self.__token_user_id) is not int:
                         self.__token_user_id = self.__token_user_id()
                     user_id = self.__token_user_id
                 params = {
                     "category_id": category_id,
                     "pmin": pmin,
                     "pmax": pmax,
@@ -2896,15 +2983,15 @@
                     18 - escape-from-tarkov - Escape From Tarkov
 
                     19 - vpn - VPN
 
                     20 - tiktok - TikTok
 
                     22 - discord - Discord
-
+1
                     23 - cinema - Online Cinema
 
                     24 - telegram - Telegram
 
                     25 - youtube - YouTube
 
                     26 - spotify - Spotify
@@ -3075,15 +3162,15 @@
                 :param title: The word or words contained in the account title
                 :param search_params: Search params for your request. Example {"category_id":19} will return only VPN accounts
 
                 :return: json server response
 
                 """
 
-                if user_id is None:  # Tweak
+                if user_id is None:  # Tweak 1
                     if type(self.__token_user_id) is not int:
                         self.__token_user_id = self.__token_user_id()
                     user_id = self.__token_user_id
                 params = {
                     "user_id": user_id,
                     "category_id": category_id,
                     "pmin": pmin,
@@ -3164,15 +3251,15 @@
                 :param title: The word or words contained in the account title
                 :param search_params: Search params for your request. Example {"category_id":19} will return only VPN accounts
 
                 :return: json server response
 
                 """
 
-                if user_id is None:  # Tweak
+                if user_id is None:  # Tweak 1
                     if type(self.__token_user_id) is not int:
                         self.__token_user_id = self.__token_user_id()
                     user_id = self.__token_user_id
                 params = {
                     "category_id": category_id,
                     "pmin": pmin,
                     "pmax": pmax,
@@ -3285,24 +3372,24 @@
                 :param comment: Comment for money transfers
                 :param is_hold: Display hold operations
                 :param show_payments_stats: Display payment stats for selected period (outgoing value, incoming value)
 
                 :return: json server response
 
                 """
-                if True:  # Костыль, пока не пофиксят недочет #43
+                if True:  # Tweak 0
                     if is_hold:
                         is_hold = 1
                     else:
                         is_hold = 0
                     if show_payments_stats:
                         show_payments_stats = 1
                     else:
                         show_payments_stats = 0
-                if user_id is None:  # Tweak
+                if user_id is None:  # Tweak 1
                     if type(self.__token_user_id) is not int:
                         self.__token_user_id = self.__token_user_id()
                     user_id = self.__token_user_id
                 params = {
                     "user_id": user_id,
                     "operation_type": operation_type,
                     "pmin": pmin,
@@ -3357,43 +3444,51 @@
                     "hold_length_value": hold_length_value,
                     "hold_length_option": hold_length_option
                 }
                 return LolzteamApi.send_request(self=self.__api, method="POST", url=url, params=params)
 
             @staticmethod
             def generate_link(amount: int, user_id: int = None, username: str = None, comment: str = None,
-                              redirect_url: str = None, currency: str = None, hold: bool = None):
+                              redirect_url: str = None, currency: str = None, hold: bool = None,
+                              hold_length: int = None, hold_option: str = None):
                 """
                 Generate payment link
 
                 Required scopes: None
 
                 :param amount: Amount to send in your currency.
                 :param user_id: ID of user to transfer money
                 :param username: Username to transfer money
                 :param comment: Payment comment.
                 :param redirect_url: Redirect url. User who paid on this link will be redirected to this url
                 :param currency: Using currency for amount. Allowed values: cny, usd, rub, eur, uah, kzt, byn, gbp
                 :param hold: Hold transfer or not
-
+                :param hold_length: Hold length ( max 1 month )
+                :param hold_option: Hold option. Can be "hours","days","weeks","months"
                 :return: string payment url
                 """
-                if True:  # Костыль, пока не пофиксят недочет #43
+                if True:  # Tweak 0
                     if hold:
                         hold = 1
                     else:
                         hold = 0
+                if hold_option in ["hour", "day", "week", "month"]:
+                    hold_option += "s"
+                if hold_option not in ["hours", "days", "weeks", "months"]:
+                    raise Exception("""Invalid hold_option. It can be only "hours","days","weeks" and "months" """)
                 params = {
                     "user_id": user_id,
                     "username": username,
                     "amount": amount,
                     "comment": comment,
                     "redirect": redirect_url,
                     "currency": currency,
-                    "hold": hold
+                    "hold": hold,
+                    "hold_length_value": hold_length,
+                    "hold_length_option": hold_option
                 }
                 url = "https://lzt.market/balance/transfer"
                 req = requests.models.PreparedRequest()
                 req.prepare_url(url=url, params=params)
                 return req.url
 
         class __Managing:
@@ -3555,15 +3650,15 @@
 
                 :param item_id: ID of item.
                 :param _cancel: Cancel change password recommendation. It will be helpful, if you don't want to change password and get login data
 
                 :return: json server response
                 """
                 url = f"https://api.lzt.market/{item_id}/change-password"
-                if True:  # Костыль, пока не пофиксят недочет #43
+                if True:  # Tweak 0
                     if _cancel:
                         _cancel = 1
                     else:
                         _cancel = 0
                 params = {
                     "_cancel": _cancel
                 }
@@ -3785,15 +3880,15 @@
 
                 :param item_id: ID of item.
                 :param buy_without_validation: Use TRUE if you want to buy account without account data validation (not safe)
 
                 :return: json server response
                 """
                 url = f"https://api.lzt.market/{item_id}/confirm-buy"
-                if True:  # Костыль, пока не пофиксят недочет #43
+                if True:  # Tweak 0
                     if buy_without_validation:
                         buy_without_validation = 1
                     else:
                         buy_without_validation = 0
                 params = {
                     "buy_without_validation": buy_without_validation
                 }
@@ -3810,15 +3905,15 @@
                 :param item_id: ID of item.
                 :param price: Currenct price of account in your currency
                 :param buy_without_validation: Use TRUE if you want to buy account without account data validation (not safe)
 
                 :return: json server response
                 """
                 url = f"https://api.lzt.market/{item_id}/fast-buy"
-                if True:  # Костыль, пока не пофиксят недочет #43
+                if True:  # Tweak 0
                     if buy_without_validation:
                         buy_without_validation = 1
                     else:
                         buy_without_validation = 0
                 params = {
                     "price": price,
                     "buy_without_validation": buy_without_validation
@@ -3865,15 +3960,15 @@
                 :param extra: Extra params for account checking. E.g. you need to put cookies to extra[cookies] if you want to upload TikTok/Fortnite/Epic Games account
                 :param resell_item_id: Put item id, if you are trying to resell item.
                 :param random_proxy: Pass True, if you get captcha in previous response
 
                 :return: json server response
                 """
                 url = f"https://api.lzt.market/{item_id}/goods/check"
-                if True:  # Костыль, пока не пофиксят недочет #43
+                if True:  # Tweak 0
                     if random_proxy:
                         random_proxy = 1
                     else:
                         random_proxy = 0
                     if close_item:
                         close_item = 1
                     else:
@@ -3942,15 +4037,15 @@
                 :param allow_ask_discount: Allow users to ask discount for this account.
                 :param proxy_id: Using proxy id for account checking.
                 :param random_proxy: Pass True, if you get captcha in previous response
 
                 :return: json server response
                 """
                 url = f"https://api.lzt.market/item/add"
-                if True:  # Костыль, пока не пофиксят недочет #43
+                if True:  # Tweak 0
                     if random_proxy:
                         random_proxy = 1
                     else:
                         random_proxy = 0
                 params = {
                     "category_id": category_id,
                     "price": price,
@@ -4024,15 +4119,15 @@
                 :param login: Account login (or email)
                 :param password: Account password
                 :param login_password: Account login data format login:password
                 :param extra: Extra params for account checking. E.g. you need to put cookies to extra[cookies] if you want to upload TikTok/Fortnite/Epic Games account
                 :return: json server response
                 """
                 url = f"https://api.lzt.market/item/fast-sell"
-                if True:  # Костыль, пока не пофиксят недочет #43
+                if True:  # Tweak 0
                     if random_proxy:
                         random_proxy = 1
                     else:
                         random_proxy = 0
                 params = {
                     "category_id": category_id,
                     "price": price,
```

### Comparing `LolzteamApi-1.0.19/LolzteamApi.egg-info/PKG-INFO` & `LolzteamApi-1.0.20/LolzteamApi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.19
+Version: 1.0.20
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.19 Summary: A library that
+Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.20 Summary: A library that
 contains all the methods of the Lolzteam API (Market/Forum) Home-page: https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api Author: AS7RID Author-email:
 as7ridwork@gmail.com Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # Lolzteam Python API
                              [Material_Bread_logo]
 [![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
```

### Comparing `LolzteamApi-1.0.19/PKG-INFO` & `LolzteamApi-1.0.20/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.19
+Version: 1.0.20
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.19 Summary: A library that
+Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.20 Summary: A library that
 contains all the methods of the Lolzteam API (Market/Forum) Home-page: https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api Author: AS7RID Author-email:
 as7ridwork@gmail.com Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # Lolzteam Python API
                              [Material_Bread_logo]
 [![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
```

### Comparing `LolzteamApi-1.0.19/README.md` & `LolzteamApi-1.0.20/README.md`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.19/setup.py` & `LolzteamApi-1.0.20/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = ["requests", "beautifulsoup4"]
 
 setuptools.setup(
     name="LolzteamApi",
-    version="1.0.19",
+    version="1.0.20",
     author="AS7RID",
     author_email="as7ridwork@gmail.com",
     description="A library that contains all the methods of the Lolzteam API (Market/Forum)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AS7RIDENIED/Lolzteam_Python_Api",
     packages=setuptools.find_packages(),
```

