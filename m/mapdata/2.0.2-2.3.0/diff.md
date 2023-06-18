# Comparing `tmp/mapdata-2.0.2.tar.gz` & `tmp/mapdata-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-2.0.2.tar", last modified: Thu Jun 15 16:50:49 2023, max compression
+gzip compressed data, was "mapdata-2.3.0.tar", last modified: Sun Jun 18 15:44:26 2023, max compression
```

## Comparing `mapdata-2.0.2.tar` & `mapdata-2.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-15 16:50:49.913339 mapdata-2.0.2/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.0.2/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.0.2/MANIFEST.in
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     3583 2023-06-15 16:50:49.913339 mapdata-2.0.2/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     2385 2023-06-15 03:39:51.000000 mapdata-2.0.2/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-15 16:50:49.913339 mapdata-2.0.2/mapdata/
--rwxrwxr-x   0 dreas     (1000) dreas     (1000)   158095 2023-06-15 16:13:20.000000 mapdata-2.0.2/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-15 16:50:49.913339 mapdata-2.0.2/mapdata.egg-info/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     3583 2023-06-15 16:50:49.000000 mapdata-2.0.2/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-06-15 16:50:49.000000 mapdata-2.0.2/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-15 16:50:49.000000 mapdata-2.0.2/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-15 16:50:49.000000 mapdata-2.0.2/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-06-15 16:50:49.913339 mapdata-2.0.2/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1313 2023-06-15 16:44:07.000000 mapdata-2.0.2/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-18 15:44:26.192525 mapdata-2.3.0/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.3.0/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.3.0/MANIFEST.in
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     3583 2023-06-18 15:44:26.192525 mapdata-2.3.0/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     2385 2023-06-15 03:39:51.000000 mapdata-2.3.0/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-18 15:44:26.192525 mapdata-2.3.0/mapdata/
+-rwxrwxr-x   0 dreas     (1000) dreas     (1000)   168929 2023-06-18 14:39:13.000000 mapdata-2.3.0/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-18 15:44:26.192525 mapdata-2.3.0/mapdata.egg-info/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     3583 2023-06-18 15:44:26.000000 mapdata-2.3.0/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-06-18 15:44:26.000000 mapdata-2.3.0/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-18 15:44:26.000000 mapdata-2.3.0/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-18 15:44:26.000000 mapdata-2.3.0/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-06-18 15:44:26.192525 mapdata-2.3.0/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1313 2023-06-17 22:05:15.000000 mapdata-2.3.0/setup.py
```

### Comparing `mapdata-2.0.2/LICENSE.txt` & `mapdata-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-2.0.2/PKG-INFO` & `mapdata-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.0.2
+Version: 2.3.0
 Summary: An interactive map and table explorer for geographic coordinates in a CSV file
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
```

### Comparing `mapdata-2.0.2/README.md` & `mapdata-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mapdata-2.0.2/mapdata/mapdata.py` & `mapdata-2.3.0/mapdata/mapdata.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # 	The GNU General Public License is available at <http://www.gnu.org/licenses/>
 #
 # AUTHOR
 #	Dreas Nielsen (RDN)
 #
 # ==================================================================
 
-version = "2.0.2"
-vdate = "2023-06-15"
+version = "2.3.0"
+vdate = "2023-06-17"
 
 copyright = "2023"
 
 
 import sys
 import os.path
 import io
@@ -57,14 +57,15 @@
 import odf.opendocument
 import odf.table
 import odf.text
 import odf.number
 import odf.style
 import xlrd
 import openpyxl
+import numpy as np
 import matplotlib
 matplotlib.use('TkAgg')
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg, NavigationToolbar2Tk
 
 
 # Default name of configuration file.  Files with other names may be read.
@@ -77,20 +78,22 @@
 
 
 # Default options
 multiselect = "0"
 #-- Default location marker.  This may be overridden
 location_marker = "triangle_open"
 location_color = "black"
+use_data_marker = True
+use_data_color = True
 #-- Selected item marker
 select_symbol = "wedge"
 select_color = "red"
 #-- Label appearance
 label_color = "black"
-label_font = "Tahoma"		# use default
+label_font = "Liberation Sans"
 label_size = 10
 label_bold = False
 label_position = "below"	# above or below
 
 
 #-- Operational configuration
 # Whether to use a temporary file for Sqlite (as opposed to memory).
@@ -529,15 +532,15 @@
 	try:
 		float(v)
 		return True
 	except ValueError:
 		return False
 
 def dt_type(v):
-	# Type of date/time: timestamp, date, time, or None
+	# Type of date/time: timestamp, date, or None
 	if v is None or (type(v) is str and v.strip() == ''):
 		return None
 	t = None
 	try:
 		t = dateparser.isoparse(v)
 	except:
 		try:
@@ -661,14 +664,16 @@
 					self.win._root().withdraw()
 					fatal_error("Could not read table from %s, sheet %s" % (src_name, sheet), kwargs={'parent': self.win})
 		self.win.protocol("WM_DELETE_WINDOW", self.cancel)
 		self.data_src_name = src_name
 		self.win.title("Map of %s" % src_name)
 		self.headers = headers
 		self.rows = rows
+		# Set the font
+		self.mapfont = self.makefont()
 		# Set the application window icon
 		#win_icon = tk.BitmapImage(data=win_icon_xbm, foreground="black", background="tan")
 		#self.win.iconbitmap(win_icon)
 		# Source and possibly un-projected crs
 		self.src_crs = crs
 		self.crs = crs
 		# Created column names for un-projected coordinates
@@ -688,15 +693,15 @@
 		# List of PlotDialog objects, so they can have data pushed or be deleted.
 		self.plot_list = []
 		# Database connection is set in 'add_data()'; variables are initialized here
 		self.dbtmpdir = None
 		self.dbname = None
 		self.db = None
 		# Create default markers for the map
-		self.loc_marker_icon = tk.BitmapImage(data=icon_xbm[location_marker], foreground=location_color)
+		self.loc_marker_icon = self.set_get_loc_marker()
 		# Initializes selection marker to the global settings
 		self.set_sel_marker(select_symbol, select_color)
 		# Create icons for the buttonbar
 		expand_icon = tk.BitmapImage(data=expand_xbm, foreground="black")
 		focus_icon = tk.BitmapImage(data=wedge_sm_xbm, foreground="red")
 		zoom_sel_icon = tk.BitmapImage(data=wedges_3_xbm, foreground="red")
 		unselect_icon = tk.BitmapImage(data=cancel_xbm, foreground="black")
@@ -803,14 +808,29 @@
 		self.win.minsize(width=400, height=400)
 		# Set table status message
 		self.set_status()
 		# Just export the map and quit?
 		if map_export_file is not None:
 			self.imageoutputfile = map_export_file
 			self.win.after(export_time_sec * 1000, self.export_map_and_quit)
+	def makefont(self):
+		global label_font, label_size, label_bold
+		fams = tkfont.families()
+		if not label_font in fams:
+			alt_fonts = ["Liberation Sans", "Arial", "Helvetica", "Nimbus Sans", "Liberation Sans", "Trebuchet MS", "Tahoma", "DejaVu Sans", "Bitstream Vera Sans", "Open Sans"]
+			font_found = False
+			for f in alt_fonts:
+				if f in fams:
+					label_font = f
+					font_found = True
+					break
+			if not font_found:
+				label_font = tkfont.nametofont("TkDefaultFont").actual()["family"]
+		boldstr = "normal" if not label_bold else "bold"
+		return tkfont.Font(family=label_font, size=label_size, weight=boldstr)
 	def available_tile_servers(self):
 		# Return a list of those without API keys or for which API keys are provided
 		avail = []
 		for k in bm_servers:
 			if self.tile_url(k) is not None:
 				avail.append(k)
 		return avail
