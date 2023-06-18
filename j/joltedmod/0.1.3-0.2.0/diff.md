# Comparing `tmp/joltedmod-0.1.3.tar.gz` & `tmp/joltedmod-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joltedmod-0.1.3.tar", max compression
+gzip compressed data, was "joltedmod-0.2.0.tar", max compression
```

## Comparing `joltedmod-0.1.3.tar` & `joltedmod-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1101 2023-06-01 12:22:59.095108 joltedmod-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2023-06-01 12:51:13.405416 joltedmod-0.1.3/README.md
--rw-r--r--   0        0        0      311 2023-06-01 13:03:57.935186 joltedmod-0.1.3/jolted_mod/__init__.py
--rw-r--r--   0        0        0     3108 2023-06-05 06:39:34.991191 joltedmod-0.1.3/jolted_mod/block.py
--rw-r--r--   0        0        0      569 2023-06-01 12:59:00.270039 joltedmod-0.1.3/jolted_mod/block_factory.py
--rw-r--r--   0        0        0       91 2023-06-01 12:22:59.233084 joltedmod-0.1.3/jolted_mod/cell_type.py
--rw-r--r--   0        0        0      890 2023-06-05 06:48:24.698768 joltedmod-0.1.3/jolted_mod/config.py
--rw-r--r--   0        0        0     7706 2023-06-05 06:44:15.371897 joltedmod-0.1.3/jolted_mod/content_generator.py
--rw-r--r--   0        0        0     4014 2023-06-05 07:00:49.244856 joltedmod-0.1.3/jolted_mod/main.py
--rw-r--r--   0        0        0     7264 2023-06-05 07:04:40.600941 joltedmod-0.1.3/jolted_mod/template_generator.py
--rw-r--r--   0        0        0      649 2023-06-05 07:07:18.545347 joltedmod-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 joltedmod-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-06-01 12:22:59.095108 joltedmod-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2012 2023-06-18 07:56:10.874764 joltedmod-0.2.0/README.md
+-rw-r--r--   0        0        0     1344 2023-06-17 15:04:17.835987 joltedmod-0.2.0/jolted_mod/LLM_service.py
+-rw-r--r--   0        0        0      311 2023-06-01 13:03:57.935186 joltedmod-0.2.0/jolted_mod/__init__.py
+-rw-r--r--   0        0        0     3749 2023-06-18 08:19:58.255349 joltedmod-0.2.0/jolted_mod/block.py
+-rw-r--r--   0        0        0      606 2023-06-18 08:18:31.554627 joltedmod-0.2.0/jolted_mod/block_factory.py
+-rw-r--r--   0        0        0       91 2023-06-01 12:22:59.233084 joltedmod-0.2.0/jolted_mod/cell_type.py
+-rw-r--r--   0        0        0     1934 2023-06-17 17:42:19.311605 joltedmod-0.2.0/jolted_mod/config.py
+-rw-r--r--   0        0        0     7925 2023-06-18 08:24:25.496650 joltedmod-0.2.0/jolted_mod/content_generator.py
+-rw-r--r--   0        0        0     4855 2023-06-18 08:25:07.509677 joltedmod-0.2.0/jolted_mod/main.py
+-rw-r--r--   0        0        0       93 2023-06-17 15:54:34.751488 joltedmod-0.2.0/jolted_mod/module_types.py
+-rw-r--r--   0        0        0     9644 2023-06-18 08:09:02.777342 joltedmod-0.2.0/jolted_mod/template_generator.py
+-rw-r--r--   0        0        0      685 2023-06-18 08:26:33.718197 joltedmod-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 joltedmod-0.2.0/PKG-INFO
```

### Comparing `joltedmod-0.1.3/LICENSE` & `joltedmod-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joltedmod-0.1.3/jolted_mod/block_factory.py` & `joltedmod-0.2.0/jolted_mod/block_factory.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-from jolted_mod.block import Block, SeedBlock, ExplanatoryBlock, KnowledgeTestingBlock
+from jolted_mod.block import (
+    Block,
+    SeedBlock,
+    ExplanatoryBlock,
+    KnowledgeTestingBlock,
+)
+
 
 class BlockFactory:
     BLOCK_TYPES = {
-        'SeedBlock': SeedBlock,
-        'ExplanatoryBlock': ExplanatoryBlock,
-        'KnowledgeTestingBlock': KnowledgeTestingBlock,
+        "SEED_BLOCK": SeedBlock,
+        "EXPLANATORY_BLOCK": ExplanatoryBlock,
+        "KNOWLEDGE_TESTING_BLOCK": KnowledgeTestingBlock,
     }
