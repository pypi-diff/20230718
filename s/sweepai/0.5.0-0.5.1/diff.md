# Comparing `tmp/sweepai-0.5.0.tar.gz` & `tmp/sweepai-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.5.0.tar", max compression
+gzip compressed data, was "sweepai-0.5.1.tar", max compression
```

## Comparing `sweepai-0.5.0.tar` & `sweepai-0.5.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.5.0/LICENSE
--rw-r--r--   0        0        0     6010 2023-07-17 05:32:34.580144 sweepai-0.5.0/README.md
--rw-r--r--   0        0        0     1411 2023-07-17 05:49:03.619675 sweepai-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.5.0/sweepai/__init__.py
--rw-r--r--   0        0        0    12496 2023-07-16 01:12:44.721526 sweepai-0.5.0/sweepai/api.py
--rw-r--r--   0        0        0     7211 2023-07-17 05:32:34.590144 sweepai-0.5.0/sweepai/app/api_client.py
--rw-r--r--   0        0        0    13088 2023-07-14 19:18:34.070923 sweepai-0.5.0/sweepai/app/backend.py
--rw-r--r--   0        0        0     1167 2023-07-13 01:02:13.144171 sweepai-0.5.0/sweepai/app/cli.py
--rw-r--r--   0        0        0     3645 2023-07-17 05:32:34.590144 sweepai-0.5.0/sweepai/app/config.py
--rw-r--r--   0        0        0    18069 2023-07-17 05:48:47.959641 sweepai-0.5.0/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.5.0/sweepai/core/__init__.py
--rw-r--r--   0        0        0    18286 2023-07-14 23:37:58.184540 sweepai-0.5.0/sweepai/core/chat.py
--rw-r--r--   0        0        0     2880 2023-07-13 01:02:13.144171 sweepai-0.5.0/sweepai/core/code_repair.py
--rw-r--r--   0        0        0      775 2023-07-17 05:32:34.590144 sweepai-0.5.0/sweepai/core/edit_chunk.py
--rw-r--r--   0        0        0     8790 2023-07-14 23:37:58.184540 sweepai-0.5.0/sweepai/core/entities.py
--rw-r--r--   0        0        0      535 2023-07-13 01:02:13.144171 sweepai-0.5.0/sweepai/core/gha_extraction.py
--rw-r--r--   0        0        0    18704 2023-07-17 05:32:34.590144 sweepai-0.5.0/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3489 2023-07-13 01:02:13.144171 sweepai-0.5.0/sweepai/core/react.py
--rw-r--r--   0        0        0    22536 2023-07-17 05:32:34.590144 sweepai-0.5.0/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    13594 2023-07-13 01:02:13.144171 sweepai-0.5.0/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     3207 2023-07-16 01:12:44.721526 sweepai-0.5.0/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.5.0/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     7145 2023-07-17 05:32:34.590144 sweepai-0.5.0/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     2613 2023-07-13 22:20:26.750590 sweepai-0.5.0/sweepai/handlers/on_check_suite.py
--rw-r--r--   0        0        0    10275 2023-07-16 01:12:44.721526 sweepai-0.5.0/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     4042 2023-07-13 01:02:13.144171 sweepai-0.5.0/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    20526 2023-07-16 01:12:44.721526 sweepai-0.5.0/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.5.0/sweepai/slack.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.5.0/sweepai/utils/__init__.py
--rw-r--r--   0        0        0     3809 2023-07-16 01:12:44.721526 sweepai-0.5.0/sweepai/utils/chat_logger.py
--rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.5.0/sweepai/utils/config/__init__.py
--rw-r--r--   0        0        0     2761 2023-07-14 17:53:38.131398 sweepai-0.5.0/sweepai/utils/config/client.py
--rw-r--r--   0        0        0     3478 2023-07-17 05:32:34.590144 sweepai-0.5.0/sweepai/utils/config/server.py
--rw-r--r--   0        0        0     7968 2023-07-17 05:32:34.590144 sweepai-0.5.0/sweepai/utils/diff.py
--rw-r--r--   0        0        0      675 2023-07-13 01:02:13.147504 sweepai-0.5.0/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5256 2023-07-13 01:02:13.147504 sweepai-0.5.0/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8449 2023-07-14 18:26:12.305858 sweepai-0.5.0/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0      100 2023-07-13 01:02:13.147504 sweepai-0.5.0/sweepai/utils/hash.py
--rw-r--r--   0        0        0     5585 2023-07-13 01:02:13.147504 sweepai-0.5.0/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      849 2023-07-13 01:02:13.147504 sweepai-0.5.0/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1528 2023-07-13 01:02:13.147504 sweepai-0.5.0/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11648 2023-07-13 01:02:13.147504 sweepai-0.5.0/sweepai/utils/utils.py
--rw-r--r--   0        0        0     7210 2023-07-17 05:49:15.952933 sweepai-0.5.0/setup.py
--rw-r--r--   0        0        0     6989 2023-07-17 05:49:15.953366 sweepai-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.5.1/LICENSE
+-rw-r--r--   0        0        0     6010 2023-07-17 23:56:59.585924 sweepai-0.5.1/README.md
+-rw-r--r--   0        0        0     1411 2023-07-17 23:57:18.305948 sweepai-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.5.1/sweepai/__init__.py
+-rw-r--r--   0        0        0    12496 2023-07-16 01:12:44.721526 sweepai-0.5.1/sweepai/api.py
+-rw-r--r--   0        0        0     7184 2023-07-17 23:56:59.585924 sweepai-0.5.1/sweepai/app/api_client.py
+-rw-r--r--   0        0        0    13088 2023-07-14 19:18:34.070923 sweepai-0.5.1/sweepai/app/backend.py
+-rw-r--r--   0        0        0     1295 2023-07-17 23:56:59.585924 sweepai-0.5.1/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3645 2023-07-17 23:46:04.508567 sweepai-0.5.1/sweepai/app/config.py
+-rw-r--r--   0        0        0    18158 2023-07-17 23:56:59.585924 sweepai-0.5.1/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.5.1/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    18282 2023-07-17 23:56:59.585924 sweepai-0.5.1/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2880 2023-07-13 01:02:13.144171 sweepai-0.5.1/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0      775 2023-07-17 05:32:34.590144 sweepai-0.5.1/sweepai/core/edit_chunk.py
+-rw-r--r--   0        0        0     8790 2023-07-14 23:37:58.184540 sweepai-0.5.1/sweepai/core/entities.py
+-rw-r--r--   0        0        0      535 2023-07-13 01:02:13.144171 sweepai-0.5.1/sweepai/core/gha_extraction.py
+-rw-r--r--   0        0        0    18704 2023-07-17 05:32:34.590144 sweepai-0.5.1/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3489 2023-07-13 01:02:13.144171 sweepai-0.5.1/sweepai/core/react.py
+-rw-r--r--   0        0        0    22536 2023-07-17 05:32:34.590144 sweepai-0.5.1/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    13594 2023-07-13 01:02:13.144171 sweepai-0.5.1/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     3207 2023-07-16 01:12:44.721526 sweepai-0.5.1/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.5.1/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     7145 2023-07-17 05:32:34.590144 sweepai-0.5.1/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     2613 2023-07-13 22:20:26.750590 sweepai-0.5.1/sweepai/handlers/on_check_suite.py
+-rw-r--r--   0        0        0    10275 2023-07-16 01:12:44.721526 sweepai-0.5.1/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     4042 2023-07-13 01:02:13.144171 sweepai-0.5.1/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    20525 2023-07-17 23:56:59.589258 sweepai-0.5.1/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.5.1/sweepai/slack.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.5.1/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0     3809 2023-07-16 01:12:44.721526 sweepai-0.5.1/sweepai/utils/chat_logger.py
+-rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.5.1/sweepai/utils/config/__init__.py
+-rw-r--r--   0        0        0     2761 2023-07-14 17:53:38.131398 sweepai-0.5.1/sweepai/utils/config/client.py
+-rw-r--r--   0        0        0     3478 2023-07-17 05:32:34.590144 sweepai-0.5.1/sweepai/utils/config/server.py
+-rw-r--r--   0        0        0     7968 2023-07-17 05:32:34.590144 sweepai-0.5.1/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      675 2023-07-13 01:02:13.147504 sweepai-0.5.1/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5256 2023-07-13 01:02:13.147504 sweepai-0.5.1/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8449 2023-07-14 18:26:12.305858 sweepai-0.5.1/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0      100 2023-07-13 01:02:13.147504 sweepai-0.5.1/sweepai/utils/hash.py
+-rw-r--r--   0        0        0     5585 2023-07-13 01:02:13.147504 sweepai-0.5.1/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      849 2023-07-13 01:02:13.147504 sweepai-0.5.1/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1528 2023-07-13 01:02:13.147504 sweepai-0.5.1/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11648 2023-07-13 01:02:13.147504 sweepai-0.5.1/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     7210 2023-07-17 23:59:15.547109 sweepai-0.5.1/setup.py
+-rw-r--r--   0        0        0     6989 2023-07-17 23:59:15.547921 sweepai-0.5.1/PKG-INFO
```

### Comparing `sweepai-0.5.0/LICENSE` & `sweepai-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/README.md` & `sweepai-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to your desired repos
 2. Read about [recipes](docs/Recipes.md) for best use cases.
 2. Create a new issue in your repo. The issue should describe the problem or feature you want Sweep to address. For example, you could write "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"
 3. Respond with a message like "Sweep: use a different package instead" to have Sweep retry the issue or pull request. You can also comment on the code for minor changes! 💡 Hint: commenting "revert" reverts all edits in a file.
 
 We support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.
 