@@ -867,14 +887,19 @@
 			mkr.delete()
 			new_marker = self.map_widget.set_marker(mposition[0], mposition[1], icon=micon)
 			new_markers.append(new_marker)
 		self.sel_map_markers = new_markers
 	def draw_sel_markers(self):
 		for mkr in self.sel_map_markers:
 			mkr.draw()
+	def set_get_loc_marker(self):
+		mkr_key = "%s %s" % (location_color, location_marker)
+		if mkr_key not in custom_icons:
+			custom_icons[mkr_key] = tk.BitmapImage(data=icon_xbm[location_marker], foreground=location_color)
+		return custom_icons[mkr_key]
 	def redraw_loc_markers(self, tdata):
 		# tdata is the treeview control containing the data table.
 		while len(self.loc_map_markers) > 0:
 			self.loc_map_markers.pop().delete()
 		self.draw_loc_markers(tdata)
 	def draw_loc_markers(self, tdata):
 		# tdata is the treeview control containing the data table.
@@ -898,38 +923,34 @@
 				if self.min_lon is None or lon_val < self.min_lon:
 					self.min_lon = lon_val
 				if self.max_lon is None or lon_val > self.max_lon:
 					self.max_lon = lon_val
 				if self.color_index is None and self.symbol_index is None:
 					marker_icon = self.loc_marker_icon
 				else:
-					if self.color_index is None:
+					if self.color_index is None or not use_data_color:
 						color = location_color
 					else:
 						color = rowdata[self.color_index].lower()
 						if color not in color_names:
 							color = location_color
-					if self.symbol_index is None:
+					if self.symbol_index is None or not use_data_marker:
 						symbol = location_marker
 					else:
 						symbol = rowdata[self.symbol_index].lower()
 						if symbol not in icon_xbm:
 							symbol = location_marker
 					mkr_key = "%s %s" % (color, symbol)
 					if mkr_key not in custom_icons:
 						custom_icons[mkr_key] = tk.BitmapImage(data=icon_xbm[symbol], foreground=color)
 					marker_icon = custom_icons[mkr_key]
 				if self.label_index is not None:
 					lbl = rowdata[self.label_index]
-					if label_bold:
-						font_spec = "%s %s bold" % (label_font, label_size)
-					else:
-						font_spec = "%s %s" % (label_font, label_size)
 					mkr = self.map_widget.set_marker(lat_val, lon_val, icon=marker_icon,
-							text=lbl, font=font_spec, text_color=label_color,
+							text=lbl, font=self.mapfont, text_color=label_color,
 							command=self.map_sel_table)
 					self.loc_map_markers.append(mkr)
 				else:
 					mkr = self.map_widget.set_marker(lat_val, lon_val, icon=marker_icon, command=self.map_sel_table)
 					self.loc_map_markers.append(mkr)
 			else:
 				self.missing_latlon += 1
@@ -1331,14 +1352,41 @@
 					color = select_color
 				symb_name = "%s %s" % (color, symbol)
 				if symb_name not in custom_icons:
 					custom_icons[symb_name] = tk.BitmapImage(data=icon_xbm[symbol], foreground=color)
 				select_symbol = symbol
 				select_color = color
 				self.sel_marker_icon = custom_icons[symb_name]
+		def change_labeling():
+			global location_marker, location_color, use_data_marker, use_data_color
+			global label_font, label_size, label_bold, label_position
+			lbl_dlg = LabelDialog(map_menu, self.headers, self.label_col)
+			mkr, clr, datamkr, dataclr, column, ffam, fsize, fbold, pos = lbl_dlg.get_labeling()
+			fsize = int(fsize)
+			fbold = False if "0" else True
+			if mkr is not None:
+				if mkr != location_marker or clr != location_color or datamkr != use_data_marker or \
+						dataclr != use_data_color or column != self.label_col or ffam != label_font or \
+						fsize != label_size or fbold != label_bold or pos != label_position:
+							fontchanged = ffam != label_font or fsize != label_size or fbold != label_bold
+							location_marker = mkr
+							location_color = clr
+							use_data_marker = datamkr
+							use_data_color = dataclr
+							self.label_col = column if column != '' else None
+							label_font = ffam
+							label_size = fsize
+							label_bold = fbold
+							label_position = pos
+							if fontchanged:
+								self.mapfont = self.makefont()
+							self.loc_marker_icon = self.set_get_loc_marker()
+							self.label_index = self.headers.index(self.label_col) if self.label_col is not None and self.label_col != '' else None
+							self.redraw_loc_markers(self.tbl)
+							self.redraw_sel_markers()
 		def import_symbol_file():
 			sd = ImportSymbolDialog()
 			name, fn = sd.run()
 			if name is not None and fn is not None:
 				import_symbol(name, fn)
 				fqfn = os.path.abspath(fn)
 				symb_spec = (name, fqfn)
@@ -1371,14 +1419,17 @@
 				if select_symbol != pre_symbol or select_color != pre_color:
 					self.set_sel_marker(select_symbol, select_color)
 				# Redraw markers if any setting has changed
 				if location_marker != pre_loc_symbol or location_color != pre_loc_color or \
 						label_color != pre_label_color or label_font != pre_label_font or \
 						label_size != pre_label_size or label_bold != pre_label_bold or \
 						label_position != pre_label_position:
+							if label_font != pre_label_font or label_size != pre_label_size or label_bold != pre_label_bold:
+								self.mapfont = self.makefont()
+							self.loc_marker_icon = self.set_get_loc_marker()
 							self.redraw_loc_markers(self.tbl)
 							self.redraw_sel_markers()
 				global config_files_user
 				config_files_user.append(os.path.abspath(fn))
 		def save_config():
 			fn = tkfiledialog.asksaveasfilename(filetypes=([('Config files', '.conf')]))
 			if fn != '':
@@ -1394,50 +1445,61 @@
 				f.write("\n[symbols]\n")
 				for s in imported_symbols:
 					f.write("%s=%s\n" % (s[0], s[1]))
 				f.write("\n[defaults]\n")
 				f.write("basemap=%s\n" % self.basemap_var.get())
 				f.write("location_marker=%s\n" % location_marker)
 				f.write("location_color=%s\n" % location_color)
-				f.write("multilselect=%s\n" % ('Yes' if self.multiselect_var == '1' else 'No'))
+				f.write("use_data_marker=%s\n" % use_data_marker)
+				f.write("use_data_color=%s\n" % use_data_color)
+				f.write("multilselect=%s\n" % ('Yes' if self.multiselect_var.get() == '1' else 'No'))
 				f.write("select_symbol=%s\n" % select_symbol)
 				f.write("select_color=%s\n" % select_color)
 				f.write("label_color=%s\n" % label_color)
 				f.write("label_font=%s\n" % label_font)
 				f.write("label_size=%s\n" % label_size)
 				f.write("label_bold=%s\n" % ('No' if not label_bold else 'Yes'))
 				f.write("label_position=%s\n" % label_position)
 		def show_data_types():
 			dlg = MsgDialog("Data Types", "Data types, data completeness, and number of unique\nnon-missing values for columns of the data table:")
 			tframe, tdata = treeview_table(dlg.content_frame, self.data_types, ["Column", "Type", "Missing", "Unique"], "browse")
 			tframe.grid(row=0, column=0, sticky=tk.NSEW)
 			dlg.show()
 		def run_query():
 			dlg = QueryDialog(self.headers, self.db, self.whereclause)
-			whereclause = dlg.get_where()
+			whereclause, action = dlg.get_where()
 			if whereclause is not None:
 				sqlcmd = "SELECT treeviewid FROM mapdata WHERE %s" % whereclause
 				cur = self.db.cursor()
 				try:
 					result = cur.execute(sqlcmd)
 					id_list = [r[0] for r in result.fetchall()]
-					cur.close()
 				except:
+					cur.close()
 					warning("Invalid data selection expression: %s" % whereclause, kwargs={})
 				else:
+					cur.close()
 					self.whereclause = whereclause
 					# Enable multiselect
 					global multiselect
 					multiselect = "1"
 					self.multiselect_var.set("1")
 					self.tbl.configure(selectmode = tk.EXTENDED)
-					# Remove any existing selections
-					self.unselect_map()
-					# Add new selections
-					self.tbl.selection_set(tuple(id_list))
+					if action == "Replace":
+						# Remove any existing selections
+						self.unselect_map()
+						self.tbl.selection_set(tuple(id_list))
+					elif action == "Add":
+						# Add new selections
+						all_selections = tuple(set(self.tbl.selection()) | set(id_list))
+						self.tbl.selection_set(all_selections)
+					else:
+						# Remove
+						diff_selections = tuple(set(self.tbl.selection()) - set(id_list))
+						self.tbl.selection_set(diff_selections)
 					self.mark_map(None)
 					self.set_status()
 		def invert_selections():
 			selected = self.tbl.selection()
 			new_selections = []
 			for iid in self.tbl.get_children():
 				if not iid in selected:
@@ -1481,14 +1543,15 @@
 		file_menu.add_command(label="Read config", command = read_config_file, underline=0)
 		file_menu.add_command(label="Save config", command = save_config, underline=0)
 		file_menu.add_command(label="Quit", command = self.cancel, underline=0)
 		tbl_menu.add_command(label="Un-select all", command = self.unselect_map, underline=0)
 		tbl_menu.add_command(label="Export selected", command = save_table, underline=1)
 		tbl_menu.add_command(label="Data types", command = show_data_types, underline=5)
 		map_menu.add_command(label="Change marker", command = change_marker, underline=7)
+		map_menu.add_command(label="Change labeling", command = change_labeling, underline=7)
 		map_menu.add_command(label="Zoom selected", command = self.zoom_selected, underline=5)
 		map_menu.add_command(label="Zoom full", command = self.zoom_full, underline=5)
 		map_menu.add_command(label="Center on selection", command = self.focus_map, underline=0)
 		map_menu.add_command(label="Un-select all", command = self.unselect_map, underline=0)
 		map_menu.add_command(label="Change CRS", command = self.change_crs, underline=1)
 		map_menu.add_command(label="Export", command = save_map, underline=1)
 		sel_menu.add_command(label="Invert", command = invert_selections, underline=0)
@@ -1498,43 +1561,148 @@
 		plot_menu.add_command(label="Close all", command = self.close_all_plots, underline=0)
 		help_menu.add_command(label="Online help", command = online_help, underline=7)
 		help_menu.add_command(label="Config files", command = show_config_files, underline=0)
 		help_menu.add_command(label="About", command = show_about, underline=0)
 
 
 
+class LabelDialog(object):
+	def __init__(self, parent, column_list, label_col):
+		columns = ['']
+		columns.extend(column_list)
+		label_col = '' if label_col is None else label_col
+		self.dlg = tk.Toplevel()
+		self.dlg.title("Change Labeling")
+		prompt_frame = tk.Frame(self.dlg)
+		prompt_frame.grid(row=0, column=0, sticky=tk.NSEW, pady=(3,3))
+		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
+		btn_frame.grid(row=1, column=0, sticky=tk.EW, pady=(3,3))
+		btn_frame.columnconfigure(0, weight=1)
+		#
+		symbol_lbl = ttk.Label(prompt_frame, text="Location symbol:")
+		symbol_lbl.grid(row=0, column=0, sticky=tk.E, padx=(6,3))
+		self.symbol_var = tk.StringVar(self.dlg, location_marker)
+		symbol_vals = list(icon_xbm.keys())
+		symbol_vals.sort()
+		self.symbol_opts = ttk.Combobox(prompt_frame, state="readonly", textvariable=self.symbol_var,
+				values=symbol_vals, width=15)
+		self.symbol_opts.grid(row=0, column=1, columnspan=3, sticky=tk.W, padx=(6,3))
+		color_lbl = ttk.Label(prompt_frame, text="Color:")
+		color_lbl.grid(row=1, column=0, sticky=tk.E, padx=(3,3), pady=(3,3))
+		self.color_var = tk.StringVar(self.dlg, location_color)
+		color_opts = ttk.Combobox(prompt_frame, state="readonly", textvariable=self.color_var,
+				values=list(select_colors), width=15)
+		color_opts.grid(row=1, column=1, columnspan=3, sticky=tk.W, padx=(6,3), pady=(3,3))
+		#
+		self.use_data_marker_var = tk.StringVar(prompt_frame, use_data_marker)
+		ck_use_data_marker = ttk.Checkbutton(prompt_frame, text="Use data symbol", variable=self.use_data_marker_var)
+		ck_use_data_marker.grid(row=0, column=3, columnspan=2, sticky=tk.W, padx=(3,6), pady=(3,3))
+		self.use_data_color_var = tk.StringVar(prompt_frame, use_data_color)
+		ck_use_color_marker = ttk.Checkbutton(prompt_frame, text="Use data color", variable=self.use_data_color_var)
+		ck_use_color_marker.grid(row=1, column=3, columnspan=2, sticky=tk.W, padx=(3,6), pady=(3,3))
+		#
+		self.col_var = tk.StringVar(prompt_frame, label_col)
+		col_lbl = ttk.Label(prompt_frame, text = "Data column:")
+		col_lbl.grid(row=2, column=0, sticky=tk.E, padx=(6,3), pady=(6,3))
+		col_opts = ttk.Combobox(prompt_frame, state="readonly", textvariable=self.col_var,
+				values=columns, width=40)
+		col_opts.grid(row=2, column=1, columnspan=4, sticky=tk.W, padx=(3,6), pady=(3,3))
+		#
+		self.font_var = tk.StringVar(prompt_frame, label_font)
+		font_lbl = ttk.Label(prompt_frame, text="Font:")
+		font_lbl.grid(row=3, column=0, sticky=tk.E, padx=(3,3), pady=(6,3))
+		fonts = list(set(list(tkfont.families())))
+		fonts.sort()
+		font_opts = ttk.Combobox(prompt_frame, state="readonly", textvariable=self.font_var,
+				values=fonts, width=25)
+		font_opts.grid(row=3, column=1, columnspan=3, sticky=tk.W, padx=(3,3), pady=(3,3))
+		self.bold_var = tk.StringVar(prompt_frame, "0" if not label_bold else "1")
+		ck_bold = ttk.Checkbutton(prompt_frame, text="Bold", variable=self.bold_var)
+		ck_bold.grid(row=3, column=4, sticky=tk.W, padx=(3,6), pady=(3,3))
+		self.size_var = tk.IntVar(prompt_frame, label_size)
+		#
+		size_lbl = ttk.Label(prompt_frame, text="Size:")
+		size_lbl.grid(row=4, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
+		size_opt = ttk.Combobox(prompt_frame, state="normal", textvariable=self.size_var,
+				values=[8, 10, 12, 14, 16, 20, 24], width=3)
+		size_opt.grid(row=4, column=1, sticky=tk.W, padx=(6,3), pady=(3,3))
+		self.position_var = tk.StringVar(prompt_frame, label_position)
+		position_lbl = ttk.Label(prompt_frame, text="Position:")
+		position_lbl.grid(row=4, column=2, sticky=tk.E, padx=(3,3), pady=(3,3))
+		position_sel = ttk.Combobox(prompt_frame, state="readonly", textvariable=self.position_var,
+				values=["above", "below"], width=6)
+		position_sel.grid(row=4, column=3, sticky=tk.W, padx=(3,6), pady=(3,3))
+		#
+		# Buttons
+		self.canceled = False
+		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help, underline=0)
+		help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		self.dlg.bind("<Alt-h>", self.do_help)
+		ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select, underline=0)
+		ok_btn.grid(row=0, column=1, sticky=tk.E, padx=(3,3))
+		self.dlg.bind('<Alt-o>', self.do_select)
+		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
+		cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=(3,6))
+		self.dlg.bind("<Return>", self.do_select)
+		self.dlg.bind("<Escape>", self.do_cancel)
+	def do_help(self, *args):
+		webbrowser.open("https://mapdata.osdn.io/dialogs.html#change-labeling", new=2, autoraise=True)
+	def do_cancel(self, *args):
+		self.canceled = True
+		self.dlg.destroy()
+	def do_select(self, *args):
+		self.canceled = False
+		self.dlg.destroy()
+	def get_labeling(self):
+		self.dlg.grab_set()
+		center_window(self.dlg)
+		self.dlg.resizable(False, False)
+		self.symbol_opts.focus()
+		self.dlg.wait_window(self.dlg)
+		if not self.canceled:
+			return (self.symbol_var.get(), self.color_var.get(), self.use_data_marker_var.get(),
+					self.use_data_color_var.get(), self.col_var.get(), self.font_var.get(), self.size_var.get(),
+					self.bold_var.get(), self.position_var.get())
+		else:
+			return (None,None,None,None,None,None,None,None,None)
+
+
+
 class MarkerDialog(object):
 	def __init__(self, parent):
 		self.dlg = tk.Toplevel()
 		self.dlg.title("Change Marker")
 		prompt_frame = tk.Frame(self.dlg)
 		prompt_frame.grid(row=0, column=0, sticky=tk.NSEW, pady=(3,3))
 		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
 		btn_frame.grid(row=1, column=0, sticky=tk.EW, pady=(3,3))
 		btn_frame.columnconfigure(0, weight=1)
