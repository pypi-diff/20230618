# Comparing `tmp/kultimate-0.2.8.tar.gz` & `tmp/kultimate-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kultimate-0.2.8.tar", max compression
+gzip compressed data, was "kultimate-0.2.9.tar", max compression
```

## Comparing `kultimate-0.2.8.tar` & `kultimate-0.2.9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     3673 2023-06-17 01:35:44.660558 kultimate-0.2.8/README.md
--rw-r--r--   0        0        0      211 2023-06-17 00:35:38.560480 kultimate-0.2.8/kultimate/__init__.py
--rw-r--r--   0        0        0     2191 2023-06-17 00:35:38.560480 kultimate-0.2.8/kultimate/app.css
--rw-r--r--   0        0        0    22125 2023-06-17 01:40:14.290564 kultimate-0.2.8/kultimate/app.py
--rw-r--r--   0        0        0      168 2023-06-17 00:35:38.560480 kultimate-0.2.8/kultimate/screens/__init__.py
--rw-r--r--   0        0        0      897 2023-06-16 20:11:44.883725 kultimate-0.2.8/kultimate/screens/addTask.py
--rw-r--r--   0        0        0     1658 2023-06-17 01:51:58.863913 kultimate-0.2.8/kultimate/screens/create_file.py
--rw-r--r--   0        0        0      992 2023-06-17 00:52:35.603836 kultimate-0.2.8/kultimate/screens/deleteTask.py
--rw-r--r--   0        0        0      986 2023-06-16 20:10:08.290390 kultimate-0.2.8/kultimate/screens/edit_task.py
--rw-r--r--   0        0        0      815 2023-06-15 16:47:43.396777 kultimate-0.2.8/kultimate/screens/selectFile.py
--rw-r--r--   0        0        0      175 2023-06-17 00:35:38.563814 kultimate-0.2.8/kultimate/utils/__init__.py
--rw-r--r--   0        0        0     2222 2023-06-17 01:53:14.730581 kultimate-0.2.8/kultimate/utils/app_config.py
--rw-r--r--   0        0        0     1614 2023-06-17 01:49:15.327242 kultimate-0.2.8/kultimate/utils/create_file.py
--rw-r--r--   0        0        0     2048 2023-06-15 16:30:13.640087 kultimate-0.2.8/kultimate/utils/html_to_markdown.py
--rw-r--r--   0        0        0     1885 2023-06-16 17:10:49.190158 kultimate-0.2.8/kultimate/utils/parser_html.py
--rw-r--r--   0        0        0     1084 2023-06-02 22:13:35.823860 kultimate-0.2.8/kultimate/utils/process_yaml.py
--rw-r--r--   0        0        0      743 2023-06-16 16:51:32.056800 kultimate-0.2.8/kultimate/utils/prueba.py
--rw-r--r--   0        0        0      127 2023-06-07 23:20:48.314373 kultimate-0.2.8/kultimate/widgets/__init__.py
--rw-r--r--   0        0        0      620 2023-06-09 21:48:51.266124 kultimate-0.2.8/kultimate/widgets/directory.py
--rw-r--r--   0        0        0      426 2023-06-07 21:05:08.384197 kultimate-0.2.8/kultimate/widgets/stages.py
--rw-r--r--   0        0        0      122 2023-06-07 21:03:56.964196 kultimate-0.2.8/kultimate/widgets/stagesContainer.py
--rw-r--r--   0        0        0      136 2023-06-09 19:45:57.286316 kultimate-0.2.8/kultimate/widgets/task.py
--rw-r--r--   0        0        0      606 2023-06-17 01:53:34.323915 kultimate-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 kultimate-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     3829 2023-06-17 22:39:29.161092 kultimate-0.2.9/README.md
+-rw-r--r--   0        0        0      211 2023-06-17 00:35:38.560480 kultimate-0.2.9/kultimate/__init__.py
+-rw-r--r--   0        0        0     2677 2023-06-17 22:38:25.647758 kultimate-0.2.9/kultimate/app.css
+-rw-r--r--   0        0        0    23480 2023-06-17 22:38:25.647758 kultimate-0.2.9/kultimate/app.py
+-rw-r--r--   0        0        0      168 2023-06-17 00:35:38.560480 kultimate-0.2.9/kultimate/screens/__init__.py
+-rw-r--r--   0        0        0      897 2023-06-16 20:11:44.883725 kultimate-0.2.9/kultimate/screens/addTask.py
+-rw-r--r--   0        0        0     1658 2023-06-17 01:51:58.863913 kultimate-0.2.9/kultimate/screens/create_file.py
+-rw-r--r--   0        0        0      992 2023-06-17 00:52:35.603836 kultimate-0.2.9/kultimate/screens/deleteTask.py
+-rw-r--r--   0        0        0      986 2023-06-16 20:10:08.290390 kultimate-0.2.9/kultimate/screens/edit_task.py
+-rw-r--r--   0        0        0      815 2023-06-15 16:47:43.396777 kultimate-0.2.9/kultimate/screens/selectFile.py
+-rw-r--r--   0        0        0      212 2023-06-17 22:38:25.651091 kultimate-0.2.9/kultimate/utils/__init__.py
+-rw-r--r--   0        0        0     2222 2023-06-17 01:53:14.730581 kultimate-0.2.9/kultimate/utils/app_config.py
+-rw-r--r--   0        0        0     1614 2023-06-17 01:49:15.327242 kultimate-0.2.9/kultimate/utils/create_file.py
+-rw-r--r--   0        0        0     2048 2023-06-15 16:30:13.640087 kultimate-0.2.9/kultimate/utils/html_to_markdown.py
+-rw-r--r--   0        0        0     1051 2023-06-17 22:38:25.651091 kultimate-0.2.9/kultimate/utils/important_task.py
+-rw-r--r--   0        0        0     1885 2023-06-16 17:10:49.190158 kultimate-0.2.9/kultimate/utils/parser_html.py
+-rw-r--r--   0        0        0     1084 2023-06-02 22:13:35.823860 kultimate-0.2.9/kultimate/utils/process_yaml.py
+-rw-r--r--   0        0        0      743 2023-06-16 16:51:32.056800 kultimate-0.2.9/kultimate/utils/prueba.py
+-rw-r--r--   0        0        0      127 2023-06-07 23:20:48.314373 kultimate-0.2.9/kultimate/widgets/__init__.py
+-rw-r--r--   0        0        0      620 2023-06-09 21:48:51.266124 kultimate-0.2.9/kultimate/widgets/directory.py
+-rw-r--r--   0        0        0      426 2023-06-07 21:05:08.384197 kultimate-0.2.9/kultimate/widgets/stages.py
+-rw-r--r--   0        0        0      122 2023-06-07 21:03:56.964196 kultimate-0.2.9/kultimate/widgets/stagesContainer.py
+-rw-r--r--   0        0        0      136 2023-06-09 19:45:57.286316 kultimate-0.2.9/kultimate/widgets/task.py
+-rw-r--r--   0        0        0      687 2023-06-17 22:41:16.404428 kultimate-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4537 1970-01-01 00:00:00.000000 kultimate-0.2.9/PKG-INFO
```

### Comparing `kultimate-0.2.8/README.md` & `kultimate-0.2.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -5,30 +5,29 @@
 Aplicación CLI Python para manejar archivos markdown como tableros Kanban.
 Programado con [textual](https://textual.textualize.io/).
 
 ## Requerimientos
 
 `python = "^3.10"`
 
-Se ha probado en Linux, y tal vez funcione en MacOS.
-
 ## Instalación
 
 ```sh
 pip install kultimate
 ```
 
 ## Configuración
 
 Trabajo en progreso
 
 ## Uso
 
 |                     | Teclas para operar la aplicación              |
 | ------------------- | --------------------------------------------- |
+| ¡                   | Marcar/desmarcar tarea como importante        |
 | j, flecha abajo     | ir a la tarea de abajo                        |
 | k, flecha arriba    | ir a la tarea de arriba                       |
 | l, flecha izquierda | ir a la columna de la derecha                 |
 | h, flecha derecha   | ir a la columna de la izquierda               |
 | J                   | Llevar la tarea hacia arriba                  |
 | K                   | Llevar la tarea hacia abajo                   |
 | L                   | Cambiar la tarea a la columna de la derecha   |
@@ -37,14 +36,18 @@
 | o                   | Agregar tarea al final de la columna actual   |
 | ctrl+l              | Mueve la tarea a la última columna            |
 | ctrl+d              | Borra la tarea seleccionada                   |
 | q                   | Salir de la aplicación                        |
 
 ## ToDo
 
+- [ ] TODO: Marcar tareas importantes
+- [ ] TODO: Al cargar las tareas, agregar clase de importante si la marca está
+      presente
+- [ ] TODO: Copiar tareas al portapapeles
 - [x] DONE: Crear nuevo archivo. Usar el esqueleto creado en el archivo de configuración
 - [x] DONE: Rehacer la configuración de la aplicación.
 - [x] DONE: Hacer esqueleto para crear los nuevos archivos.
 - [x] DONE: Si no existe directorio crearlo.
 - [x] DONE: Reducir el tamaño de la caja para capturar las tareas.
 - [x] DONE: Editar tareas
 - [x] DONE: Al mover las tareas entre columnas visualmente se ve bien, pero al
@@ -56,15 +59,14 @@
 - [x] DONE: Enviar tareas a la última columna.
 - Operaciones en archivo.
   - [x] DONE: Convertir html a markdown al grabar.
   - [x] DONE: Grabar el archivo a disco.
 
 ## Quizás
 
-- [ ] TODO: Marcar tareas importantes
 - [ ] TODO: Agregar columnas.
 - [ ] TODO: Mover columnas.
 - [ ] TODO: Duplicar tareas.
 - [ ] TODO: Agregar sub tareas.
 - [ ] TODO: Crear un color nuevo para la última columna.
 - [ ] TODO: Seleccionar tareas con click del ratón.
 - [x] DONE: Cambiar Task al widget Input.
```

### Comparing `kultimate-0.2.8/kultimate/app.css` & `kultimate-0.2.9/kultimate/app.css`

 * *Files 8% similar despite different names*

```diff
@@ -40,33 +40,62 @@
   border: tall $success;
   margin: 1;
   padding: 1;
   color: $background-darken-3; /* ya no mover */
   background: $success-darken-1;
 }
 
