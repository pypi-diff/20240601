# Comparing `tmp/jjowl-0.2.7.tar.gz` & `tmp/jjowl-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jjowl-0.2.7.tar", last modified: Mon Jan  3 10:37:00 2022, max compression
+gzip compressed data, was "jjowl-0.2.8.tar", last modified: Mon Jan 31 15:13:13 2022, max compression
```

## Comparing `jjowl-0.2.7.tar` & `jjowl-0.2.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      498 2021-12-07 13:39:27.576575 jjowl-0.2.7/jjowl.md
--rwxr-xr-x   0        0        0     2267 2022-01-03 09:56:48.891483 jjowl-0.2.7/jjowl/__init__.py
--rwxr-xr-x   0        0        0    20736 2021-09-25 09:53:32.584587 jjowl-0.2.7/jjowl/jjowl.bak
--rwxr-xr-x   0        0        0    20939 2021-12-31 00:33:07.585646 jjowl-0.2.7/jjowl/jjowl.py
--rwxr-xr-x   0        0        0     9200 2021-12-09 18:46:51.876289 jjowl-0.2.7/jjowl/ont_convert.py
--rw-r--r--   0        0        0      765 2021-12-30 16:50:16.367982 jjowl-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 jjowl-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      498 2021-12-07 13:39:27.576575 jjowl-0.2.8/jjowl.md
+-rwxr-xr-x   0        0        0     2267 2022-01-31 15:09:11.644894 jjowl-0.2.8/jjowl/__init__.py
+-rwxr-xr-x   0        0        0    20736 2021-09-25 09:53:32.584587 jjowl-0.2.8/jjowl/jjowl.bak
+-rwxr-xr-x   0        0        0    20939 2021-12-31 00:33:07.585646 jjowl-0.2.8/jjowl/jjowl.py
+-rwxr-xr-x   0        0        0     9295 2022-01-31 15:08:38.836969 jjowl-0.2.8/jjowl/ont_convert.py
+-rw-r--r--   0        0        0      763 2022-01-31 14:58:32.070152 jjowl-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 jjowl-0.2.8/PKG-INFO
```

### Comparing `jjowl-0.2.7/jjowl/__init__.py` & `jjowl-0.2.8/jjowl/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,8 +60,8 @@
 
 # Description
 """
 
 from .jjowl import *
 from .ont_convert import *
 
-__version__ = "0.2.7"
+__version__ = "0.2.8"
```

### Comparing `jjowl-0.2.7/jjowl/jjowl.bak` & `jjowl-0.2.8/jjowl/jjowl.bak`

 * *Files identical despite different names*

### Comparing `jjowl-0.2.7/jjowl/jjowl.py` & `jjowl-0.2.8/jjowl/jjowl.py`

 * *Files identical despite different names*

### Comparing `jjowl-0.2.7/jjowl/ont_convert.py` & `jjowl-0.2.8/jjowl/ont_convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python3
 """ VERY EXPERIMENTAL :  module for opinied command line processing of OWL ontologies
 
 # Synopsis
 
     jjtmd2ttl [option] file.t.md ...
-      ## convert markdown with yaml metadate in turtle (seealso pandoc)
+      ## convert markdown with yaml metadate into turtle (seealso pandoc)
 
     jjtable2ttl [option] file.csv ...
       -F '#'            - Fiels separator (def: '::')
       -f ','            - sub field separatos (def: '[;,]')
       -h 'headerLine'   - set a "header line" (def: first line)
          Ex:  jjtable2ttl -F : -h 'Id::uid::gid::name::' /etc/passwd
       ## convert csv  metadate in turtle 
@@ -61,14 +61,16 @@
  rdfs:
     label :    s:iri   o:literal
     range
     domain
     subClassOf :           
 '''
 
+## parse markdown with YAML-metadata  ( jjmd2ttl )
+
 def md2py(c):
     """ files(markdown with initial yaml metadata) → docs = [ doc ] """
     docs=[]
     for txt in c.slurp():
         doc={}
         ex=match(r'\s*---(.*?)---(.*)',txt,flags=re.S)
         if not ex:
@@ -208,15 +210,15 @@
     return r
 
 def main_tmd2ttl():            ## main -- tmd2ttl
     c=clfilter(opt="do:")     ## option values in c.opt dictionary
     ds = md2py(c)
     print(docs2ttl(ds))
 
-#=== parse table
+#=== parse table (jjtable2ttl)
 
 def parse_head(h: str, opt ):
     fs  = opt.get('-F','::')
     fs2 = ':'
     idclass,*ftits = split(fr'\s*{fs}\s*',h.strip())
     for i,f in enumerate(ftits):
         a = match(fr'(.+){fs2}(.+)',f)
@@ -269,15 +271,15 @@
     return docs
 
 def main_table2ttl():
     c = clfilter(opt="h:do:F:f:v")     ## option values in c.opt dictionary
     ds = table2py(c)
     print(docs2ttl(ds))
 
-## jjyaml2ttl
+## parse a multi-yaml file: (jjyaml2ttl)
 
 def yamls2py(c):
     """ files( ("---" yaml)+ ) → docs = [ doc ] """
     docs =[]
     for txt in c.slurp():
         txt= sub(r'\t','    ',txt) 
         try:
```

### Comparing `jjowl-0.2.7/pyproject.toml` & `jjowl-0.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 dependencies = [
   "rdflib", 
   "jjcli",
   "owlrl", 
   "unidecode", 
-  "pyyaml" ]
+  "pyyaml"]
 readme = "jjowl.md"
 
 [project.urls]
 Home = "https://natura.di.uminho.pt/jjowl"
 
 [project.scripts]
 
@@ -26,8 +26,8 @@
 owlclass  = "jjowl:mclass"
 owlprops  = "jjowl:mprops"
 owllabel2term  = "jjowl:mlabel2term"
 owlxdxf = "jjowl:mxdxf"
 owlhtml = "jjowl:mhtml"
 jjtmd2ttl = "jjowl:main_tmd2ttl"
 jjtable2ttl = "jjowl:main_table2ttl"
-jjyaml2ttl = "jjowl:main_yaml2ttl"
+jjyaml2ttl= "jjowl:main_yaml2ttl"
```

### Comparing `jjowl-0.2.7/PKG-INFO` & `jjowl-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jjowl
-Version: 0.2.7
+Version: 0.2.8
 Summary: VERY EXPERIMENTAL :  module for opinied command line processing of OWL ontologies
 Author-email: JJoao <jj@di.uminho.pt>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: rdflib
 Requires-Dist: jjcli
 Requires-Dist: owlrl
```