-### 🖥️ Sweep Chat
+### 🗨️ Sweep Chat
 Sweep Chat allows you to interact with Sweep and GitHub locally. You can collaborate on the plan with Sweep, and then have it create the pull request for you. Here's how to use Sweep Chat:
 
 **Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository
 
 1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**
     - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.
     - This runs GitHub authentication in your browser.
```

#### html2text {}

```diff
@@ -24,15 +24,15 @@
 for best use cases. 2. Create a new issue in your repo. The issue should
 describe the problem or feature you want Sweep to address. For example, you
 could write "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory" 3.
 Respond with a message like "Sweep: use a different package instead" to have
 Sweep retry the issue or pull request. You can also comment on the code for
 minor changes! ð¡ Hint: commenting "revert" reverts all edits in a file. We
 support all languages GPT4 supports, including Python, Typescript, Rust, Go,
-Java, C# and C++. ### ð¥ï¸ Sweep Chat Sweep Chat allows you to interact with
+Java, C# and C++. ### ð¨ï¸ Sweep Chat Sweep Chat allows you to interact with
 Sweep and GitHub locally. You can collaborate on the plan with Sweep, and then
 have it create the pull request for you. Here's how to use Sweep Chat:
 **Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai)
 to your repository 1. Run `pip3 install sweepai && sweep`. Note that you need
 **python 3.10+.** - Alternatively run `pip3 install --force-reinstall sweepai
 && sweep` if the previous command fails. - This runs GitHub authentication in
 your browser. 2. Copy the ðµ blue 8-digit code from your terminal into the