+Task.is_important {
+  border: tall $error-darken-3;
+  background: $error-lighten-3;
+}
+
 /* DONE: Cambiar colores de tareas seleccionadas */
 /* DONE: Cambiar colores de la tarea que está seleccionada actualmente*/
 ._actual > Task {
   color: $background-darken-3;
   border: tall $warning;
   background: $warning-lighten-1;
 }
 
 ._actual > Task._active {
   color: $background-darken-3;
   border: inner $error-lighten-2;
   background: $warning-lighten-1;
 }
 
-DeleteTask, AddTask, SelectAFile, EditTask, CreateFile {
+Stage > Task._is_important {
+  color: $background-darken-3;
+  border: inner $error-darken-2;
+  background: $error-lighten-3;
+}
+
+._actual > Task._active._is_important {
+  color: $background-darken-3;
+  border: inner $warning-lighten-1;
+  background: $error-lighten-3;
+}
+
+._actual > Task._is_important {
+  color: $background-darken-3;
+  border: inner $error-darken-2;
+  background: $error-lighten-3;
+}
+
+DeleteTask,
+AddTask,
+SelectAFile,
+EditTask,
+CreateFile {
   align: center middle;
 }
 
-#add_task, #edit_task, #add_file {
+#add_task,
+#edit_task,
+#add_file {
   grid-size: 2;
   grid-gutter: 1 2;
   grid-rows: 1fr 3;
   padding: 0 1;
   width: 60;
   height: 5;
   border: thick $error-lighten-2 80%;
@@ -102,23 +131,24 @@
   padding: 0 1;
   width: 60;
   height: 11;
   border: thick $error-lighten-2 80%;
   background: $surface;
 }
 
