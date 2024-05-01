# Comparing `tmp/htagui-0.5.5.tar.gz` & `tmp/htagui-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagui-0.5.5.tar", max compression
+gzip compressed data, was "htagui-0.5.6.tar", max compression
```

## Comparing `htagui-0.5.5.tar` & `htagui-0.5.6.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0     1065 2024-04-27 17:54:08.463275 htagui-0.5.5/LICENSE
--rw-r--r--   0        0        0     8233 2024-04-27 17:54:08.463275 htagui-0.5.5/README.md
--rw-r--r--   0        0        0      330 2024-04-27 17:54:09.143282 htagui-0.5.5/htagui/__init__.py
--rw-r--r--   0        0        0      846 2024-04-27 17:54:08.463275 htagui-0.5.5/htagui/all.py
--rw-r--r--   0        0        0      750 2024-04-27 17:54:08.463275 htagui-0.5.5/htagui/basics/__init__.py
--rw-r--r--   0        0        0    11400 2024-04-27 17:54:08.463275 htagui-0.5.5/htagui/basics/bases.py
--rw-r--r--   0        0        0      771 2024-04-27 17:54:08.463275 htagui-0.5.5/htagui/bulma/__init__.py
--rw-r--r--   0        0        0   656453 2024-04-27 17:54:08.467275 htagui-0.5.5/htagui/bulma/bases.py
--rw-r--r--   0        0        0     4268 2024-04-27 17:54:08.467275 htagui-0.5.5/htagui/common.py
--rw-r--r--   0        0        0     3401 2024-04-27 17:54:08.467275 htagui-0.5.5/htagui/dialog.py
--rw-r--r--   0        0        0     1856 2024-04-27 17:54:08.467275 htagui-0.5.5/htagui/flex.py
--rw-r--r--   0        0        0      771 2024-04-27 17:54:08.467275 htagui-0.5.5/htagui/form.py
--rw-r--r--   0        0        0     3795 2024-04-27 17:54:08.467275 htagui-0.5.5/htagui/ifields.py
--rw-r--r--   0        0        0      922 2024-04-27 17:54:08.467275 htagui-0.5.5/htagui/md/__init__.py
--rw-r--r--   0        0        0    10941 2024-04-27 17:54:08.467275 htagui-0.5.5/htagui/md/bases.py
--rw-r--r--   0        0        0      774 2024-04-27 17:54:08.467275 htagui-0.5.5/htagui/shoelace/__init__.py
--rw-r--r--   0        0        0     8632 2024-04-27 17:54:08.467275 htagui-0.5.5/htagui/shoelace/bases.py
--rw-r--r--   0        0        0     9619 2024-04-27 17:54:08.467275 htagui-0.5.5/htagui/splitters.py
--rw-r--r--   0        0        0     1441 2024-04-27 17:54:08.467275 htagui-0.5.5/htagui/tabs.py
--rw-r--r--   0        0        0     1069 2024-04-27 17:54:09.143282 htagui-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     9466 1970-01-01 00:00:00.000000 htagui-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-01 11:41:38.108568 htagui-0.5.6/LICENSE
+-rw-r--r--   0        0        0     8505 2024-05-01 11:41:38.108568 htagui-0.5.6/README.md
+-rw-r--r--   0        0        0      330 2024-05-01 11:41:38.360570 htagui-0.5.6/htagui/__init__.py
+-rw-r--r--   0        0        0      892 2024-05-01 11:41:38.108568 htagui-0.5.6/htagui/all.py
+-rw-r--r--   0        0        0      750 2024-05-01 11:41:38.108568 htagui-0.5.6/htagui/basics/__init__.py
+-rw-r--r--   0        0        0    11404 2024-05-01 11:41:38.108568 htagui-0.5.6/htagui/basics/bases.py
+-rw-r--r--   0        0        0      771 2024-05-01 11:41:38.108568 htagui-0.5.6/htagui/bulma/__init__.py
+-rw-r--r--   0        0        0   656501 2024-05-01 11:41:38.108568 htagui-0.5.6/htagui/bulma/bases.py
+-rw-r--r--   0        0        0     4268 2024-05-01 11:41:38.108568 htagui-0.5.6/htagui/common.py
+-rw-r--r--   0        0        0     3401 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/dialog.py
+-rw-r--r--   0        0        0      648 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/fileupload.py
+-rw-r--r--   0        0        0     1856 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/flex.py
+-rw-r--r--   0        0        0      785 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/fluent/__init__.py
+-rw-r--r--   0        0        0     8538 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/fluent/bases.py
+-rw-r--r--   0        0        0      771 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/form.py
+-rw-r--r--   0        0        0     3795 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/ifields.py
+-rw-r--r--   0        0        0      922 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/md/__init__.py
+-rw-r--r--   0        0        0    10945 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/md/bases.py
+-rw-r--r--   0        0        0      774 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/shoelace/__init__.py
+-rw-r--r--   0        0        0     8489 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/shoelace/bases.py
+-rw-r--r--   0        0        0     9619 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/splitters.py
+-rw-r--r--   0        0        0     1441 2024-05-01 11:41:38.112568 htagui-0.5.6/htagui/tabs.py
+-rw-r--r--   0        0        0     1069 2024-05-01 11:41:38.360570 htagui-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     9738 1970-01-01 00:00:00.000000 htagui-0.5.6/PKG-INFO
```

### Comparing `htagui-0.5.5/LICENSE` & `htagui-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `htagui-0.5.5/README.md` & `htagui-0.5.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -163,14 +163,27 @@
 ux = ui.Dialog( self )
 form = ui.Form( onsubmit=lambda dico: ux.notify(str(dico)) )
 form <= ui.Input(_name="mystring",_placeholder="input something")
 form <= ui.Button("ok")
 self <= form
 ```
 
+## Object FileUpload
+
+A simple surcharge of Tag.input( _type='file'...) which call a method to upload the selected file.
+
+```python
+import htagui as ui
+
+def uploaded(name:str, content:bytes):
+    print(name,content)
+
+self <= ui.FileUpload( uploaded , _multiple=True)
+```
+
 ## Object Tabs
 
 An htag class to easily create tabs structure. And provides somes attributs/methods to interact with it.
 
 ```python
 import htagui as ui
 tab1 = Tag.div("content1",name="tab1") # tab object needs a `name` property !
```

### Comparing `htagui-0.5.5/htagui/all.py` & `htagui-0.5.6/htagui/all.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 
 # global objects
 from .form import Form
 from .tabs import Tabs
 from .dialog import Dialog
 from .splitters import HSplit, VSplit
 from .ifields import IText,ITextarea,IRange,IBool,ISelect,IRadios
+from .fileupload import FileUpload
 
 class App(Tag.body):
     _ui=None
     
     @property
     def ui(self):
         if self._ui is None:
             self._ui = Dialog(self)
         return self._ui
 
 # global methods
 from .flex import hflex,vflex  # utilities (Htag contructor methods)
 
 
-ALL=[App,Form,Tabs,Dialog,HSplit,VSplit,IText,ITextarea,IRange,IBool,ISelect,IRadios]
+ALL=[App,Form,Tabs,Dialog,HSplit,VSplit,IText,ITextarea,IRange,IBool,ISelect,IRadios,FileUpload]
```

### Comparing `htagui-0.5.5/htagui/basics/__init__.py` & `htagui-0.5.6/htagui/basics/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.5/htagui/basics/bases.py` & `htagui-0.5.6/htagui/basics/bases.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     statics=STATICS
     def init(self,title,**a):
         self <= title
         self["class"].add("button")
 
 class Spinner(Tag.span):
     statics=STATICS
-    def init(self):
+    def init(self,**a):
         self["class"].add("spinner")
 
 class Input(Tag.input):
     statics=STATICS
     def init(self,**a):
         self["class"].add("input")
         if not self.attrs.get("type"):