```

### Comparing `sweepai-0.5.0/pyproject.toml` & `sweepai-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.5.0"
+version = "0.5.1"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.urls]
```

### Comparing `sweepai-0.5.0/sweepai/api.py` & `sweepai-0.5.1/sweepai/api.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/app/api_client.py` & `sweepai-0.5.1/sweepai/app/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,14 @@
             messages: list[tuple[str | None, str | None]],
             snippets: list[Snippet] = [],
             do_add_plan: bool = True,
             functions: list[Function] = [],
             function_call: Any = "auto",
             model: str = "gpt-4-0613"
     ):
-        print(do_add_plan)
         with httpx.Client(timeout=30) as client:  # sometimes this step is slow
             with client.stream(
                     'POST',
                     self.api_endpoint + '/chat_stream',
                     json={
                         "messages": messages,
                         "snippets": [snippet.dict() for snippet in snippets],
```

### Comparing `sweepai-0.5.0/sweepai/app/backend.py` & `sweepai-0.5.1/sweepai/app/backend.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/app/cli.py` & `sweepai-0.5.1/sweepai/app/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,44 @@
+import os
 import typer
-
+import sys
 from sweepai.app.config import SweepChatConfig
+from subprocess import call
 
 epilog = "Sweep is a AI junior developer. Docs at https://docs.sweep.dev, install at https://github.com/apps/sweep-ai and support at https://discord.gg/sweep-ai."
 
 typer_app = typer.Typer(epilog=epilog)
 
 
 # @app.callback()
 @typer_app.command()
 def start():
     """
     Launch Sweep Chat in the browser
     """
     SweepChatConfig.load()
-    from sweepai.app.ui import demo
+    
     print("\033[93m⭐ Remember to star our repo at https://github.com/sweepai/sweep! \033[0m")
-    demo.queue()
-    demo.launch(inbrowser=True)
 
+    # hacky solution based on https://stackoverflow.com/a/45047992 to keep the context on Gradio Blocks
+    call([os.path.basename(sys.executable), "sweepai/app/ui.py"])
+    
 
 @typer_app.command()
 def auth():
     """
     Reauthenticate with Github API for Sweep to work (for token expiry)
     """
     SweepChatConfig.load(recreate=True)
     print("Setup completed successfully!")
     print("\033[93m⭐ Remember to star our repo at https://github.com/sweepai/sweep! \033[0m")
 
 
 def app():
     # hacky solution based on https://github.com/tiangolo/typer/issues/18#issuecomment-1577788949
-    import sys
     commands = {'start', 'auth'}
     sys.argv.append('start') if sys.argv[-1] not in commands else None
     typer_app()
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `sweepai-0.5.0/sweepai/app/config.py` & `sweepai-0.5.1/sweepai/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/app/ui.py` & `sweepai-0.5.1/sweepai/app/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,21 +159,21 @@
             repo_full_name = gr.Dropdown(choices=[repo.full_name for repo in repos], label="Repo full name",
                                          value=lambda: config.repo_full_name or "")
         print("Indexing files...")
         with gr.Column(scale=4):
             file_names = gr.Dropdown(choices=get_files(config.repo_full_name), multiselect=True, label="Files",
                                      value=lambda: global_state.file_paths)
         print("Indexed files!")
-        repo_full_name.change(get_files_update, repo_full_name, file_names)
+        repo_full_name.change(fn=get_files_update, inputs=repo_full_name, outputs=file_names)
         with gr.Column(scale=1):
             restart_button = gr.Button("Restart")
 
     with gr.Row():
         with gr.Column(scale=2):
-            chatbot = gr.Chatbot(height=400, value=lambda: global_state.chat_history)
+            chatbot = gr.Chatbot(height=600, value=lambda: global_state.chat_history)
         with gr.Column():
             with gr.Row():
                 snippets_text = gr.Markdown(value=lambda: global_state.snippets_text, elem_id="snippets")
 
     with gr.Row():
         plan = gr.List(
             value=[[filename + ": " + instructions] for filename, instructions in global_state.plan] or [[""]],
@@ -214,15 +214,15 @@
         config.state = global_state
         config.save()
         return [], [], [[""]]
 
 
     restart_button.click(clear_inputs, None, [file_names, chatbot, plan])
 
-    file_names.change(get_files_update, repo_full_name, chatbot)
+    file_names.change(fn=get_files_update, inputs=repo_full_name, outputs=file_names)
 
     searched = False
     selected_snippets = []
     file_to_str = {}
 
 
     def repo_name_change(repo_full_name):
@@ -253,15 +253,15 @@
             if file_name not in file_to_str:
                 add_file_to_dict(file_name)
         snippets_text = "### Relevant snippets:\n" + "\n\n".join(
             [file_to_str[snippet.file_path] for snippet in selected_snippets])
         return snippets_text
 
 
-    repo_full_name.change(repo_name_change, [repo_full_name], [msg])
+    repo_full_name.change(fn=repo_name_change, inputs=[repo_full_name], outputs=[msg])
 
 
     def add_file_to_dict(file_name):
         global file_to_str
         global path_to_contents
         global repo
         if file_name in path_to_contents:
@@ -285,15 +285,15 @@
             if file_name in path_to_contents:
                 selected_snippets.append(
                     Snippet(content=path_to_contents[file_name], start=0, end=path_to_contents[file_name].count('\n'),
                             file_path=file_name))
         return file_names, build_string()
 
 
-    file_names.change(file_names_change, [file_names], [file_names, snippets_text])
+    file_names.change(fn=file_names_change, inputs=[file_names], outputs=[file_names, snippets_text])
 
     def handle_message_submit(repo_full_name: str, user_message: str, history: list[tuple[str | None, str | None]]):
         if not repo_full_name:
             raise gr.Error("Set the repository name first")
         return gr.update(value="", interactive=False), history + [[user_message, None]], gr.Button.update(
             interactive=False)
 
@@ -459,8 +459,8 @@
             raise gr.Error(str(e))
 
 
     create_pr_button.click(on_create_pr_button_click, [chatbot, plan], [chatbot, create_pr_button])
 
 if __name__ == "__main__":
     demo.queue()
-    demo.launch()
+    demo.launch(inbrowser=True)
```

### Comparing `sweepai-0.5.0/sweepai/core/chat.py` & `sweepai-0.5.1/sweepai/core/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,17 +221,16 @@
         logger.info(f"Using the model {model}, with {max_tokens} tokens remaining")
         global retry_counter
         retry_counter = 0
         if functions:
             @backoff.on_exception(
                 backoff.expo,
                 Exception,
-                max_tries=12,
+                max_tries=5,
                 jitter=backoff.random_jitter,
-
             )
             def fetch():
                 global retry_counter
                 retry_counter += 1
                 token_sub = retry_counter * 200
                 try:
                     output = None
@@ -280,15 +279,15 @@
             logger.info(f"Output to call openai:\n{result}")
             return result
 
         else:
             @backoff.on_exception(
                 backoff.expo,
                 Exception,
-                max_tries=12,
+                max_tries=5,
                 jitter=backoff.random_jitter,
             )
             def fetch():
                 global retry_counter
                 retry_counter += 1
                 token_sub = retry_counter * 200
                 try:
@@ -330,15 +329,15 @@
 
         assert ANTHROPIC_API_KEY is not None
         client = anthropic.Client(api_key=ANTHROPIC_API_KEY)
 
         @backoff.on_exception(
             backoff.expo,
             Exception,
-            max_tries=12,
+            max_tries=5,
             jitter=backoff.random_jitter,
         )
         def fetch() -> tuple[str, str]:
             logger.warning(f"Calling anthropic...")
             results = client.completion(
                 prompt=messages_raw,
                 stop_sequences=[anthropic.HUMAN_PROMPT],
```

### Comparing `sweepai-0.5.0/sweepai/core/code_repair.py` & `sweepai-0.5.1/sweepai/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/core/edit_chunk.py` & `sweepai-0.5.1/sweepai/core/edit_chunk.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/core/entities.py` & `sweepai-0.5.1/sweepai/core/entities.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/core/gha_extraction.py` & `sweepai-0.5.1/sweepai/core/gha_extraction.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/core/prompts.py` & `sweepai-0.5.1/sweepai/core/prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/core/react.py` & `sweepai-0.5.1/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/core/sweep_bot.py` & `sweepai-0.5.1/sweepai/core/sweep_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/core/vector_db.py` & `sweepai-0.5.1/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/events.py` & `sweepai-0.5.1/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/handlers/create_pr.py` & `sweepai-0.5.1/sweepai/handlers/create_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/handlers/on_check_suite.py` & `sweepai-0.5.1/sweepai/handlers/on_check_suite.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/handlers/on_comment.py` & `sweepai-0.5.1/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/handlers/on_review.py` & `sweepai-0.5.1/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/handlers/on_ticket.py` & `sweepai-0.5.1/sweepai/handlers/on_ticket.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
             issue_comment.edit(first_comment)
             break
     if issue_comment is None:
         issue_comment = current_issue.create_comment(first_comment)
 
     # Comment edit function
     past_messages = {}
-    current_index = {}
+    current_index = 0
 
     def edit_sweep_comment(message: str, index: int, pr_message=""):
         nonlocal current_index
         # -1 = error, -2 = retry
         # Only update the progress bar if the issue generation errors.
         errored = (index == -1)
         if index >= 0:
```

### Comparing `sweepai-0.5.0/sweepai/utils/chat_logger.py` & `sweepai-0.5.1/sweepai/utils/chat_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/utils/config/client.py` & `sweepai-0.5.1/sweepai/utils/config/client.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/utils/config/server.py` & `sweepai-0.5.1/sweepai/utils/config/server.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/utils/diff.py` & `sweepai-0.5.1/sweepai/utils/diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/utils/event_logger.py` & `sweepai-0.5.1/sweepai/utils/event_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/utils/file_change_functions.py` & `sweepai-0.5.1/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/utils/github_utils.py` & `sweepai-0.5.1/sweepai/utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/utils/prompt_constructor.py` & `sweepai-0.5.1/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/utils/scorer.py` & `sweepai-0.5.1/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/utils/snippets.py` & `sweepai-0.5.1/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/sweepai/utils/utils.py` & `sweepai-0.5.1/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.5.0/setup.py` & `sweepai-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 
 entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app',
                      'sweepai = sweepai.app.cli:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': 'Sweep software chores',
-    'long_description': '<p align="center">\n    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">\n</p>\n<p align="center">\n    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev">\n    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">\n</a>\n<a href="https://docs.sweep.dev/">\n    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">\n</a> \n<a href="https://discord.gg/sweep-ai">\n    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />\n</a>\n<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">\n<a href="https://pepy.tech/project/sweepai">\n    <img src="https://static.pepy.tech/badge/sweepai/month" />\n</a>\n<a href="https://github.com/sweepai/sweep">\n    <img src="https://img.shields.io/github/stars/sweepai/sweep" />\n</a>\n<a href="https://twitter.com/sweep__ai">\n    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />\n</a>\n</p>\n\n<b>Sweep</b> is an AI junior developer that transforms bug reports & feature requests into code changes.\n\nDescribe bugs, small features, and refactors like you would to a junior developer, and Sweep:\n1. 🔍 reads your codebase\n2. 📝 plans the changes\n3. ⚡**writes a pull request with code**⚡\n\nSee highlights at https://docs.sweep.dev/examples.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🌠 Features\n* 🔧 Turns issues directly into pull requests (without an IDE)\n* 👀 Addresses developer replies & comments on its PRs\n* 🕵️\u200d♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/blogs/building-code-search))\n* 🎊 New: Fixes PRs based on Github Actions feedback\n* 🎊 New: Sweep Chat, a local interface for Sweep (see below)\n\n## 🚀 Getting Started\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address. Here are the steps to get started:\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to your desired repos\n2. Read about [recipes](docs/Recipes.md) for best use cases.\n2. Create a new issue in your repo. The issue should describe the problem or feature you want Sweep to address. For example, you could write "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"\n3. Respond with a message like "Sweep: use a different package instead" to have Sweep retry the issue or pull request. You can also comment on the code for minor changes! 💡 Hint: commenting "revert" reverts all edits in a file.\n\nWe support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep and GitHub locally. You can collaborate on the plan with Sweep, and then have it create the pull request for you. Here\'s how to use Sweep Chat:\n\n**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository\n\n1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**\n    - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.\n    - This runs GitHub authentication in your browser.\n\n2. Copy the 🔵 blue 8-digit code from your terminal into the page. You should only need to do the authentication once.  \n    - Wait a few seconds and Sweep Chat will start. \n\n3. Choose a repository from the dropdown at the top (the Github app must be installed to this repository).\n    - ⚡ Start chatting with Sweep Chat! ⚡\n\n\n![Screenshot_20230711_015033](https://github.com/sweepai/sweep/assets/26889185/ed9f05d8-ef86-4f2a-9bca-acdfa24990ac)\n\nTips:\n* 🔍 Relevant searched files will show up on the right. \n* 🔘 Sweep Chat creates PRs when the "Create PR" button is clicked. \n* 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.\n\n## 💰 Pricing\n* We charge $120/month for 60 GPT4 tickets per month.\n* For unpaid users, we offer 5 free GPT4 tickets per month.\n* We also offer unlimited GPT3.5 tickets.\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/).\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features. Each task required us to open our IDE to fix simple bugs. So we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default)\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n## 🗺️ Roadmap\nSee [🗺️ Roadmap](https://docs.sweep.dev/roadmap)\n\n## ⭐ Star History\n\n[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear about us!\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
+    'long_description': '<p align="center">\n    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">\n</p>\n<p align="center">\n    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev">\n    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">\n</a>\n<a href="https://docs.sweep.dev/">\n    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">\n</a> \n<a href="https://discord.gg/sweep-ai">\n    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />\n</a>\n<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">\n<a href="https://pepy.tech/project/sweepai">\n    <img src="https://static.pepy.tech/badge/sweepai/month" />\n</a>\n<a href="https://github.com/sweepai/sweep">\n    <img src="https://img.shields.io/github/stars/sweepai/sweep" />\n</a>\n<a href="https://twitter.com/sweep__ai">\n    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />\n</a>\n</p>\n\n<b>Sweep</b> is an AI junior developer that transforms bug reports & feature requests into code changes.\n\nDescribe bugs, small features, and refactors like you would to a junior developer, and Sweep:\n1. 🔍 reads your codebase\n2. 📝 plans the changes\n3. ⚡**writes a pull request with code**⚡\n\nSee highlights at https://docs.sweep.dev/examples.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🌠 Features\n* 🔧 Turns issues directly into pull requests (without an IDE)\n* 👀 Addresses developer replies & comments on its PRs\n* 🕵️\u200d♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/blogs/building-code-search))\n* 🎊 New: Fixes PRs based on Github Actions feedback\n* 🎊 New: Sweep Chat, a local interface for Sweep (see below)\n\n## 🚀 Getting Started\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address. Here are the steps to get started:\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to your desired repos\n2. Read about [recipes](docs/Recipes.md) for best use cases.\n2. Create a new issue in your repo. The issue should describe the problem or feature you want Sweep to address. For example, you could write "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"\n3. Respond with a message like "Sweep: use a different package instead" to have Sweep retry the issue or pull request. You can also comment on the code for minor changes! 💡 Hint: commenting "revert" reverts all edits in a file.\n\nWe support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.\n\n### 🗨️ Sweep Chat\nSweep Chat allows you to interact with Sweep and GitHub locally. You can collaborate on the plan with Sweep, and then have it create the pull request for you. Here\'s how to use Sweep Chat:\n\n**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository\n\n1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**\n    - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.\n    - This runs GitHub authentication in your browser.\n\n2. Copy the 🔵 blue 8-digit code from your terminal into the page. You should only need to do the authentication once.  \n    - Wait a few seconds and Sweep Chat will start. \n\n3. Choose a repository from the dropdown at the top (the Github app must be installed to this repository).\n    - ⚡ Start chatting with Sweep Chat! ⚡\n\n\n![Screenshot_20230711_015033](https://github.com/sweepai/sweep/assets/26889185/ed9f05d8-ef86-4f2a-9bca-acdfa24990ac)\n\nTips:\n* 🔍 Relevant searched files will show up on the right. \n* 🔘 Sweep Chat creates PRs when the "Create PR" button is clicked. \n* 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.\n\n## 💰 Pricing\n* We charge $120/month for 60 GPT4 tickets per month.\n* For unpaid users, we offer 5 free GPT4 tickets per month.\n* We also offer unlimited GPT3.5 tickets.\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/).\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features. Each task required us to open our IDE to fix simple bugs. So we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default)\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n## 🗺️ Roadmap\nSee [🗺️ Roadmap](https://docs.sweep.dev/roadmap)\n\n## ⭐ Star History\n\n[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear about us!\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils',
 'sweepai.utils.config'] package_data = \ {'': ['*']} install_requires = \
 ['GitPython>=3.1.31,<4.0.0', 'PyGithub==1.58.2', 'config-path>=1.0.3,<2.0.0',
 'gradio>=3.35.2,<4.0.0', 'loguru>=0.6.0,<0.7.0', 'pyyaml>=6.0,<7.0',
 'requests>=2.28.2,<3.0.0', 'tabulate>=0.9.0,<0.10.0', 'typer>=0.9.0,<0.10.0',
 'urllib3<2.0.0'] entry_points = \ {'console_scripts': ['sweep =
 sweepai.app.cli:app', 'sweepai = sweepai.app.cli:app']} setup_kwargs =
-{ 'name': 'sweepai', 'version': '0.5.0', 'description': 'Sweep software
+{ 'name': 'sweepai', 'version': '0.5.1', 'description': 'Sweep software
 chores', 'long_description': '
  \n [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
                                 3e61f57ad233]\n
 \n
              \n Bug Reports & Feature Requests â¶  Code Changes\n
 \n\n
 \n\n_[Landing_Page]\n\n\n_[Docs]\n \n\n_[https://dcbadge.vercel.app/api/server/
@@ -37,15 +37,15 @@
 cases.\n2. Create a new issue in your repo. The issue should describe the
 problem or feature you want Sweep to address. For example, you could write
 "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"\n3. Respond
 with a message like "Sweep: use a different package instead" to have Sweep
 retry the issue or pull request. You can also comment on the code for minor
 changes! ð¡ Hint: commenting "revert" reverts all edits in a file.\n\nWe
 support all languages GPT4 supports, including Python, Typescript, Rust, Go,
-Java, C# and C++.\n\n### ð¥ï¸ Sweep Chat\nSweep Chat allows you to interact
+Java, C# and C++.\n\n### ð¨ï¸ Sweep Chat\nSweep Chat allows you to interact
 with Sweep and GitHub locally. You can collaborate on the plan with Sweep, and
 then have it create the pull request for you. Here\'s how to use Sweep Chat:
 \n\n**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/
 sweep-ai) to your repository\n\n1. Run `pip3 install sweepai && sweep`. Note
 that you need **python 3.10+.**\n - Alternatively run `pip3 install --force-
 reinstall sweepai && sweep` if the previous command fails.\n - This runs GitHub
 authentication in your browser.\n\n2. Copy the ðµ blue 8-digit code from your
```

### Comparing `sweepai-0.5.0/PKG-INFO` & `sweepai-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.5.0
+Version: 0.5.1
 Summary: Sweep software chores
 Author: Kevin Lu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
@@ -79,15 +79,15 @@
 1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to your desired repos
 2. Read about [recipes](docs/Recipes.md) for best use cases.
 2. Create a new issue in your repo. The issue should describe the problem or feature you want Sweep to address. For example, you could write "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"
 3. Respond with a message like "Sweep: use a different package instead" to have Sweep retry the issue or pull request. You can also comment on the code for minor changes! 💡 Hint: commenting "revert" reverts all edits in a file.
 
 We support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.
 
-### 🖥️ Sweep Chat
+### 🗨️ Sweep Chat
 Sweep Chat allows you to interact with Sweep and GitHub locally. You can collaborate on the plan with Sweep, and then have it create the pull request for you. Here's how to use Sweep Chat:
 
 **Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository
 
 1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**
     - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.
     - This runs GitHub authentication in your browser.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sweepai Version: 0.5.0 Summary: Sweep software
+Metadata-Version: 2.1 Name: sweepai Version: 0.5.1 Summary: Sweep software
 chores Author: Kevin Lu Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: GitPython
 (>=3.1.31,<4.0.0) Requires-Dist: PyGithub (==1.58.2) Requires-Dist: config-path
 (>=1.0.3,<2.0.0) Requires-Dist: gradio (>=3.35.2,<4.0.0) Requires-Dist: loguru
 (>=0.6.0,<0.7.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: requests
 (>=2.28.2,<3.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist:
@@ -37,15 +37,15 @@
 for best use cases. 2. Create a new issue in your repo. The issue should
 describe the problem or feature you want Sweep to address. For example, you
 could write "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory" 3.
 Respond with a message like "Sweep: use a different package instead" to have
 Sweep retry the issue or pull request. You can also comment on the code for
 minor changes! ð¡ Hint: commenting "revert" reverts all edits in a file. We
 support all languages GPT4 supports, including Python, Typescript, Rust, Go,
-Java, C# and C++. ### ð¥ï¸ Sweep Chat Sweep Chat allows you to interact with
+Java, C# and C++. ### ð¨ï¸ Sweep Chat Sweep Chat allows you to interact with
 Sweep and GitHub locally. You can collaborate on the plan with Sweep, and then
 have it create the pull request for you. Here's how to use Sweep Chat:
 **Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai)
 to your repository 1. Run `pip3 install sweepai && sweep`. Note that you need
 **python 3.10+.** - Alternatively run `pip3 install --force-reinstall sweepai
 && sweep` if the previous command fails. - This runs GitHub authentication in
 your browser. 2. Copy the ðµ blue 8-digit code from your terminal into the
```

