# Comparing `tmp/Omnicon_DDSDocGen-2.1.1-0-cp37-cp37m-win_amd64.whl.zip` & `tmp/Omnicon_DDSDocGen-2.2.1-0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,19 @@
-Zip file size: 57510 bytes, number of entries: 18
+Zip file size: 51986 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat     2039 b- defN 22-Nov-17 05:41 Omnicon_DDSDocGen/DocGenInterface.py
--rw-rw-rw-  2.0 fat    35463 b- defN 23-Mar-15 19:02 Omnicon_DDSDocGen/DocGenLogic.py
+-rw-rw-rw-  2.0 fat    35235 b- defN 23-Jun-18 07:10 Omnicon_DDSDocGen/DocGenLogic.py
 -rw-rw-rw-  2.0 fat    10756 b- defN 23-Mar-13 18:48 Omnicon_DDSDocGen/DocxGen.py
 -rw-rw-rw-  2.0 fat      884 b- defN 23-Mar-13 18:48 Omnicon_DDSDocGen/ErrorListHandler.py
 -rw-rw-rw-  2.0 fat    12992 b- defN 23-Mar-13 18:48 Omnicon_DDSDocGen/LatexGen.py
--rw-rw-rw-  2.0 fat     3676 b- defN 23-Mar-13 18:48 Omnicon_DDSDocGen/Logger.py
--rw-rw-rw-  2.0 fat     3274 b- defN 23-Mar-15 18:24 Omnicon_DDSDocGen/Omnicon_DDSDocGen.py
+-rw-rw-rw-  2.0 fat     3707 b- defN 23-Jun-16 14:01 Omnicon_DDSDocGen/Logger.py
+-rw-rw-rw-  2.0 fat     3625 b- defN 23-Jun-18 07:10 Omnicon_DDSDocGen/Omnicon_DDSDocGen.py
 -rw-rw-rw-  2.0 fat     1581 b- defN 23-Mar-13 18:48 Omnicon_DDSDocGen/PdfGen.py
 -rw-rw-rw-  2.0 fat    38422 b- defN 23-Mar-13 18:48 Omnicon_DDSDocGen/SingleChapterGenerator.py
 -rw-rw-rw-  2.0 fat    21970 b- defN 23-Mar-15 18:24 Omnicon_DDSDocGen/Template.docx
 -rw-rw-rw-  2.0 fat      636 b- defN 22-Nov-17 06:04 Omnicon_DDSDocGen/Utils.py
--rw-rw-rw-  2.0 fat      540 b- defN 23-Mar-13 18:48 Omnicon_DDSDocGen/__init__.py
--rw-rw-rw-  2.0 fat    23766 b- defN 22-Nov-02 05:41 Omnicon_DDSDocGen/docGenMain.py
--rw-rw-rw-  2.0 fat     1148 b- defN 23-Mar-15 19:11 Omnicon_DDSDocGen-2.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6929 b- defN 23-Mar-15 19:11 Omnicon_DDSDocGen-2.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-15 19:11 Omnicon_DDSDocGen-2.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Mar-15 19:11 Omnicon_DDSDocGen-2.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1594 b- defN 23-Mar-15 19:11 Omnicon_DDSDocGen-2.1.1.dist-info/RECORD
-18 files, 165780 bytes uncompressed, 54874 bytes compressed:  66.9%
+-rw-rw-rw-  2.0 fat      574 b- defN 23-Jun-18 07:26 Omnicon_DDSDocGen/__init__.py
+-rw-rw-rw-  2.0 fat     1148 b- defN 23-Jun-18 07:31 Omnicon_DDSDocGen-2.2.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7460 b- defN 23-Jun-18 07:31 Omnicon_DDSDocGen-2.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-18 07:31 Omnicon_DDSDocGen-2.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jun-18 07:31 Omnicon_DDSDocGen-2.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1505 b- defN 23-Jun-18 07:31 Omnicon_DDSDocGen-2.2.1.dist-info/RECORD
+17 files, 142644 bytes uncompressed, 49488 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -30,26 +30,23 @@
 
 Filename: Omnicon_DDSDocGen/Utils.py
 Comment: 
 
 Filename: Omnicon_DDSDocGen/__init__.py
 Comment: 
 
-Filename: Omnicon_DDSDocGen/docGenMain.py
+Filename: Omnicon_DDSDocGen-2.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: Omnicon_DDSDocGen-2.1.1.dist-info/LICENSE
+Filename: Omnicon_DDSDocGen-2.2.1.dist-info/METADATA
 Comment: 
 