-    
+
     @staticmethod
-    def create_block(block_config):
-        block_type = block_config['type']
+    def create_block(block_config: dict) -> Block:
+        block_type = block_config["type"]
         block_class = BlockFactory.BLOCK_TYPES.get(block_type)
         if not block_class:
             raise ValueError(f"Invalid block type: {block_type}")
         return block_class(**block_config)
```

### Comparing `joltedmod-0.1.3/jolted_mod/config.py` & `joltedmod-0.2.0/jolted_mod/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,18 @@
 prompts = {
-    "SeedBlock": "Behave as a {identity} who is explaining {topic} to {target_audience}",
-    "ExplanatoryBlock": "This is a {type_of_cell} block in a Jupyter Notebook. Use appropriate headers for chapter sections if of type Markdown. Do not give solutions if this is a Code block. Explain {topic} by {method_of_teaching} in a way that is relatable to {target_audience}. Be careful not to be overly dramatic and not to talk down to the audience.",
+    "SeedBlock": "Produce output for a textbook or tutorial module as written by a {identity} who is explaining {topic} to {target_audience}",
+
+    "ExplanatoryBlock": "This is a {type_of_cell} block in a Jupyter Notebook. Use appropriate headers for chapter sections if of type Markdown. Do not give solutions if this is a Code block. Explain {topic} by {instructional_event} in a way that is relatable to {target_audience}. Be careful not to be overly dramatic and not to talk down to the audience.",
+
+    "ExplanatoryBlockKC": "You are producing a jupyter notebook based tutorial for {target_audience} about {knowledge_component} by {instructional_event}. Assume your output is part of a tutorial that covers the other aspects of {topic}. DO NOT REPEAT AN INTRODUCTION, SUMMARY, OR ANY OTHER CONTENT. ONLY PRODUCE CONTENT ON {knowledge_component}",
+
     "KnowledgeTestingBlock": {
         "markdown": "Design {n} {question_type} of an appropriate difficulty for {target_audience} about that {topic}",
-        "code": "Create code with empty methods that have comments for what they should do but no implementation to answer the following question: {context_content}. After that, create 3 assertion tests that the student will use to test if they have implemented their",
+        "code": "Create code with empty methods that have comments for what they should do but no implementation to answer the following question: {context_content}. After that, create 3 assertion tests that the student will use to test if they have implemented their solution correctly",
     },
+
+    "KnowledgeTestingBlockKC": {
+        "markdown": "Design {n} {question_type} of an appropriate difficulty for {target_audience} about that {knowledge_component}. Do not produce a solution, just the question. DO NOT REPEAT AN INTRODUCTION, SUMMARY, OR ANY OTHER CONTENT. ONLY PRODUCE CONTENT ON {knowledge_component}",
+        "code": "Create code with empty methods that have comments for what they should do but no implementation to answer the following question: {context_content}. After that, create 3 assertion tests that the student will use to test if they have implemented their solution correctly",
+    },
+
 }
```

### Comparing `joltedmod-0.1.3/jolted_mod/content_generator.py` & `joltedmod-0.2.0/jolted_mod/content_generator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,137 +1,172 @@
-import os
-import openai
-import asyncio
-import time
+from typing import List, Tuple, Any, Optional
 import aiohttp
 import aiofiles
 import nbformat as nbf
-import markdown2
-from markdownify import markdownify as md
-import json
 import uuid
 from alive_progress import alive_bar
 from colorama import Fore, Style
-from jolted_mod.block import Block
+import asyncio
 from jolted_mod.cell_type import CellType
+import openai
+import os
 from jolted_mod.block_factory import BlockFactory
