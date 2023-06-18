# Comparing `tmp/wgd-2.0.18.tar.gz` & `tmp/wgd-2.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wgd-2.0.18.tar", last modified: Sat Jun 17 12:59:14 2023, max compression
+gzip compressed data, was "dist/wgd-2.0.19.tar", last modified: Sun Jun 18 07:45:54 2023, max compression
```

## Comparing `wgd-2.0.18.tar` & `wgd-2.0.19.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-17 12:59:14.156237 wgd-2.0.18/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.18/LICENSE
--rwxrwxrwx   0 heche     (1000) heche     (1000)    47387 2023-06-17 12:59:14.156237 wgd-2.0.18/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)    47149 2023-06-17 12:28:46.000000 wgd-2.0.18/README.md
--rwxrwxrwx   0 heche     (1000) heche     (1000)    52094 2023-06-17 12:58:16.000000 wgd-2.0.18/cli.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-06-17 12:59:14.157405 wgd-2.0.18/setup.cfg
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1904 2023-06-17 12:59:03.000000 wgd-2.0.18/setup.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-17 12:59:14.139747 wgd-2.0.18/test/
--rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-06-06 22:05:06.000000 wgd-2.0.18/test/test_core.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-17 12:59:14.149236 wgd-2.0.18/wgd/
--rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.18/wgd/__init__.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.18/wgd/beast.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.18/wgd/cluster.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     8819 2022-12-04 21:40:23.000000 wgd-2.0.18/wgd/codeml.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   135263 2023-06-15 13:48:21.000000 wgd-2.0.18/wgd/core.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    17148 2023-03-17 14:15:45.000000 wgd-2.0.18/wgd/mcmctree.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.18/wgd/mix.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   103616 2023-06-06 22:05:06.000000 wgd-2.0.18/wgd/peak.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)     4722 2023-06-06 22:05:06.000000 wgd-2.0.18/wgd/postplot.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    17378 2023-06-15 09:47:26.000000 wgd-2.0.18/wgd/syn.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)    28647 2023-06-06 22:05:06.000000 wgd-2.0.18/wgd/utils.py
--rwxrwxrwx   0 heche     (1000) heche     (1000)   144926 2023-06-17 12:20:32.000000 wgd-2.0.18/wgd/viz.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-17 12:59:14.155238 wgd-2.0.18/wgd.egg-info/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    47387 2023-06-17 12:59:14.000000 wgd-2.0.18/wgd.egg-info/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)      385 2023-06-17 12:59:14.000000 wgd-2.0.18/wgd.egg-info/SOURCES.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-06-17 12:59:14.000000 wgd-2.0.18/wgd.egg-info/dependency_links.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       32 2023-06-17 12:59:14.000000 wgd-2.0.18/wgd.egg-info/entry_points.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)      749 2023-06-17 12:59:14.000000 wgd-2.0.18/wgd.egg-info/requires.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2023-06-17 12:59:14.000000 wgd-2.0.18/wgd.egg-info/top_level.txt
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-18 07:45:54.949756 wgd-2.0.19/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    35071 2022-09-25 05:52:37.000000 wgd-2.0.19/LICENSE
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    48426 2023-06-18 07:45:54.949756 wgd-2.0.19/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    48188 2023-06-18 07:41:38.000000 wgd-2.0.19/README.md
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    52989 2023-06-18 07:39:20.000000 wgd-2.0.19/cli.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-06-18 07:45:54.949756 wgd-2.0.19/setup.cfg
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1904 2023-06-18 07:42:00.000000 wgd-2.0.19/setup.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-18 07:45:54.933493 wgd-2.0.19/test/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     4521 2023-06-06 22:05:06.000000 wgd-2.0.19/test/test_core.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-18 07:45:54.949756 wgd-2.0.19/wgd/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      711 2022-09-25 05:52:37.000000 wgd-2.0.19/wgd/__init__.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    31126 2022-12-22 23:06:45.000000 wgd-2.0.19/wgd/beast.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     1685 2022-09-30 07:30:21.000000 wgd-2.0.19/wgd/cluster.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     8819 2022-12-04 21:40:23.000000 wgd-2.0.19/wgd/codeml.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   135263 2023-06-15 13:48:21.000000 wgd-2.0.19/wgd/core.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    17148 2023-03-17 14:15:45.000000 wgd-2.0.19/wgd/mcmctree.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    14140 2023-03-01 13:14:50.000000 wgd-2.0.19/wgd/mix.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   103616 2023-06-06 22:05:06.000000 wgd-2.0.19/wgd/peak.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     4722 2023-06-06 22:05:06.000000 wgd-2.0.19/wgd/postplot.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    17378 2023-06-15 09:47:26.000000 wgd-2.0.19/wgd/syn.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    28647 2023-06-06 22:05:06.000000 wgd-2.0.19/wgd/utils.py
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   145288 2023-06-18 06:57:28.000000 wgd-2.0.19/wgd/viz.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-06-18 07:45:54.949756 wgd-2.0.19/wgd.egg-info/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    48426 2023-06-18 07:45:54.000000 wgd-2.0.19/wgd.egg-info/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      385 2023-06-18 07:45:54.000000 wgd-2.0.19/wgd.egg-info/SOURCES.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-06-18 07:45:54.000000 wgd-2.0.19/wgd.egg-info/dependency_links.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       32 2023-06-18 07:45:54.000000 wgd-2.0.19/wgd.egg-info/entry_points.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      749 2023-06-18 07:45:54.000000 wgd-2.0.19/wgd.egg-info/requires.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        8 2023-06-18 07:45:54.000000 wgd-2.0.19/wgd.egg-info/top_level.txt
```

### Comparing `wgd-2.0.18/LICENSE` & `wgd-2.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `wgd-2.0.18/PKG-INFO` & `wgd-2.0.19/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: wgd
-Version: 2.0.18
-Summary: wgd
-Home-page: http://github.com/heche-psb/wgd
-Author: Hengchi Chen
-Author-email: heche@psb.vib-ugent.be
-License: GPL
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 
 # `wgd v2` : a suite tool of WGD inference and timing
 
 [![Build Status](https://app.travis-ci.com/heche-psb/wgd.svg?branch=phylodating)](https://app.travis-ci.com/heche-psb/wgd)
 [![Documentation Status](https://readthedocs.org/projects/wgdv2/badge/?version=latest)](https://wgdv2.readthedocs.io/en/latest/?badge=latest)
 [![license](https://img.shields.io/pypi/l/wgd.svg)](https://pypi.python.org/pypi/wgd)
@@ -249,14 +238,18 @@
 -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
 -ms, --maxsize, the maximum family size to include, default 200
 -r, --ks_range, the Ks range in colored dotplot, default (0, 5)
 --iadhore_options, the parameter setting in iadhore, default 
 -ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
 -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
 -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+-mgn, --mingenenum, the minimum number of genes for a segment to be considered, default 30
+-ds, --dotsize, the dot size in dot plot, default 1
+-aa, --apalpha, the opacity of anchor dots, default 1
+-ha, --hoalpha, the opacity of homolog dots, default 0.1
 ```
 
 The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
 ```
 wgd viz (option)
 --------------------------------------------------------------------------------
 -d, --datafile, the Ks datafile, default None
@@ -279,14 +272,19 @@
 -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
 -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
 -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
 -epk, --extraparanomeks, extra paranome Ks data to plot in the mixed Ks distribution, default None
 -pag, --plotapgmm, flag option, whether to plot mixture modeling of anchor Ks in the mixed Ks distribution, if the flag was set, the mixture modeling of anchor Ks will be plotted
 -pem, --plotelmm, flag option, whether to plot elmm mixture modeling of paranome Ks in the mixed Ks distribution, if the flag was set, the elmm mixture modeling of paranome Ks will be plotted
 -c, --components, the range of the number of components to fit in anchor Ks mixture modeling, default (1,4)
+-mgn, --mingenenum, the minimum number of genes for a segment to be considered, default 30
+-psy, --plotsyn, flag option, whether to initiate the synteny plot, if the flag was set, the synteny plot will be produced
+-ds, --dotsize, the dot size in dot plot, default 1
+-aa, --apalpha, the opacity of anchor dots, default 1
+-ha, --hoalpha, the opacity of homolog dots, default 0.1
 ```
 
 ## Usage
 
 Here we provided the basic usage for each program.
 
 ### wgd dmd