-		symbol_lbl = ttk.Label(prompt_frame, text="Symbol:")
-		symbol_lbl.grid(row=0, column=0, sticky=tk.E, padx=(3,3))
-		self.symbol_var = tk.StringVar(self.dlg, "wedge")
+		symbol_lbl = ttk.Label(prompt_frame, text="Marker symbol:")
+		symbol_lbl.grid(row=0, column=0, sticky=tk.E, padx=(6,3))
+		self.symbol_var = tk.StringVar(self.dlg, select_symbol)
 		symbol_vals = list(icon_xbm.keys())
-		self.symbol_opts = tk.OptionMenu(prompt_frame, self.symbol_var, *symbol_vals)
-		self.symbol_opts.configure(width=15)
-		self.symbol_opts.grid(row=0, column=1, sticky=tk.W, padx=(3,3))
+		symbol_vals.sort()
+		self.symbol_opts = ttk.Combobox(prompt_frame, state="readonly", textvar=self.symbol_var,
+				values=symbol_vals, width=15)
+		self.symbol_opts.grid(row=0, column=1, sticky=tk.W, padx=(3,6))
 		color_lbl = ttk.Label(prompt_frame, text="Color:")
-		color_lbl.grid(row=1, column=0, sticky=tk.E, padx=(3,3))
-		self.color_var = tk.StringVar(self.dlg, "red")
+		color_lbl.grid(row=1, column=0, sticky=tk.E, padx=(6,3))
+		self.color_var = tk.StringVar(self.dlg, select_color)
 		color_vals = list(select_colors)
-		color_opts = tk.OptionMenu(prompt_frame, self.color_var, *color_vals)
-		color_opts.configure(width=15)
-		color_opts.grid(row=1, column=1, sticky=tk.W, padx=(3,3))
+		color_opts = ttk.Combobox(prompt_frame, state="readonly", textvar=self.color_var,
+				values=color_vals, width=15)
+		color_opts.grid(row=1, column=1, sticky=tk.W, padx=(3,6))
 		# Buttons
 		self.canceled = False
-		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help)
+		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help, underline=0)
 		help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
-		ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select)
+		self.dlg.bind("<Alt-h>", self.do_help)
+		ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select, underline=0)
 		ok_btn.grid(row=0, column=1, sticky=tk.E, padx=(3,3))
+		self.dlg.bind('<Alt-o>', self.do_select)
 		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
 		cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=(3,6))
 		self.dlg.bind("<Return>", self.do_select)
 		self.dlg.bind("<Escape>", self.do_cancel)
 	def do_help(self, *args):
 		webbrowser.open("https://mapdata.osdn.io/dialogs.html#change-marker", new=2, autoraise=True)
 	def do_cancel(self, *args):
@@ -1559,17 +1727,17 @@
 	def __init__(self):
 		def get_fn():
 			fn = tkfiledialog.askopenfilename(filetypes=([('X11 bitmaps', '.xbm')]))
 			if fn != '':
 				self.fn_var.set(fn)
 		def check_enable(*args):
 			if self.fn_var.get() != '' and self.symbol_var.get() != '':
-				ok_btn["state"] = tk.NORMAL
+				self.ok_btn["state"] = tk.NORMAL
 			else:
-				ok_btn["state"] = tk.DISABLED
+				self.ok_btn["state"] = tk.DISABLED
 		self.dlg = tk.Toplevel()
 		self.dlg.title("Import X11 Bitmap Symbol")
 		prompt_frame = tk.Frame(self.dlg)
 		prompt_frame.grid(row=0, column=0, sticky=tk.NSEW, pady=(3,3))
 		button_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
 		button_frame.grid(row=1, column=0, columnspan=3, sticky=tk.EW, pady=(3,3))
 		button_frame.columnconfigure(0, weight=1)
@@ -1591,31 +1759,34 @@
 		fn_entry = ttk.Entry(prompt_frame, textvariable=self.fn_var)
 		fn_entry.configure(width=64)
 		fn_entry.grid(row=1, column=1, sticky=tk.EW, padx=(3,3))
 		fn_btn = ttk.Button(prompt_frame, text="Browse", command=get_fn)
 		fn_btn.grid(row=1, column=2, sticky=tk.W)
 		# Buttons
 		self.canceled = False
-		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help)
+		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help, underline=0)
 		help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
-		ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select)
-		ok_btn["state"] = tk.DISABLED
-		ok_btn.grid(row=0, column=1, sticky=tk.E, padx=(3,3))
+		self.dlg.bind("<Alt-h>", self.do_help)
+		self.ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select, underline=0)
+		self.ok_btn["state"] = tk.DISABLED
+		self.ok_btn.grid(row=0, column=1, sticky=tk.E, padx=(3,3))
+		self.dlg.bind('<Alt-o>', self.do_select)
 		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
 		cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=(3,6))
 		self.dlg.bind("<Return>", self.do_select)
 		self.dlg.bind("<Escape>", self.do_cancel)
 	def do_help(self, *args):
 		webbrowser.open("https://mapdata.osdn.io/dialogs.html#import-symbol", new=2, autoraise=True)
 	def do_cancel(self, *args):
 		self.canceled = True
 		self.dlg.destroy()
 	def do_select(self, *args):
-		self.canceled = False
-		self.dlg.destroy()
+		if self.ok_btn["state"] != tk.DISABLED:
+			self.canceled = False
+			self.dlg.destroy()
 	def run(self):
 		self.dlg.grab_set()
 		center_window(self.dlg)
 		self.dlg.resizable(False, False)
 		self.symbol_entry.focus()
 		self.dlg.wait_window(self.dlg)
 		if not self.canceled:
@@ -1734,18 +1905,20 @@
 		title_label = ttk.Label(opt_col_frame, text="Description:")
 		title_label.grid(row=2, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
 		self.title_var = tk.StringVar(opt_col_frame, '')
 		title_entry = ttk.Entry(opt_col_frame, width=60, textvariable=self.title_var)
 		title_entry.grid(row=2, column=1, columnspan=3, sticky=tk.EW, padx=(3,6), pady=(3,3))
 		# Buttons
 		self.canceled = False
-		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help)
+		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help, underline=0)
 		help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
-		ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select)
+		self.dlg.bind("<Alt-h>", self.do_help)
+		ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select, underline=0)
 		ok_btn.grid(row=0, column=1, sticky=tk.E, padx=3)