-Filename: Omnicon_DDSDocGen-2.1.1.dist-info/METADATA
+Filename: Omnicon_DDSDocGen-2.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: Omnicon_DDSDocGen-2.1.1.dist-info/WHEEL
+Filename: Omnicon_DDSDocGen-2.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: Omnicon_DDSDocGen-2.1.1.dist-info/top_level.txt
-Comment: 
-
-Filename: Omnicon_DDSDocGen-2.1.1.dist-info/RECORD
+Filename: Omnicon_DDSDocGen-2.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Omnicon_DDSDocGen/DocGenLogic.py

```diff
@@ -68,21 +68,22 @@
     current_union_enum_vector: List[Any]
     level_of_Discriminator: int
     union_label_to_userComment_dictionary: Dict[str, str]
     name_of_previous_element: str
     is_all_types_ok: bool
     levels_skipped: List[int]
 
-    def __init__(self, logging_verbosity) -> None:
+    def __init__(self, logging_verbosity, progress_callback_function) -> None:
         # :param logging_verbosity: The requested level of logging. Could be either 'CRITICAL','ERROR','WARNING',
         #                         'INFO' or 'DEBUG'. NOTE: This parameter is optional; Default is 'INFO'.
+
+        self.check_progress_callback_function_signature(progress_callback_function)
+        self.update_external_progress_callback_function = progress_callback_function
+
         self.single_chapter_generator = None
-        factory_configuration = Omnicon.FactoryConfiguration()
-        factory_configuration.loggerConfiguration.verbosity = Omnicon.LogSeverityLevel.info
-        Omnicon.GenericDDSEngine.SetFactoryConfiguration(factory_configuration)
 
         self.logger = Logger.init_logger(__name__, logging_verbosity)
 
         self.check_artifacts_integrity()
 
         self.header_titles = ("Hierarchy", "Field", "Type", "Description/Metadata")
         # Create an automatic dictionary to link between indexes and column-titles
@@ -115,44 +116,51 @@
     def init_and_run_engine(self, input_files_and_dirs_list: list) -> None:
         """
         This creates an engine instance and performs init and run with the desired configurations.
         :param input_files_and_dirs_list: A string that holds the path of the folder that holds the input_pointer files
         """
         # Create an engine instance:
         self.engine = Omnicon.GenericDDSEngine()
+        try:
+            factory_configuration = Omnicon.FactoryConfiguration()
+            factory_configuration.loggerConfiguration.verbosity = Omnicon.LogSeverityLevel.info
+            Omnicon.GenericDDSEngine.SetFactoryConfiguration(factory_configuration)
+        except:
+            pass
+
         # Create an engine configuration object:
         engine_configuration = Omnicon.EngineConfiguration()
-
         # Set the parameters:
+        engine_configuration.threadPoolSize = 3
         # Go over the new list and append it into the configuration file path vector:
         for input_file in input_files_and_dirs_list:
             engine_configuration.ddsConfigurationFilesPath.append(input_file)
         # Perform the introspection:
         engine_configuration.engineOperationMode = \
             Omnicon.EngineOperationMode.TYPE_INTROSPECTION
         # init the engine:
         self.logger.debug("init engine...")
-        is_engine_ok = self.engine.Init(engine_configuration)
-
-        # Check if the init went well
-        if is_engine_ok is False:
-            error_message: str = "Error! Problem with engine configuration. Might be an issue with the license."
-            self.logger.error(error_message)
-            ErrorListHandler.add_entry(LogLevel.ERROR, error_message)
-            raise Exception(error_message)
 
+        self.engine.Init(engine_configuration)
         self.logger.info("Engine was init successfully")
         # Run the engine:
-        is_engine_ok = self.engine.Run()
-        # Check if the init went well
-        if is_engine_ok is False:
-            error_message: str = "Failed to run the engine."
-            self.logger.error(error_message)
-            ErrorListHandler.add_entry(LogLevel.ERROR, error_message)
-            raise Exception("Error! Engine run FAILED!")
+        self.engine.Run()
+        # When Init() went well, make a log entry:
+        self.logger.debug("Engine is now up and running")
+
+    def shutdown_engine(self):
+        try:
+            self.logger.debug("Shutting down Omnicon engine")
+            if self.engine:
+                self.engine.Shutdown()
+                del self.engine
+                self.engine = None
+            self.logger.debug("Engine shutdown is complete")
+        except Exception as error:
+            self.logger.error("shutdown_introspection_engine exception occurred:", error)
 
     @staticmethod
     def order_topics_by_xml(topic_names_to_types_xml: str, alphabet_order_list: list):
         """
         This function returns a list of topic
         :param topic_names_to_types_xml:
         :param alphabet_order_list:
@@ -194,15 +202,15 @@
         is_at_least_one_type_ok: bool = False
         # Run the introspection for each data type:
         iteration_number: int = 1
         num_of_chapters: int = len(DDSTopicToTypeXMLMapping.keys())
         self.calculate_total_work_for_progress_bar(num_of_chapters)
 
         for topic, DDS_type in DDSTopicToTypeXMLMapping.items():
-            self.update_progress_bar(iteration_number)
+            self.update_progress_bar(iteration_number, DDS_type)
             iteration_number += 1
             # Generate a new chapter for that topic / type:
             try:
                 self.single_chapter_generator.generate_single_chapter(topic, DDS_type)
             except Exception as e:
                 self.logger.error(Exception, e)
                 # Signal that there is an issue with one of the types.
@@ -234,28 +242,30 @@
         """
         This function determines the numbers that would be used to calculate the progress (for the progress bar)
         :param num_of_chapters: The total number of chapters from the given XML
         :return:
         """
         self.num_of_chapters = num_of_chapters
         self.work_per_format = num_of_chapters +  int(num_of_chapters / 5)
-        self.total_steps = self.total_num_of_formats * self.work_per_format
+        shutdown_overhead = int((self.total_num_of_formats * self.work_per_format) / 8)
+        self.total_steps = self.total_num_of_formats * self.work_per_format + shutdown_overhead
 
-    def update_progress_bar(self, iteration_number: int):
+    def update_progress_bar(self, iteration_number: int, DDS_type: str):
         """
         This function updates the progress bar by calling the function provided by the user, taking into
         consideration the total num of  formats required by the user, the current iteration within the format currently
          under work, and adding 10% to the total work required for file saving overhead.
         :param iteration_number: The iteration number - where are we in terms of progress
+        :param DDS_type: A string that says which DDS type is parsed now
         :return: None
         """
         if self.update_external_progress_callback_function is not None:
             if self.is_progress_bar_func_ok:
                 current_step = iteration_number + (self.work_per_format * (self.current_format_num -1))
-                info = f"{ErrorListHandler.get_current_module().lower()}_parse"
+                info = f"{ErrorListHandler.get_current_module().lower()}: Parsing {DDS_type}"
                 try:
                     self.update_external_progress_callback_function(self.total_steps, current_step, info)
                 except Exception:
                     self.is_progress_bar_func_ok = False
                     warning_text = f"There seems to be a problem with the provided progress bar callback function. " \
                                    f"Please refer to README.md for the required progress bar function."
                     ErrorListHandler.add_entry(LogLevel.WARNING, warning_text)
@@ -263,15 +273,15 @@
     def update_progress_save(self):
         """
         This function updates the progress bar by calling the function provided by the user, letting him know now we
         are saving a file and that might take a while.
         :return: None
         """
         current_step = (self.current_format_num - 1) * self.work_per_format + self.num_of_chapters
-        info = f"{ErrorListHandler.get_current_module().lower()}_save"
+        info = f"{ErrorListHandler.get_current_module().lower()}: Saving to disk. Might take a while..."
 
         if self.update_external_progress_callback_function is not None:
             if self.is_progress_bar_func_ok:
                 try:
                     self.update_external_progress_callback_function(self.total_steps, current_step, info)
                 except Exception:
                     self.is_progress_bar_func_ok = False
@@ -279,15 +289,15 @@
                                    f"Please refer to README.md for the required progress bar function."
                     ErrorListHandler.add_entry(LogLevel.WARNING, warning_text)
 
     def update_progress_end(self):
         if self.update_external_progress_callback_function is not None:
             if self.is_progress_bar_func_ok:
                 try:
-                    state_txt = f"{ErrorListHandler.get_current_module().lower()}_save"
+                    state_txt = f"DocGen operation is completed."
                     self.update_external_progress_callback_function(1, 1, state_txt)
                 except Exception:
                     self.is_progress_bar_func_ok = False
                     warning_text = f"There seems to be a problem with the provided progress bar callback function. " \
                                    f"Please refer to README.md for the required progress bar function."
                     ErrorListHandler.add_entry(LogLevel.WARNING, warning_text)
 
@@ -312,15 +322,15 @@
         # A flag that holds TRUE (when at least one chapter (type) was written. False when no chapter was written):
         is_at_least_one_type_ok: bool = False
         iteration_number: int = 1
         num_of_chapters: int = len(DDS_type_list)
         self.calculate_total_work_for_progress_bar(num_of_chapters)
 
         for DDS_type in DDS_type_list:
-            self.update_progress_bar(iteration_number)
+            self.update_progress_bar(iteration_number, DDS_type)
             iteration_number += 1
             if DDS_type.isNested is False:
                 # Add a chapter only when the type is not a nested one:
                 try:
                     self.single_chapter_generator.generate_single_chapter("", DDS_type.fullName)
                 except Exception as err:
                     # Signal that there is an issue with one of the types.
@@ -337,15 +347,14 @@
     def check_input_types(self,
                           input_files_and_dirs_list: list,
                           output_file_name: str,
                           title: str,
                           version: str,
                           topic_names_to_types_xml_path: str,
                           output_folder: str,
-                          progress_callback_function: Callable[[], Any],
                           output_formats: list):
         if type(input_files_and_dirs_list) != list:
             error_message: str = f"Invalid input! Parameter <input_files_and_dirs_list>: '{input_files_and_dirs_list}' is: " \
                                  f"{type(input_files_and_dirs_list)}. Should be of class 'list'."
             raise Exception(error_message)
 
         if type(output_file_name) != str:
@@ -375,21 +384,14 @@
             raise Exception(error_message)
 
         if type(output_formats) != list:
             error_message: str = f"Invalid input! Parameter <output_formats> '{output_formats}' is: " \
                                  f"{type(output_formats)}. Should be of class 'list'."
             raise Exception(error_message)
 
-        if progress_callback_function != None:
-            if not isinstance(progress_callback_function, types.FunctionType):
-                error_message: str = f"Invalid input! Parameter <progress_callback_function> " \
-                                     f"'{progress_callback_function}' is: " \
-                                     f"{type(progress_callback_function)}. Should be of class 'function'."
-                raise Exception(error_message)
-
     def check_output_format_list(self, output_format_list):
         error_message: str
         example_message: str = "Please add a list of requested formats. For example: ['pdf']. " \
                                "Another example: ['docx', 'pdf']."
         if output_format_list == None:
             error_message = f"Invalid input! Parameter <output_format> is 'None'. {example_message}"
             raise Exception(error_message)
@@ -430,14 +432,21 @@
         if input_files_and_dirs_list == None:
             error_message = f"input_files_and_dirs_list is None. Cannot create an ICD without type file(s) or" \
                             f" a folder that contains at least one."
             raise Exception(error_message)
 
     @staticmethod
     def check_progress_callback_function_signature(progress_callback_function):
+        if progress_callback_function != None:
+            if not isinstance(progress_callback_function, types.FunctionType):
+                error_message: str = f"Invalid input! Parameter <progress_callback_function> " \
+                                     f"'{progress_callback_function}' is: " \
+                                     f"{type(progress_callback_function)}. Should be of class 'function'."
+                raise Exception(error_message)
+
         # define an allowed signature with 3 parameters
         if progress_callback_function != None:
 
             # get the signature of OF
             signature = inspect.signature(progress_callback_function)
             num_params = len(signature.parameters)
             # compare the signatures
@@ -449,34 +458,32 @@
     def check_input(self,
                     input_files_and_dirs_list: list,
                     output_file_name: str,
                     title: str,
                     version: str,
                     topic_names_to_types_xml_path: str,
                     output_folder: str,
-                    progress_callback_function: Callable[[], Any],
                     output_formats: list):
         """
         This function checks several aspects of the input. IF there is an issue, an exception is thrown.
         """
         self.check_input_types(input_files_and_dirs_list, output_file_name, title, version,
                                topic_names_to_types_xml_path,
-                               output_folder, progress_callback_function, output_formats)
+                               output_folder, output_formats)
 
         self.check_output_format_list(output_formats)
 
         # check if output folder even exists
         self.check_path(output_folder)  # SEE NOTE BElOW
         # NOTE: Since there is a list of requested type files, we check (for each type file) if the output file
         # is open at a later stage, when calling that type file's docGen's init method (for example, in the case
         # of a PDF, the test happens in LatexDocGen.__init__)
 
         self.check_type_files_not_empty(input_files_and_dirs_list)
 
-        self.check_progress_callback_function_signature(progress_callback_function)
 
 
 
     def save_file_to_requested_folder(self,
                                       output_file_name: str, output_folder: str, temp_folder: str, output_type: str):
         """
         This function copies the requested file from the temp location to the requested location.
@@ -517,18 +524,16 @@
                                     dds_types_files: list,
                                     dds_topics_types_mapping: str,
                                     output_file_name: str,
                                     title: str,
                                     version: str,
                                     order_alphabetically: bool,
                                     output_folder: str,
-                                    output_formats:[list],
-                                    progress_callback_function: Callable[[], Any]) -> List[str]:
+                                    output_formats:[list]) -> List[str]:
 
-        self.update_external_progress_callback_function = progress_callback_function
         self.total_num_of_formats = len(output_formats)
 
         self.is_all_types_ok = True  # An indicator that helps to know whether all types went well
 
         self.init_and_run_engine(dds_types_files)
 
         now: datetime = datetime.now()
@@ -603,14 +608,15 @@
 
                     is_at_least_one_file_created = True
 
                 except Exception as err:
                     ErrorListHandler.add_entry(LogLevel.ERROR, str(err))
                     self.logger.error(str(err), exc_info=True)
 
+        self.shutdown_engine()
         self.update_progress_end()
         time.sleep(0.5)
 
         ErrorListHandler.update_current_module_name("general")
         if is_at_least_one_file_created == False:
             warning_message = "There was an issue creating the files. Please refer to the log for more information."
             self.logger.error(warning_message)
@@ -634,16 +640,15 @@
                           dds_types_files: list,
                           dds_topics_types_mapping: str = "",
                           output_file_name: str = "ICD",
                           title: str = "ICD",
                           version: str = "1.0",
                           order_alphabetically: bool = True,
                           output_folder: str = "",
-                          output_formats=None,
-                          progress_callback_function: Callable[[], Any] = None) -> (bool, List[str]):
+                          output_formats=None) -> (bool, List[str]):
         """
         Start the doc generation process.
         :param dds_types_files: (list of strings) A list of file or folders names, in an order specified
                                            by the user according to files dependencies.
         :param dds_topics_types_mapping: (string) An XML file that contains a DDS topic to type mapping. NOTE: This
                                               parameter is optional; Sending an empty string ("") will switch ICD from
                                                topic-based to type-based document, meaning chapters will be types and
@@ -655,41 +660,40 @@
         :param version: The document's version number - This string will be added to the top page of the ICD.
                         NOTE: This parameter is optional; Default is "1.0"
         :param order_alphabetically: Whether to order to generated document topics/types alphabetically or according to
                                     the loaded files order
         :param output_folder: (string) The user's output folder of choice. NOTE: This parameter is optional;
                               Default is current working directory.
         :param output_formats: A list of desired output formats as strings. for example: ["docx", "pdf"]
-        :param progress_callback_function: A 'pointer' to the function that updates the progress bar.
 
 
         :return: tuple of (bool, list). bool: True upon success. list: list of errors that happened along the way
         """
         is_document_generated: bool = False
         try:
 
             self.check_input(dds_types_files, output_file_name, title, version, dds_topics_types_mapping,
-                             output_folder, progress_callback_function, output_formats)
+                             output_folder, output_formats)
 
             self.logger.info(f"type_file_path_list: {dds_types_files}")
             self.logger.info(f"topic_names_to_types_xml_path: {dds_topics_types_mapping}")
             self.logger.info(f"output_folder: {output_folder}")
             self.logger.info(f"output_file_name: {output_file_name}")
 
             self.run_engine_and_generate_ICD(dds_types_files,
                                             dds_topics_types_mapping,
                                             output_file_name,
                                             title,
                                             version,
                                             order_alphabetically,
                                             output_folder,
-                                            output_formats,
-                                            progress_callback_function)
+                                            output_formats)
 
             is_document_generated = True
 
         except Exception as err:
             self.logger.error(err, exc_info=True)
             ErrorListHandler.add_entry(LogLevel.ERROR,err)
+            self.shutdown_engine()
 
 
         return (is_document_generated, ErrorListHandler.get_error_list())
```