@@ -443,14 +441,16 @@
 
 The dot plots without *K*<sub>S</sub> annotation will also be automately produced, as shown below.
 
 ![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot_unit_gene.png)
 
 ![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
 
+Note that the opacity of anchor dots and all homolog dots can be set by the option `apalpha` and `hoalpha` separately. If one just wants to see the anchor dots, setting the `hoalpha` as 0 (or other minuscule values) will do. If one wants to see the distribution of whole dots better, setting the `hoalpha` higher (and `apalpha` lower) will do. The `dotsize` option can be called to adjust the size of dots.
+
 A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
 
 ![](data/Syndepth.svg)
 
 We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
 
 ```
```

### Comparing `wgd-2.0.18/README.md` & `wgd-2.0.19/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: wgd
+Version: 2.0.19
+Summary: wgd
+Home-page: http://github.com/heche-psb/wgd
+Author: Hengchi Chen
+Author-email: heche@psb.vib-ugent.be
+License: GPL
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 
 # `wgd v2` : a suite tool of WGD inference and timing
 
 [![Build Status](https://app.travis-ci.com/heche-psb/wgd.svg?branch=phylodating)](https://app.travis-ci.com/heche-psb/wgd)
 [![Documentation Status](https://readthedocs.org/projects/wgdv2/badge/?version=latest)](https://wgdv2.readthedocs.io/en/latest/?badge=latest)
 [![license](https://img.shields.io/pypi/l/wgd.svg)](https://pypi.python.org/pypi/wgd)
@@ -238,14 +249,18 @@
 -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
 -ms, --maxsize, the maximum family size to include, default 200
 -r, --ks_range, the Ks range in colored dotplot, default (0, 5)
 --iadhore_options, the parameter setting in iadhore, default 
 -ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
 -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
 -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+-mgn, --mingenenum, the minimum number of genes for a segment to be considered, default 30
+-ds, --dotsize, the dot size in dot plot, default 1
+-aa, --apalpha, the opacity of anchor dots, default 1
+-ha, --hoalpha, the opacity of homolog dots, default 0.1
 ```
 
 The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
 ```
 wgd viz (option)
 --------------------------------------------------------------------------------
 -d, --datafile, the Ks datafile, default None
@@ -268,14 +283,19 @@
 -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
 -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
 -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
 -epk, --extraparanomeks, extra paranome Ks data to plot in the mixed Ks distribution, default None
 -pag, --plotapgmm, flag option, whether to plot mixture modeling of anchor Ks in the mixed Ks distribution, if the flag was set, the mixture modeling of anchor Ks will be plotted
 -pem, --plotelmm, flag option, whether to plot elmm mixture modeling of paranome Ks in the mixed Ks distribution, if the flag was set, the elmm mixture modeling of paranome Ks will be plotted
 -c, --components, the range of the number of components to fit in anchor Ks mixture modeling, default (1,4)
+-mgn, --mingenenum, the minimum number of genes for a segment to be considered, default 30
+-psy, --plotsyn, flag option, whether to initiate the synteny plot, if the flag was set, the synteny plot will be produced
+-ds, --dotsize, the dot size in dot plot, default 1
+-aa, --apalpha, the opacity of anchor dots, default 1
+-ha, --hoalpha, the opacity of homolog dots, default 0.1
 ```
 
 ## Usage
 
 Here we provided the basic usage for each program.
 
 ### wgd dmd
@@ -432,14 +452,16 @@
 
 The dot plots without *K*<sub>S</sub> annotation will also be automately produced, as shown below.
 
 ![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot_unit_gene.png)
 
 ![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
 
+Note that the opacity of anchor dots and all homolog dots can be set by the option `apalpha` and `hoalpha` separately. If one just wants to see the anchor dots, setting the `hoalpha` as 0 (or other minuscule values) will do. If one wants to see the distribution of whole dots better, setting the `hoalpha` higher (and `apalpha` lower) will do. The `dotsize` option can be called to adjust the size of dots.
+
 A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
 
 ![](data/Syndepth.svg)
 
 We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
 
 ```
```

### Comparing `wgd-2.0.18/cli.py` & `wgd-2.0.19/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,23 +517,26 @@
 @click.option('--rel_height', '-rh', type=float, default=0.4, show_default=True, help='relative height at which the peak width is measured')
 @click.option('--minseglen', '-mg', default=10000, show_default=True, help="minimum length (ratio if <=1) of segments to show in marco-synteny")
 @click.option('--keepredun', '-kr', is_flag=True, help='keep redundant multiplicons')
 @click.option('--extraparanomeks', '-epk', default=None, help='extra paranome ks data')
 @click.option('--plotapgmm', '-pag', is_flag=True, help='plot mixture modeling of anchor pairs')
 @click.option('--plotelmm', '-pem', is_flag=True, help='plot elmm mixture modeling')
 @click.option('--components', '-n', nargs=2, default=(1, 4), show_default=True, help="range of number of components to fit")
-@click.option('--mingenenum', '-mgn', default=30, type=int, show_default=True, help="min number of genes on segments to be considered")
+@click.option('--mingenenum', '-mgn', default=30, type=int, show_default=True, help="minimum number of genes on segments to be considered")
 @click.option('--plotsyn', '-psy', is_flag=True, help='plot synteny')
+@click.option('--dotsize', '-ds', type=float, default=1, show_default=True, help='size of dots')
+@click.option('--apalpha', '-aa', type=float, default=1, show_default=True, help='opacity of anchor dots')
+@click.option('--hoalpha', '-ha', type=float, default=0.1, show_default=True, help='opacity of homolog dots')
 def viz(**kwargs):
     """
     Visualization of Ks distribution or synteny
     """
     _viz(**kwargs)
 
-def _viz(datafile,spair,outdir,gsmap,plotkde,reweight,em_iterations,em_initializations,prominence_cutoff,segments,minlen,maxsize,anchorpoints,multiplicon,genetable,rel_height,speciestree,onlyrootout,minseglen,keepredun,extraparanomeks,plotapgmm,plotelmm,components,mingenenum,plotsyn):
+def _viz(datafile,spair,outdir,gsmap,plotkde,reweight,em_iterations,em_initializations,prominence_cutoff,segments,minlen,maxsize,anchorpoints,multiplicon,genetable,rel_height,speciestree,onlyrootout,minseglen,keepredun,extraparanomeks,plotapgmm,plotelmm,components,mingenenum,plotsyn,dotsize,apalpha,hoalpha):
     from wgd.viz import elmm_plot, apply_filters, multi_sp_plot, default_plot,all_dotplots,filter_by_minlength,dotplotunitgene,dotplotingene,filter_mingenumber
     from wgd.core import _mkdir
     from wgd.syn import get_anchors,get_multi,get_segments_profile,get_chrom_gene,get_mp_geneorder,transformunit
     from wgd.peak import formatv2
     if datafile!=None: prefix = os.path.basename(datafile)
     _mkdir(outdir)
     if plotsyn:
@@ -548,21 +551,21 @@
         df_multi = get_multi('',userdf2=multiplicon)
         ordered_genes_perchrom_allsp, gene_orders = get_chrom_gene(table,outdir)
         #ordered_mp = get_mp_geneorder(gene_orders,'',outdir,table,userdf4=multipliconpairs)
         segs = get_segments_profile(df_multi,keepredun,'',userdf3=segments)
         segs,table,df_multi,removed_scfa = filter_by_minlength(table,segs,minlen,df_multi,keepredun,outdir,minseglen)
         segs_gene_unit, gene_order_dict_allsp = transformunit(segs,ordered_genes_perchrom_allsp,outdir)
         segs = filter_mingenumber(segs_gene_unit,mingenenum)
-        dotplotingene(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=df_anchor,ksdf=df,maxsize=maxsize)
+        dotplotingene(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=df_anchor,ksdf=df,maxsize=maxsize,dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha)
         #dotplotunitgene(ordered_genes_perchrom_allsp,segs_gene_unit,removed_scfa,outdir,mingenenum,table_orig,ordered_mp,ksdf=df)
-        figs = all_dotplots(table, segs, df_multi, minseglen, anchors=df_anchor, maxsize=maxsize, minlen=minlen, outdir=outdir, Ks = df)
+        figs = all_dotplots(table, segs, df_multi, minseglen, anchors=df_anchor, maxsize=maxsize, minlen=minlen, outdir=outdir, Ks = df, dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha)
         for k, v in figs.items():
             v.savefig(os.path.join(outdir, "{}.dot.svg".format(k)))
             v.savefig(os.path.join(outdir, "{}.dot.pdf".format(k)))
-            v.savefig(os.path.join(outdir, "{}.dot.png".format(k)),dpi=1200)
+            v.savefig(os.path.join(outdir, "{}.dot.png".format(k)),dpi=500)
         logging.info('Done')
         exit()
     ksdb_df = pd.read_csv(datafile,header=0,index_col=0,sep='\t')
     df = apply_filters(ksdb_df, [("dS", 0., 5.)])
     ylabel = "Duplications" if spair == () else "Homologous pairs"
     if len(spair)!= 0: multi_sp_plot(df,spair,gsmap,outdir,onlyrootout,title=prefix,ylabel=ylabel,viz=True,plotkde=plotkde,reweight=reweight,sptree=speciestree,ap = anchorpoints, extraparanomeks=extraparanomeks,plotapgmm=plotapgmm,plotelmm=plotelmm,components=components,max_EM_iterations=em_iterations,num_EM_initializations=em_initializations,peak_threshold=prominence_cutoff,rel_height=rel_height)
     fig = default_plot(df, title=prefix, bins=50, ylabel=ylabel)
@@ -595,23 +598,26 @@
     type=float, help='Ks range to use for colored dotplot')
 @click.option('--iadhore_options', default="",
     help="other options for I-ADHoRe, as a comma separated string, "
          "e.g. gap_size=30,q_value=0.75,prob_cutoff=0.05")
 @click.option('--ancestor', '-ac', default=None,show_default=True,help='assumed ancestor species')
 @click.option('--minseglen', '-mg', default=10000, show_default=True, help="min length of segments in ratio if <= 1")
 @click.option('--keepredun', '-kr', is_flag=True, help='keep redundant multiplicons')
-@click.option('--mingenenum', '-mgn', default=30, type=int, show_default=True, help="min number of genes on segments to be considered")
+@click.option('--mingenenum', '-mgn', default=30, type=int, show_default=True, help="minimum number of genes on segments to be considered")
+@click.option('--dotsize', '-ds', type=float, default=1, show_default=True, help='size of dots')
+@click.option('--apalpha', '-aa', type=float, default=1, show_default=True, help='opacity of anchor dots')
+@click.option('--hoalpha', '-ha', type=float, default=0.1, show_default=True, help='opacity of homolog dots')
 def syn(**kwargs):
     """
     Co-linearity and anchor inference using I-ADHoRe.
     """
     _syn(**kwargs)
 
 def _syn(families, gff_files, ks_distribution, outdir, feature, attribute,
-        minlen, maxsize, ks_range, iadhore_options, ancestor, minseglen, keepredun, mingenenum):
+        minlen, maxsize, ks_range, iadhore_options, ancestor, minseglen, keepredun, mingenenum, dotsize, apalpha, hoalpha):
     """
     Co-linearity and anchor inference using I-ADHoRe.
     """
     from wgd.syn import make_gene_table, configure_adhore, run_adhore
     from wgd.syn import get_anchors, get_anchor_ksd, get_segments_profile, get_multi, get_chrom_gene, transformunit, get_mp_geneorder
     from wgd.viz import default_plot, apply_filters, all_dotplots, syntenic_dotplot_ks_colored,filter_by_minlength,dotplotunitgene,dotplotingene,filter_mingenumber
     from wgd.peak import formatv2
@@ -660,23 +666,23 @@
     segs = filter_mingenumber(segs_gene_unit,mingenenum)
     #if ks_distribution: segs_gene_unit_ks = getsegks(segs_gene_unit,ks_distribution,ordered_genes_perchrom_allsp)
     df_ks = None
     if ks_distribution!=None:
         ksdb_df = pd.read_csv(ks_distribution,header=0,index_col=0,sep='\t')
         ksdb_df = formatv2(ksdb_df)
         df_ks = apply_filters(ksdb_df, [("dS", 0., 5.)])
-    dotplotingene(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=anchors,ksdf=df_ks,maxsize=maxsize)
+    dotplotingene(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=anchors,ksdf=df_ks,maxsize=maxsize,dotsize=dotsize,apalpha=apalpha, hoalpha=hoalpha)
     #dotplotunitgene(ordered_genes_perchrom_allsp,segs_gene_unit,removed_scfa,outdir,mingenenum,table_orig,ordered_mp,ksdf=df_ks)
     # dotplot
     #logging.info("Generating dot plots")
-    figs = all_dotplots(table, segs, multi, minseglen, anchors=anchors, maxsize=maxsize, minlen=minlen, outdir=outdir, ancestor=ancestor, Ks = df_ks) 
+    figs = all_dotplots(table, segs, multi, minseglen, anchors=anchors, maxsize=maxsize, minlen=minlen, outdir=outdir, ancestor=ancestor, Ks = df_ks, dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha) 
     for k, v in figs.items():
         v.savefig(os.path.join(outdir, "{}.dot.svg".format(k)))
         v.savefig(os.path.join(outdir, "{}.dot.pdf".format(k)))
-        v.savefig(os.path.join(outdir, "{}.dot.png".format(k)))
+        v.savefig(os.path.join(outdir, "{}.dot.png".format(k)),dpi=500)
     plt.close()
 
     # anchor Ks distributions
     if ks_distribution:
         ylabel = "Duplications"
         if len(gff_files) == 2:
             ylabel = "RBH orthologs"
```

### Comparing `wgd-2.0.18/setup.py` & `wgd-2.0.19/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='wgd',
-    version='2.0.18',
+    version='2.0.19',
     packages=['wgd'],
     url='http://github.com/heche-psb/wgd',
     license='GPL',
     author='Hengchi Chen',
     author_email='heche@psb.vib-ugent.be',
     description='wgd',
     long_description=long_description,
```

### Comparing `wgd-2.0.18/test/test_core.py` & `wgd-2.0.19/test/test_core.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.18/wgd/__init__.py` & `wgd-2.0.19/wgd/__init__.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.18/wgd/beast.py` & `wgd-2.0.19/wgd/beast.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.18/wgd/cluster.py` & `wgd-2.0.19/wgd/cluster.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.18/wgd/codeml.py` & `wgd-2.0.19/wgd/codeml.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.18/wgd/core.py` & `wgd-2.0.19/wgd/core.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.18/wgd/mcmctree.py` & `wgd-2.0.19/wgd/mcmctree.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.18/wgd/mix.py` & `wgd-2.0.19/wgd/mix.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.18/wgd/peak.py` & `wgd-2.0.19/wgd/peak.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.18/wgd/postplot.py` & `wgd-2.0.19/wgd/postplot.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.18/wgd/syn.py` & `wgd-2.0.19/wgd/syn.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.18/wgd/utils.py` & `wgd-2.0.19/wgd/utils.py`

 * *Files identical despite different names*

### Comparing `wgd-2.0.18/wgd/viz.py` & `wgd-2.0.19/wgd/viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -1780,15 +1780,15 @@
     else:
         return np.median(Ks)
 
 def getpairks(pair,ksdf):
     Ks_dict = {pair:ks for pair,ks in zip(ksdf.index,ksdf['dS'])}
     return Ks_dict.get(pair,None)
 
-def plotdp_ig(ax,dfx,dfy,spx,spy,table,gene_orders,anchor=None,ksdf=None,maxsize=200,showks=False):
+def plotdp_ig(ax,dfx,dfy,spx,spy,table,gene_orders,anchor=None,ksdf=None,maxsize=200,showks=False,dotsize=0.8,apalpha=1, hoalpha=0.1):
     dfx,dfy = dfx.set_index('Coordinates'),dfy.set_index('Coordinates')
     leng_info_x,leng_info_y = {},{}
     gene_list = {gene:li for gene,li in zip(table.index,table['scaffold'])}
     if spx != spy:
         gene_list = {spx:{},spy:{}}
         for gene,sp,li in zip(table.index,table['species'],table['scaffold']):
             if sp != spx and sp != spy:
@@ -1838,19 +1838,19 @@
     if showks:
         if not (ksdf is None):
             norm = matplotlib.colors.Normalize(vmin=np.min(Ks_ages), vmax=np.max(Ks_ages))
             c_m = matplotlib.cm.rainbow
             s_m = ScalarMappable(cmap=c_m, norm=norm)
             s_m.set_array([])
     if not showks:
-        ax.scatter(xs, ys, s=0.4, color = 'k', alpha=0.01)
-        ax.scatter(xs_ap, ys_ap, s=0.4, color = 'r', alpha=1)
+        ax.scatter(xs, ys, s=dotsize, color = 'k', alpha=hoalpha)
+        ax.scatter(xs_ap, ys_ap, s=dotsize, color = 'r', alpha=apalpha)
     else:
-        ax.scatter(xs, ys, s=0.4, color=[c_m(norm(c)) for c in co], alpha=0.01)
-        ax.scatter(xs_ap, ys_ap, s=0.4, color=[c_m(norm(c)) for c in co_ap], alpha=1)
+        ax.scatter(xs, ys, s=dotsize, color=[c_m(norm(c)) for c in co], alpha=hoalpha)
+        ax.scatter(xs_ap, ys_ap, s=dotsize, color=[c_m(norm(c)) for c in co_ap], alpha=apalpha)
     #ax.scatter(xs_ap, ys_ap, s=0.4, alpha=0.5)
     xlim,ylim = xtick[-1],ytick[-1]
     ax.set_xlim(0, xlim)
     ax.set_ylim(0, ylim)
     ax.vlines(xtick, ymin=0, ymax=ylim, alpha=0.8, color="k")
     ax.hlines(ytick, xmin=0, xmax=xlim, alpha=0.8, color="k")
     ax.set_xlabel("{}".format(spx))
@@ -2063,48 +2063,48 @@
             spx,spy = sp_list[i],sp_list[j]
             fig, ax = plotbackbone_dpug(spx,spy,ordered_genes_perchrom_allsp,removed_scfa,segs,mingenenum,MP,gene_genome,ksdf=ksdf)
             figs[spx + "-vs-" + spy] = fig
     for prefix, fig in figs.items():
         fname = os.path.join(outdir, "{}.line_unit_gene.svg".format(prefix))
         fig.savefig(fname)
 
-def plotdotplotingene(spx,spy,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=None,ksdf=None,maxsize=200,showks=False):
+def plotdotplotingene(spx,spy,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=None,ksdf=None,maxsize=200,showks=False,dotsize=0.8, apalpha=1, hoalpha=0.1):
     fig, ax = plt.subplots(1, 1, figsize=(10,10))
     dfx = ordered_genes_perchrom_allsp[spx].copy().drop(removed_scfa[spx],axis=1)
     dfy = ordered_genes_perchrom_allsp[spy].copy().drop(removed_scfa[spy],axis=1)
-    ax = plotdp_ig(ax,dfx,dfy,spx,spy,table,gene_orders,anchor=anchor,ksdf=ksdf,maxsize=maxsize,showks=showks)
+    ax = plotdp_ig(ax,dfx,dfy,spx,spy,table,gene_orders,anchor=anchor,ksdf=ksdf,maxsize=maxsize,showks=showks,dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha)
     fig.tight_layout()
     return fig, ax
 
-def dotplotingene(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=None,ksdf=None,maxsize=200):
+def dotplotingene(ordered_genes_perchrom_allsp,removed_scfa,outdir,table,gene_orders,anchor=None,ksdf=None,maxsize=200,dotsize=0.8, apalpha=1, hoalpha=0.1):
     sp_list = list(ordered_genes_perchrom_allsp.keys())
     gene_list = {gene:li for gene,li in zip(table.index,table['scaffold'])}
     gene_genome = {gene:sp for gene,sp in zip(table.index,table['species'])}
     figs = {}
     logging.info("Making dotplot (in unit of genes)")
     for i in range(len(sp_list)):
         for j in range(i,len(sp_list)):
             spx,spy = sp_list[i],sp_list[j]
             logging.info("{0} vs. {1}".format(spx,spy))
-            fig, ax = plotdotplotingene(spx,spy,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=anchor,ksdf=ksdf)
+            fig, ax = plotdotplotingene(spx,spy,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=anchor,ksdf=ksdf,dotsize=dotsize,apalpha=apalpha, hoalpha=hoalpha)
             figs[spx + "-vs-" + spy] = fig
             if not (ksdf is None):
-                figks, ax = plotdotplotingene(spx,spy,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=anchor,ksdf=ksdf,showks=True)
+                figks, ax = plotdotplotingene(spx,spy,table,removed_scfa,ordered_genes_perchrom_allsp,gene_orders,anchor=anchor,ksdf=ksdf,showks=True,dotsize=dotsize, apalpha=apalpha, hoalpha=hoalpha)
                 figs[spx + "-vs-" + spy + "_Ks"] = figks
     for prefix, fig in figs.items():
         fname = os.path.join(outdir, "{}.dot_unit_gene.svg".format(prefix))
         fig.savefig(fname)
         fname = os.path.join(outdir, "{}.dot_unit_gene.png".format(prefix))
-        fig.savefig(fname,dpi=1200)
+        fig.savefig(fname,dpi=500)
         fname = os.path.join(outdir, "{}.dot_unit_gene.pdf".format(prefix))
         fig.savefig(fname)
     plt.close()
 
 # dot plot stuff
-def all_dotplots(df, segs, multi, minseglen, anchors=None, ancestor=None, Ks=None, **kwargs):
+def all_dotplots(df, segs, multi, minseglen, anchors=None, ancestor=None, Ks=None, dotsize = 0.8, apalpha=1, hoalpha=0.1, **kwargs):
     """
     Generate dot plots for all pairs of species in `df`, coloring anchor pairs.
     """
     # Note that the Chr ID in gff3 file should not be alleen int or float
     if not (Ks is None):
         ks_dict = {pair:ks for pair,ks in zip(Ks.index,Ks['dS'])}
     gdf = list(df.groupby("species"))
@@ -2141,29 +2141,29 @@
             #print(xs)
             #print(ys)
             #for i,j in zip(df.x,df.y): print((i,j))
             if df is None:  # HACK, in case we're dealing with RBH orthologs...
                 continue
             #for x,y in zip(df.x,df.y): ax.scatter(x, y, s=1, color="k", alpha=0.1)
             #print((len(list(itertools.chain(df.x))),len(list(itertools.chain(df.y)))))
-            ax.scatter(list(itertools.chain(df.x)), list(itertools.chain(df.y)), s=0.4, color="k", alpha=0.01)
+            ax.scatter(list(itertools.chain(df.x)), list(itertools.chain(df.y)), s=dotsize, color="k", alpha=hoalpha)
             if not (Ks is None):
                 for i,x,y in zip(df.index,df['x'],df['y']):
                     ksage = ks_dict.get(i,None)
                     if ksage == None:
                         continue
                     ksages.append(ksage)
                     Ksages.append(ksage)
                     xxs.append(x)
                     yys.append(y)
             #ax.scatter(np.array(df.x,dtype=float), np.array(df.y,dtype=float), s=1, color="k", alpha=0.1)
             if not (anchors is None):
                 andf = df.join(anchors, how="inner")
                 #for x,y in zip(andf.x,andf.y): ax.scatter(x, y, s=1, color="r", alpha=0.9)
-                ax.scatter(list(itertools.chain(andf.x)), list(itertools.chain(andf.y)), s=0.4, color="r", alpha=1)
+                ax.scatter(list(itertools.chain(andf.x)), list(itertools.chain(andf.y)), s=dotsize, color="r", alpha=apalpha)
                 if not (Ks is None):
                     for i,x,y in zip(andf.index,andf['x'],andf['y']):
                         ksage = ks_dict.get(i,None)
                         if ksage == None:
                             continue
                         ksages_ap.append(ksage)
                         xxs_ap.append(x)
@@ -2193,16 +2193,16 @@
                 figks, axks = plt.subplots(1, 1, figsize=(10,10))
                 axks2 = axks.twinx()
                 axks3 = axks.twiny()
                 norm = matplotlib.colors.Normalize(vmin=np.min(Ksages), vmax=np.max(Ksages))
                 c_m = matplotlib.cm.rainbow
                 s_m = ScalarMappable(cmap=c_m, norm=norm)
                 s_m.set_array([])
-                axks.scatter(xxs, yys, s=0.4, color=[c_m(norm(c)) for c in ksages], alpha=0.01)
-                axks.scatter(xxs_ap, yys_ap, s=0.4, color=[c_m(norm(c)) for c in ksages_ap], alpha=1)
+                axks.scatter(xxs, yys, s=dotsize, color=[c_m(norm(c)) for c in ksages], alpha=hoalpha)
+                axks.scatter(xxs_ap, yys_ap, s=dotsize, color=[c_m(norm(c)) for c in ksages_ap], alpha=apalpha)
                 axks.set_xlim(0, xlim)
                 axks.set_ylim(0, ylim)
                 axks.vlines(xs+[xmax], ymin=0, ymax=ylim, alpha=0.8, color="k")
                 axks.hlines(ys+[ymax], xmin=0, xmax=xlim, alpha=0.8, color="k")
                 axks.set_xlabel("{}".format(spx))
                 axks.set_ylabel("{}".format(spy))
                 axks2.set_yticklabels(axks.get_yticks() / 1e6)
```

### Comparing `wgd-2.0.18/wgd.egg-info/PKG-INFO` & `wgd-2.0.19/wgd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wgd
-Version: 2.0.18
+Version: 2.0.19
 Summary: wgd
 Home-page: http://github.com/heche-psb/wgd
 Author: Hengchi Chen
 Author-email: heche@psb.vib-ugent.be
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -249,14 +249,18 @@
 -ml, --minlen, the minimum length of a scaffold to be included in dotplot, default -1, if -1 was set, the 10% of the longest scaffold will be set
 -ms, --maxsize, the maximum family size to include, default 200
 -r, --ks_range, the Ks range in colored dotplot, default (0, 5)
 --iadhore_options, the parameter setting in iadhore, default 
 -ac, --ancestor, the assumed ancestor species, default None, a option that is still in development
 -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
 -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
+-mgn, --mingenenum, the minimum number of genes for a segment to be considered, default 30
+-ds, --dotsize, the dot size in dot plot, default 1
+-aa, --apalpha, the opacity of anchor dots, default 1
+-ha, --hoalpha, the opacity of homolog dots, default 0.1
 ```
 
 The program `wgd viz` can realize the visualization of *K*<sub>S</sub> age distribution and synteny.
 ```
 wgd viz (option)
 --------------------------------------------------------------------------------
 -d, --datafile, the Ks datafile, default None
@@ -279,14 +283,19 @@
 -rh, --rel_height, the relative height at which the peak width is measured, default 0.4
 -mg, --minseglen, the minimum length of segments to include in ratio if <= 1, default 100000
 -kr, --keepredun, flag option, whether to keep redundant multiplicons, if the flag was set, the redundant multiplicons will be kept
 -epk, --extraparanomeks, extra paranome Ks data to plot in the mixed Ks distribution, default None
 -pag, --plotapgmm, flag option, whether to plot mixture modeling of anchor Ks in the mixed Ks distribution, if the flag was set, the mixture modeling of anchor Ks will be plotted
 -pem, --plotelmm, flag option, whether to plot elmm mixture modeling of paranome Ks in the mixed Ks distribution, if the flag was set, the elmm mixture modeling of paranome Ks will be plotted
 -c, --components, the range of the number of components to fit in anchor Ks mixture modeling, default (1,4)
+-mgn, --mingenenum, the minimum number of genes for a segment to be considered, default 30
+-psy, --plotsyn, flag option, whether to initiate the synteny plot, if the flag was set, the synteny plot will be produced
+-ds, --dotsize, the dot size in dot plot, default 1
+-aa, --apalpha, the opacity of anchor dots, default 1
+-ha, --hoalpha, the opacity of homolog dots, default 0.1
 ```
 
 ## Usage
 
 Here we provided the basic usage for each program.
 
 ### wgd dmd
@@ -443,14 +452,16 @@
 
 The dot plots without *K*<sub>S</sub> annotation will also be automately produced, as shown below.
 
 ![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot_unit_gene.png)
 
 ![](data/Aquilegia_coerulea-vs-Aquilegia_coerulea.dot.png)
 
+Note that the opacity of anchor dots and all homolog dots can be set by the option `apalpha` and `hoalpha` separately. If one just wants to see the anchor dots, setting the `hoalpha` as 0 (or other minuscule values) will do. If one wants to see the distribution of whole dots better, setting the `hoalpha` higher (and `apalpha` lower) will do. The `dotsize` option can be called to adjust the size of dots.
+
 A further associated Syndepth plot shows that there are more than 80 duplicated segments, which dominates the whole collinear ratio category.
 
 ![](data/Syndepth.svg)
 
 We can fit an ELMM mixture model upon the whole paranome *K*<sub>S</sub> age distribution to see more accurately the significance and location of potential WGDs, using the command line below.
 
 ```
```

### Comparing `wgd-2.0.18/wgd.egg-info/requires.txt` & `wgd-2.0.19/wgd.egg-info/requires.txt`

 * *Files identical despite different names*