+		self.dlg.bind('<Alt-o>', self.do_select)
 		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
 		cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=(3,6))
 		ok_btn["state"] = tk.DISABLED
 		self.dlg.bind("<Return>", self.do_select)
 		self.dlg.bind("<Escape>", self.do_cancel)
 		self.dlg.resizable(False, False)
 	def do_help(self, *args):
@@ -1887,16 +2060,17 @@
 				wiz2_frame.lift()
 
 		w1btn_frame = tk.Frame(wiz1_frame, borderwidth=3, relief=tk.RIDGE)
 		w1btn_frame.grid(row=2, column=0, sticky=tk.EW, padx=(3,3), pady=(3,3))
 		w1btn_frame.columnconfigure(0, weight=1)
 		self.canceled = False
 		#
-		w1help_btn = ttk.Button(w1btn_frame, text="Help", command=self.do_help)
+		w1help_btn = ttk.Button(w1btn_frame, text="Help", command=self.do_help, underline=0)
 		w1help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		self.dlg.bind("<Alt-h>", self.do_help)
 		w1next_btn = ttk.Button(w1btn_frame, text="Next", command=w1_next)
 		w1next_btn.grid(row=0, column=1, sticky=tk.E, padx=3)
 		w1cancel_btn = ttk.Button(w1btn_frame, text="Cancel", command=self.do_cancel)
 		w1cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=(3,6))
 		w1next_btn["state"] = tk.DISABLED
 		self.dlg.bind("<Escape>", self.do_cancel)
 
@@ -1947,16 +2121,17 @@
 				self.col_sel["values"] = self.header_list
 				wiz3_frame.lift()
 
 		w2btn_frame = tk.Frame(wiz2_frame, borderwidth=3, relief=tk.RIDGE)
 		w2btn_frame.grid(row=2, column=0, sticky=tk.EW, padx=(3,3), pady=(3,3))
 		w2btn_frame.columnconfigure(0, weight=1)
 		#
-		w2help_btn = ttk.Button(w2btn_frame, text="Help", command=self.do_help)
+		w2help_btn = ttk.Button(w2btn_frame, text="Help", command=self.do_help, underline=0)
 		w2help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		self.dlg.bind("<Alt-h>", self.do_help)
 		w2prev_btn = ttk.Button(w2btn_frame, text="Back", command=w2_back)
 		w2prev_btn.grid(row=0, column=1, sticky=tk.E, padx=3)
 		w2next_btn = ttk.Button(w2btn_frame, text="Next", command=w2_next)
 		w2next_btn.grid(row=0, column=2, sticky=tk.E, padx=3)
 		w2cancel_btn = ttk.Button(w2btn_frame, text="Cancel", command=self.do_cancel)
 		w2cancel_btn.grid(row=0, column=3, sticky=tk.E, padx=(3,6))
 		w2next_btn["state"] = tk.DISABLED
@@ -2013,20 +2188,22 @@
 		def w3_back():
 			wiz2_frame.lift()
 
 		w3btn_frame = tk.Frame(wiz3_frame, borderwidth=3, relief=tk.RIDGE)
 		w3btn_frame.grid(row=2, column=0, sticky=tk.EW, padx=(3,3), pady=(3,3))
 		w3btn_frame.columnconfigure(0, weight=1)
 		#
-		w3help_btn = ttk.Button(w3btn_frame, text="Help", command=self.do_help)
+		w3help_btn = ttk.Button(w3btn_frame, text="Help", command=self.do_help, underline=0)
 		w3help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		self.dlg.bind("<Alt-h>", self.do_help)
 		w3prev_btn = ttk.Button(w3btn_frame, text="Back", command=w3_back)
 		w3prev_btn.grid(row=0, column=1, sticky=tk.E, padx=3)
-		w3ok_btn = ttk.Button(w3btn_frame, text="OK", command=self.do_select)
+		w3ok_btn = ttk.Button(w3btn_frame, text="OK", command=self.do_select, underline=0)
 		w3ok_btn.grid(row=0, column=2, sticky=tk.E, padx=3)
+		self.dlg.bind('<Alt-o>', self.do_select)
 		w3cancel_btn = ttk.Button(w3btn_frame, text="Cancel", command=self.do_cancel)
 		w3cancel_btn.grid(row=0, column=3, sticky=tk.E, padx=(3,6))
 		w3ok_btn["state"] = tk.DISABLED
 	
 	def do_help(self, *args):
 		webbrowser.open("https://mapdata.osdn.io/dialogs.html#open-spreadsheet-data-file", new=2, autoraise=True)
 	def do_cancel(self, *args):
@@ -2364,16 +2541,17 @@
 					self.lon_sel["values"] = self.header_list
 					self.sym_sel["values"] = self.header_list
 					self.col_sel["values"] = self.header_list
 					wiz2_frame.lift()
 				conn.close()
 
 
-		w1help_btn = ttk.Button(w1btnframe, text="Help", command=self.do_help)
+		w1help_btn = ttk.Button(w1btnframe, text="Help", command=self.do_help, underline=0)
 		w1help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		self.dlg.bind("<Alt-h>", self.do_help)
 		w1next_btn = ttk.Button(w1btnframe, text="Next", command=w1_next)
 		w1next_btn.grid(row=0, column=1, sticky=tk.E, padx=3)
 		w1cancel_btn = ttk.Button(w1btnframe, text="Cancel", command=self.do_cancel)
 		w1cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=(3,6))
 		w1next_btn["state"] = tk.DISABLED
 		self.dlg.bind("<Escape>", self.do_cancel)
 		
@@ -2441,20 +2619,22 @@
 		def w2_back():
 			wiz1_frame.lift()
 
 		w2btn_frame = tk.Frame(wiz2_frame, borderwidth=3, relief=tk.RIDGE)
 		w2btn_frame.grid(row=2, column=0, sticky=tk.S+tk.EW, padx=(3,3), pady=(3,3))
 		w2btn_frame.columnconfigure(0, weight=1)
 		#
-		w2help_btn = ttk.Button(w2btn_frame, text="Help", command=self.do_help)
+		w2help_btn = ttk.Button(w2btn_frame, text="Help", command=self.do_help, underline=0)
 		w2help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		self.dlg.bind("<Alt-h>", self.do_help)
 		w2prev_btn = ttk.Button(w2btn_frame, text="Back", command=w2_back)
 		w2prev_btn.grid(row=0, column=1, sticky=tk.E, padx=3)
-		w2ok_btn = ttk.Button(w2btn_frame, text="OK", command=self.do_select)
+		w2ok_btn = ttk.Button(w2btn_frame, text="OK", command=self.do_select, underline=0)
 		w2ok_btn.grid(row=0, column=2, sticky=tk.E, padx=3)
+		self.dlg.bind('<Alt-o>', self.do_select)
 		w2cancel_btn = ttk.Button(w2btn_frame, text="Cancel", command=self.do_cancel)
 		w2cancel_btn.grid(row=0, column=3, sticky=tk.E, padx=(3,6))
 		w2ok_btn["state"] = tk.DISABLED
 	
 
 		# Bindings
 		self.dlg.bind('<Return>', self.do_select)
@@ -2506,18 +2686,20 @@
 		crs_lbl = ttk.Label(prompt_frame, text="New CRS:")
 		crs_lbl.grid(row=0, column=0, sticky=tk.E, padx=(3,3))
 		self.crs_var = tk.IntVar(self.dlg, current_crs)
 		self.crs_entry = ttk.Entry(prompt_frame, width=12, textvariable=self.crs_var)
 		self.crs_entry.grid(row=0, column=1, sticky=tk.W, padx=(3,3))
 		# Buttons
 		self.canceled = False
-		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help)
+		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help, underline=0)
 		help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
-		ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select)
+		self.dlg.bind("<Alt-h>", self.do_help)
+		ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select, underline=0)
 		ok_btn.grid(row=0, column=1, sticky=tk.E, padx=(3,3))