## Omnicon_DDSDocGen/Logger.py

```diff
@@ -1,8 +1,9 @@
 import logging
+import sys
 
 # # TODO - TO SAVE FILES WITH TIME ROTATION + UNIQUE FILE NAME
 # # fh = logging.FileHandler('DocGen' + '.log', mode='w')
 # from datetime import datetime
 # from logging.handlers import TimedRotatingFileHandler
 #
 # log_file_name = f"myapp-{datetime.now().strftime('%Y-%m-%d_%H-%M-%S')}.log"
@@ -64,15 +65,15 @@
     # Start by setting the root logger:
     verbosity_level = parse_logging_level(verbosity)
     root_logger = logging.getLogger()
     root_logger.setLevel(verbosity_level)
     root_logger.propagate = False
 
     # create console handler with a higher log level
-    ch = logging.StreamHandler()
+    ch = logging.StreamHandler(stream=sys.stdout)
     ch.setLevel(verbosity_level)
     # create formatter and add it to the handlers
     formatter = logging.Formatter('[%(levelname)s] %(asctime)s - %(name)s - %(message)s')
     ch.setFormatter(formatter)
     # add the handlers to the root logger
     root_logger.addHandler(ch)
     # TODO Removed file handler untill we come up with a solution that allows running multiple exe
@@ -80,15 +81,15 @@
     # fh = logging.FileHandler('DocGen' + '.log', mode='w')
     # TODO - TO SAVE FILES WITH TIME ROTATION + UNIQUE FILE NAME (instead of previous line)
     # fh = TimedRotatingFileHandler(log_file_name, when="midnight", interval=1, backupCount=7)
     # fh.setLevel(logging.DEBUG)
     # fh.setFormatter(formatter)
     # root_logger.addHandler(fh)
 	# prevent propagting to stderr
-    root_logger.propagate = False
+    # root_logger.propagate = False
 
     # Then create the current module's logger (that will use the root logger's configuration):
     logger = logging.getLogger(module_name)
     return logger
 
 
 def add_logger(module_name = None):
```