+from jolted_mod.LLM_service import chat_completion_create
+from jolted_mod.block import Block, BLOCK_TYPES
+from jolted_mod.module_types import ModuleType
+
+
+class ContentGeneratorError(Exception):
+    pass
 
 
 class ContentGenerator:
-    def __init__(self, model="gpt-3.5-turbo", system_block=None, max_tokens=1024, n=1, stop=None, temperature=0.7, blocks=None):
+    def __init__(
+        self,
+        model: str = "gpt-3.5-turbo",
+        system_block: Optional[Block] = None,
+        max_tokens: int = 1024,
+        n: int = 1,
+        stop: Any = None,
+        temperature: float = 0.7,
+        blocks: List[Block] = [],
+    ):
         self.model = model
         self.system_block = system_block
         self.max_tokens = max_tokens
         self.n = n
         self.stop = stop
         self.temperature = temperature
         self._set_api_key()
         self.blocks = blocks
 
     def _set_api_key(self):
         """Set OpenAI API key from the environment variable."""
-        openai.api_key = os.environ.get("OPENAI_API_KEY")
-        if not openai.api_key:
-            raise ValueError("Environment variable OPENAI_API_KEY not set")
-
-    async def create_notebook(self, config_file):
-        """Create a Jupyter Notebook file from the given config file."""
-        nb = nbf.v4.new_notebook()
-        blocks = await self.create_content(config_file)
-        await self._generate_notebook_cells(blocks, nb)
-        return nb
-
-    async def create_wiki(self, config_file):
-        """Create a wiki file from the given config file."""
-        blocks = await self.create_content(config_file)
-        return await self._create_markdown_text(blocks)
-
-    async def create_content(self, config_file):
-        """Create content for blocks from the given config file asynchronously."""
-        async with aiohttp.ClientSession() as self._session:
-            blocks = await self._parse_config_file(config_file)
-            await self._update_context(config_file, blocks)
-
-            if blocks[0].type == 'SeedBlock':
-                self.system_block = blocks[0]
-                blocks.pop(0)
+        try:
+            openai.api_key = os.environ.get("OPENAI_API_KEY")
+            if not openai.api_key:
+                raise ValueError("Environment variable OPENAI_API_KEY not set")
+        except Exception as e:
+            raise ContentGeneratorError(f"Failed to set API key: {e}")
+
+    async def create_module(self, config: dict, type: ModuleType) -> Any:
+        """Create a Module of type JupyterNotebook or Wiki (markdown) Notebook from the given config dictionary."""
+        try:
+            blocks = await self._parse_config(config)
+        except Exception as e:
+            raise ContentGeneratorError(f"Failed to parse config: {e}")
+
+        try:
+            await self._update_context(config, blocks)
+        except Exception as e:
+            raise ContentGeneratorError(f"Failed to update context: {e}")
+
+        if blocks[0].type == BLOCK_TYPES.SEED_BLOCK.name:
+            self.system_block = blocks.pop(0)
+
+        try:
+            async with aiohttp.ClientSession() as self._session:
+                blocks = await self._generate_all_block_content(blocks)
+        except Exception as e:
+            raise ContentGeneratorError(f"Failed to generate block content: {e}")
+
+        module: Any
+        try:
+            if type == ModuleType.NOTEBOOK:
+                nb = nbf.v4.new_notebook()
+                module = self._generate_notebook_cells(blocks, nb)
+            elif type == ModuleType.WIKI:
+                module = self._create_markdown_text(blocks)
             else:
-                self.system_block = None
-
-            await self._generate_all_block_content(blocks)
-            return blocks
-
-
-    async def _generate_notebook_cells(self, blocks, nb):
-        """Generate notebook cells from given blocks asynchronously."""
-        for block in blocks:
-            if block.cell_type == CellType.CODE:
-                new_cell = nbf.v4.new_code_cell(block.content)
-                new_cell['id'] = str(uuid.uuid4())  # Generate and set cell id
-                nb.cells.append(new_cell)
-            elif block.cell_type == CellType.MARKDOWN:
-                nb.cells.append(nbf.v4.new_markdown_cell(block.content))
-        return nb
-
-    async def _create_markdown_text(self, blocks):
-        """Create a markdown file from the given blocks."""
-        markdown_text = ""
-        for block in blocks:
-            markdown_text += (block.content)
-        return markdown_text
-
-
-    @staticmethod
-    async def _update_context(config_file, blocks):
-        """Update block context using the given config file asynchronously."""
-        async with aiofiles.open(config_file, mode='r') as f:
-            config = json.loads(await f.read())
-            for block, block_config in zip(blocks, config['blocks']):
-                if 'context' in block_config and block_config['context'] is not None:
-                    block.set_context(blocks[block_config['context']])
-
-    @staticmethod
-    async def _parse_config_file(config_file):
-        """Parse the given config file and create blocks asynchronously."""
-        async with aiofiles.open(config_file, mode='r') as f:
-            config = json.loads(await f.read())
-            blocks = []
-            for block_config in config['blocks']:
+                raise ValueError(f"Invalid module type: {type}")
+        except Exception as e:
+            raise ContentGeneratorError(f"Failed to create module: {e}")
+
+        return module
+
+    async def _parse_config(self, config: dict) -> List[Block]:
+        """Parse the given config dictionary and create blocks asynchronously."""
+        try:
+            blocks: List[Block] = []
+            for block_config in config["blocks"]:
                 block = BlockFactory.create_block(block_config)
                 blocks.append(block)
+
             return blocks
+        except Exception as e:
+            raise ContentGeneratorError(f"Failed to parse config: {e}")
 
-    async def _generate_all_block_content(self, blocks):
+    async def _update_context(self, config: dict, blocks: List[Block]) -> None:
+        """Update block context using the given config dictionary asynchronously."""
+        try:
+            for block, block_config in zip(blocks, config["blocks"]):
+                if "context" in block_config and block_config["context"] is not None:
+                    block.set_context(blocks[block_config["context"]])
+        except Exception as e:
+            raise ContentGeneratorError(f"Failed to update context: {e}")
+
+    async def _generate_all_block_content(self, blocks: List[Block]) -> List[Block]:
         """Generate content for all blocks asynchronously."""
-        dependent_blocks, independent_blocks = self._split_blocks(blocks)
+        try:
+            dependent_blocks, independent_blocks = self._split_blocks(blocks)
 
-        title_color = f"{Fore.CYAN}{Style.BRIGHT}Generating block content{Style.RESET_ALL}"
-        spinner_style = 'waves'
+            spinner_style = "waves"
 
-        with alive_bar(len(blocks), title=title_color, spinner=spinner_style, bar="smooth") as pbar:
-            for block in dependent_blocks:
-                await self.generate_block_content(block)
-                pbar()
-            await asyncio.gather(*[self.generate_block_content(block) for block in independent_blocks])
-            pbar(len(independent_blocks))
+            with alive_bar(len(blocks), spinner=spinner_style, bar="smooth") as pbar:
+                await asyncio.gather(
+                    *[
+                        self.generate_block_content(block)
+                        for block in independent_blocks
+                    ]
+                )
+                pbar(len(independent_blocks))
+                for block in dependent_blocks:
+                    await self.generate_block_content(block)
+                    pbar(len(dependent_blocks))
+            return blocks
+        except Exception as e:
+            raise ContentGeneratorError(f"Failed to generate block content: {e}")
 
-    @staticmethod
-    def _split_blocks(blocks):
+    def _split_blocks(self, blocks: List[Block]) -> Tuple[List[Block], List[Block]]:
         """Split blocks into dependent and independent blocks."""
-        dependent_blocks = [
-            block for block in blocks if block.context is not None]
-        independent_blocks = [
-            block for block in blocks if block.context is None]
+        try:
+            dependent_blocks = [block for block in blocks if block.context is not None]
+            independent_blocks = [block for block in blocks if block.context is None]
+            return dependent_blocks, independent_blocks
+        except Exception as e:
+            raise ContentGeneratorError(f"Failed to split blocks: {e}")
+
+    def _generate_notebook_cells(self, blocks: List[Block], nb: Any) -> Any:
+        """Generate notebook cells from given blocks asynchronously."""
+        try:
+            for block in blocks:
+                if block.cell_type == CellType.CODE:
+                    new_cell = nbf.v4.new_code_cell(block.content)
+                    new_cell["id"] = str(uuid.uuid4())  # Generate and set cell id
+                    nb.cells.append(new_cell)
+                elif block.cell_type == CellType.MARKDOWN:
+                    nb.cells.append(nbf.v4.new_markdown_cell(block.content))
+            return nb
+        except Exception as e:
+            raise ContentGeneratorError(f"Failed to generate notebook cells: {e}")
 