+		self.dlg.bind('<Alt-o>', self.do_select)
 		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
 		cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=(3,6))
 		self.dlg.bind("<Return>", self.do_select)
 		self.dlg.bind("<Escape>", self.do_cancel)
 	def do_help(self, *args):
 		webbrowser.open("https://mapdata.osdn.io/dialogs.html#change-crs", new=2, autoraise=True)
 	def do_cancel(self, *args):
@@ -2557,14 +2739,16 @@
 		sql_frame = tk.Frame(query_frame)
 		sql_frame.grid(row=0, column=0, sticky=tk.NSEW, padx=(3,3), pady=(3,3))
 		sql_frame.rowconfigure(0, weight=1)
 		sql_frame.columnconfigure(0, weight=1)
 		col_frame = tk.Frame(query_frame)
 		col_frame.grid(row=0, column=1, sticky=tk.NS, padx=(3,3), pady=(3,3))
 		col_frame.rowconfigure(0, weight=1)
+		act_frame = tk.Frame(query_frame)
+		act_frame.grid(row=1, column=0, sticky=tk.EW, padx=(3,3), pady=(3,3))
 		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
 		btn_frame.grid(row=2, column=0, sticky=tk.EW, pady=(3,3))
 		btn_frame.columnconfigure(0, weight=1)
 		# Prompt
 		prompt_lbl = ttk.Label(prompt_frame, wraplength=300, justify=tk.LEFT, text="Enter an expression below to identify the data rows that you want to select.  The syntax of this expression should correspond to a SQL 'WHERE' clause.  Column names with non-alphanumeric characters should be double-quoted.  String literals should be single-quoted.  The '%' character is a wildcard.  Ctrl-Enter completes entry.")
 		prompt_lbl.grid(row=0, column=0, sticky=tk.EW, padx=(3,3))
 		def wrap_prompt(event):
@@ -2588,18 +2772,14 @@
 		colsel.grid(row=1, column=0, sticky=tk.NW, padx=(3,3), pady=(3,3))
 		tv_frame = tk.Frame(col_frame)
 		tv_frame.grid(row=2, column=0, sticky=tk.NS, padx=(3,3), pady=(3,3))
 		col_frame.rowconfigure(0, weight=0)
 		col_frame.rowconfigure(1, weight=0)
 		col_frame.rowconfigure(2, weight=1)
 		def colval_to_sql(event):
-			#sel_items = self.tv_tbl.selection()
-			#if not sel_items:
-			#	return
-			#item_iid = sel_items[0]
 			item_iid = self.tv_tbl.identify('item', event.x, event.y)
 			item_val = self.tv_tbl.item(item_iid, "values")[0]
 			if not isfloat(item_val):
 				item_val = "'%s'" % item_val
 			self.sql_text.insert(tk.END, " "+item_val)
 		def list_col_vals(event):
 			curs = db_conn.cursor()
@@ -2609,20 +2789,28 @@
 			for widget in tv_frame.winfo_children():
 				widget.destroy()
 			tblframe, self.tv_tbl = treeview_table(tv_frame, rowset, [col_var.get()])
 			tblframe.grid(column=0, row=0, sticky=tk.NSEW)
 			curs.close()
 			self.tv_tbl.bind("<Double-1>", colval_to_sql)
 		colsel.bind("<<ComboboxSelected>>", list_col_vals)
+		# Action selection
+		self.act_var = tk.StringVar(act_frame, "Replace")
+		act_lbl = ttk.Label(act_frame, text="Action:")
+		act_lbl.grid(row=0, column=0, sticky=tk.E, padx=(6,3))
+		act_sel = ttk.Combobox(act_frame, state="readonly", textvariable=self.act_var, values=["Replace", "Add", "Remove"], width=8)
+		act_sel.grid(row=0, column=1, sticky=tk.W, padx=(3,6))
 		# Buttons
 		self.canceled = False
-		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help)
+		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help, underline=0)
 		help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
-		ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select)
+		self.dlg.bind("<Alt-h>", self.do_help)
+		ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select, underline=0)
 		ok_btn.grid(row=0, column=1, sticky=tk.E, padx=(3,3))
+		self.dlg.bind('<Alt-o>', self.do_select)
 		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
 		cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=(3,6))
 		self.dlg.bind("<Escape>", self.do_cancel)
 		self.dlg.bind("<Control-Return>", self.do_select)
 	def do_help(self, *args):
 		webbrowser.open("https://mapdata.osdn.io/dialogs.html#query-data", new=2, autoraise=True)
 	def do_cancel(self, *args):
@@ -2634,17 +2822,17 @@
 		self.dlg.destroy()
 	def get_where(self):
 		self.dlg.grab_set()
 		center_window(self.dlg)
 		self.sql_text.focus()
 		self.dlg.wait_window(self.dlg)
 		if not self.canceled:
-			return self.sql
+			return (self.sql, self.act_var.get())
 		else:
-			return None
+			return (None, None)
 
 
 class PlotDialog(object):
 	def __init__(self, parent, column_specs):
 		self.parent = parent
 		self.column_specs = column_specs
 		self.dataset = None
@@ -2669,15 +2857,15 @@
 		ctrl_frame = tk.Frame(self.dlg)
 		ctrl_frame.grid(row=1, column=0, sticky=tk.N+tk.EW)
 
 		self.type_var = tk.StringVar(ctrl_frame, "")
 		type_lbl = ttk.Label(ctrl_frame, text="Plot type:")
 		type_lbl.grid(row=0, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
 		self.type_sel = ttk.Combobox(ctrl_frame, state="readonly", textvariable=self.type_var, width=20,
-				values=["Box plot", "Category counts", "Line plot", "Scatter plot", "Value counts",  "Y range plot"])
+				values=["Box plot", "Category counts", "Empirical CDF", "Histogram", "Line plot", "Scatter plot", "Y range plot"])
 		self.type_sel.grid(row=0, column=1, sticky=tk.W, padx=(3,6), pady=(3,3))
 		self.type_sel.bind("<<ComboboxSelected>>", self.set_xy)
 
 		self.sel_only_var = tk.StringVar(ctrl_frame, "0")
 		self.sel_only_ck = ttk.Checkbutton(ctrl_frame, text="Selected data only", command=self.q_redraw, variable=self.sel_only_var,
 				onvalue="1", offvalue="0")
 		self.sel_only_ck.grid(row=1, column=0, columnspan=2, sticky=tk.W, padx=(6,6), pady=(3,3))
@@ -2726,27 +2914,29 @@
 		btn_frame.columnconfigure(0, weight=1)
 		btn_frame.grid(row=3, column=0, sticky=tk.EW, pady=(3,3))
 		btn_frame.columnconfigure(0, weight=0)
 		btn_frame.columnconfigure(1, weight=0)
 		btn_frame.columnconfigure(2, weight=0)
 		btn_frame.columnconfigure(3, weight=1)
 		self.canceled = False
-		self.help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help)
+		self.help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help, underline=0)
 		self.help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		self.dlg.bind("<Alt-h>", self.do_help)
 		self.data_btn = ttk.Button(btn_frame, text="Source Data", state="disabled", command=self.show_data)
 		self.data_btn.grid(row=0, column=1, sticky=tk.W, padx=(3,3))
 		self.plot_data_btn = ttk.Button(btn_frame, text="Plot Data", state="disabled", command=self.show_plot_data)
 		self.plot_data_btn.grid(row=0, column=2, sticky=tk.W, padx=(3,6))
-		close_btn = ttk.Button(btn_frame, text="Close", command=self.do_close)
+		close_btn = ttk.Button(btn_frame, text="Close", command=self.do_close, underline=0)
 		close_btn.grid(row=0, column=3, sticky=tk.E, padx=(6,6))
+		self.dlg.bind("<Alt-c>", self.do_close)
 		self.dlg.bind("<Escape>", self.do_close)
 		center_window(self.dlg)
 		raise_window(self.dlg)
 