## Omnicon_DDSDocGen/Omnicon_DDSDocGen.py

```diff
@@ -1,29 +1,39 @@
 from typing import Any, Callable, List
 from . import DocGenLogic
 
 
 class DDSDocGen():
-    def __init__(self, logging_verbosity: str = "INFO") -> None:
+    def __init__(self, logging_verbosity: str = "INFO",
+                          progress_callback_function: Callable[[], Any] = None) -> None:
         """
         :param logging_verbosity: The requested level of logging. Could be either 'CRITICAL','ERROR','WARNING',
                                 'INFO' or 'DEBUG'. NOTE: This parameter is optional; Default is 'INFO'.
         """
-        self.__document_generator = DocGenLogic.DocumentGenerator(logging_verbosity)
+        progress_function = progress_callback_function
+        if progress_callback_function is None:
+           progress_function = self.__my_progress_callback_function
+
+        self.__document_generator = DocGenLogic.DocumentGenerator(logging_verbosity, progress_function)
+
+    @staticmethod
+    def __my_progress_callback_function(total_steps: int, current_step: int, info: str):
+        percentage = (current_step / total_steps) * 100
+        print(f"{int(percentage)}% complete, {info}")
+
 
     def generate_document(self,
                           dds_types_files: list,
                           dds_topics_types_mapping: str = "",
                           output_file_name: str = "ICD",
                           title: str = "ICD",
                           version: str = "1.0",
                           order_alphabetically: bool = True,
                           output_folder: str = "",
-                          output_formats=None,
-                          progress_callback_function: Callable[[], Any] = None
+                          output_formats=None
                           ) -> (bool, List[str]):
         """
         Start the doc generation process.
         :param dds_types_files: A list of DDS XML type files or folders.
             :param dds_topics_types_mapping: (string) An XML file that contains a DDS topic to type mapping. NOTE: This
                                               parameter is optional; In case the mapping is not provided, a type-based
                                               ICD will be generated.
@@ -48,10 +58,9 @@
             dds_types_files=dds_types_files,
             dds_topics_types_mapping=dds_topics_types_mapping,
             output_file_name=output_file_name,
             title=title,
             version=version,
             order_alphabetically=order_alphabetically,
             output_folder=output_folder,
-            output_formats=output_formats,
-            progress_callback_function=progress_callback_function
+            output_formats=output_formats
         )
```