-#question, #the_vertical {
+#question,
+#the_vertical {
   column-span: 2;
   height: 1fr;
   width: 100%;
   content-align: center middle;
 }
 
 RadioSet {
-    width: 50%;
+  width: 50%;
 }
 
 #question-1 {
   column-span: 2;
   height: 3;
   width: 100%;
   content-align: center middle;
```

### Comparing `kultimate-0.2.8/kultimate/app.py` & `kultimate-0.2.9/kultimate/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from textual.app import App, ComposeResult
 from textual.css.query import QueryError
 from textual.reactive import var
 from textual.widgets import Footer, Header
 
 from .screens import AddTask, CreateFile, DeleteTask, EditTask, SelectAFile
-from .utils import ParserMarkdown, StagesToMarkdown, create_new_markdown_file
+from .utils import MarkTask, ParserMarkdown, StagesToMarkdown, create_new_markdown_file
 from .widgets import Directory, Stage, StagesContainer, Task
 
 # DONE: Hay errores al navegar entre las columnas.
 
 
 class KanbanUltimate(App):
     """The main app class"""
@@ -34,14 +34,15 @@
         ("a", "add_task", "Add Task"),  # DONE: Guardar archivo
         ("e", "edit_task", "Edit Task"),  # DONE: Guardar archivo
         ("ctrl+l", "mark_as_done", "Mark as Done"),  # DONE: Guardar archivo
         ("ctrl+d", "delete_task", "Delete Task"),  # DONE: Guardar archivo
         ("ctrl+n", "new_file", "Create New File"),  # DONE: Guardar archivo
         ("q", "quit", "Quit"),
         # inician las teclas sin leyendas
