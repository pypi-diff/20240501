# Comparing `tmp/helpful_assistant-0.0.9.tar.gz` & `tmp/helpful_assistant-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helpful_assistant-0.0.9.tar", last modified: Mon Apr 22 23:40:26 2024, max compression
+gzip compressed data, was "helpful_assistant-0.1.0.tar", last modified: Wed May  1 01:41:32 2024, max compression
```

## Comparing `helpful_assistant-0.0.9.tar` & `helpful_assistant-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:40:26.666676 helpful_assistant-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-04-22 23:40:22.000000 helpful_assistant-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-22 23:40:26.666676 helpful_assistant-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-22 23:40:22.000000 helpful_assistant-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-22 23:40:22.000000 helpful_assistant-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:40:26.666676 helpful_assistant-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:40:26.662676 helpful_assistant-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:40:26.662676 helpful_assistant-0.0.9/src/helpful_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-22 23:40:22.000000 helpful_assistant-0.0.9/src/helpful_assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-22 23:40:22.000000 helpful_assistant-0.0.9/src/helpful_assistant/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-04-22 23:40:22.000000 helpful_assistant-0.0.9/src/helpful_assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-22 23:40:22.000000 helpful_assistant-0.0.9/src/helpful_assistant/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-22 23:40:22.000000 helpful_assistant-0.0.9/src/helpful_assistant/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-22 23:40:22.000000 helpful_assistant-0.0.9/src/helpful_assistant/module.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-22 23:40:22.000000 helpful_assistant-0.0.9/src/helpful_assistant/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:40:26.666676 helpful_assistant-0.0.9/src/helpful_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-22 23:40:26.000000 helpful_assistant-0.0.9/src/helpful_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-22 23:40:26.000000 helpful_assistant-0.0.9/src/helpful_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:40:26.000000 helpful_assistant-0.0.9/src/helpful_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 23:40:26.000000 helpful_assistant-0.0.9/src/helpful_assistant.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:41:32.026998 helpful_assistant-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-05-01 01:41:27.000000 helpful_assistant-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-01 01:41:32.026998 helpful_assistant-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-01 01:41:27.000000 helpful_assistant-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-01 01:41:27.000000 helpful_assistant-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 01:41:32.026998 helpful_assistant-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:41:32.022998 helpful_assistant-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:41:32.026998 helpful_assistant-0.1.0/src/helpful_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-01 01:41:27.000000 helpful_assistant-0.1.0/src/helpful_assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-01 01:41:27.000000 helpful_assistant-0.1.0/src/helpful_assistant/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9092 2024-05-01 01:41:27.000000 helpful_assistant-0.1.0/src/helpful_assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-01 01:41:27.000000 helpful_assistant-0.1.0/src/helpful_assistant/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-01 01:41:27.000000 helpful_assistant-0.1.0/src/helpful_assistant/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-01 01:41:27.000000 helpful_assistant-0.1.0/src/helpful_assistant/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-01 01:41:27.000000 helpful_assistant-0.1.0/src/helpful_assistant/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:41:32.026998 helpful_assistant-0.1.0/src/helpful_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-01 01:41:32.000000 helpful_assistant-0.1.0/src/helpful_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-01 01:41:32.000000 helpful_assistant-0.1.0/src/helpful_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 01:41:32.000000 helpful_assistant-0.1.0/src/helpful_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 01:41:32.000000 helpful_assistant-0.1.0/src/helpful_assistant.egg-info/top_level.txt
```

### Comparing `helpful_assistant-0.0.9/LICENSE` & `helpful_assistant-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `helpful_assistant-0.0.9/PKG-INFO` & `helpful_assistant-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helpful-assistant
-Version: 0.0.9
+Version: 0.1.0
 Summary: Allows LLMs to assist you with various tasks, all while being open-source!
 Author: Whitelisted
 Project-URL: Homepage, https://github.com/Whitelisted1/Helpful-Assistant
 Project-URL: Issues, https://github.com/Whitelisted1/Helpful-Assistant/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `helpful_assistant-0.0.9/README.md` & `helpful_assistant-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `helpful_assistant-0.0.9/pyproject.toml` & `helpful_assistant-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "helpful-assistant"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Whitelisted" },
 ]
 description = "Allows LLMs to assist you with various tasks, all while being open-source!"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `helpful_assistant-0.0.9/src/helpful_assistant/assistant.py` & `helpful_assistant-0.1.0/src/helpful_assistant/assistant.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,34 +9,45 @@
 from .events import EventManager
 
 if TYPE_CHECKING:
     from .action import Action
 
 
 class Assistant:
-    def __init__(self, llm_class: object, *args, **kwargs) -> None:
+    def __init__(self, llm_class: object, allow_conversation_history_modification: bool = False, *args, **kwargs) -> None:
+        """
+        Initializes a new Assistant instance.
+
+        Parameters:
+        llm_class (object): The class of the LLM which is used to generate model output.
+        allow_conversation_history_modification (bool, defaults to False): Allows or disallows the local modification of any Conversation's past messages. If using a back-and-forth API, set this to False.
+        """
+
         self.llm = llm_class
+        self.allow_conversation_history_modification = allow_conversation_history_modification
+
         self.conversation_list: List[Conversation] = []
         self.module_list: List[Module] = []
         self.event_manager = EventManager()
 
     def get_system_message(self) -> str:
         return 'This application has different modules and actions. Modules contain actions, and are simply categorizers. Actions are able to be run and return information.\n\nDo not talk about how you are unable to return real-time information. You must ONLY use modules and actions provided in this conversation. Do not assume there are actions available to you, unless provided in this conversation.'
 
     def new_conversation(self, name: str = "Conversation", history: Optional[List[Message]] = None) -> Conversation:
         """
         Creates a new conversation.
 
         Parameters:
         name (str, optional, defaults to "Conversation"): The name to the conversation.
-        history (list of messages, optional, defaults to None.): A list of messages in the current conversation.
+        history (list of messages, optional, defaults to None): A list of messages in the current conversation.
 
         Returns:
         Conversation: A new conversation instance.
         """
+
         c = Conversation(name=name, history=history, assistant=self)
         self.conversation_list.append(c)
         return c
 
     def remove_conversation(self, conversation: Conversation) -> None:
         """
         Removes a conversation from the conversation list. Calls the conversation's `discard` function.
@@ -44,28 +55,29 @@
         Parameters:
         conversation (Conversation): The conversation to remove and discard.
         """
 
         self.event_manager.trigger_event("conversation_discard", conversation)
         self.conversation_list.remove(conversation)
 
-
     def add_module(self, module: Module) -> None:
         """
         Appends a module to the Assistant object.
 
         Parameters:
         module (Module): A Module object to append to the assistant's module list.
         """
+
         self.module_list.append(module)
 
     def convert_modules_to_llm_readable(self) -> str:
         """
         Converts modules to the format given to the LLM.
         """
+
         return "\n".join([f"{module.name} ({module.definition})" for module in self.module_list])
 
     def generate(self, conversation: Conversation, stream: bool = False, allow_action_execution: bool = True) -> Union[Stream, str]:
         """
         Generates content from an LLM.
 
         Parameters:
@@ -73,27 +85,35 @@
         stream (bool, optional, defaults to False): Should the output be returned as a generator.
         allow_action_execution (bool, defaults to True): Allow for actions to be executed by the LLM.
 
         Returns:
         Union[Stream, str]: A Stream object or a string depending on the stream parameter. The output from the LLM.
         """
 
-        generation_conversation = self.new_conversation(history=copy.deepcopy(conversation.history))
+        # if we are allowing the modification of conversation histories, then make a copy which we will modify
+        # otherwise, just use the original conversation
+        if self.allow_conversation_history_modification:
+            generation_conversation = self.new_conversation(history=copy.deepcopy(conversation.history))
+        else:
+            generation_conversation = conversation
 
         if allow_action_execution:
             # execute a task, if needed, and add that information to the covnersation
             task_output, used_module, used_action = self._app_action_cycle(conversation)
 
-            # if the task actually ran append it to user input
+            # if the task actually ran then set it for the message
             if task_output is not None:
-                generation_conversation.history[-1].content += f"\n\n(An action was run. Action Output: ```{task_output}```. Use this output in your response, if applicable.)"
+                generation_conversation.history[-1].set_action_output(f"(An action was run. Action Output: ```{task_output}```. Use this output in your response, if applicable)")
 
         def conversation_callback(x):
             conversation._add_to_history(Message("assistant", "".join(x)))
-            generation_conversation.discard()
+
+            # don't discard this conversation if it is not a copy
+            if self.allow_conversation_history_modification:
+                generation_conversation.discard()
 
         # Make a Stream object that adds the generation result to history once it has completed
         output = Stream(self.llm.generate(generation_conversation, stream=stream), conversation_callback)
 
         # return the Stream object
         return output
 
@@ -105,18 +125,18 @@
         conversation (Conversation): The Conversation object in which to get data from
 
         Returns:
         List[Union[str, None], Union[Module, None], Union[Action, None]]: The output from the action run, the module used, and the action run.
         """
 
         # create a new conversation
-        action_conversation = self.new_conversation(history=[Message("system", f'This application has different modules and actions. Here are your available modules:\n\n{self.convert_modules_to_llm_readable()}\n\nYou must only use the provided modules and actions in this conversation.')])
+        action_conversation = self.new_conversation(history=[Message("system", f'This application has different modules and actions. Here are your available modules:\n```\n{self.convert_modules_to_llm_readable()}\n```\nYou must only use the provided modules and actions in this conversation.')])
 
-        # split conversation history into newlines, excluding the system prompt
-        user_message_history = "\n".join(f"{m.role}: {m.content}" for m in conversation.get_by_role("user"))
+        # split conversation history into newlines, excluding the action outputs
+        user_message_history = "\n".join(f"{m.role}: {m.get_content(include_action_output=False)}" for m in conversation.get_by_role("user"))
 
         # Make a prompt for the model to choose a module
         modules_prompt = f'''Given the user prompts, respond with the name of the module you want to learn more about. Only use modules relevant to the latest user message. Respond with "null" if none apply.\n\n```\n{user_message_history}\n```'''
         action_conversation.history.append(Message("user", modules_prompt))
 
 
         # Get the model output and append it to conversation_history
```

### Comparing `helpful_assistant-0.0.9/src/helpful_assistant/conversation.py` & `helpful_assistant-0.1.0/src/helpful_assistant/conversation.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,14 +6,21 @@
     from .assistant import Assistant
 
 
 class Message:
     def __init__(self, role: str, content: str) -> None:
         self.role = role
         self.content = content
+        self.action_output: Union[str, None] = None
+
+    def set_action_output(self, action_output: str):
+        self.action_output = action_output
+
+    def get_content(self, include_action_output=True):
+        return self.content + (("\n\n" + self.action_output) if self.action_output is not None and include_action_output else "")
 
     def __str__(self) -> str:
         return self.content
 
 
 class Conversation:
     def __init__(self, name: str = "Conversation", history: Optional[List[Message]] = None, assistant: Optional[Assistant] = None) -> None:
```

### Comparing `helpful_assistant-0.0.9/src/helpful_assistant/events.py` & `helpful_assistant-0.1.0/src/helpful_assistant/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         """
         Trigger an event given an event name and data for the listeners.
 
         Parameters:
         event_name (str): Name of the event.
         event_data (object): The event data which will be passed to the listeners.
         """
+
         # if the event does not have any listeners then stop
         if event_name not in self.listeners:
             return
 
         # call the listeners
         for callback in self.listeners[event_name]:
             callback(event_data)
```

### Comparing `helpful_assistant-0.0.9/src/helpful_assistant/module.py` & `helpful_assistant-0.1.0/src/helpful_assistant/module.py`

 * *Files identical despite different names*

### Comparing `helpful_assistant-0.0.9/src/helpful_assistant.egg-info/PKG-INFO` & `helpful_assistant-0.1.0/src/helpful_assistant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helpful-assistant
-Version: 0.0.9
+Version: 0.1.0
 Summary: Allows LLMs to assist you with various tasks, all while being open-source!
 Author: Whitelisted
 Project-URL: Homepage, https://github.com/Whitelisted1/Helpful-Assistant
 Project-URL: Issues, https://github.com/Whitelisted1/Helpful-Assistant/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