-        return dependent_blocks, independent_blocks
+    def _create_markdown_text(self, blocks: List[Block]) -> str:
+        """Create a markdown file from the given blocks."""
+        try:
+            markdown_text = ""
+            for block in blocks:
+                markdown_text += block.content
+            return markdown_text
+        except Exception as e:
+            raise ContentGeneratorError(f"Failed to create markdown text: {e}")
 
     async def generate_block_content(self, block):
         while True:
             try:
-                response = await self.chat_completion_create(
+                response = await chat_completion_create(
                     session=self._session,
                     model=self.model,
                     messages=[
                         {
                             "role": "system",
                             "content": self.system_block.generate_prompt(),
                         },
@@ -143,48 +178,17 @@
                     temperature=self.temperature,
                 )
                 block.set_content(response["choices"][0]["message"]["content"])
                 break  # If the response was successful, break out of the loop
 
             except Exception as e:
                 if "429" in str(e):  # Check if the error code is 429
-                    wait_time = 60  # You can set this to the desired waiting time in seconds
-                    print(
-                        f"Error 429 encountered. Retrying in {wait_time} seconds...")
-                    # Use asyncio.sleep instead of time.sleep for async code
-                    await asyncio.sleep(wait_time)
-                else:
-                    raise  # If it's another exception, raise it as usual
-
-    @staticmethod
-    async def chat_completion_create(session, model, messages, max_tokens, n, stop, temperature):
-        url = f"https://api.openai.com/v1/chat/completions"
-        headers = {
-            "Content-Type": "application/json",
-            "Authorization": f"Bearer {openai.api_key}",
-        }
-
-        data = {
-            "model": model,
-            "messages": messages,
-            "max_tokens": max_tokens,
-            "n": n,
-            "stop": stop,
-            "temperature": temperature,
-        }
-
-        while True:
-            try:
-                async with session.post(url, headers=headers, json=data) as response:
-                    if response.status != 200:
-                        raise Exception(f"Error: {response.status}, {await response.text()}")
-                    return await response.json()
-
-            except Exception as e:
-                if "429" in str(e):  # Check if the error code is 429
-                    wait_time = 60  # You can set this to the desired waiting time in seconds
-                    print(
-                        f"Error 429 encountered. Retrying in {wait_time} seconds...")
+                    wait_time = (
+                        60  # You can set this to the desired waiting time in seconds
+                    )
+                    print(f"Error 429 encountered. Retrying in {wait_time} seconds...")
                     # Use asyncio.sleep instead of time.sleep for async code
                     await asyncio.sleep(wait_time)
                 else:
-                    raise  # If it's another exception, raise it as usual
+                    raise ContentGeneratorError(
+                        f"Failed to generate block content: {e}"
+                    )  # If it's another exception, raise it as ContentGeneratorError
```

### Comparing `joltedmod-0.1.3/pyproject.toml` & `joltedmod-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "JoltEdMod"
-version = "0.1.3"
+version = "0.2.0"
 description = "JoltEd self-documenting learning module"
 authors = ["Nathan Laundry"]
 license = "MIT" 
 readme = "README.md"
 packages = [{include = "jolted_mod"}]
 
 [tool.poetry.dependencies]
@@ -13,14 +13,16 @@
 nbformat = "^5.8.0"
 markdown2 = "^2.4.8"
 markdownify = "^0.11.6"
 tqdm = "^4.65.0"
 aiofiles = "^23.1.0"
 alive-progress = "^3.1.3"
 colorama = "^0.4.6"
+nbf = "^0.0.5"
+pydantic = "^1.10.9"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 
 [build-system]
```