## Omnicon_DDSDocGen/__init__.py

```diff
@@ -1,10 +1,11 @@
 # from .DocGenLogic import DocumentGenerator
 import os
 import sys
+from .Omnicon_DDSDocGen import *
 
 sys.path.append(os.path.dirname(os.path.realpath(__file__)))
 from Omnicon_DDSDocGen import Logger
 from Omnicon_DDSDocGen import Utils
 from Omnicon_DDSDocGen import DocGenLogic
 from Omnicon_DDSDocGen.DocGenInterface import DocGenInterface
 from Omnicon_DDSDocGen import SingleChapterGenerator
```

## Comparing `Omnicon_DDSDocGen-2.1.1.dist-info/LICENSE` & `Omnicon_DDSDocGen-2.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Omnicon_DDSDocGen-2.1.1.dist-info/METADATA` & `Omnicon_DDSDocGen-2.2.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: Omnicon-DDSDocGen
-Version: 2.1.1
+Version: 2.2.1
 Summary: DDS Document Generator
 Home-page: https://www.OmniconSystems.com
 Author-email: Omnicon Distributed Systems LTD <info@OmniconSystems.com>
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Communications
 Classifier: Topic :: Documentation
-Requires-Python: ~=3.7
+Requires-Python: <4.0,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: build (==0.9.0)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: docx2pdf (==0.1.8)
 Requires-Dist: importlib-metadata (==5.0.0)
 Requires-Dist: importlib-resources (==5.10.0)
 Requires-Dist: lxml (==4.9.1)