-	def do_help(self):
+	def do_help(self, *args):
 		webbrowser.open("https://mapdata.osdn.io/dialogs.html#plot-dialog", new=2, autoraise=True)
 
 	def show_data(self):
 		# Show data that have been collected for plotting, but not summarized as needed for a particular plot type.
 		if self.dataset is not None:
 			dlg = MsgDialog("Source Data", "Original data:")
 			variables = len(self.dataset)
@@ -2757,15 +2947,15 @@
 					row.append(self.dataset[j][i])
 				rowwise_data.append(row)
 			tframe, tdata = treeview_table(dlg.content_frame, rowwise_data, self.data_labels)
 			tframe.grid(row=0, column=0, sticky=tk.NSEW)
 			dlg.show()
 
 	def show_plot_data(self):
-		# Show data that have been collected for plotting, but not summarized as needed for a particular plot type.
+		# Show data as summarized for a particular plot type.
 		if self.plot_data is not None:
 			dlg = MsgDialog("Data for Plotting", "Data to be plotted:")
 			variables = len(self.plot_data)
 			rowwise_data = []
 			max_data_len = max([len(self.plot_data[i]) for i in range(variables)])
 			for i in range(max_data_len):
 				row = []
@@ -2777,44 +2967,46 @@
 						row.append(None)
 				rowwise_data.append(row)
 			tframe, tdata = treeview_table(dlg.content_frame, rowwise_data, self.plot_data_labels)
 			tframe.grid(row=0, column=0, sticky=tk.NSEW)
 			dlg.show()
 
 	def set_xy(self, *args):
-		# Enable X and Y value selection, and set values based on plot type and column types.
-		# Conditionally (re)draw the plot.
+		# Enable X and Y value selection, and set Combobox values based on plot type and column types.
 		self.plotfig.clear()
 		self.plot_axes = self.plotfig.add_subplot(111)
 		self.plotfig_canvas.draw()
 		self.dataset = None
 		self.data_labels = None
 		self.plot_data = None
 		self.plot_data_labels = None
 		self.data_btn["state"] = "disabled"
 		self.plot_data_btn["state"] = "disabled"
 		categ_columns = [c[0] for c in self.column_specs if c[1] == "string"]
+		# quant_columns includes date and timestamp columns
 		quant_columns = [c[0] for c in self.column_specs if c[1] != "string"]
+		numeric_columns = [c[0] for c in self.column_specs if c[1] in ("int", "float")]
+		date_columns = [c[0] for c in self.column_specs if c[1] == "date"]
 		plot_type = self.type_var.get()
 		self.x_var.set('')
 		self.y_var.set('')
 		if plot_type == "Category counts":
 			self.x_sel["values"] = categ_columns
 			self.xlog_ck["state"] = "disabled"
 			self.x_sel["state"] = "readonly"
 			self.y_sel["state"] = "disabled"
 			self.ylog_ck["state"] = "disabled"
-		elif plot_type == "Value counts":
-			self.x_sel["values"] = quant_columns
+		elif plot_type in ("Histogram", "Empirical CDF"):
+			self.x_sel["values"] = numeric_columns
 			self.xlog_ck["state"] = "normal"
 			self.x_sel["state"] = "readonly"
 			self.y_sel["state"] = "disabled"
 			self.ylog_ck["state"] = "disabled"
 		elif plot_type == "Box plot":
-			self.x_sel["values"] = categ_columns
+			self.x_sel["values"] = list(set(categ_columns) | set(date_columns))
 			self.xlog_ck["state"] = "disabled"
 			self.y_sel["values"] = quant_columns
 			self.x_sel["state"] = "readonly"
 			self.y_sel["state"] = "readonly"
 			self.ylog_ck["state"] = "normal"
 		else:
 			self.x_sel["values"] = quant_columns
@@ -2823,15 +3015,15 @@
 			self.x_sel["state"] = "readonly"
 			self.y_sel["state"] = "readonly"
 			self.ylog_ck["state"] = "normal"
 
 	def q_redraw(self, *args):
 		# Conditionally (re)draw the plot.
 		plot_type = self.type_var.get()
-		can_redraw = (plot_type in ("Category counts", "Value counts") and self.x_var.get() != '') \
+		can_redraw = (plot_type in ("Category counts", "Empirical CDF", "Histogram") and self.x_var.get() != '') \
 				or (plot_type in ("Scatter plot", "Line plot", "Box plot", "Y range plot") and self.x_var.get() != '' and self.y_var.get() != '')
 		if can_redraw:
 			self.plotfig.clear()
 			self.plot_axes = self.plotfig.add_subplot(111)
 			self.plotfig_canvas.draw()
 			self.get_data()
 			if self.dataset is not None:
@@ -2876,64 +3068,72 @@
 				for i in range(len(clean_data[0])):
 					clean_data[0][i] = cast_fn(clean_data[0][i])
 			if self.y_sel["state"] != "disabled" and self.y_var.get() != "" and len(clean_data) > 1:
 				y_data_type = [cs[1] for cs in self.column_specs if cs[0] == self.y_var.get()][0]
 				cast_fn = data_type_cast_fn(y_data_type)
 				for i in range(len(clean_data[1])):
 					clean_data[1][i] = cast_fn(clean_data[1][i])
-			# Log-transform data if specified.
-			if (self.xlog_ck["state"] != "disabled" and self.xlog_var.get() == "1") or (self.ylog_ck["state"] != "disabled" and self.ylog_var.get() == "1" and len(clean_data) > 1):
-				log_data = [[] for _ in clean_data]
-				log_error = False
-				if self.xlog_ck["state"] != "disabled" and self.xlog_var.get() == "1":
-					for i in range(len(clean_data[0])):
-						try:
-							log_data[0].append(math.log10(clean_data[0][i]))
-						except:
-							log_error = True
-							break
-				else:
-					log_data[0] = clean_data[0]
-				if not log_error and self.ylog_ck["state"] != "disabled" and self.ylog_var.get() == "1" and len(clean_data) > 1:
-					for i in range(len(clean_data[1])):
-						try:
-							log_data[1].append(math.log10(clean_data[1][i]))
-						except:
-							log_error = True
-							break
-				else:
-					if len(clean_data) > 1:
-						log_data[1] = clean_data[1]
-				if not log_error:
-					clean_data = log_data
-				log_data = None
-			self.dataset = clean_data
+			# Set data labels
 			if self.y_var.get() != '':
 				self.data_labels = [self.x_var.get(), self.y_var.get()]
 			else:
 				self.data_labels = [self.x_var.get()]
+			# Log-transform data if specified.
+			log_data = [[] for _ in clean_data]
+			log_error = False
+			if self.xlog_ck["state"] != "disabled" and self.xlog_var.get() == "1":
+				for i in range(len(clean_data[0])):
+					try:
+						log_data[0].append(math.log10(clean_data[0][i]))
+					except:
+						log_error = True
+						break
+				if not log_error:
+					clean_data[0] = log_data[0]
+					self.data_labels[0] = "Log10 of " + self.x_var.get()
+			if self.ylog_ck["state"] != "disabled" and self.ylog_var.get() == "1" and len(clean_data) > 1:
+				log_error = False
+				for i in range(len(clean_data[1])):
+					try:
+						log_data[1].append(math.log10(clean_data[1][i]))
+					except:
+						log_error = True
+						break
+				if not log_error:
+					clean_data[1] = log_data[1]
+					self.data_labels[1] = "Log10 of " + self.y_var.get()
+			log_data = None
+			#
+			self.dataset = clean_data
 			self.data_btn["state"] = "normal"
 			# Summarize and sort the data as needed for each type of plot.
 			if plot_type == "Category counts":
 				# Count of values for each X, ordered by X
 				counter = collections.Counter(self.dataset[0])
 				x_vals = list(counter.keys())
 				x_vals.sort()
 				x_counts = [counter[k] for k in x_vals]
 				self.plot_data = [x_vals, x_counts]