+        ("¡", "mark_as_important"),
         ("l, right", "go_to_right"),
         ("h, left", "go_to_left"),
         ("j, down", "go_to_down"),
         ("k, up", "go_to_up"),
         ("J, shift+down", "move_down"),  # DONE: Guardar archivo
         ("K, shift+up", "move_up"),  # DONE: Guardar archivo
         ("H, shift+left", "move_left"),  # DONE: Guardar archivo
@@ -52,14 +53,15 @@
     # home_directory = "Dropbox/kanban2"
     is_directory_visible = False
     total_stages = 0
     current_stage = 0
     # Classes para la columna y la tarea activa
     class_for_active_stage = "_actual"
     class_for_active_task = "_active"
+    class_for_important_task = "_is_important"
     # Archivo md en el que se está trabajando
     actual_file = var("")
     # Variables para las tareas
     # poner a cero cuando se presione l o h
     current_task = 0
     total_tasks = 0
     # variable para guardar los archivos
@@ -408,14 +410,42 @@
             if self.current_stage > 0:
                 self.current_stage -= 1
             else:
                 self.current_stage = self.total_stages
 
             self.__activate_stage(old_stage)
 
+    def action_mark_as_important(self) -> None:
+        """Marcar la tarea como importante"""
+        # Comprobar si existen tareas
+        try:
+            if not self.list_tasks:
+                return
+        except AttributeError:
+            return
+
+        # obtener el texto de la tarea
+        text_for_task = str(self.list_tasks[self.current_task].renderable)
+        # pasarla por MarkTask
+        the_task = MarkTask(text_for_task)
+        # actualizar la tarea
+        the_task.toggle()
+        self.list_tasks[self.current_task].update(the_task.line)
+        # doing
+        if the_task.is_important:
+            # si es importante, agregar la clase self.is_important
+            self.list_tasks[self.current_task].add_class(self.class_for_important_task)
+        else:
+            # si no lo es, quitar la clase self.is_important
+            self.list_tasks[self.current_task].remove_class(
+                self.class_for_important_task
+            )
+        # guardar a disco
+        self.__save_to_file()
+
     # DONE: Moverse entre tareas con j y k
     def action_go_to_down(self) -> None:
         """Ir a la tarea de abajo"""
         # ¿en qué columna estoy?
         # obtener la tarea activa: self.current_task es la tarea actual
         # quitar la clase de tarea activa
         if self.list_tasks:
@@ -583,14 +613,19 @@
                 new_stage = Stage()
                 new_stage.set_title(stage)
                 # DONE:Errores al desplegar los movimientos entre J y K
                 # DONE: Mover tareas con H y L
                 first_task = True
                 for task in board[stage]:
                     new_task = Task(task)
+                    # determinar si es una tarea importante
+                    important_task = MarkTask(task)
+                    if important_task.is_important:
+                        new_task.add_class(self.class_for_important_task)
+
                     await new_stage.mount(new_task)
                     # DONE: Que la primer tarea obtenga el foco
                     if index == 0 and first_task:
                         new_task.focus()
                         first_task = False
                         new_task.add_class(self.class_for_active_task)