```

### Comparing `htagui-0.5.5/htagui/bulma/__init__.py` & `htagui-0.5.6/htagui/bulma/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.5/htagui/bulma/bases.py` & `htagui-0.5.6/htagui/bulma/bases.py`

 * *Files 0% similar despite different names*

```diff
@@ -40647,383 +40647,386 @@
 0009ec60: 726d 3a20 726f 7461 7465 2830 6465 6729  rm: rotate(0deg)
 0009ec70: 3b0a 2020 2020 7d0a 2020 2020 3130 3025  ;.    }.    100%
 0009ec80: 207b 0a20 2020 2020 2020 2074 7261 6e73   {.        trans
 0009ec90: 666f 726d 3a20 726f 7461 7465 2833 3630  form: rotate(360
 0009eca0: 6465 6729 3b0a 2020 2020 7d0a 2020 2020  deg);.    }.    
 0009ecb0: 7d20 2020 2020 2020 2020 0a22 2222 2020  }         ."""  
 0009ecc0: 2020 0a20 2020 2064 6566 2069 6e69 7428    .    def init(
-0009ecd0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-0009ece0: 656c 665b 2263 6c61 7373 225d 3d22 7370  elf["class"]="sp
-0009ecf0: 696e 6e65 7222 0a0a 0a63 6c61 7373 2053  inner"...class S
-0009ed00: 656c 6563 7428 5461 672e 6469 7629 3a0a  elect(Tag.div):.
-0009ed10: 2020 2020 7374 6174 6963 733d 5354 4154      statics=STAT
-0009ed20: 4943 530a 2020 2020 6465 6620 696e 6974  ICS.    def init
-0009ed30: 2873 656c 662c 6f70 7469 6f6e 733a 4c69  (self,options:Li
-0009ed40: 7374 4f72 4469 6374 2c20 2a2a 6129 3a0a  stOrDict, **a):.
-0009ed50: 2020 2020 2020 2020 7365 6c66 2e6f 7074          self.opt
-0009ed60: 696f 6e73 3d65 6e73 7572 6564 6963 7428  ions=ensuredict(
-0009ed70: 6f70 7469 6f6e 7329 0a20 2020 2020 2020  options).       
-0009ed80: 2073 656c 665b 2263 6c61 7373 225d 2e61   self["class"].a
-0009ed90: 6464 2822 7365 6c65 6374 2229 0a20 2020  dd("select").   
-0009eda0: 2020 2020 2073 656c 662e 7265 7265 6e64       self.rerend
-0009edb0: 6572 2873 656c 662e 6174 7472 732e 6765  er(self.attrs.ge
-0009edc0: 7428 2276 616c 7565 2229 290a 0a20 2020  t("value"))..   
-0009edd0: 2064 6566 2072 6572 656e 6465 7228 7365   def rerender(se
-0009ede0: 6c66 2c76 616c 7565 293a 0a20 2020 2020  lf,value):.     
-0009edf0: 2020 2077 6974 6820 5461 672e 7365 6c65     with Tag.sele
-0009ee00: 6374 2820 5f6f 6e63 6861 6e67 653d 6622  ct( _onchange=f"
-0009ee10: 646f 6375 6d65 6e74 2e67 6574 456c 656d  document.getElem
-0009ee20: 656e 7442 7949 6428 277b 6964 2873 656c  entById('{id(sel
-0009ee30: 6629 7d27 292e 7661 6c75 653d 6576 656e  f)}').value=even
-0009ee40: 742e 7461 7267 6574 2e76 616c 7565 222c  t.target.value",
-0009ee50: 5f6e 616d 653d 7365 6c66 2e61 7474 7273  _name=self.attrs
-0009ee60: 2e67 6574 2822 6e61 6d65 2229 2c5f 7265  .get("name"),_re
-0009ee70: 7175 6972 6564 3d73 656c 662e 6174 7472  quired=self.attr
-0009ee80: 732e 6765 7428 2272 6571 7569 7265 6422  s.get("required"
-0009ee90: 2920 2920 6173 2073 656c 6563 743a 0a20  ) ) as select:. 
-0009eea0: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-0009eeb0: 2c76 2069 6e20 7365 6c66 2e6f 7074 696f  ,v in self.optio
-0009eec0: 6e73 2e69 7465 6d73 2829 3a0a 2020 2020  ns.items():.    
-0009eed0: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
-0009eee0: 6374 203c 3d20 5461 672e 6f70 7469 6f6e  ct <= Tag.option
-0009eef0: 2876 2c5f 7661 6c75 653d 6b2c 5f73 656c  (v,_value=k,_sel
-0009ef00: 6563 7465 643d 2828 7374 7228 7661 6c75  ected=((str(valu
-0009ef10: 6529 3d3d 7374 7228 6b29 2929 290a 2020  e)==str(k)))).  
-0009ef20: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
-0009ef30: 2820 7365 6c65 6374 2029 0a0a 636c 6173  ( select )..clas
-0009ef40: 7320 5261 6469 6f73 2854 6167 2e73 7061  s Radios(Tag.spa
-0009ef50: 6e29 3a0a 2020 2020 7374 6174 6963 733d  n):.    statics=
-0009ef60: 5354 4154 4943 530a 2020 2020 6465 6620  STATICS.    def 
-0009ef70: 696e 6974 2873 656c 662c 6f70 7469 6f6e  init(self,option
-0009ef80: 733a 4c69 7374 4f72 4469 6374 2c20 2a2a  s:ListOrDict, **
-0009ef90: 6129 3a0a 2020 2020 2020 2020 7365 6c66  a):.        self
-0009efa0: 2e6f 7074 696f 6e73 203d 2065 6e73 7572  .options = ensur
-0009efb0: 6564 6963 7428 6f70 7469 6f6e 7329 0a20  edict(options). 
-0009efc0: 2020 2020 2020 2073 656c 665b 2263 6c61         self["cla
-0009efd0: 7373 225d 2e61 6464 2822 636f 6e74 726f  ss"].add("contro
-0009efe0: 6c22 290a 2020 2020 2020 2020 7365 6c66  l").        self
-0009eff0: 2e72 6572 656e 6465 7228 2073 656c 662e  .rerender( self.
-0009f000: 6174 7472 732e 6765 7428 2276 616c 7565  attrs.get("value
-0009f010: 222c 4e6f 6e65 2920 290a 2020 2020 0a20  ",None) ).    . 
-0009f020: 2020 2064 6566 2072 6572 656e 6465 7228     def rerender(
-0009f030: 7365 6c66 2c76 616c 7565 293a 0a20 2020  self,value):.   
-0009f040: 2020 2020 2022 2222 2073 7065 6369 616c       """ special
-0009f050: 206d 6574 686f 6420 2873 6565 2069 6669   method (see ifi
-0009f060: 656c 6473 292c 2074 6f20 7265 7265 6e64  elds), to rerend
-0009f070: 6572 2061 6c6c 2074 6865 2077 6964 6765  er all the widge
-0009f080: 7420 2874 6f20 6176 6f69 6420 746f 2064  t (to avoid to d
-0009f090: 6561 6c20 7769 7468 206a 7329 2222 220a  eal with js)""".
-0009f0a0: 2020 2020 2020 2020 7365 6c66 2e63 6c65          self.cle
-0009f0b0: 6172 2829 0a20 2020 2020 2020 2066 6f72  ar().        for
-0009f0c0: 206b 2c76 2069 6e20 7365 6c66 2e6f 7074   k,v in self.opt
-0009f0d0: 696f 6e73 2e69 7465 6d73 2829 3a0a 2020  ions.items():.  
-0009f0e0: 2020 2020 2020 2020 2020 6970 743d 5461            ipt=Ta
-0009f0f0: 672e 696e 7075 7428 0a20 2020 2020 2020  g.input(.       
-0009f100: 2020 2020 2020 2020 205f 7479 7065 3d22           _type="
-0009f110: 7261 6469 6f22 2c0a 2020 2020 2020 2020  radio",.        
-0009f120: 2020 2020 2020 2020 5f76 616c 7565 3d6b          _value=k
-0009f130: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0009f140: 2020 5f6e 616d 653d 7365 6c66 2e61 7474    _name=self.att
-0009f150: 7273 2e67 6574 2822 6e61 6d65 222c 7374  rs.get("name",st
-0009f160: 7228 6964 2873 656c 6629 2929 2c20 2020  r(id(self))),   
-0009f170: 2020 2020 2020 2020 2020 2320 6e65 6564            # need
-0009f180: 2061 206e 616d 6520 746f 2062 6520 7661   a name to be va
-0009f190: 6c69 640a 2020 2020 2020 2020 2020 2020  lid.            
-0009f1a0: 2020 2020 5f63 6865 636b 6564 3d28 7374      _checked=(st
-0009f1b0: 7228 7661 6c75 6529 3d3d 7374 7228 6b29  r(value)==str(k)
-0009f1c0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0009f1d0: 2020 205f 7265 7175 6972 6564 3d62 6f6f     _required=boo
-0009f1e0: 6c28 7365 6c66 2e61 7474 7273 2e67 6574  l(self.attrs.get
-0009f1f0: 2822 7265 7175 6972 6564 222c 4e6f 6e65  ("required",None
-0009f200: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-0009f210: 2020 2020 5f72 6561 646f 6e6c 793d 626f      _readonly=bo
-0009f220: 6f6c 2873 656c 662e 6174 7472 732e 6765  ol(self.attrs.ge
-0009f230: 7428 2272 6561 646f 6e6c 7922 2c4e 6f6e  t("readonly",Non
-0009f240: 6529 292c 0a20 2020 2020 2020 2020 2020  e)),.           
-0009f250: 2020 2020 205f 6f6e 6368 616e 6765 3d66       _onchange=f
-0009f260: 2264 6f63 756d 656e 742e 6765 7445 6c65  "document.getEle
-0009f270: 6d65 6e74 4279 4964 2827 7b69 6428 7365  mentById('{id(se
-0009f280: 6c66 297d 2729 2e76 616c 7565 3d27 7b6b  lf)}').value='{k
-0009f290: 7d27 3b22 0a20 2020 2020 2020 2020 2020  }';".           
-0009f2a0: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
-0009f2b0: 656c 6620 3c3d 2054 6167 2e64 6976 2854  elf <= Tag.div(T
-0009f2c0: 6167 2e6c 6162 656c 2820 6970 7420 2b22  ag.label( ipt +"
-0009f2d0: 2022 2b20 7620 2c5f 636c 6173 733d 2272   "+ v ,_class="r
-0009f2e0: 6164 696f 2229 290a 0a23 2323 2323 2323  adio"))..#######
+0009ecd0: 7365 6c66 2c2a 2a61 293a 0a20 2020 2020  self,**a):.     
+0009ece0: 2020 2073 656c 665b 2263 6c61 7373 225d     self["class"]
+0009ecf0: 3d22 7370 696e 6e65 7222 0a0a 0a63 6c61  ="spinner"...cla
+0009ed00: 7373 2053 656c 6563 7428 5461 672e 6469  ss Select(Tag.di
+0009ed10: 7629 3a0a 2020 2020 7374 6174 6963 733d  v):.    statics=
+0009ed20: 5354 4154 4943 530a 2020 2020 6465 6620  STATICS.    def 
+0009ed30: 696e 6974 2873 656c 662c 6f70 7469 6f6e  init(self,option
+0009ed40: 733a 4c69 7374 4f72 4469 6374 2c20 2a2a  s:ListOrDict, **
+0009ed50: 6129 3a0a 2020 2020 2020 2020 7365 6c66  a):.        self
+0009ed60: 2e6f 7074 696f 6e73 3d65 6e73 7572 6564  .options=ensured
+0009ed70: 6963 7428 6f70 7469 6f6e 7329 0a20 2020  ict(options).   
+0009ed80: 2020 2020 2073 656c 665b 2263 6c61 7373       self["class
+0009ed90: 225d 2e61 6464 2822 7365 6c65 6374 2229  "].add("select")
+0009eda0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+0009edb0: 7265 6e64 6572 2873 656c 662e 6174 7472  render(self.attr
+0009edc0: 732e 6765 7428 2276 616c 7565 2229 290a  s.get("value")).
+0009edd0: 0a20 2020 2064 6566 2072 6572 656e 6465  .    def rerende
+0009ede0: 7228 7365 6c66 2c76 616c 7565 293a 0a20  r(self,value):. 
+0009edf0: 2020 2020 2020 2077 6974 6820 5461 672e         with Tag.
+0009ee00: 7365 6c65 6374 2820 5f6f 6e63 6861 6e67  select( _onchang
+0009ee10: 653d 6622 646f 6375 6d65 6e74 2e67 6574  e=f"document.get
+0009ee20: 456c 656d 656e 7442 7949 6428 277b 6964  ElementById('{id
+0009ee30: 2873 656c 6629 7d27 292e 7661 6c75 653d  (self)}').value=
+0009ee40: 6576 656e 742e 7461 7267 6574 2e76 616c  event.target.val
+0009ee50: 7565 222c 5f6e 616d 653d 7365 6c66 2e61  ue",_name=self.a
+0009ee60: 7474 7273 2e67 6574 2822 6e61 6d65 2229  ttrs.get("name")
+0009ee70: 2c5f 7265 7175 6972 6564 3d73 656c 662e  ,_required=self.
+0009ee80: 6174 7472 732e 6765 7428 2272 6571 7569  attrs.get("requi
+0009ee90: 7265 6422 2920 2920 6173 2073 656c 6563  red") ) as selec
+0009eea0: 743a 0a20 2020 2020 2020 2020 2020 2066  t:.            f
+0009eeb0: 6f72 206b 2c76 2069 6e20 7365 6c66 2e6f  or k,v in self.o
+0009eec0: 7074 696f 6e73 2e69 7465 6d73 2829 3a0a  ptions.items():.
+0009eed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0009eee0: 7365 6c65 6374 203c 3d20 5461 672e 6f70  select <= Tag.op
+0009eef0: 7469 6f6e 2876 2c5f 7661 6c75 653d 6b2c  tion(v,_value=k,
+0009ef00: 5f73 656c 6563 7465 643d 2828 7374 7228  _selected=((str(
+0009ef10: 7661 6c75 6529 3d3d 7374 7228 6b29 2929  value)==str(k)))
+0009ef20: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+0009ef30: 6c65 6172 2820 7365 6c65 6374 2029 0a0a  lear( select )..
+0009ef40: 636c 6173 7320 5261 6469 6f73 2854 6167  class Radios(Tag
+0009ef50: 2e73 7061 6e29 3a0a 2020 2020 7374 6174  .span):.    stat
+0009ef60: 6963 733d 5354 4154 4943 530a 2020 2020  ics=STATICS.    
+0009ef70: 6465 6620 696e 6974 2873 656c 662c 6f70  def init(self,op
+0009ef80: 7469 6f6e 733a 4c69 7374 4f72 4469 6374  tions:ListOrDict
+0009ef90: 2c20 2a2a 6129 3a0a 2020 2020 2020 2020  , **a):.        
+0009efa0: 7365 6c66 2e6f 7074 696f 6e73 203d 2065  self.options = e
+0009efb0: 6e73 7572 6564 6963 7428 6f70 7469 6f6e  nsuredict(option
+0009efc0: 7329 0a20 2020 2020 2020 2073 656c 665b  s).        self[
+0009efd0: 2263 6c61 7373 225d 2e61 6464 2822 636f  "class"].add("co
+0009efe0: 6e74 726f 6c22 290a 2020 2020 2020 2020  ntrol").        
+0009eff0: 7365 6c66 2e72 6572 656e 6465 7228 2073  self.rerender( s
+0009f000: 656c 662e 6174 7472 732e 6765 7428 2276  elf.attrs.get("v
+0009f010: 616c 7565 222c 4e6f 6e65 2920 290a 2020  alue",None) ).  
+0009f020: 2020 0a20 2020 2064 6566 2072 6572 656e    .    def reren
+0009f030: 6465 7228 7365 6c66 2c76 616c 7565 293a  der(self,value):
+0009f040: 0a20 2020 2020 2020 2022 2222 2073 7065  .        """ spe
+0009f050: 6369 616c 206d 6574 686f 6420 2873 6565  cial method (see
+0009f060: 2069 6669 656c 6473 292c 2074 6f20 7265   ifields), to re
+0009f070: 7265 6e64 6572 2061 6c6c 2074 6865 2077  render all the w
+0009f080: 6964 6765 7420 2874 6f20 6176 6f69 6420  idget (to avoid 
+0009f090: 746f 2064 6561 6c20 7769 7468 206a 7329  to deal with js)
+0009f0a0: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
+0009f0b0: 2e63 6c65 6172 2829 0a20 2020 2020 2020  .clear().       
+0009f0c0: 2066 6f72 206b 2c76 2069 6e20 7365 6c66   for k,v in self
+0009f0d0: 2e6f 7074 696f 6e73 2e69 7465 6d73 2829  .options.items()
+0009f0e0: 3a0a 2020 2020 2020 2020 2020 2020 6970  :.            ip
+0009f0f0: 743d 5461 672e 696e 7075 7428 0a20 2020  t=Tag.input(.   
+0009f100: 2020 2020 2020 2020 2020 2020 205f 7479               _ty
+0009f110: 7065 3d22 7261 6469 6f22 2c0a 2020 2020  pe="radio",.    
+0009f120: 2020 2020 2020 2020 2020 2020 5f76 616c              _val
+0009f130: 7565 3d6b 2c0a 2020 2020 2020 2020 2020  ue=k,.          
+0009f140: 2020 2020 2020 5f6e 616d 653d 7365 6c66        _name=self
+0009f150: 2e61 7474 7273 2e67 6574 2822 6e61 6d65  .attrs.get("name
+0009f160: 222c 7374 7228 6964 2873 656c 6629 2929  ",str(id(self)))
+0009f170: 2c20 2020 2020 2020 2020 2020 2020 2320  ,             # 
+0009f180: 6e65 6564 2061 206e 616d 6520 746f 2062  need a name to b
+0009f190: 6520 7661 6c69 640a 2020 2020 2020 2020  e valid.        
+0009f1a0: 2020 2020 2020 2020 5f63 6865 636b 6564          _checked
+0009f1b0: 3d28 7374 7228 7661 6c75 6529 3d3d 7374  =(str(value)==st
+0009f1c0: 7228 6b29 292c 0a20 2020 2020 2020 2020  r(k)),.         
+0009f1d0: 2020 2020 2020 205f 7265 7175 6972 6564         _required
+0009f1e0: 3d62 6f6f 6c28 7365 6c66 2e61 7474 7273  =bool(self.attrs
+0009f1f0: 2e67 6574 2822 7265 7175 6972 6564 222c  .get("required",
+0009f200: 4e6f 6e65 2929 2c0a 2020 2020 2020 2020  None)),.        
+0009f210: 2020 2020 2020 2020 5f72 6561 646f 6e6c          _readonl
+0009f220: 793d 626f 6f6c 2873 656c 662e 6174 7472  y=bool(self.attr
+0009f230: 732e 6765 7428 2272 6561 646f 6e6c 7922  s.get("readonly"
+0009f240: 2c4e 6f6e 6529 292c 0a20 2020 2020 2020  ,None)),.       
+0009f250: 2020 2020 2020 2020 205f 6f6e 6368 616e           _onchan
+0009f260: 6765 3d66 2264 6f63 756d 656e 742e 6765  ge=f"document.ge
+0009f270: 7445 6c65 6d65 6e74 4279 4964 2827 7b69  tElementById('{i
+0009f280: 6428 7365 6c66 297d 2729 2e76 616c 7565  d(self)}').value
+0009f290: 3d27 7b6b 7d27 3b22 0a20 2020 2020 2020  ='{k}';".       
+0009f2a0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0009f2b0: 2020 2073 656c 6620 3c3d 2054 6167 2e64     self <= Tag.d
+0009f2c0: 6976 2854 6167 2e6c 6162 656c 2820 6970  iv(Tag.label( ip
+0009f2d0: 7420 2b22 2022 2b20 7620 2c5f 636c 6173  t +" "+ v ,_clas
+0009f2e0: 733d 2272 6164 696f 2229 290a 0a23 2323  s="radio"))..###
 0009f2f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0009f300: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0009f310: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0009f320: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0009f330: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-0009f340: 2323 2044 6961 6c6f 6720 6f62 6a65 6374  ## Dialog object
-0009f350: 730a 2323 2323 2323 2323 2323 2323 2323  s.##############
+0009f330: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0009f340: 2323 230a 2323 2044 6961 6c6f 6720 6f62  ###.## Dialog ob
+0009f350: 6a65 6374 730a 2323 2323 2323 2323 2323  jects.##########
 0009f360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0009f370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0009f380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0009f390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0009f3a0: 2323 2323 2323 2323 0a63 6c61 7373 2045  ########.class E
-0009f3b0: 6d70 7479 2854 6167 2e64 6976 293a 0a20  mpty(Tag.div):. 
-0009f3c0: 2020 2064 6566 2069 6e69 7428 7365 6c66     def init(self
-0009f3d0: 2c6d 6574 6174 6167 293a 0a20 2020 2020  ,metatag):.     
-0009f3e0: 2020 2073 656c 662e 636c 6561 7228 290a     self.clear().
-0009f3f0: 0a0a 636c 6173 7320 4d6f 6461 6c42 6c6f  ..class ModalBlo
-0009f400: 636b 2854 6167 2e64 6976 293a 0a20 2020  ck(Tag.div):.   
-0009f410: 2064 6566 2069 6e69 7428 7365 6c66 2c6d   def init(self,m
-0009f420: 6574 6174 6167 2c6f 626a 293a 0a20 2020  etatag,obj):.   
-0009f430: 2020 2020 2073 656c 665b 2763 6c61 7373       self['class
-0009f440: 275d 3d22 6d6f 6461 6c20 6973 2d61 6374  ']="modal is-act
-0009f450: 6976 6522 0a20 2020 2020 2020 2073 656c  ive".        sel
-0009f460: 6620 3c3d 2054 6167 2e64 6976 285f 636c  f <= Tag.div(_cl
-0009f470: 6173 733d 226d 6f64 616c 2d62 6163 6b67  ass="modal-backg
-0009f480: 726f 756e 6422 2920 2b20 6f62 6a0a 0a63  round") + obj..c
-0009f490: 6c61 7373 2050 6f70 5061 6765 2854 6167  lass PopPage(Tag
-0009f4a0: 2e64 6976 293a 0a20 2020 2064 6566 2069  .div):.    def i
-0009f4b0: 6e69 7428 7365 6c66 2c6d 6574 6174 6167  nit(self,metatag
-0009f4c0: 2c6f 626a 293a 0a20 2020 2020 2020 2073  ,obj):.        s
-0009f4d0: 656c 665b 2763 6c61 7373 275d 2e61 6464  elf['class'].add
-0009f4e0: 2822 636f 6e74 656e 7422 290a 2020 2020  ("content").    
-0009f4f0: 2020 2020 7365 6c66 5b22 7374 796c 6522      self["style"
-0009f500: 5d2e 7365 7428 2270 6f73 6974 696f 6e22  ].set("position"
-0009f510: 2c22 6669 7865 6422 290a 2020 2020 2020  ,"fixed").      
-0009f520: 2020 7365 6c66 5b22 7374 796c 6522 5d2e    self["style"].
-0009f530: 7365 7428 2274 6f70 222c 2230 7078 2229  set("top","0px")
-0009f540: 0a20 2020 2020 2020 2073 656c 665b 2273  .        self["s
-0009f550: 7479 6c65 225d 2e73 6574 2822 626f 7474  tyle"].set("bott
-0009f560: 6f6d 222c 2230 7078 2229 0a20 2020 2020  om","0px").     
-0009f570: 2020 2073 656c 665b 2273 7479 6c65 225d     self["style"]
-0009f580: 2e73 6574 2822 7269 6768 7422 2c22 3070  .set("right","0p
-0009f590: 7822 290a 2020 2020 2020 2020 7365 6c66  x").        self
-0009f5a0: 5b22 7374 796c 6522 5d2e 7365 7428 226c  ["style"].set("l
-0009f5b0: 6566 7422 2c22 3070 7822 290a 2020 2020  eft","0px").    
-0009f5c0: 2020 2020 7365 6c66 5b22 7374 796c 6522      self["style"
-0009f5d0: 5d2e 7365 7428 227a 2d69 6e64 6578 222c  ].set("z-index",
-0009f5e0: 2235 3030 2229 0a20 2020 2020 2020 2073  "500").        s
-0009f5f0: 656c 665b 2273 7479 6c65 225d 2e73 6574  elf["style"].set
-0009f600: 2822 6261 636b 6772 6f75 6e64 222c 2277  ("background","w
-0009f610: 6869 7465 2229 0a20 2020 2020 2020 2073  hite").        s
-0009f620: 656c 6620 3c3d 206f 626a 0a0a 636c 6173  elf <= obj..clas
-0009f630: 7320 4d6f 6461 6c41 6c65 7274 284d 6f64  s ModalAlert(Mod
-0009f640: 616c 426c 6f63 6b29 3a0a 2020 2020 6465  alBlock):.    de
-0009f650: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-0009f660: 6d65 7461 7461 672c 6f62 6a2c 7773 697a  metatag,obj,wsiz
-0009f670: 653a 666c 6f61 743d 4e6f 6e65 293a 0a20  e:float=None):. 
-0009f680: 2020 2020 2020 2069 6620 7773 697a 6520         if wsize 
-0009f690: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0009f6a0: 2020 2020 2020 2020 2070 7769 6474 683d           pwidth=
-0009f6b0: 6622 7b69 6e74 2877 7369 7a65 2a31 3030  f"{int(wsize*100
-0009f6c0: 297d 2522 2020 2020 2020 2020 0a20 2020  )}%"        .   
-0009f6d0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0009f6e0: 2020 2020 2020 2070 7769 6474 683d 4e6f         pwidth=No
-0009f6f0: 6e65 0a20 2020 2020 2020 206f 626a 203d  ne.        obj =
-0009f700: 2054 6167 2e64 6976 286f 626a 2c5f 636c   Tag.div(obj,_cl
-0009f710: 6173 733d 2262 6f78 2229 0a20 2020 2020  ass="box").     
-0009f720: 2020 206f 626a 3d54 6167 2e64 6976 286f     obj=Tag.div(o
-0009f730: 626a 2c5f 636c 6173 733d 226d 6f64 616c  bj,_class="modal
-0009f740: 2d63 6f6e 7465 6e74 2229 0a20 2020 2020  -content").     
-0009f750: 2020 204d 6f64 616c 426c 6f63 6b2e 5f5f     ModalBlock.__
-0009f760: 696e 6974 5f5f 2873 656c 662c 6d65 7461  init__(self,meta
-0009f770: 7461 672c 6f62 6a29 0a20 2020 2020 2020  tag,obj).       
-0009f780: 2073 656c 662e 6368 696c 6473 5b30 5d5b   self.childs[0][
-0009f790: 226f 6e63 6c69 636b 225d 3d6d 6574 6174  "onclick"]=metat
-0009f7a0: 6167 2e73 7465 7065 7665 6e74 2829 0a20  ag.stepevent(). 
-0009f7b0: 2020 2020 2020 2069 6620 7077 6964 7468         if pwidth
-0009f7c0: 3a0a 2020 2020 2020 2020 2020 2020 6f62  :.            ob
-0009f7d0: 6a5b 2273 7479 6c65 225d 3d66 2277 6964  j["style"]=f"wid
-0009f7e0: 7468 3a7b 7077 6964 7468 7d3b 220a 2020  th:{pwidth};".  
-0009f7f0: 2020 2020 2020 7365 6c66 202b 3d20 5461        self += Ta
-0009f800: 672e 6275 7474 6f6e 285f 636c 6173 733d  g.button(_class=
-0009f810: 226d 6f64 616c 2d63 6c6f 7365 2069 732d  "modal-close is-
-0009f820: 6c61 7267 6522 2c5f 6172 6961 5f6c 6162  large",_aria_lab
-0009f830: 656c 3d22 636c 6f73 6522 2c5f 6f6e 636c  el="close",_oncl
-0009f840: 6963 6b3d 6d65 7461 7461 672e 7374 6570  ick=metatag.step
-0009f850: 6576 656e 7428 2929 0a0a 0a63 6c61 7373  event())...class
-0009f860: 204d 6f64 616c 436f 6e66 6972 6d28 4d6f   ModalConfirm(Mo
-0009f870: 6461 6c41 6c65 7274 293a 0a20 2020 2064  dalAlert):.    d
-0009f880: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-0009f890: 2c6d 6574 6174 6167 2c6f 626a 2c63 6229  ,metatag,obj,cb)
-0009f8a0: 3a0a 2020 2020 2020 2020 6465 6620 6361  :.        def ca
-0009f8b0: 6c6c 2865 7629 3a0a 2020 2020 2020 2020  ll(ev):.        
-0009f8c0: 2020 2020 6d65 7461 7461 672e 7374 6570      metatag.step
-0009f8d0: 2829 0a20 2020 2020 2020 2020 2020 2072  ().            r
-0009f8e0: 6574 7572 6e20 6362 2820 6576 2e74 6172  eturn cb( ev.tar
-0009f8f0: 6765 742e 7661 6c20 290a 2020 2020 2020  get.val ).      
-0009f900: 2020 200a 2020 2020 2020 2020 626f 783d     .        box=
-0009f910: 5b20 0a20 2020 2020 2020 2020 2020 2054  [ .            T
-0009f920: 6167 2e64 6976 286f 626a 292c 0a20 2020  ag.div(obj),.   
-0009f930: 2020 2020 2020 2020 2042 7574 746f 6e28           Button(
-0009f940: 2259 6573 222c 7661 6c3d 5472 7565 2c5f  "Yes",val=True,_
-0009f950: 6f6e 636c 6963 6b3d 6361 6c6c 292c 0a20  onclick=call),. 
-0009f960: 2020 2020 2020 2020 2020 2042 7574 746f             Butto
-0009f970: 6e28 224e 6f22 2c76 616c 3d46 616c 7365  n("No",val=False
-0009f980: 2c5f 6f6e 636c 6963 6b3d 6361 6c6c 292c  ,_onclick=call),
-0009f990: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
-0009f9a0: 2020 204d 6f64 616c 416c 6572 742e 5f5f     ModalAlert.__
-0009f9b0: 696e 6974 5f5f 2873 656c 662c 6d65 7461  init__(self,meta
-0009f9c0: 7461 672c 626f 7829 0a0a 636c 6173 7320  tag,box)..class 
-0009f9d0: 4d6f 6461 6c50 726f 6d70 7428 4d6f 6461  ModalPrompt(Moda
-0009f9e0: 6c41 6c65 7274 293a 0a20 2020 2064 6566  lAlert):.    def
-0009f9f0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c6d   __init__(self,m
-0009fa00: 6574 6174 6167 2c20 7661 6c75 652c 7469  etatag, value,ti
-0009fa10: 746c 652c 6362 293a 0a20 2020 2020 2020  tle,cb):.       
-0009fa20: 2064 6566 2063 616c 6c28 6469 636f 293a   def call(dico):
-0009fa30: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
-0009fa40: 6174 6167 2e73 7465 7028 290a 2020 2020  atag.step().    
-0009fa50: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-0009fa60: 6228 2064 6963 6f5b 2270 726f 6d70 7476  b( dico["promptv
-0009fa70: 616c 7565 225d 2029 0a20 2020 2020 2020  alue"] ).       
-0009fa80: 2077 6974 6820 466f 726d 286f 6e73 7562   with Form(onsub
-0009fa90: 6d69 743d 6361 6c6c 2920 6173 2066 3a0a  mit=call) as f:.
-0009faa0: 2020 2020 2020 2020 2020 2020 662b 3d54              f+=T
-0009fab0: 6167 2e64 6976 2820 7469 746c 6520 290a  ag.div( title ).
-0009fac0: 2020 2020 2020 2020 2020 2020 662b 3d54              f+=T
-0009fad0: 6167 2e64 6976 2820 496e 7075 7428 5f76  ag.div( Input(_v
-0009fae0: 616c 7565 3d76 616c 7565 2c5f 6e61 6d65  alue=value,_name
-0009faf0: 3d22 7072 6f6d 7074 7661 6c75 6522 2c6a  ="promptvalue",j
-0009fb00: 733d 2273 656c 662e 666f 6375 7328 293b  s="self.focus();
-0009fb10: 7365 6c66 2e73 656c 6563 7428 2922 2c20  self.select()", 
-0009fb20: 5f61 7574 6f66 6f63 7573 3d54 7275 6529  _autofocus=True)
-0009fb30: 202c 5f73 7479 6c65 3d22 7061 6464 696e   ,_style="paddin
-0009fb40: 673a 3470 7820 3022 290a 2020 2020 2020  g:4px 0").      
-0009fb50: 2020 2020 2020 662b 3d42 7574 746f 6e28        f+=Button(
-0009fb60: 224f 6b22 2029 0a20 2020 2020 2020 2020  "Ok" ).         
-0009fb70: 2020 2066 2b3d 4275 7474 6f6e 2822 4361     f+=Button("Ca
-0009fb80: 6e63 656c 222c 5f74 7970 653d 2262 7574  ncel",_type="but
-0009fb90: 746f 6e22 2c5f 6f6e 636c 6963 6b3d 6d65  ton",_onclick=me
-0009fba0: 7461 7461 672e 7374 6570 6576 656e 7428  tatag.stepevent(
-0009fbb0: 2929 0a20 2020 2020 2020 204d 6f64 616c  )).        Modal
-0009fbc0: 416c 6572 742e 5f5f 696e 6974 5f5f 2873  Alert.__init__(s
-0009fbd0: 656c 662c 6d65 7461 7461 672c 6629 0a20  elf,metatag,f). 
-0009fbe0: 2020 2020 2020 200a 636c 6173 7320 4472         .class Dr
-0009fbf0: 6177 6572 2854 6167 2e64 6976 293a 0a20  awer(Tag.div):. 
-0009fc00: 2020 2064 6566 2069 6e69 7428 7365 6c66     def init(self
-0009fc10: 2c6d 6574 6174 6167 2c6f 626a 2c6d 6f64  ,metatag,obj,mod
-0009fc20: 653a 7374 7229 3a0a 2020 2020 2020 2020  e:str):.        
-0009fc30: 7369 7a65 3d35 300a 2020 2020 2020 2020  size=50.        
-0009fc40: 6966 206d 6f64 653d 3d22 6c65 6674 223a  if mode=="left":
-0009fc50: 0a20 2020 2020 2020 2020 2020 2074 2c72  .            t,r
-0009fc60: 2c62 2c6c 3d20 2822 3070 7822 2c66 227b  ,b,l= ("0px",f"{
-0009fc70: 7369 7a65 7d25 222c 2230 7078 222c 2230  size}%","0px","0
-0009fc80: 7078 2229 0a20 2020 2020 2020 2065 6c69  px").        eli
-0009fc90: 6620 6d6f 6465 3d3d 2272 6967 6874 223a  f mode=="right":
-0009fca0: 0a20 2020 2020 2020 2020 2020 2074 2c72  .            t,r
-0009fcb0: 2c62 2c6c 3d20 2822 3070 7822 2c22 3070  ,b,l= ("0px","0p
-0009fcc0: 7822 2c22 3070 7822 2c66 227b 7369 7a65  x","0px",f"{size
-0009fcd0: 7d25 2229 0a20 2020 2020 2020 2065 6c69  }%").        eli
-0009fce0: 6620 6d6f 6465 3d3d 2262 6f74 746f 6d22  f mode=="bottom"
-0009fcf0: 3a0a 2020 2020 2020 2020 2020 2020 742c  :.            t,
-0009fd00: 722c 622c 6c3d 2866 227b 7369 7a65 7d25  r,b,l=(f"{size}%
-0009fd10: 222c 2230 7078 222c 2230 7078 222c 2230  ","0px","0px","0
-0009fd20: 7078 2229 0a20 2020 2020 2020 2065 6c69  px").        eli
-0009fd30: 6620 6d6f 6465 3d3d 2274 6f70 223a 0a20  f mode=="top":. 
-0009fd40: 2020 2020 2020 2020 2020 2074 2c72 2c62             t,r,b
-0009fd50: 2c6c 3d20 2822 3070 7822 2c22 3070 7822  ,l= ("0px","0px"
-0009fd60: 2c66 227b 7369 7a65 7d25 222c 2230 7078  ,f"{size}%","0px
-0009fd70: 2229 0a0a 2020 2020 2020 2020 7365 6c66  ")..        self
-0009fd80: 203c 3d20 566f 696c 6528 5f6f 6e6d 6f75   <= Voile(_onmou
-0009fd90: 7365 646f 776e 3d6d 6574 6174 6167 2e73  sedown=metatag.s
-0009fda0: 7465 7065 7665 6e74 2829 290a 2020 2020  tepevent()).    
-0009fdb0: 2020 2020 7365 6c66 203c 3d20 5461 672e      self <= Tag.
-0009fdc0: 6469 7628 206f 626a 202c 5f73 7479 6c65  div( obj ,_style
-0009fdd0: 3d66 2270 6f73 6974 696f 6e3a 6669 7865  =f"position:fixe
-0009fde0: 643b 746f 703a 7b74 7d3b 626f 7474 6f6d  d;top:{t};bottom
-0009fdf0: 3a7b 627d 3b6c 6566 743a 7b6c 7d3b 7269  :{b};left:{l};ri
-0009fe00: 6768 743a 7b72 7d3b 6261 636b 6772 6f75  ght:{r};backgrou
-0009fe10: 6e64 3a77 6869 7465 3b62 6f72 6465 722d  nd:white;border-
-0009fe20: 7261 6469 7573 3a30 7078 3b62 6f78 2d73  radius:0px;box-s
-0009fe30: 6861 646f 773a 2072 6762 6128 302c 2030  hadow: rgba(0, 0
-0009fe40: 2c20 302c 2030 2e33 3529 2030 7078 2035  , 0, 0.35) 0px 5
-0009fe50: 7078 2031 3570 783b 3b7a 2d69 6e64 6578  px 15px;;z-index
-0009fe60: 3a31 3030 313b 7061 6464 696e 673a 3130  :1001;padding:10
-0009fe70: 7078 2229 0a0a 636c 6173 7320 506f 7028  px")..class Pop(
-0009fe80: 5461 672e 6469 7629 3a0a 2020 2020 6465  Tag.div):.    de
-0009fe90: 6620 696e 6974 2873 656c 662c 6d65 7461  f init(self,meta
-0009fea0: 7461 672c 6f62 6a2c 7879 3a74 7570 6c65  tag,obj,xy:tuple
-0009feb0: 293a 0a20 2020 2020 2020 2078 2c79 3d78  ):.        x,y=x
-0009fec0: 790a 2020 2020 2020 2020 7365 6c66 203c  y.        self <
-0009fed0: 3d20 566f 696c 6554 7261 6e73 7061 7265  = VoileTranspare
-0009fee0: 6e74 285f 6f6e 6d6f 7573 6564 6f77 6e3d  nt(_onmousedown=
-0009fef0: 6d65 7461 7461 672e 6269 6e64 2e70 6f70  metatag.bind.pop
-0009ff00: 636c 6f73 6528 292c 5f6f 6e63 6f6e 7465  close(),_onconte
-0009ff10: 7874 6d65 6e75 3d22 6576 656e 742e 7374  xtmenu="event.st
-0009ff20: 6f70 5072 6f70 6167 6174 696f 6e28 293b  opPropagation();
-0009ff30: 7265 7475 726e 2066 616c 7365 2229 0a20  return false"). 
-0009ff40: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-0009ff50: 6a73 3d22 2222 2866 756e 6374 696f 6e28  js="""(function(
-0009ff60: 7461 672c 782c 7929 207b 0a20 2020 2020  tag,x,y) {.     
-0009ff70: 2020 2020 2020 2074 6167 2e73 7479 6c65         tag.style
-0009ff80: 3d22 706f 7369 7469 6f6e 3a66 6978 6564  ="position:fixed
-0009ff90: 3b7a 2d69 6e64 6578 3a32 3030 313b 7061  ;z-index:2001;pa
-0009ffa0: 6464 696e 673a 3270 783b 6c65 6674 3a22  dding:2px;left:"
-0009ffb0: 2b78 2b22 7078 3b74 6f70 3a22 2b79 2b22  +x+"px;top:"+y+"
-0009ffc0: 7078 223b 0a20 2020 2020 2020 2020 2020  px";.           
-0009ffd0: 206c 6574 2062 773d 7769 6e64 6f77 2e69   let bw=window.i
-0009ffe0: 6e6e 6572 5769 6474 683b 0a20 2020 2020  nnerWidth;.     
-0009fff0: 2020 2020 2020 206c 6574 2062 683d 7769         let bh=wi
-000a0000: 6e64 6f77 2e69 6e6e 6572 4865 6967 6874  ndow.innerHeight
-000a0010: 3b0a 2020 2020 2020 2020 2020 2020 6c65  ;.            le
-000a0020: 7420 773d 7461 672e 636c 6965 6e74 5769  t w=tag.clientWi
-000a0030: 6474 683b 0a20 2020 2020 2020 2020 2020  dth;.           
-000a0040: 206c 6574 2068 3d74 6167 2e63 6c69 656e   let h=tag.clien
-000a0050: 7448 6569 6768 743b 0a20 2020 2020 2020  tHeight;.       
-000a0060: 2020 2020 2069 6628 782b 7720 3e20 6277       if(x+w > bw
-000a0070: 2920 783d 6277 2d77 3b0a 2020 2020 2020  ) x=bw-w;.      
-000a0080: 2020 2020 2020 6966 2879 2b68 203e 2062        if(y+h > b
-000a0090: 6829 2079 3d62 682d 683b 0a20 2020 2020  h) y=bh-h;.     
-000a00a0: 2020 2020 2020 2074 6167 2e73 7479 6c65         tag.style
-000a00b0: 3d22 706f 7369 7469 6f6e 3a66 6978 6564  ="position:fixed
-000a00c0: 3b7a 2d69 6e64 6578 3a32 3030 313b 7061  ;z-index:2001;pa
-000a00d0: 6464 696e 673a 3270 783b 6c65 6674 3a22  dding:2px;left:"
-000a00e0: 2b78 2b22 7078 3b74 6f70 3a22 2b79 2b22  +x+"px;top:"+y+"
-000a00f0: 7078 223b 0a20 2020 2020 2020 207d 2928  px";.        })(
-000a0100: 7365 6c66 2c25 732c 2573 2922 2222 2025  self,%s,%s)""" %
-000a0110: 2028 782c 7929 0a0a 2020 2020 2020 2020   (x,y)..        
-000a0120: 7365 6c66 203c 3d20 5461 672e 6469 7628  self <= Tag.div(
-000a0130: 206f 626a 202c 6a73 3d6a 7329 0a63 6c61   obj ,js=js).cla
-000a0140: 7373 2054 6f61 7374 2854 6167 2e64 6976  ss Toast(Tag.div
-000a0150: 293a 0a20 2020 2064 6566 2069 6e69 7428  ):.    def init(
-000a0160: 7365 6c66 2c6d 6169 6e5f 6e6f 6e5f 7573  self,main_non_us
-000a0170: 6564 2c6f 626a 2c74 696d 656f 7574 3d31  ed,obj,timeout=1
-000a0180: 3030 3029 3a0a 2020 2020 2020 2020 7365  000):.        se
-000a0190: 6c66 203c 3d20 5461 672e 6469 7628 6f62  lf <= Tag.div(ob
-000a01a0: 6a2c 5f73 7479 6c65 3d22 706f 7369 7469  j,_style="positi
-000a01b0: 6f6e 3a66 6978 6564 3b72 6967 6874 3a31  on:fixed;right:1
-000a01c0: 3070 783b 626f 7474 6f6d 3a31 3070 783b  0px;bottom:10px;
-000a01d0: 7a2d 696e 6465 783a 3130 3031 3b22 2c20  z-index:1001;", 
-000a01e0: 5f63 6c61 7373 3d22 6e6f 7469 6669 6361  _class="notifica
-000a01f0: 7469 6f6e 2069 732d 6c69 6e6b 2069 732d  tion is-link is-
-000a0200: 6c69 6768 7422 290a 2020 2020 2020 2020  light").        
-000a0210: 7365 6c66 2e6a 733d 2273 6574 5469 6d65  self.js="setTime
-000a0220: 6f75 7428 2066 756e 6374 696f 6e28 2920  out( function() 
-000a0230: 7b73 656c 662e 7265 6d6f 7665 2829 7d20  {self.remove()} 
-000a0240: 2c20 2573 2922 2025 2074 696d 656f 7574  , %s)" % timeout
-000a0250: 0a0a 2323 2323 2323 2323 2323 2323 2323  ..##############
-000a0260: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000a0270: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000a0280: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0009f3a0: 2323 2323 2323 2323 2323 2323 0a63 6c61  ############.cla
+0009f3b0: 7373 2045 6d70 7479 2854 6167 2e64 6976  ss Empty(Tag.div
+0009f3c0: 293a 0a20 2020 2064 6566 2069 6e69 7428  ):.    def init(
+0009f3d0: 7365 6c66 2c6d 6574 6174 6167 293a 0a20  self,metatag):. 
+0009f3e0: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
+0009f3f0: 7228 290a 0a0a 636c 6173 7320 4d6f 6461  r()...class Moda
+0009f400: 6c42 6c6f 636b 2854 6167 2e64 6976 293a  lBlock(Tag.div):
+0009f410: 0a20 2020 2064 6566 2069 6e69 7428 7365  .    def init(se
+0009f420: 6c66 2c6d 6574 6174 6167 2c6f 626a 293a  lf,metatag,obj):
+0009f430: 0a20 2020 2020 2020 2073 656c 665b 2763  .        self['c
+0009f440: 6c61 7373 275d 3d22 6d6f 6461 6c20 6973  lass']="modal is
+0009f450: 2d61 6374 6976 6522 0a20 2020 2020 2020  -active".       
+0009f460: 2073 656c 6620 3c3d 2054 6167 2e64 6976   self <= Tag.div
+0009f470: 285f 636c 6173 733d 226d 6f64 616c 2d62  (_class="modal-b
+0009f480: 6163 6b67 726f 756e 6422 2920 2b20 6f62  ackground") + ob
+0009f490: 6a0a 0a63 6c61 7373 2050 6f70 5061 6765  j..class PopPage
+0009f4a0: 2854 6167 2e64 6976 293a 0a20 2020 2064  (Tag.div):.    d
+0009f4b0: 6566 2069 6e69 7428 7365 6c66 2c6d 6574  ef init(self,met
+0009f4c0: 6174 6167 2c6f 626a 293a 0a20 2020 2020  atag,obj):.     
+0009f4d0: 2020 2073 656c 665b 2763 6c61 7373 275d     self['class']
+0009f4e0: 2e61 6464 2822 636f 6e74 656e 7422 290a  .add("content").
+0009f4f0: 2020 2020 2020 2020 7365 6c66 5b22 7374          self["st
+0009f500: 796c 6522 5d2e 7365 7428 2270 6f73 6974  yle"].set("posit
+0009f510: 696f 6e22 2c22 6669 7865 6422 290a 2020  ion","fixed").  
+0009f520: 2020 2020 2020 7365 6c66 5b22 7374 796c        self["styl
+0009f530: 6522 5d2e 7365 7428 2274 6f70 222c 2230  e"].set("top","0
+0009f540: 7078 2229 0a20 2020 2020 2020 2073 656c  px").        sel
+0009f550: 665b 2273 7479 6c65 225d 2e73 6574 2822  f["style"].set("
+0009f560: 626f 7474 6f6d 222c 2230 7078 2229 0a20  bottom","0px"). 
+0009f570: 2020 2020 2020 2073 656c 665b 2273 7479         self["sty
+0009f580: 6c65 225d 2e73 6574 2822 7269 6768 7422  le"].set("right"
+0009f590: 2c22 3070 7822 290a 2020 2020 2020 2020  ,"0px").        
+0009f5a0: 7365 6c66 5b22 7374 796c 6522 5d2e 7365  self["style"].se
+0009f5b0: 7428 226c 6566 7422 2c22 3070 7822 290a  t("left","0px").
+0009f5c0: 2020 2020 2020 2020 7365 6c66 5b22 7374          self["st
+0009f5d0: 796c 6522 5d2e 7365 7428 227a 2d69 6e64  yle"].set("z-ind
+0009f5e0: 6578 222c 2235 3030 2229 0a20 2020 2020  ex","500").     
+0009f5f0: 2020 2073 656c 665b 2273 7479 6c65 225d     self["style"]
+0009f600: 2e73 6574 2822 6261 636b 6772 6f75 6e64  .set("background
+0009f610: 222c 2277 6869 7465 2229 0a20 2020 2020  ","white").     
+0009f620: 2020 2073 656c 6620 3c3d 206f 626a 0a0a     self <= obj..
+0009f630: 636c 6173 7320 4d6f 6461 6c41 6c65 7274  class ModalAlert
+0009f640: 284d 6f64 616c 426c 6f63 6b29 3a0a 2020  (ModalBlock):.  
+0009f650: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0009f660: 656c 662c 6d65 7461 7461 672c 6f62 6a2c  elf,metatag,obj,
+0009f670: 7773 697a 653a 666c 6f61 743d 4e6f 6e65  wsize:float=None
+0009f680: 293a 0a20 2020 2020 2020 2069 6620 7773  ):.        if ws
+0009f690: 697a 6520 6973 206e 6f74 204e 6f6e 653a  ize is not None:
+0009f6a0: 0a20 2020 2020 2020 2020 2020 2070 7769  .            pwi
+0009f6b0: 6474 683d 6622 7b69 6e74 2877 7369 7a65  dth=f"{int(wsize
+0009f6c0: 2a31 3030 297d 2522 2020 2020 2020 2020  *100)}%"        
+0009f6d0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0009f6e0: 2020 2020 2020 2020 2020 2070 7769 6474             pwidt
+0009f6f0: 683d 4e6f 6e65 0a20 2020 2020 2020 206f  h=None.        o
+0009f700: 626a 203d 2054 6167 2e64 6976 286f 626a  bj = Tag.div(obj
+0009f710: 2c5f 636c 6173 733d 2262 6f78 2229 0a20  ,_class="box"). 
+0009f720: 2020 2020 2020 206f 626a 3d54 6167 2e64         obj=Tag.d
+0009f730: 6976 286f 626a 2c5f 636c 6173 733d 226d  iv(obj,_class="m
+0009f740: 6f64 616c 2d63 6f6e 7465 6e74 222c 5f6f  odal-content",_o
+0009f750: 6e6d 6f75 7365 646f 776e 3d22 6576 656e  nmousedown="even
+0009f760: 742e 7374 6f70 5072 6f70 6167 6174 696f  t.stopPropagatio
+0009f770: 6e28 293b 2229 0a20 2020 2020 2020 204d  n();").        M
+0009f780: 6f64 616c 426c 6f63 6b2e 5f5f 696e 6974  odalBlock.__init
+0009f790: 5f5f 2873 656c 662c 6d65 7461 7461 672c  __(self,metatag,
+0009f7a0: 6f62 6a29 0a20 2020 2020 2020 2073 656c  obj).        sel
+0009f7b0: 662e 6368 696c 6473 5b30 5d5b 226f 6e6d  f.childs[0]["onm
+0009f7c0: 6f75 7365 646f 776e 225d 3d6d 6574 6174  ousedown"]=metat
+0009f7d0: 6167 2e73 7465 7065 7665 6e74 2829 0a20  ag.stepevent(). 
+0009f7e0: 2020 2020 2020 2069 6620 7077 6964 7468         if pwidth
+0009f7f0: 3a0a 2020 2020 2020 2020 2020 2020 6f62  :.            ob
+0009f800: 6a5b 2273 7479 6c65 225d 3d66 2277 6964  j["style"]=f"wid
+0009f810: 7468 3a7b 7077 6964 7468 7d3b 220a 2020  th:{pwidth};".  
+0009f820: 2020 2020 2020 7365 6c66 202b 3d20 5461        self += Ta
+0009f830: 672e 6275 7474 6f6e 285f 636c 6173 733d  g.button(_class=
+0009f840: 226d 6f64 616c 2d63 6c6f 7365 2069 732d  "modal-close is-
+0009f850: 6c61 7267 6522 2c5f 6172 6961 5f6c 6162  large",_aria_lab
+0009f860: 656c 3d22 636c 6f73 6522 2c5f 6f6e 636c  el="close",_oncl
+0009f870: 6963 6b3d 6d65 7461 7461 672e 7374 6570  ick=metatag.step
+0009f880: 6576 656e 7428 2929 0a0a 0a63 6c61 7373  event())...class
+0009f890: 204d 6f64 616c 436f 6e66 6972 6d28 4d6f   ModalConfirm(Mo
+0009f8a0: 6461 6c41 6c65 7274 293a 0a20 2020 2064  dalAlert):.    d
+0009f8b0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+0009f8c0: 2c6d 6574 6174 6167 2c6f 626a 2c63 6229  ,metatag,obj,cb)
+0009f8d0: 3a0a 2020 2020 2020 2020 6465 6620 6361  :.        def ca
+0009f8e0: 6c6c 2865 7629 3a0a 2020 2020 2020 2020  ll(ev):.        
+0009f8f0: 2020 2020 6d65 7461 7461 672e 7374 6570      metatag.step
+0009f900: 2829 0a20 2020 2020 2020 2020 2020 2072  ().            r
+0009f910: 6574 7572 6e20 6362 2820 6576 2e74 6172  eturn cb( ev.tar
+0009f920: 6765 742e 7661 6c20 290a 2020 2020 2020  get.val ).      
+0009f930: 2020 200a 2020 2020 2020 2020 626f 783d     .        box=
+0009f940: 5b20 0a20 2020 2020 2020 2020 2020 2054  [ .            T
+0009f950: 6167 2e64 6976 286f 626a 292c 0a20 2020  ag.div(obj),.   
+0009f960: 2020 2020 2020 2020 2042 7574 746f 6e28           Button(
+0009f970: 2259 6573 222c 7661 6c3d 5472 7565 2c5f  "Yes",val=True,_
+0009f980: 6f6e 636c 6963 6b3d 6361 6c6c 292c 0a20  onclick=call),. 
+0009f990: 2020 2020 2020 2020 2020 2042 7574 746f             Butto
+0009f9a0: 6e28 224e 6f22 2c76 616c 3d46 616c 7365  n("No",val=False
+0009f9b0: 2c5f 6f6e 636c 6963 6b3d 6361 6c6c 292c  ,_onclick=call),
+0009f9c0: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
+0009f9d0: 2020 204d 6f64 616c 416c 6572 742e 5f5f     ModalAlert.__
+0009f9e0: 696e 6974 5f5f 2873 656c 662c 6d65 7461  init__(self,meta
+0009f9f0: 7461 672c 626f 7829 0a0a 636c 6173 7320  tag,box)..class 
+0009fa00: 4d6f 6461 6c50 726f 6d70 7428 4d6f 6461  ModalPrompt(Moda
+0009fa10: 6c41 6c65 7274 293a 0a20 2020 2064 6566  lAlert):.    def
+0009fa20: 205f 5f69 6e69 745f 5f28 7365 6c66 2c6d   __init__(self,m
+0009fa30: 6574 6174 6167 2c20 7661 6c75 652c 7469  etatag, value,ti
+0009fa40: 746c 652c 6362 293a 0a20 2020 2020 2020  tle,cb):.       
+0009fa50: 2064 6566 2063 616c 6c28 6469 636f 293a   def call(dico):
+0009fa60: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+0009fa70: 6174 6167 2e73 7465 7028 290a 2020 2020  atag.step().    
+0009fa80: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+0009fa90: 6228 2064 6963 6f5b 2270 726f 6d70 7476  b( dico["promptv
+0009faa0: 616c 7565 225d 2029 0a20 2020 2020 2020  alue"] ).       
+0009fab0: 2077 6974 6820 466f 726d 286f 6e73 7562   with Form(onsub
+0009fac0: 6d69 743d 6361 6c6c 2920 6173 2066 3a0a  mit=call) as f:.
+0009fad0: 2020 2020 2020 2020 2020 2020 662b 3d54              f+=T
+0009fae0: 6167 2e64 6976 2820 7469 746c 6520 290a  ag.div( title ).
+0009faf0: 2020 2020 2020 2020 2020 2020 662b 3d54              f+=T
+0009fb00: 6167 2e64 6976 2820 496e 7075 7428 5f76  ag.div( Input(_v
+0009fb10: 616c 7565 3d76 616c 7565 2c5f 6e61 6d65  alue=value,_name
+0009fb20: 3d22 7072 6f6d 7074 7661 6c75 6522 2c6a  ="promptvalue",j
+0009fb30: 733d 2273 656c 662e 666f 6375 7328 293b  s="self.focus();
+0009fb40: 7365 6c66 2e73 656c 6563 7428 2922 2c20  self.select()", 
+0009fb50: 5f61 7574 6f66 6f63 7573 3d54 7275 6529  _autofocus=True)
+0009fb60: 202c 5f73 7479 6c65 3d22 7061 6464 696e   ,_style="paddin
+0009fb70: 673a 3470 7820 3022 290a 2020 2020 2020  g:4px 0").      
+0009fb80: 2020 2020 2020 662b 3d42 7574 746f 6e28        f+=Button(
+0009fb90: 224f 6b22 2029 0a20 2020 2020 2020 2020  "Ok" ).         
+0009fba0: 2020 2066 2b3d 4275 7474 6f6e 2822 4361     f+=Button("Ca
+0009fbb0: 6e63 656c 222c 5f74 7970 653d 2262 7574  ncel",_type="but
+0009fbc0: 746f 6e22 2c5f 6f6e 636c 6963 6b3d 6d65  ton",_onclick=me
+0009fbd0: 7461 7461 672e 7374 6570 6576 656e 7428  tatag.stepevent(
+0009fbe0: 2929 0a20 2020 2020 2020 204d 6f64 616c  )).        Modal
+0009fbf0: 416c 6572 742e 5f5f 696e 6974 5f5f 2873  Alert.__init__(s
+0009fc00: 656c 662c 6d65 7461 7461 672c 6629 0a20  elf,metatag,f). 
+0009fc10: 2020 2020 2020 200a 636c 6173 7320 4472         .class Dr
+0009fc20: 6177 6572 2854 6167 2e64 6976 293a 0a20  awer(Tag.div):. 
+0009fc30: 2020 2064 6566 2069 6e69 7428 7365 6c66     def init(self
+0009fc40: 2c6d 6574 6174 6167 2c6f 626a 2c6d 6f64  ,metatag,obj,mod
+0009fc50: 653a 7374 7229 3a0a 2020 2020 2020 2020  e:str):.        
+0009fc60: 7369 7a65 3d35 300a 2020 2020 2020 2020  size=50.        
+0009fc70: 6966 206d 6f64 653d 3d22 6c65 6674 223a  if mode=="left":
+0009fc80: 0a20 2020 2020 2020 2020 2020 2074 2c72  .            t,r
+0009fc90: 2c62 2c6c 3d20 2822 3070 7822 2c66 227b  ,b,l= ("0px",f"{
+0009fca0: 7369 7a65 7d25 222c 2230 7078 222c 2230  size}%","0px","0
+0009fcb0: 7078 2229 0a20 2020 2020 2020 2065 6c69  px").        eli
+0009fcc0: 6620 6d6f 6465 3d3d 2272 6967 6874 223a  f mode=="right":
+0009fcd0: 0a20 2020 2020 2020 2020 2020 2074 2c72  .            t,r
+0009fce0: 2c62 2c6c 3d20 2822 3070 7822 2c22 3070  ,b,l= ("0px","0p
+0009fcf0: 7822 2c22 3070 7822 2c66 227b 7369 7a65  x","0px",f"{size
+0009fd00: 7d25 2229 0a20 2020 2020 2020 2065 6c69  }%").        eli
+0009fd10: 6620 6d6f 6465 3d3d 2262 6f74 746f 6d22  f mode=="bottom"
+0009fd20: 3a0a 2020 2020 2020 2020 2020 2020 742c  :.            t,
+0009fd30: 722c 622c 6c3d 2866 227b 7369 7a65 7d25  r,b,l=(f"{size}%
+0009fd40: 222c 2230 7078 222c 2230 7078 222c 2230  ","0px","0px","0
+0009fd50: 7078 2229 0a20 2020 2020 2020 2065 6c69  px").        eli
+0009fd60: 6620 6d6f 6465 3d3d 2274 6f70 223a 0a20  f mode=="top":. 
+0009fd70: 2020 2020 2020 2020 2020 2074 2c72 2c62             t,r,b
+0009fd80: 2c6c 3d20 2822 3070 7822 2c22 3070 7822  ,l= ("0px","0px"
+0009fd90: 2c66 227b 7369 7a65 7d25 222c 2230 7078  ,f"{size}%","0px
+0009fda0: 2229 0a0a 2020 2020 2020 2020 7365 6c66  ")..        self
+0009fdb0: 203c 3d20 566f 696c 6528 5f6f 6e6d 6f75   <= Voile(_onmou
+0009fdc0: 7365 646f 776e 3d6d 6574 6174 6167 2e73  sedown=metatag.s
+0009fdd0: 7465 7065 7665 6e74 2829 290a 2020 2020  tepevent()).    
+0009fde0: 2020 2020 7365 6c66 203c 3d20 5461 672e      self <= Tag.
+0009fdf0: 6469 7628 206f 626a 202c 5f73 7479 6c65  div( obj ,_style
+0009fe00: 3d66 2270 6f73 6974 696f 6e3a 6669 7865  =f"position:fixe
+0009fe10: 643b 746f 703a 7b74 7d3b 626f 7474 6f6d  d;top:{t};bottom
+0009fe20: 3a7b 627d 3b6c 6566 743a 7b6c 7d3b 7269  :{b};left:{l};ri
+0009fe30: 6768 743a 7b72 7d3b 6261 636b 6772 6f75  ght:{r};backgrou
+0009fe40: 6e64 3a77 6869 7465 3b62 6f72 6465 722d  nd:white;border-
+0009fe50: 7261 6469 7573 3a30 7078 3b62 6f78 2d73  radius:0px;box-s
+0009fe60: 6861 646f 773a 2072 6762 6128 302c 2030  hadow: rgba(0, 0
+0009fe70: 2c20 302c 2030 2e33 3529 2030 7078 2035  , 0, 0.35) 0px 5
+0009fe80: 7078 2031 3570 783b 3b7a 2d69 6e64 6578  px 15px;;z-index
+0009fe90: 3a31 3030 313b 7061 6464 696e 673a 3130  :1001;padding:10
+0009fea0: 7078 2229 0a0a 636c 6173 7320 506f 7028  px")..class Pop(
+0009feb0: 5461 672e 6469 7629 3a0a 2020 2020 6465  Tag.div):.    de
+0009fec0: 6620 696e 6974 2873 656c 662c 6d65 7461  f init(self,meta
+0009fed0: 7461 672c 6f62 6a2c 7879 3a74 7570 6c65  tag,obj,xy:tuple
+0009fee0: 293a 0a20 2020 2020 2020 2078 2c79 3d78  ):.        x,y=x
+0009fef0: 790a 2020 2020 2020 2020 7365 6c66 203c  y.        self <
+0009ff00: 3d20 566f 696c 6554 7261 6e73 7061 7265  = VoileTranspare
+0009ff10: 6e74 285f 6f6e 6d6f 7573 6564 6f77 6e3d  nt(_onmousedown=
+0009ff20: 6d65 7461 7461 672e 6269 6e64 2e70 6f70  metatag.bind.pop
+0009ff30: 636c 6f73 6528 292c 5f6f 6e63 6f6e 7465  close(),_onconte
+0009ff40: 7874 6d65 6e75 3d22 6576 656e 742e 7374  xtmenu="event.st
+0009ff50: 6f70 5072 6f70 6167 6174 696f 6e28 293b  opPropagation();
+0009ff60: 7265 7475 726e 2066 616c 7365 2229 0a20  return false"). 
+0009ff70: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0009ff80: 6a73 3d22 2222 2866 756e 6374 696f 6e28  js="""(function(
+0009ff90: 7461 672c 782c 7929 207b 0a20 2020 2020  tag,x,y) {.     
+0009ffa0: 2020 2020 2020 2074 6167 2e73 7479 6c65         tag.style
+0009ffb0: 3d22 706f 7369 7469 6f6e 3a66 6978 6564  ="position:fixed
+0009ffc0: 3b7a 2d69 6e64 6578 3a32 3030 313b 7061  ;z-index:2001;pa
+0009ffd0: 6464 696e 673a 3270 783b 6c65 6674 3a22  dding:2px;left:"
+0009ffe0: 2b78 2b22 7078 3b74 6f70 3a22 2b79 2b22  +x+"px;top:"+y+"
+0009fff0: 7078 223b 0a20 2020 2020 2020 2020 2020  px";.           
+000a0000: 206c 6574 2062 773d 7769 6e64 6f77 2e69   let bw=window.i
+000a0010: 6e6e 6572 5769 6474 683b 0a20 2020 2020  nnerWidth;.     
+000a0020: 2020 2020 2020 206c 6574 2062 683d 7769         let bh=wi
+000a0030: 6e64 6f77 2e69 6e6e 6572 4865 6967 6874  ndow.innerHeight
+000a0040: 3b0a 2020 2020 2020 2020 2020 2020 6c65  ;.            le
+000a0050: 7420 773d 7461 672e 636c 6965 6e74 5769  t w=tag.clientWi
+000a0060: 6474 683b 0a20 2020 2020 2020 2020 2020  dth;.           
+000a0070: 206c 6574 2068 3d74 6167 2e63 6c69 656e   let h=tag.clien
+000a0080: 7448 6569 6768 743b 0a20 2020 2020 2020  tHeight;.       
+000a0090: 2020 2020 2069 6628 782b 7720 3e20 6277       if(x+w > bw
+000a00a0: 2920 783d 6277 2d77 3b0a 2020 2020 2020  ) x=bw-w;.      
+000a00b0: 2020 2020 2020 6966 2879 2b68 203e 2062        if(y+h > b
+000a00c0: 6829 2079 3d62 682d 683b 0a20 2020 2020  h) y=bh-h;.     
+000a00d0: 2020 2020 2020 2074 6167 2e73 7479 6c65         tag.style
+000a00e0: 3d22 706f 7369 7469 6f6e 3a66 6978 6564  ="position:fixed
+000a00f0: 3b7a 2d69 6e64 6578 3a32 3030 313b 7061  ;z-index:2001;pa
+000a0100: 6464 696e 673a 3270 783b 6c65 6674 3a22  dding:2px;left:"
+000a0110: 2b78 2b22 7078 3b74 6f70 3a22 2b79 2b22  +x+"px;top:"+y+"
+000a0120: 7078 223b 0a20 2020 2020 2020 207d 2928  px";.        })(
+000a0130: 7365 6c66 2c25 732c 2573 2922 2222 2025  self,%s,%s)""" %
+000a0140: 2028 782c 7929 0a0a 2020 2020 2020 2020   (x,y)..        
+000a0150: 7365 6c66 203c 3d20 5461 672e 6469 7628  self <= Tag.div(
+000a0160: 206f 626a 202c 6a73 3d6a 7329 0a63 6c61   obj ,js=js).cla
+000a0170: 7373 2054 6f61 7374 2854 6167 2e64 6976  ss Toast(Tag.div
+000a0180: 293a 0a20 2020 2064 6566 2069 6e69 7428  ):.    def init(
+000a0190: 7365 6c66 2c6d 6169 6e5f 6e6f 6e5f 7573  self,main_non_us
+000a01a0: 6564 2c6f 626a 2c74 696d 656f 7574 3d31  ed,obj,timeout=1
+000a01b0: 3030 3029 3a0a 2020 2020 2020 2020 7365  000):.        se
+000a01c0: 6c66 203c 3d20 5461 672e 6469 7628 6f62  lf <= Tag.div(ob
+000a01d0: 6a2c 5f73 7479 6c65 3d22 706f 7369 7469  j,_style="positi
+000a01e0: 6f6e 3a66 6978 6564 3b72 6967 6874 3a31  on:fixed;right:1
+000a01f0: 3070 783b 626f 7474 6f6d 3a31 3070 783b  0px;bottom:10px;
+000a0200: 7a2d 696e 6465 783a 3130 3031 3b22 2c20  z-index:1001;", 
+000a0210: 5f63 6c61 7373 3d22 6e6f 7469 6669 6361  _class="notifica
+000a0220: 7469 6f6e 2069 732d 6c69 6e6b 2069 732d  tion is-link is-
+000a0230: 6c69 6768 7422 290a 2020 2020 2020 2020  light").        
+000a0240: 7365 6c66 2e6a 733d 2273 6574 5469 6d65  self.js="setTime
+000a0250: 6f75 7428 2066 756e 6374 696f 6e28 2920  out( function() 
+000a0260: 7b73 656c 662e 7265 6d6f 7665 2829 7d20  {self.remove()} 
+000a0270: 2c20 2573 2922 2025 2074 696d 656f 7574  , %s)" % timeout
+000a0280: 0a0a 2323 2323 2323 2323 2323 2323 2323  ..##############
 000a0290: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000a02a0: 2323 2323 2323 2323 0a0a 636c 6173 7320  ########..class 
-000a02b0: 5461 6273 2854 6167 2e64 6976 293a 0a20  Tabs(Tag.div):. 
-000a02c0: 2020 2064 6566 2069 6e69 7428 7365 6c66     def init(self
-000a02d0: 2c6d 6574 6174 6167 2c73 656c 6563 7465  ,metatag,selecte
-000a02e0: 643d 3029 3a0a 2020 2020 2020 2020 756c  d=0):.        ul
-000a02f0: 203d 2054 6167 2e75 6c28 290a 2020 2020   = Tag.ul().    
-000a0300: 2020 2020 666f 7220 6964 782c 6920 696e      for idx,i in
-000a0310: 2065 6e75 6d65 7261 7465 286d 6574 6174   enumerate(metat
-000a0320: 6167 2e5f 7461 6273 293a 0a20 2020 2020  ag._tabs):.     
-000a0330: 2020 2020 2020 206e 616d 6520 3d20 6861         name = ha
-000a0340: 7361 7474 7228 692c 226e 616d 6522 2920  sattr(i,"name") 
-000a0350: 616e 6420 692e 6e61 6d65 206f 7220 223f  and i.name or "?
-000a0360: 286e 616d 6529 3f22 0a20 2020 2020 2020  (name)?".       
-000a0370: 2020 2020 2075 6c2b 3d54 6167 2e6c 6928       ul+=Tag.li(
-000a0380: 2054 6167 2e61 286e 616d 6529 2c20 5f6f   Tag.a(name), _o
-000a0390: 6e63 6c69 636b 203d 206d 6574 6174 6167  nclick = metatag
-000a03a0: 2e73 7465 7065 7665 6e74 2873 656c 6563  .stepevent(selec
-000a03b0: 743d 6964 7829 2c20 5f63 6c61 7373 3d22  t=idx), _class="
-000a03c0: 6973 2d61 6374 6976 6522 2069 6620 6964  is-active" if id
-000a03d0: 783d 3d73 656c 6563 7465 6420 656c 7365  x==selected else
-000a03e0: 2022 2229 0a20 2020 2020 2020 2073 656c   "").        sel
-000a03f0: 663c 3d54 6167 2e64 6976 2875 6c2c 5f63  f<=Tag.div(ul,_c
-000a0400: 6c61 7373 3d22 7461 6273 2229 0a20 2020  lass="tabs").   
-000a0410: 2020 2020 2069 6620 6d65 7461 7461 672e       if metatag.
-000a0420: 5f74 6162 733a 2073 656c 663c 3d6d 6574  _tabs: self<=met
-000a0430: 6174 6167 2e5f 7461 6273 5b73 656c 6563  atag._tabs[selec
-000a0440: 7465 645d 0a                             ted].
+000a02a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000a02b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000a02c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000a02d0: 2323 2323 2323 2323 0a0a 636c 6173 7320  ########..class 
+000a02e0: 5461 6273 2854 6167 2e64 6976 293a 0a20  Tabs(Tag.div):. 
+000a02f0: 2020 2064 6566 2069 6e69 7428 7365 6c66     def init(self
+000a0300: 2c6d 6574 6174 6167 2c73 656c 6563 7465  ,metatag,selecte
+000a0310: 643d 3029 3a0a 2020 2020 2020 2020 756c  d=0):.        ul
+000a0320: 203d 2054 6167 2e75 6c28 290a 2020 2020   = Tag.ul().    
+000a0330: 2020 2020 666f 7220 6964 782c 6920 696e      for idx,i in
+000a0340: 2065 6e75 6d65 7261 7465 286d 6574 6174   enumerate(metat
+000a0350: 6167 2e5f 7461 6273 293a 0a20 2020 2020  ag._tabs):.     
+000a0360: 2020 2020 2020 206e 616d 6520 3d20 6861         name = ha
+000a0370: 7361 7474 7228 692c 226e 616d 6522 2920  sattr(i,"name") 
+000a0380: 616e 6420 692e 6e61 6d65 206f 7220 223f  and i.name or "?
+000a0390: 286e 616d 6529 3f22 0a20 2020 2020 2020  (name)?".       
+000a03a0: 2020 2020 2075 6c2b 3d54 6167 2e6c 6928       ul+=Tag.li(
+000a03b0: 2054 6167 2e61 286e 616d 6529 2c20 5f6f   Tag.a(name), _o
+000a03c0: 6e63 6c69 636b 203d 206d 6574 6174 6167  nclick = metatag
+000a03d0: 2e73 7465 7065 7665 6e74 2873 656c 6563  .stepevent(selec
+000a03e0: 743d 6964 7829 2c20 5f63 6c61 7373 3d22  t=idx), _class="
+000a03f0: 6973 2d61 6374 6976 6522 2069 6620 6964  is-active" if id
+000a0400: 783d 3d73 656c 6563 7465 6420 656c 7365  x==selected else
+000a0410: 2022 2229 0a20 2020 2020 2020 2073 656c   "").        sel
+000a0420: 663c 3d54 6167 2e64 6976 2875 6c2c 5f63  f<=Tag.div(ul,_c
+000a0430: 6c61 7373 3d22 7461 6273 2229 0a20 2020  lass="tabs").   
+000a0440: 2020 2020 2069 6620 6d65 7461 7461 672e       if metatag.
+000a0450: 5f74 6162 733a 2073 656c 663c 3d6d 6574  _tabs: self<=met
+000a0460: 6174 6167 2e5f 7461 6273 5b73 656c 6563  atag._tabs[selec
+000a0470: 7465 645d 0a                             ted].
```

### Comparing `htagui-0.5.5/htagui/common.py` & `htagui-0.5.6/htagui/common.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.5/htagui/dialog.py` & `htagui-0.5.6/htagui/dialog.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.5/htagui/flex.py` & `htagui-0.5.6/htagui/flex.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.5/htagui/form.py` & `htagui-0.5.6/htagui/form.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.5/htagui/ifields.py` & `htagui-0.5.6/htagui/ifields.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.5/htagui/md/__init__.py` & `htagui-0.5.6/htagui/md/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.5/htagui/md/bases.py` & `htagui-0.5.6/htagui/md/bases.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     statics=STATICS
     def init(self,title,**a):
         self <= Tag.md_ripple() + title
         self["style"].set("margin","1px")
 
 class Spinner(Tag.md_circular_progress):
     statics=STATICS
-    def init(self):
+    def init(self,**a):
         self["indeterminate"]=True
 
 class Input(Tag.input):
     statics= STATICS
     def init(self,*a,**k):
         type=self.attrs.get("type")
         if type is None or type=="text":
```

### Comparing `htagui-0.5.5/htagui/shoelace/__init__.py` & `htagui-0.5.6/htagui/shoelace/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.5/htagui/shoelace/bases.py` & `htagui-0.5.6/htagui/shoelace/bases.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         autoclosemenu( self.parent )
         return list(self._entries.values())[int(idx)]()
 
 
 
 class Spinner(Tag.sl_spinner):
     statics=STATICS
-    def init(self):
+    def init(self,**a):
         self["style"]="font-size: 32px; --track-width: 8px;"
 
 
 class Select(Tag.sl_select):
     statics=STATICS
     def init(self,options:ListOrDict, **a):
         options = ensuredict(options)
@@ -167,18 +167,14 @@
             self <= obj
             self.js += "self.addEventListener( 'sl-request-close', function(ev) { ev.preventDefault() });"
 
     def close(self,ev=None):
         self.call( "try{self.hide()}catch(e){}")    # the self.hide crash in some cases ?!?
 
 
-class ModalBox(ModalAlert):
-    def __init__(self,metatag,obj,size:float=.6):
-        ModalAlert.__init__(self,metatag,obj,pwidth=f"{size*100}%")
-
 class ModalBlock(ModalAlert):
     def __init__(self,metatag,obj):
         ModalAlert.__init__(self,metatag,obj,closable=False)
 
 class ModalConfirm(ModalAlert):
     def __init__(self,metatag,obj,cb):
         def call(ev):
```

### Comparing `htagui-0.5.5/htagui/splitters.py` & `htagui-0.5.6/htagui/splitters.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.5/htagui/tabs.py` & `htagui-0.5.6/htagui/tabs.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.5/pyproject.toml` & `htagui-0.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagui"
-version = "0.5.5" # auto-updated
+version = "0.5.6" # auto-updated
 description = "GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','gui', 'electron', "cef", "asyncio", "guy", "desktop", "web", "mobile", "http", "websocket", "html", "pyscript"]
 homepage = "https://github.com/manatlan/htagui"
 repository = "https://github.com/manatlan/htagui"
```

### Comparing `htagui-0.5.5/PKG-INFO` & `htagui-0.5.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagui
-Version: 0.5.5
+Version: 0.5.6
 Summary: GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase
 Home-page: https://github.com/manatlan/htagui
 License: MIT
 Keywords: htag,gui,electron,cef,asyncio,guy,desktop,web,mobile,http,websocket,html,pyscript
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -190,14 +190,27 @@
 ux = ui.Dialog( self )
 form = ui.Form( onsubmit=lambda dico: ux.notify(str(dico)) )
 form <= ui.Input(_name="mystring",_placeholder="input something")
 form <= ui.Button("ok")
 self <= form
 ```
 
+## Object FileUpload
+
+A simple surcharge of Tag.input( _type='file'...) which call a method to upload the selected file.
+
+```python
+import htagui as ui
+
+def uploaded(name:str, content:bytes):
+    print(name,content)
+
+self <= ui.FileUpload( uploaded , _multiple=True)
+```
+
 ## Object Tabs
 
 An htag class to easily create tabs structure. And provides somes attributs/methods to interact with it.
 
 ```python
 import htagui as ui
 tab1 = Tag.div("content1",name="tab1") # tab object needs a `name` property !
```