-				self.plot_data_labels = [self.x_var.get(), "Count"]
+				#self.plot_data_labels = [self.x_var.get(), "Count"]
+				self.plot_data_labels = [self.data_labels[0], "Count"]
 			elif plot_type == "Box plot":
 				# A list of Y values for each X value
 				x_vals = list(set(self.dataset[0]))
 				ds = list(zip(self.dataset[0], self.dataset[1]))
 				plot_data = []
 				for x in x_vals:
 					plot_data.append([d[1] for d in ds if d[0] == x])
 				self.plot_data = plot_data
 				self.plot_data_labels = x_vals
+			elif plot_type == "Empirical CDF":
+				# Y is the fraction of data points below each X value
+				x_counts = np.unique(self.dataset[0], return_counts=True)
+				y_vals = list(np.cumsum(x_counts[1]/np.sum(x_counts[1])))
+				self.plot_data = [list(x_counts[0]), y_vals]
+				self.plot_data_labels = [self.data_labels[0], "Cumulative frequency"]
 			elif plot_type == "Y range plot":
 				# Min and max Y for each X
 				x_vals = list(set(self.dataset[0]))
 				x_vals.sort()
 				y_vals = [[None, None]] * len(x_vals)
 				plotdata = dict(zip(x_vals, y_vals))
 				for i in range(len(self.dataset[0])):
@@ -2951,50 +3151,54 @@
 			elif plot_type == "Line plot":
 				# Sort by X
 				ds = list(zip(self.dataset[0], self.dataset[1]))
 				ds.sort()
 				ds2 = list(zip(*ds))
 				self.plot_data = [list(ds2[0]), list(ds2[1])]
 				self.plot_data_labels = self.data_labels
-			elif plot_type in ("Value counts", "Scatter plot", "Y range plot"):
+			elif plot_type in ("Histogram", "Scatter plot", "Y range plot"):
 				# No special preparation
 				self.plot_data = self.dataset
 				self.plot_data_labels = self.data_labels
 			self.plot_data_btn["state"] = "normal"
 
 	def redraw(self):
 		#self.plotfig.clear()
 		#self.plot_axes = self.plotfig.add_subplot(111)
 		#self.plotfig_canvas.draw()
 		plot_type = self.type_var.get()
 		if self.plot_data is not None and len(self.plot_data[0]) > 0:
 			if plot_type == "Category counts":
 				self.plot_axes.bar(self.plot_data[0], self.plot_data[1])
-				self.plot_axes.set_xlabel(self.x_var.get())
-				self.plot_axes.set_ylabel("Counts")
-			elif plot_type == "Value counts":
+				self.plot_axes.set_xlabel(self.plot_data_labels[0])
+				self.plot_axes.set_ylabel(self.plot_data_labels[1])
+			elif plot_type == "Histogram":
 				self.plot_axes.hist(self.plot_data[0])
 				self.plot_axes.set_xlabel(self.x_var.get())
 				self.plot_axes.set_ylabel("Counts")
 			elif plot_type == "Scatter plot":
 				self.plot_axes.scatter(self.plot_data[0], self.plot_data[1])
-				self.plot_axes.set_xlabel(self.x_var.get())
-				self.plot_axes.set_ylabel(self.y_var.get())
+				self.plot_axes.set_xlabel(self.plot_data_labels[0])
+				self.plot_axes.set_ylabel(self.plot_data_labels[1])
 			elif plot_type == "Line plot":
 				self.plot_axes.plot(self.plot_data[0], self.plot_data[1])
-				self.plot_axes.set_xlabel(self.x_var.get())
-				self.plot_axes.set_ylabel(self.y_var.get())
+				self.plot_axes.set_xlabel(self.plot_data_labels[0])
+				self.plot_axes.set_ylabel(self.plot_data_labels[1])
+			elif plot_type == "Empirical CDF":
+				self.plot_axes.stackplot(self.plot_data[0], self.plot_data[1])
+				self.plot_axes.set_xlabel(self.plot_data_labels[0])
+				self.plot_axes.set_ylabel(self.plot_data_labels[1])
 			elif plot_type == "Y range plot":
 				self.plot_axes.fill_between(self.plot_data[0], self.plot_data[1], self.plot_data[2])
 				self.plot_axes.set_xlabel(self.x_var.get())
 				self.plot_axes.set_ylabel(self.y_var.get())
 			elif plot_type == "Box plot":
 				self.plot_axes.boxplot(self.plot_data, labels=self.plot_data_labels)
 				self.plot_axes.set_xlabel(self.x_var.get())
-				self.plot_axes.set_ylabel(self.y_var.get())
+				self.plot_axes.set_ylabel(self.data_labels[1])
 			self.plotfig_canvas.draw()
 			self.plot_nav.update()
 
 	def do_close(self, *args):
 		self.parent.remove_plot(self)
 		self.dlg.destroy()
 	def show(self):
@@ -3064,15 +3268,15 @@
 		db_btn.grid(row=0, column=2, sticky=tk.EW, padx=(3,3), pady=(3,3))
 		# Help and Cancel buttons
 		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
 		btn_frame.columnconfigure(0, weight=1)
 		btn_frame.grid(row=2, column=0, sticky=tk.S+tk.EW, padx=(3,3), pady=(3,3))
 		btn_frame.columnconfigure(0, weight=1)
 		self.canceled = False
-		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help)
+		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help, underline=0)
 		help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
 		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
 		cancel_btn.grid(row=0, column=0, sticky=tk.E, padx=(3,6))
 		self.dlg.bind("<Escape>", self.do_cancel)
 	def do_help(self, *args):
 		webbrowser.open("https://mapdata.osdn.io/", new=2, autoraise=True)
 	def sel_csv(self):
@@ -3796,14 +4000,24 @@
 		global location_color
 		loc_color = cp.get(_DEFAULTS_SECTION, "location_color")
 		if loc_color is not None:
 			if loc_color not in color_names:
 				warning("Invalid argument to the 'location_color' configuration option", kwargs={})
 			else:
 				location_color = loc_color
+	if cp.has_option(_DEFAULTS_SECTION, "use_data_marker"):
+		global use_data_marker
+		loc_mkr = cp.getboolean(_DEFAULTS_SECTION, "use_data_marker")
+		if loc_mkr is not None:
+			use_data_marker = loc_mkr
+	if cp.has_option(_DEFAULTS_SECTION, "use_data_color"):
+		global use_data_color
+		loc_clr = cp.getboolean(_DEFAULTS_SECTION, "use_data_color")
+		if loc_clr is not None:
+			use_data_color = loc_clr
 	if cp.has_option(_DEFAULTS_SECTION, "select_symbol"):
 		global select_symbol
 		default_symbol = cp.get(_DEFAULTS_SECTION, "select_symbol")
 		if default_symbol is not None:
 			if default_symbol not in icon_xbm:
 				warning("Unrecognized symbol name for the 'select_symbol' configuration option", kwargs={})
 			else:
```

### Comparing `mapdata-2.0.2/mapdata.egg-info/PKG-INFO` & `mapdata-2.3.0/mapdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.0.2
+Version: 2.3.0
 Summary: An interactive map and table explorer for geographic coordinates in a CSV file
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
```

### Comparing `mapdata-2.0.2/setup.py` & `mapdata-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import io
 
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 setuptools.setup(name='mapdata',
-	version='2.0.2',
+	version='2.3.0',
 	description="An interactive map and table explorer for geographic coordinates in a CSV file",
 	author='Dreas Nielsen',
 	author_email='dreas.nielsen@gmail.com',
     url='https://osdn.net/project/mapdata/',
 	scripts=['mapdata/mapdata.py'],
     license='GPL',
 	requires=['tkintermapview', 'pyproj', 'odfpy', 'openpyxl', 'xlrd', 'matplotlib'],
```