```

### Comparing `kultimate-0.2.8/kultimate/screens/addTask.py` & `kultimate-0.2.9/kultimate/screens/addTask.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.8/kultimate/screens/create_file.py` & `kultimate-0.2.9/kultimate/screens/create_file.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.8/kultimate/screens/deleteTask.py` & `kultimate-0.2.9/kultimate/screens/deleteTask.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.8/kultimate/screens/edit_task.py` & `kultimate-0.2.9/kultimate/screens/edit_task.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.8/kultimate/screens/selectFile.py` & `kultimate-0.2.9/kultimate/screens/selectFile.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.8/kultimate/utils/app_config.py` & `kultimate-0.2.9/kultimate/utils/app_config.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.8/kultimate/utils/create_file.py` & `kultimate-0.2.9/kultimate/utils/create_file.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.8/kultimate/utils/html_to_markdown.py` & `kultimate-0.2.9/kultimate/utils/html_to_markdown.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.8/kultimate/utils/parser_html.py` & `kultimate-0.2.9/kultimate/utils/parser_html.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.8/kultimate/utils/process_yaml.py` & `kultimate-0.2.9/kultimate/utils/process_yaml.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.8/kultimate/utils/prueba.py` & `kultimate-0.2.9/kultimate/utils/prueba.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.8/kultimate/widgets/directory.py` & `kultimate-0.2.9/kultimate/widgets/directory.py`

 * *Files identical despite different names*

### Comparing `kultimate-0.2.8/pyproject.toml` & `kultimate-0.2.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "kultimate"
-version = "0.2.8"
-description = ""
+version = "0.2.9"
+description = "Aplicación para manejar tableros kanban con markdown desde la línea de comandos"
 authors = ["Felipe <104157442+justafewwords4@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 textual = { extras = ["dev"], version = "^0.27.0" }
 pyyaml = "^6.0"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kultimate-0.2.8/PKG-INFO` & `kultimate-0.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kultimate
-Version: 0.2.8
-Summary: 
+Version: 0.2.9
+Summary: Aplicación para manejar tableros kanban con markdown desde la línea de comandos
 Author: Felipe
 Author-email: 104157442+justafewwords4@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
@@ -23,30 +23,29 @@
 Aplicación CLI Python para manejar archivos markdown como tableros Kanban.
 Programado con [textual](https://textual.textualize.io/).
 
 ## Requerimientos
 
 `python = "^3.10"`
 
-Se ha probado en Linux, y tal vez funcione en MacOS.
-
 ## Instalación
 
 ```sh
 pip install kultimate
 ```
 
 ## Configuración
 
 Trabajo en progreso
 
 ## Uso
 
 |                     | Teclas para operar la aplicación              |
 | ------------------- | --------------------------------------------- |
+| ¡                   | Marcar/desmarcar tarea como importante        |
 | j, flecha abajo     | ir a la tarea de abajo                        |
 | k, flecha arriba    | ir a la tarea de arriba                       |
 | l, flecha izquierda | ir a la columna de la derecha                 |
 | h, flecha derecha   | ir a la columna de la izquierda               |
 | J                   | Llevar la tarea hacia arriba                  |
 | K                   | Llevar la tarea hacia abajo                   |
 | L                   | Cambiar la tarea a la columna de la derecha   |
@@ -55,14 +54,18 @@
 | o                   | Agregar tarea al final de la columna actual   |
 | ctrl+l              | Mueve la tarea a la última columna            |
 | ctrl+d              | Borra la tarea seleccionada                   |
 | q                   | Salir de la aplicación                        |
 
 ## ToDo
 
+- [ ] TODO: Marcar tareas importantes
+- [ ] TODO: Al cargar las tareas, agregar clase de importante si la marca está
+      presente
+- [ ] TODO: Copiar tareas al portapapeles
 - [x] DONE: Crear nuevo archivo. Usar el esqueleto creado en el archivo de configuración
 - [x] DONE: Rehacer la configuración de la aplicación.
 - [x] DONE: Hacer esqueleto para crear los nuevos archivos.
 - [x] DONE: Si no existe directorio crearlo.
 - [x] DONE: Reducir el tamaño de la caja para capturar las tareas.
 - [x] DONE: Editar tareas
 - [x] DONE: Al mover las tareas entre columnas visualmente se ve bien, pero al
@@ -74,15 +77,14 @@
 - [x] DONE: Enviar tareas a la última columna.
 - Operaciones en archivo.
   - [x] DONE: Convertir html a markdown al grabar.
   - [x] DONE: Grabar el archivo a disco.
 
 ## Quizás
 
-- [ ] TODO: Marcar tareas importantes
 - [ ] TODO: Agregar columnas.
 - [ ] TODO: Mover columnas.
 - [ ] TODO: Duplicar tareas.
 - [ ] TODO: Agregar sub tareas.
 - [ ] TODO: Crear un color nuevo para la última columna.
 - [ ] TODO: Seleccionar tareas con click del ratón.
 - [x] DONE: Cambiar Task al widget Input.
```

