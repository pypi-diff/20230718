# Comparing `tmp/lemonai-0.1.2.tar.gz` & `tmp/lemonai-0.1.3.tar.gz`

## Comparing `lemonai-0.1.2.tar` & `lemonai-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0  5358251 2020-02-02 00:00:00.000000 lemonai-0.1.2/heatmap-example.gif
--rw-r--r--   0        0        0   459819 2020-02-02 00:00:00.000000 lemonai-0.1.2/heatmap-example.png
--rw-r--r--   0        0        0    71395 2020-02-02 00:00:00.000000 lemonai-0.1.2/random.txt
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 lemonai-0.1.2/test.py
--rw-r--r--   0        0        0     5603 2020-02-02 00:00:00.000000 lemonai-0.1.2/testrandom.py
--rw-r--r--   0        0        0    58482 2020-02-02 00:00:00.000000 lemonai-0.1.2/use-case-example.png
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 lemonai-0.1.2/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 lemonai-0.1.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lemonai-0.1.2/.vscode/launch.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 lemonai-0.1.2/.vscode/settings.json
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 lemonai-0.1.2/docs/tools.md
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lemonai-0.1.2/src/lemonai/__init__.py
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 lemonai-0.1.2/src/lemonai/api_wrapper.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 lemonai-0.1.2/src/lemonai/execute_workflow.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 lemonai-0.1.2/src/lemonai/filter_tools.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 lemonai-0.1.2/src/lemonai/get_integrations.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 lemonai-0.1.2/src/lemonai/tool.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lemonai-0.1.2/src/lemonai/toolkit.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 lemonai-0.1.2/src/lemonai/workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemonai-0.1.2/tests/.gitkeep
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemonai-0.1.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 lemonai-0.1.2/LICENSE
--rw-r--r--   0        0        0     9639 2020-02-02 00:00:00.000000 lemonai-0.1.2/README.md
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lemonai-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    10384 2020-02-02 00:00:00.000000 lemonai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0  5358251 2020-02-02 00:00:00.000000 lemonai-0.1.3/heatmap-example.gif
+-rw-r--r--   0        0        0   459819 2020-02-02 00:00:00.000000 lemonai-0.1.3/heatmap-example.png
+-rw-r--r--   0        0        0    71395 2020-02-02 00:00:00.000000 lemonai-0.1.3/random.txt
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 lemonai-0.1.3/test.py
+-rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 lemonai-0.1.3/testrandom.py
+-rw-r--r--   0        0        0    58482 2020-02-02 00:00:00.000000 lemonai-0.1.3/use-case-example.png
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 lemonai-0.1.3/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 lemonai-0.1.3/.github/N8N-INSTRUCTIONS.md
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 lemonai-0.1.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lemonai-0.1.3/.vscode/launch.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 lemonai-0.1.3/.vscode/settings.json
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 lemonai-0.1.3/docs/tools.md
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lemonai-0.1.3/src/lemonai/__init__.py
+-rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 lemonai-0.1.3/src/lemonai/api_wrapper.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 lemonai-0.1.3/src/lemonai/execute_workflow.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 lemonai-0.1.3/src/lemonai/filter_tools.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 lemonai-0.1.3/src/lemonai/get_integrations.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 lemonai-0.1.3/src/lemonai/tool.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lemonai-0.1.3/src/lemonai/toolkit.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 lemonai-0.1.3/src/lemonai/workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemonai-0.1.3/tests/.gitkeep
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemonai-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 lemonai-0.1.3/LICENSE
+-rw-r--r--   0        0        0     9639 2020-02-02 00:00:00.000000 lemonai-0.1.3/README.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lemonai-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    10384 2020-02-02 00:00:00.000000 lemonai-0.1.3/PKG-INFO
```

### Comparing `lemonai-0.1.2/heatmap-example.gif` & `lemonai-0.1.3/heatmap-example.gif`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.2/heatmap-example.png` & `lemonai-0.1.3/heatmap-example.png`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.2/random.txt` & `lemonai-0.1.3/random.txt`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.2/test.py` & `lemonai-0.1.3/test.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 
 os.environ["OPENAI_API_KEY"] = "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"
 # os.environ["AIRTABLE_SECRET_TOKEN"] = "patJoC5EBAvPKdAjY.42c1c66934da89b3935cad9c41c88d7de750101dfcc111e1958a3c679b01599a"
 os.environ["GITHUB_API_KEY"] = "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"
 os.environ["DISCORD_WEBHOOK_URL"] = "https://discord.com/api/webhooks/1130492847578161222/ZYS1ewlNF1IGEdnKK4TU38wSAF8e4iYUSMlMIBPCPAZDZsiw5XOntZ8JUssAyB6r2Tme"
 
 # prompt = "Get me information for Hackernews user kimburgess"
-# prompt = "Read information from Hackernews for user kimburgess and then write the results to Airtable (BaseId: app2VdQRffkyAiIcc, tableId: tblscnilGk6BHVkVn). Only write the fields 'username', 'karma' and 'created_at_i'. Please make sure that Airtable does NOT automatically convert the field types."
+# prompt = "Read information from Hackernews for user kimburgess and then append the results to Airtable (BaseId: app2VdQRffkyAiIcc, tableId: tblscnilGk6BHVkVn). Only write the fields 'username', 'karma' and 'created_at_i'. Please make sure that Airtable does NOT automatically convert the field types."
 # prompt = "Run the Hackernews Airtable User Workflow for user kimburgess, baseId app2VdQRffkyAiIcc and tableId tblscnilGk6BHVkVn. Only write the fields 'username', 'karma' and 'created_at_i' to the Airtable table. Please make sure that Airtable does NOT automatically convert the field types."
 # prompt = f"List the names of my starred repositories on Github, and rank the top 5 in descending order of their stargazer_count field. The owner is felixbrock."
 # prompt = "List only the names of my starred repositories on Github. Owner is felixbrock"
 # prompt = "List the top growing repositories that I have starred (my username is Abdus2609). Then, send a Discord message in a leaderboard format, numerically bullet pointing each repository and its growth. Also, get the description of the repository lemonai (owner felixbrock) and within the Discord message, use the description of each starred repository to explain how each tool would be relevant to lemonai."
 
 # prompt = "Get the description for a repository I am working with called lemonai (owner felixbrock). Also, get my top growing starred repositories (useername Abdus2609). Then, construct and send a Discord message that firstly displays a numerically bullet pointed leaderboard of the top growing starred repositories and their growth, and secondly explains how each tool could be useful to use in lemonai based on your analysis of lemonai's description and the description of each starred repository."
-# prompt = "Get the description for a repository I am working with called lemonai (owner felixbrock). Also, get my top growing starred repositories (useername Abdus2609). Analyse the descriptions of both the LemonAI repository and my top starred repositories. Then, send a Discord message that firstly displays a numerically bullet pointed leaderboard of the top growing starred repositories and their growth, and secondly discusses how each tool could be useful specifically to lemonai's use case based on your analysis of the descriptions of each repository."
+prompt = "Get the description for a repository I am working with called lemonai (owner felixbrock). Also, get my top growing starred repositories (useername Abdus2609). Understand the descriptions of the LemonAI repository and my top starred repositories. Then, send a Discord message that firstly displays a numerically bullet pointed leaderboard of the top growing starred repositories and their growth, and secondly discusses how each tool could be useful specifically to lemonai's use case based on your analysis of the descriptions of each repository."
+# prompt = "Get the description of the repository lemonai (owner felixbrock) and send it to my Discord channel"
+# prompt = "Get the name of all my repositories (owner Abdus2609) and send them to my Discord channel as a bullet point list"
 
 model = OpenAI(temperature=0)
-execute_workflow(model, prompt_string=prompt)
+execute_workflow(model, prompt_string=prompt, server_domain='http://localhost:1313')
```