-Requires-Dist: Omnicon-GenericDDSEngine-Py (==4.5.5)
-Requires-Dist: packaging (==21.3)
+Requires-Dist: Omnicon-GenericDDSEngine-Py (==4.6.0)
+Requires-Dist: packaging (~=21.3)
 Requires-Dist: pep517 (==0.13.0)
 Requires-Dist: pyparsing (==3.0.9)
 Requires-Dist: python-docx (==0.8.11)
 Requires-Dist: pywin32 (==305)
 Requires-Dist: tomli (==2.0.1)
 Requires-Dist: tqdm (==4.64.1)
 Requires-Dist: typing-extensions (==4.4.0)
@@ -44,15 +44,15 @@
 * An Omnnicon license is required to utilize the API. Please Contact Info@OmniconSystems.com.
 
 ## API Usage Example
 The following example generates an PDF & Docx ICD from a provided DDS "ShapeType.xml" and a topics mapping,
 "TopicNamesToTypesDefMap.xml".
 
 ```python
-from Omnicon_DDSDocGen.Omnicon_DDSDocGen import DDSDocGen
+from Omnicon_DDSDocGen import DDSDocGen
 
 try:
     doc_gen = DDSDocGen()
 except Exception as err:
     print(err)
     exit()
 
@@ -99,40 +99,44 @@
 
       <!--Topics Definition-->
       <topic name="Square" register_type_ref="ShapeTypeExtended"/>
     </domain>
   </domain_library>
 </dds>
 ```
+## CONSTRUCTOR ARGUMENTS
+| Argument                   | Type     | Description															                                                                             | Optional| Default value |
+|:---------------------------|:---------|:----------------------------------------------------------------------------------------|:---:|:---:|
+| Logging verbisity          | string   | Specifies the log verbosity level of choice (DEBUG, INFO, WARNING, ERROR or CRITICAL)                  |  *  |  "INFO"
+| progress_callback_function | function | A 'pointer' to the function that updates the progress bar.  [(see below)](#Progress Callback Function) |  *  |  (A default function will print to console)
+
+### Progress Callback Function
+The progress bar callback function provides the user continues updated on the document generation progress.
+The DocGen will invoke the provided function with the following information:
+1. total_steps - total number of steps for the current generation process. 
+2. current_step - current step the generation process is currently at.
+3. info - additional optional textual information regarding the current step (e.g. "saving docx")
+
+```python
+ProgressBarCallbackExample(total_steps: int, current_step: int, info: str)    
+```
+
 
 ## API Arguments
 
 | Argument                      |Type            |Description															  | Optional| Default value |
 |:------------------------------|:----|:------------------------------------------								  |:---:|:---:|
 | dds_types_files     | list[str] | A list of file or folders names, in an order specified by the user according to files dependencies.|   |  |
 | dds_xml_topic_definition	| string    | An XML file that contains a DDS topic to type mapping. Sending an empty string ("") will switch ICD from topic-based to type-based document|  *  | (creates type based document)|
 | output_file_name		        | string    | The user's file name of choice | * | "ICD"  |
 | title			                | string    | The title/heading  of the document. This string will be added to the first page of the document. |  *  | "ICD" |
 | version            			| string    | The document's version number - This string will be added to the top page of the ICD. | * | "1.0"  |
 | order_alphabetically          | bool      | Select the order of generated document topics/types: alphabetically or according to the loaded files order |  *  | True (alphabetically)|
 | output_folder                 | string    | The user's output folder of choice	|  *  |current working directory|
 | output_formats				| list[str] |  A list of desired output formats as strings (list must contain at least one option)  |    | 
-| progress_callback_function  | function  | A 'pointer' to the function that updates the progress bar.  [(see below)](#Progress Callback Function)|  *  |  None
-
-### Progress Callback Function
-The progress bar callback function provides the user continues updated on the document generation progress.
-The DocGen will invoke the provided function with the following information:
-1. total_steps - total number of steps for the current generation process. 
-2. current_step - current step the generation process is currently at.
-3. info - additional optional textual information regarding the current step (e.g. "saving docx")
-
-```python
-ProgressBarCallbackExample(total_steps: int, current_step: int, info: str)    
-```
-
 
 
 ## API Return values
 **The API returns a tuple: (bool, list[str]).**
 * The boolean indicates whether a document was created (True) or not (False).
 * The list of strings holds information regarding the creation of the file(s), such as errors detected in a certain topic/type.
```

## Comparing `Omnicon_DDSDocGen-2.1.1.dist-info/RECORD` & `Omnicon_DDSDocGen-2.2.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Omnicon_DDSDocGen/DocGenInterface.py,sha256=xoSvfv3Qu2pRtKGUJduuBAw07qqLP8Tf8sVYU8oxs0Y,2039
-Omnicon_DDSDocGen/DocGenLogic.py,sha256=bzb3agUPGBtz19knB7Uimodh5LtxiWYvEZ_b7B7CvTk,35463
+Omnicon_DDSDocGen/DocGenLogic.py,sha256=yhuZHOP0lvMdxZB7wAYEbNWqFbWh5cMZkUH9Em7Y54A,35235
 Omnicon_DDSDocGen/DocxGen.py,sha256=GIdv9jRilyd1vNaTh19CixO6_eIfHinLW8BYXXDJFNE,10756
 Omnicon_DDSDocGen/ErrorListHandler.py,sha256=1cOO2UOBmURPBUSvIqNYYMsPeReFtZXOqt1gk5MFwEs,884
 Omnicon_DDSDocGen/LatexGen.py,sha256=wqO62A1pK8-CXZox201ddZPQXplwS1hX0Q3ljp2w1As,12992
-Omnicon_DDSDocGen/Logger.py,sha256=eewzaA2Owyvt0TzEECulFnAG7S-Yd4Zv_MTR0g3NSBI,3676
-Omnicon_DDSDocGen/Omnicon_DDSDocGen.py,sha256=k4pndvCD2qnxWv3nRmNx3VqPihSLtG_sJEM9hcY3LhE,3274
+Omnicon_DDSDocGen/Logger.py,sha256=mxd7uJEn_A-gmqbjcdEmn-YSmGzN4ebQsAUv6rDhbcU,3707
+Omnicon_DDSDocGen/Omnicon_DDSDocGen.py,sha256=2HozdjDrX9H4WRwmso6ve1kNbWExJAJzcp9vhifXzHY,3625
 Omnicon_DDSDocGen/PdfGen.py,sha256=uSAA1ZoXCypNr4PZt-XaQQttopFCaKJDnkF9oX-k_Wk,1581
 Omnicon_DDSDocGen/SingleChapterGenerator.py,sha256=f4_aE11WRtHZowFNV_On1uT-V-mXOSRN0bW_4fwdb1E,38422
 Omnicon_DDSDocGen/Template.docx,sha256=-8AyVDLVArS6ihcf5eW0p21aF5QZ5DuSjouGsb1Lu9E,21970
 Omnicon_DDSDocGen/Utils.py,sha256=O7Uq8Nw6GZ1oopXnezATL2IYVLY-PRO4csdgCVTsH4I,636
-Omnicon_DDSDocGen/__init__.py,sha256=w1W5vChrnCFZA2nyhQdToi00GT_yAuAKMpn97lYNOaE,540
-Omnicon_DDSDocGen/docGenMain.py,sha256=2yVl8o7kuCFWDSQ22q5vxsDbmKhpWbYhII1o8HY--wE,23766
-Omnicon_DDSDocGen-2.1.1.dist-info/LICENSE,sha256=XSIwLWa6oB7ZrV1lbbzYgj5AAYxve0v6oGjWdGkvvRw,1148
-Omnicon_DDSDocGen-2.1.1.dist-info/METADATA,sha256=hsBqvR85rOp6Z8uU64tL0RzZlA4FI88uX4CQWaqeQEI,6929
-Omnicon_DDSDocGen-2.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-Omnicon_DDSDocGen-2.1.1.dist-info/top_level.txt,sha256=N_T3f3SrPcjZY7yTpuuUAzmhBoNgEvwOuwqKxGZFXEI,18
-Omnicon_DDSDocGen-2.1.1.dist-info/RECORD,,
+Omnicon_DDSDocGen/__init__.py,sha256=lTBdtMUD01scXcIuz0_gRdxKQvXGzPKg9cvLi5XmV6g,574
+Omnicon_DDSDocGen-2.2.1.dist-info/LICENSE,sha256=XSIwLWa6oB7ZrV1lbbzYgj5AAYxve0v6oGjWdGkvvRw,1148
+Omnicon_DDSDocGen-2.2.1.dist-info/METADATA,sha256=z1kWeYTXIuSKyf8kv1Wg0p8y8aFIkOshQkKVhgwcP5o,7460
+Omnicon_DDSDocGen-2.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+Omnicon_DDSDocGen-2.2.1.dist-info/top_level.txt,sha256=N_T3f3SrPcjZY7yTpuuUAzmhBoNgEvwOuwqKxGZFXEI,18
+Omnicon_DDSDocGen-2.2.1.dist-info/RECORD,,
```