### Comparing `lemonai-0.1.2/testrandom.py` & `lemonai-0.1.3/testrandom.py`

 * *Files 22% similar despite different names*

```diff
@@ -1 +1,23 @@
-print(len([{'name': 'companion-app'}, {'name': 'chatgpt.js'}, {'name': 'long_llama'}, {'name': 'htmx'}, {'name': 'scipy2023-deeplearning'}, {'name': 'gpt-researcher'}, {'name': 'The-Art-of-Linear-Algebra'}, {'name': 'gpt-prompt-engineer'}, {'name': 'Plan-and-Solve-Prompting'}, {'name': 'engine'}, {'name': 'simpleaichat'}, {'name': 'litechain'}, {'name': 'superagent'}, {'name': 'gorilla'}, {'name': 'gorilla-cli'}, {'name': 'tinyvector'}, {'name': 'valmi-activation'}, {'name': 'gpt-migrate'}, {'name': 'lemonai-server'}, {'name': 'lemonai-analytics'}, {'name': 'lemonai'}, {'name': 'ai-jsx'}, {'name': 'spacedrive'}, {'name': 'composer'}, {'name': 'chathn'}, {'name': 'kaguya'}, {'name': 'docs'}, {'name': 'openpm'}, {'name': 'workgpt'}, {'name': 'pepy'}, {'name': 'awesome-selfhosted'}, {'name': 'WizardLM'}, {'name': 'novel'}, {'name': 'OpenChat'}, {'name': 'ai'}, {'name': 'vllm'}, {'name': 'nix.dev'}, {'name': 'OpenLLM'}, {'name': 'poop'}, {'name': 'LLaMA-Efficient-Tuning'}, {'name': 'camel'}, {'name': 'tauri'}, {'name': 'machine-learning-for-trading'}, {'name': 'FinGPT'}, {'name': 'isle'}, {'name': 'FlagAI'}, {'name': 'gpt-engineer'}, {'name': 'plugnplai'}, {'name': 'cypress'}, {'name': 'bloop'}, {'name': 'listmonk'}, {'name': 'lodash'}, {'name': 'pnpm'}, {'name': 'turbo'}, {'name': 'fresh'}, {'name': 'prisma'}, {'name': 'qwik'}, {'name': 'deno'}, {'name': 'kit'}, {'name': 'astro'}, {'name': 'bun'}, {'name': 'tensor2tensor'}, {'name': 'ggml'}, {'name': 'axodox-machinelearning'}, {'name': 'onnxruntime'}, {'name': 'alphadev'}, {'name': 'ChatDB'}, {'name': 'public-apis'}, {'name': '30-seconds-of-code'}, {'name': 'gpt4free-ts'}, {'name': 'AI-For-Beginners'}, {'name': 'ledger'}, {'name': 'db'}, {'name': 'alpaca-lora'}, {'name': 'FastChat'}, {'name': 'LoRA'}, {'name': 'GPT4Tools'}, {'name': 'Awesome-Multimodal-Large-Language-Models'}, {'name': 'devops-exercises'}, {'name': 'fastapi'}, {'name': 'toolformer-pytorch'}, {'name': 'nucliadb'}, {'name': 'God-Level-Data-Science-ML-Full-Stack'}, {'name': 'blink'}, {'name': 'femtoGPT'}, {'name': 'mlc-llm'}, {'name': 'MeZO'}, {'name': 'Voyager'}, {'name': 'CodeTF'}, {'name': 'evals'}, {'name': 'gpt4free'}, {'name': 'daisyui'}, {'name': 'nvim-lspconfig'}, {'name': 'SuperAGI'}, {'name': 'localGPT'}, {'name': 'gpt4all'}, {'name': 'helicone'}, {'name': 'skip_gram'}, {'name': 'trpc'}, {'name': 'deeplake'}, {'name': 'lancedb'}, {'name': 'timely-dataflow'}, {'name': 'kafka'}, {'name': 'debezium'}, {'name': 'zookeeper'}, {'name': 'FigmaChain'}, {'name': 'NeMo-Guardrails'}, {'name': 'notion-qa'}, {'name': 'azure-search-openai-demo'}, {'name': 'ChatFiles'}, {'name': 'paper-qa'}, {'name': 'myGPTReader'}, {'name': 'ColossalAI'}, {'name': 'docarray'}, {'name': 'txtai'}, {'name': 'realtime'}, {'name': 'bottledwater-pg'}, {'name': 'databus'}, {'name': 'semantic-kernel'}, {'name': 'cognitive-search-vector-pr'}, {'name': 'open-source-alternatives'}, {'name': 'flash-attention'}, {'name': 'OpenSearch'}, {'name': 'babyagi'}, {'name': 'RedPajama-Data'}, {'name': 'dust'}, {'name': 'guardrails'}, {'name': 'langflow'}, {'name': 'fairseq'}, {'name': 'joshuto'}, {'name': 'comprehensive-rust'}, {'name': 'unstructured'}, {'name': 'mindsdb'}, {'name': 'llama-hub'}, {'name': 'sqlglot'}, {'name': 'google-research'}, {'name': 'nmslib'}, {'name': 'trogon'}, {'name': 'psychic'}, {'name': 'DB-GPT'}, {'name': 'next-enterprise'}, {'name': 'AgentGPT'}, {'name': 'awesome-langchain'}, {'name': 'awesome-mlops'}, {'name': 'Prompt-Engineering-Guide'}, {'name': 'the-algorithm'}, {'name': 'llama_index'}, {'name': 'annoy'}, {'name': 'faiss'}, {'name': 'hachi'}, {'name': 'SemanticFinder'}, {'name': 'pgvector'}, {'name': 'marqo'}, {'name': 'getting-started'}, {'name': 'GPTCache'}, {'name': 'minio'}, {'name': 'hnswlib'}, {'name': 'chroma'}, {'name': 'ImHex'}, {'name': 'menubar'}, {'name': 'developer'}, {'name': 'papers-we-love'}, {'name': 'guidance'}, {'name': 'quivr'}, {'name': 'awesome-incident-response'}, {'name': 'privateGPT'}, {'name': 'open-llms'}, {'name': 'shap-e'}, {'name': 'malloy'}, {'name': 'meilisearch'}, {'name': 'roapi'}, {'name': 'vector'}, {'name': 'polars'}, {'name': 'arrow-datafusion'}, {'name': 'phoenix'}, {'name': 'Flowise'}, {'name': 'Mr.-Ranedeer-AI-Tutor'}, {'name': 'drizzle-orm'}, {'name': 'pandas-ai'}, {'name': 'fauxpilot'}, {'name': 'tabby'}, {'name': 'evadb'}, {'name': 'helm'}, {'name': 'dbeaver'}, {'name': 'code-narrator'}, {'name': 'vscode-dbt-power-user'}, {'name': 'edgedb'}, {'name': 'ruff'}, {'name': 'langchain'}, {'name': 'uptrain'}, {'name': 'tableflow'}, {'name': 'ML-Papers-of-the-Week'}, {'name': 'JARVIS'}, {'name': 'Auto-GPT'}, {'name': 'openai-cookbook'}, {'name': 'stanford_alpaca'}, {'name': 'dolly'}, {'name': 'cleanlab'}, {'name': 'chatgpt-retrieval-plugin'}, {'name': 'deepchecks'}, {'name': 'dactyl-manuform'}, {'name': 'firenvim'}, {'name': 'chaos_genius'}, {'name': 'vim-commentary'}, {'name': 'kickstart.nvim'}, {'name': 'lsp-zero.nvim'}, {'name': 'telescope.nvim'}, {'name': 'packer.nvim'}, {'name': 'init.lua'}, {'name': 'win32yank'}, {'name': 'nvim-lua-conf'}, {'name': 'config'}, {'name': 'lago'}, {'name': 'prophet'}, {'name': 'vim-easymotion'}, {'name': 'vscode-neovim'}, {'name': 'neovim'}, {'name': 'kiteco-public'}, {'name': 'atlas'}, {'name': 'data-diff'}, {'name': 'signoz'}, {'name': 'mojo'}, {'name': 'AppFlowy'}, {'name': 'pg_jsonschema'}, {'name': 'whale'}, {'name': 'OpenMetadata'}, {'name': 'schema-registry'}, {'name': 'ngraph'}, {'name': '3d-force-graph'}, {'name': 'antlr4'}, {'name': 'calcite'}, {'name': 'mo-sql-parsing'}, {'name': 'zetasql'}, {'name': 'sqlfluff'}]))
+# print(len([{'name': 'companion-app'}, {'name': 'chatgpt.js'}, {'name': 'long_llama'}, {'name': 'htmx'}, {'name': 'scipy2023-deeplearning'}, {'name': 'gpt-researcher'}, {'name': 'The-Art-of-Linear-Algebra'}, {'name': 'gpt-prompt-engineer'}, {'name': 'Plan-and-Solve-Prompting'}, {'name': 'engine'}, {'name': 'simpleaichat'}, {'name': 'litechain'}, {'name': 'superagent'}, {'name': 'gorilla'}, {'name': 'gorilla-cli'}, {'name': 'tinyvector'}, {'name': 'valmi-activation'}, {'name': 'gpt-migrate'}, {'name': 'lemonai-server'}, {'name': 'lemonai-analytics'}, {'name': 'lemonai'}, {'name': 'ai-jsx'}, {'name': 'spacedrive'}, {'name': 'composer'}, {'name': 'chathn'}, {'name': 'kaguya'}, {'name': 'docs'}, {'name': 'openpm'}, {'name': 'workgpt'}, {'name': 'pepy'}, {'name': 'awesome-selfhosted'}, {'name': 'WizardLM'}, {'name': 'novel'}, {'name': 'OpenChat'}, {'name': 'ai'}, {'name': 'vllm'}, {'name': 'nix.dev'}, {'name': 'OpenLLM'}, {'name': 'poop'}, {'name': 'LLaMA-Efficient-Tuning'}, {'name': 'camel'}, {'name': 'tauri'}, {'name': 'machine-learning-for-trading'}, {'name': 'FinGPT'}, {'name': 'isle'}, {'name': 'FlagAI'}, {'name': 'gpt-engineer'}, {'name': 'plugnplai'}, {'name': 'cypress'}, {'name': 'bloop'}, {'name': 'listmonk'}, {'name': 'lodash'}, {'name': 'pnpm'}, {'name': 'turbo'}, {'name': 'fresh'}, {'name': 'prisma'}, {'name': 'qwik'}, {'name': 'deno'}, {'name': 'kit'}, {'name': 'astro'}, {'name': 'bun'}, {'name': 'tensor2tensor'}, {'name': 'ggml'}, {'name': 'axodox-machinelearning'}, {'name': 'onnxruntime'}, {'name': 'alphadev'}, {'name': 'ChatDB'}, {'name': 'public-apis'}, {'name': '30-seconds-of-code'}, {'name': 'gpt4free-ts'}, {'name': 'AI-For-Beginners'}, {'name': 'ledger'}, {'name': 'db'}, {'name': 'alpaca-lora'}, {'name': 'FastChat'}, {'name': 'LoRA'}, {'name': 'GPT4Tools'}, {'name': 'Awesome-Multimodal-Large-Language-Models'}, {'name': 'devops-exercises'}, {'name': 'fastapi'}, {'name': 'toolformer-pytorch'}, {'name': 'nucliadb'}, {'name': 'God-Level-Data-Science-ML-Full-Stack'}, {'name': 'blink'}, {'name': 'femtoGPT'}, {'name': 'mlc-llm'}, {'name': 'MeZO'}, {'name': 'Voyager'}, {'name': 'CodeTF'}, {'name': 'evals'}, {'name': 'gpt4free'}, {'name': 'daisyui'}, {'name': 'nvim-lspconfig'}, {'name': 'SuperAGI'}, {'name': 'localGPT'}, {'name': 'gpt4all'}, {'name': 'helicone'}, {'name': 'skip_gram'}, {'name': 'trpc'}, {'name': 'deeplake'}, {'name': 'lancedb'}, {'name': 'timely-dataflow'}, {'name': 'kafka'}, {'name': 'debezium'}, {'name': 'zookeeper'}, {'name': 'FigmaChain'}, {'name': 'NeMo-Guardrails'}, {'name': 'notion-qa'}, {'name': 'azure-search-openai-demo'}, {'name': 'ChatFiles'}, {'name': 'paper-qa'}, {'name': 'myGPTReader'}, {'name': 'ColossalAI'}, {'name': 'docarray'}, {'name': 'txtai'}, {'name': 'realtime'}, {'name': 'bottledwater-pg'}, {'name': 'databus'}, {'name': 'semantic-kernel'}, {'name': 'cognitive-search-vector-pr'}, {'name': 'open-source-alternatives'}, {'name': 'flash-attention'}, {'name': 'OpenSearch'}, {'name': 'babyagi'}, {'name': 'RedPajama-Data'}, {'name': 'dust'}, {'name': 'guardrails'}, {'name': 'langflow'}, {'name': 'fairseq'}, {'name': 'joshuto'}, {'name': 'comprehensive-rust'}, {'name': 'unstructured'}, {'name': 'mindsdb'}, {'name': 'llama-hub'}, {'name': 'sqlglot'}, {'name': 'google-research'}, {'name': 'nmslib'}, {'name': 'trogon'}, {'name': 'psychic'}, {'name': 'DB-GPT'}, {'name': 'next-enterprise'}, {'name': 'AgentGPT'}, {'name': 'awesome-langchain'}, {'name': 'awesome-mlops'}, {'name': 'Prompt-Engineering-Guide'}, {'name': 'the-algorithm'}, {'name': 'llama_index'}, {'name': 'annoy'}, {'name': 'faiss'}, {'name': 'hachi'}, {'name': 'SemanticFinder'}, {'name': 'pgvector'}, {'name': 'marqo'}, {'name': 'getting-started'}, {'name': 'GPTCache'}, {'name': 'minio'}, {'name': 'hnswlib'}, {'name': 'chroma'}, {'name': 'ImHex'}, {'name': 'menubar'}, {'name': 'developer'}, {'name': 'papers-we-love'}, {'name': 'guidance'}, {'name': 'quivr'}, {'name': 'awesome-incident-response'}, {'name': 'privateGPT'}, {'name': 'open-llms'}, {'name': 'shap-e'}, {'name': 'malloy'}, {'name': 'meilisearch'}, {'name': 'roapi'}, {'name': 'vector'}, {'name': 'polars'}, {'name': 'arrow-datafusion'}, {'name': 'phoenix'}, {'name': 'Flowise'}, {'name': 'Mr.-Ranedeer-AI-Tutor'}, {'name': 'drizzle-orm'}, {'name': 'pandas-ai'}, {'name': 'fauxpilot'}, {'name': 'tabby'}, {'name': 'evadb'}, {'name': 'helm'}, {'name': 'dbeaver'}, {'name': 'code-narrator'}, {'name': 'vscode-dbt-power-user'}, {'name': 'edgedb'}, {'name': 'ruff'}, {'name': 'langchain'}, {'name': 'uptrain'}, {'name': 'tableflow'}, {'name': 'ML-Papers-of-the-Week'}, {'name': 'JARVIS'}, {'name': 'Auto-GPT'}, {'name': 'openai-cookbook'}, {'name': 'stanford_alpaca'}, {'name': 'dolly'}, {'name': 'cleanlab'}, {'name': 'chatgpt-retrieval-plugin'}, {'name': 'deepchecks'}, {'name': 'dactyl-manuform'}, {'name': 'firenvim'}, {'name': 'chaos_genius'}, {'name': 'vim-commentary'}, {'name': 'kickstart.nvim'}, {'name': 'lsp-zero.nvim'}, {'name': 'telescope.nvim'}, {'name': 'packer.nvim'}, {'name': 'init.lua'}, {'name': 'win32yank'}, {'name': 'nvim-lua-conf'}, {'name': 'config'}, {'name': 'lago'}, {'name': 'prophet'}, {'name': 'vim-easymotion'}, {'name': 'vscode-neovim'}, {'name': 'neovim'}, {'name': 'kiteco-public'}, {'name': 'atlas'}, {'name': 'data-diff'}, {'name': 'signoz'}, {'name': 'mojo'}, {'name': 'AppFlowy'}, {'name': 'pg_jsonschema'}, {'name': 'whale'}, {'name': 'OpenMetadata'}, {'name': 'schema-registry'}, {'name': 'ngraph'}, {'name': '3d-force-graph'}, {'name': 'antlr4'}, {'name': 'calcite'}, {'name': 'mo-sql-parsing'}, {'name': 'zetasql'}, {'name': 'sqlfluff'}]))
+
+
+def get_value(curr_dict, target_key):
+    if isinstance(curr_dict, dict):
+        for key, value in curr_dict.items():
+            if key == target_key:
+                return value
+            elif isinstance(value, dict):
+                result = get_value(value, target_key)
+                if result is not None:
+                    return result
+    return None
+
+# Example usage:
+data = {'a': 1, 'b': {'c': 3, 'd': {'e': 4}}}
+
+key_to_find = 'c'
+result = get_value(data, key_to_find)
+if result is not None:
+    print(f"The value for key '{key_to_find}' is: {result}")
+else:
+    print(f"The key '{key_to_find}' was not found in the dictionary.")
```

### Comparing `lemonai-0.1.2/use-case-example.png` & `lemonai-0.1.3/use-case-example.png`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.2/docs/tools.md` & `lemonai-0.1.3/docs/tools.md`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.2/src/lemonai/api_wrapper.py` & `lemonai-0.1.3/src/lemonai/api_wrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -93,16 +93,27 @@
                 else:
                     flattened_list = json_list
 
                 reduced_response = []
                 for i in range(0, len(flattened_list)):
                     reduced_obj = {}
                     for key in key_list:
-                        reduced_obj[key] = flattened_list[i][key]
+                        reduced_obj[key] = self._get_value(flattened_list[i], key)
                     
                     reduced_response.append(reduced_obj)
             else:
                 reduced_response = {}
                 for key in key_list:
-                    reduced_response[key] = json_list[key]
+                    reduced_response[key] = self._get_value(json_list, key)
 
             return reduced_response
+
+    def _get_value(self, curr_dict, target_key):
+        if isinstance(curr_dict, dict):
+            for key, value in curr_dict.items():
+                if key == target_key:
+                    return value
+                elif isinstance(value, dict):
+                    result = self._get_value(value, target_key)
+                    if result is not None:
+                        return result
+        return None
```

### Comparing `lemonai-0.1.2/src/lemonai/execute_workflow.py` & `lemonai-0.1.3/src/lemonai/execute_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     api_keys_dict, access_tokens_dict = get_apis_from_env()
     session_id = uuid.uuid4()
 
     _wrapper = APIWrapper(llm, task=prompt_string, api_domain=server_domain)
     toolkit = Toolkit.from_api_wrapper(_wrapper, api_keys_dict, access_tokens_dict, logger, str(session_id))
     tools = toolkit.get_tools()
 
-    prompt = f"Your task is '{prompt_string}'. Focus on the ordering of the tasks given. Do not use a workflow unless it is mentioned. Your action input should be a valid JSON object where the keys are the params and the values are the value for each input parameter. The description of the tool may provide the JSON structure of the action input using round brackets () instead of curly brackets. Follow this structure for your action input. Ensure all strings in the action input are valid and terminated correctly. Your final answer should give a brief conversational overview of what you did."    
+    prompt = f"Your task is '{prompt_string}'. Focus on the ordering of the tasks given. Do not use a workflow unless it is mentioned. Your action input should be a complete and valid JSON object where the keys are the params and the values are the value for each input parameter. The description of the tool may provide the JSON structure of the action input using round brackets () instead of curly brackets. Follow this structure for your action input. Ensure all strings in the action input are valid and terminated correctly. Your final answer should give a brief conversational overview of what you did."    
     filtered_tools = filter_tools(llm=llm, task=prompt_string, tools=tools)
     
     agent = initialize_agent(
         tools=filtered_tools,
         llm=llm,
         agent=AgentType.ZERO_SHOT_REACT_DESCRIPTION,
         verbose=True
```

### Comparing `lemonai-0.1.2/src/lemonai/filter_tools.py` & `lemonai-0.1.3/src/lemonai/filter_tools.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.2/src/lemonai/get_integrations.py` & `lemonai-0.1.3/src/lemonai/get_integrations.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.2/src/lemonai/tool.py` & `lemonai-0.1.3/src/lemonai/tool.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.2/src/lemonai/toolkit.py` & `lemonai-0.1.3/src/lemonai/toolkit.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.2/.gitignore` & `lemonai-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.2/LICENSE` & `lemonai-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.2/README.md` & `lemonai-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lemonai-0.1.2/pyproject.toml` & `lemonai-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lemonai"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Felix Brockmeier", email="fe.brockmeier@gmail.com" },
 ]
 description = "Lemon AI's A Python client. Grant your LLM agents access to a wide range of APIs for read and write operations, creating copilots in minutes and unlocking the true potential of LLMs."
 readme = "README.md"
 requires-python = ">=3.8.1"
 classifiers = [
```

### Comparing `lemonai-0.1.2/PKG-INFO` & `lemonai-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemonai
-Version: 0.1.2
+Version: 0.1.3
 Summary: Lemon AI's A Python client. Grant your LLM agents access to a wide range of APIs for read and write operations, creating copilots in minutes and unlocking the true potential of LLMs.
 Project-URL: Homepage, https://github.com/felixbrock/lemonai-py-client
 Project-URL: Bug Tracker, https://github.com/felixbrock/lemonai-py-client/issues
 Author-email: Felix Brockmeier <fe.brockmeier@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lemonai Version: 0.1.2 Summary: Lemon AI's A Python
+Metadata-Version: 2.1 Name: lemonai Version: 0.1.3 Summary: Lemon AI's A Python
 client. Grant your LLM agents access to a wide range of APIs for read and write
 operations, creating copilots in minutes and unlocking the true potential of
 LLMs. Project-URL: Homepage, https://github.com/felixbrock/lemonai-py-client
 Project-URL: Bug Tracker, https://github.com/felixbrock/lemonai-py-client/
 issues Author-email: Felix Brockmeier
 brockmeier@gmail.com> License-File: LICENSE Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
```

