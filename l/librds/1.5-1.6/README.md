# Comparing `tmp/librds-1.5.tar.gz` & `tmp/librds-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librds-1.5.tar", last modified: Fri May 31 18:09:31 2024, max compression
+gzip compressed data, was "librds-1.6.tar", last modified: Sat Jun  1 20:31:47 2024, max compression
```

## Comparing `librds-1.5.tar` & `librds-1.6.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:09:31.897402 librds-1.5/
--rw-rw-rw-   0 root         (0) root         (0)    35187 2024-05-27 16:08:02.000000 librds-1.5/LICENCE
--rw-r--r--   0 root         (0) root         (0)     1834 2024-05-31 18:09:31.893402 librds-1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1177 2024-05-31 18:08:31.000000 librds-1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:09:31.889402 librds-1.5/librds/
--rw-rw-rw-   0 root         (0) root         (0)      292 2024-05-31 18:08:31.000000 librds-1.5/librds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3279 2024-05-27 16:08:02.000000 librds-1.5/librds/af.py
--rw-rw-rw-   0 root         (0) root         (0)    17334 2024-05-27 16:08:02.000000 librds-1.5/librds/charset.py
--rw-rw-rw-   0 root         (0) root         (0)     2035 2024-05-29 14:26:04.000000 librds-1.5/librds/comfort.py
--rw-rw-rw-   0 root         (0) root         (0)     3877 2024-05-31 18:08:31.000000 librds-1.5/librds/decoder.py
--rw-rw-rw-   0 root         (0) root         (0)    10886 2024-05-31 18:08:31.000000 librds-1.5/librds/generator.py
--rw-rw-rw-   0 root         (0) root         (0)      417 2024-05-27 16:08:02.000000 librds-1.5/librds/group.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-31 08:09:13.000000 librds-1.5/librds/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:09:31.893402 librds-1.5/librds.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1834 2024-05-31 18:09:31.000000 librds-1.5/librds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      364 2024-05-31 18:09:31.000000 librds-1.5/librds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 18:09:31.000000 librds-1.5/librds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-31 18:09:31.000000 librds-1.5/librds.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 18:09:31.897402 librds-1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      999 2024-05-31 18:08:31.000000 librds-1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:09:31.893402 librds-1.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4796 2024-05-28 16:54:30.000000 librds-1.5/tests/test_decoder.py
--rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-31 18:08:31.000000 librds-1.5/tests/test_groupsequencer.py
--rw-rw-rw-   0 root         (0) root         (0)      787 2024-05-31 08:09:13.000000 librds-1.5/tests/test_interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 20:31:47.744026 librds-1.6/
+-rw-rw-rw-   0 root         (0) root         (0)    35187 2024-05-27 16:08:02.000000 librds-1.6/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     1791 2024-06-01 20:31:47.744026 librds-1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1134 2024-06-01 19:53:29.000000 librds-1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 20:31:47.740026 librds-1.6/librds/
+-rw-rw-rw-   0 root         (0) root         (0)      332 2024-06-01 19:53:29.000000 librds-1.6/librds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3279 2024-05-27 16:08:02.000000 librds-1.6/librds/af.py
+-rw-rw-rw-   0 root         (0) root         (0)    17334 2024-05-27 16:08:02.000000 librds-1.6/librds/charset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3235 2024-06-01 19:53:29.000000 librds-1.6/librds/comfort.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-06-01 19:53:29.000000 librds-1.6/librds/datatypes.py
+-rw-rw-rw-   0 root         (0) root         (0)     6226 2024-06-01 19:53:29.000000 librds-1.6/librds/decoder.py
+-rw-rw-rw-   0 root         (0) root         (0)    12466 2024-06-01 19:53:29.000000 librds-1.6/librds/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-31 08:09:13.000000 librds-1.6/librds/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 20:31:47.744026 librds-1.6/librds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1791 2024-06-01 20:31:47.000000 librds-1.6/librds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      346 2024-06-01 20:31:47.000000 librds-1.6/librds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 20:31:47.000000 librds-1.6/librds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-06-01 20:31:47.000000 librds-1.6/librds.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-01 20:31:47.744026 librds-1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      999 2024-06-01 19:53:29.000000 librds-1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 20:31:47.744026 librds-1.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-31 18:08:31.000000 librds-1.6/tests/test_groupsequencer.py
+-rw-rw-rw-   0 root         (0) root         (0)      787 2024-05-31 08:09:13.000000 librds-1.6/tests/test_interfaces.py
```

### Comparing `librds-1.5/LICENCE` & `librds-1.6/LICENCE`

 * *Files identical despite different names*

### Comparing `librds-1.5/PKG-INFO` & `librds-1.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librds
-Version: 1.5
+Version: 1.6
 Summary: RDS Group Generator
 Home-page: https://flerken.zapto.org:1115/kuba/librds
 Author: kuba201
 Project-URL: Source, https://flerken.zapto.org:1115/kuba/librds
 Keywords: radiodatasystem,rds,broadcast_fm
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Telecommunications Industry
@@ -36,8 +36,8 @@
     Group(a=12288, b=0, c=0, d=0, is_version_b=None)
     Group(a=12288, b=8, c=57549, d=26729, is_version_b=False)
 ```
 
 **Note** that LibRDS required Python 3.10+ to run due to its use of `match` in the character set which is required for PS, RT, PTYN and also match is used in AF
 
 # Decoder
-LibRDS also includes a simple RDS Group decoder, so you can encode with librds and then also decode it, currently librds's decoder decodes most of the stuff it can encode (without support for tdc, in_house, ct but rest are decoded okay)
+LibRDS also includes a RDS Group decoder, so you can encode with librds and then also decode it, currently librds's decoder decodes all of the groups it can encode (such as CT, IH, TDC, etc...)
```

### Comparing `librds-1.5/README.md` & `librds-1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     Group(a=12288, b=0, c=0, d=0, is_version_b=None)
     Group(a=12288, b=8, c=57549, d=26729, is_version_b=False)
 ```
 
 **Note** that LibRDS required Python 3.10+ to run due to its use of `match` in the character set which is required for PS, RT, PTYN and also match is used in AF
 
 # Decoder
-LibRDS also includes a simple RDS Group decoder, so you can encode with librds and then also decode it, currently librds's decoder decodes most of the stuff it can encode (without support for tdc, in_house, ct but rest are decoded okay)
+LibRDS also includes a RDS Group decoder, so you can encode with librds and then also decode it, currently librds's decoder decodes all of the groups it can encode (such as CT, IH, TDC, etc...)
```

### Comparing `librds-1.5/librds/af.py` & `librds-1.6/librds/af.py`

 * *Files identical despite different names*

### Comparing `librds-1.5/librds/charset.py` & `librds-1.6/librds/charset.py`

 * *Files identical despite different names*

### Comparing `librds-1.5/librds/comfort.py` & `librds-1.6/librds/comfort.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,40 @@
 def get_from_list(input:list,index:int,default=None):
     """This is a simple function to remove index errors from the group generators"""
     try:
         return input[index]
     except IndexError:
         return default
 
+def SubstituteCharacterAtPosition(string:str, char:str, index:int):
+    """
+    This is a helper function that works like 'string[index] = char' in c
+    
+    :param string: String to process
+    :param char: The character thats going to be at that position
+    :param index: Index of the character
+    """
+    if not isinstance(string, str) or not isinstance(char,str) or not isinstance(index,int): raise Exception
+    if not (0 <= index < len(string)):
+        raise IndexError("Index out of range")
+    return string[:index] + char + string[index + 1:]
+
+class BitProcessor:
+    def set_bit(value:int, bit:int, bit_value:bool, max_number:int=16) -> int:
+        string = ("0"*(max_number-(value.bit_count())))
+        string += bin(value).removeprefix("-").removeprefix("0b")
+        if bit > len(string): raise IndexError
+        string = SubstituteCharacterAtPosition(string,("1" if bit_value else "0"),bit)
+        return int(("0b"+string),2)
+    def get_bit(value:int, bit:int, max_number:int=16) -> int:
+        string = ("0"*(max_number-(value.bit_length())))
+        string += bin(value).removeprefix("-").removeprefix("0b")
+        # return string
+        return int(("0b"+string[bit]),2)
+
 def calculate_mjd(year: int, month: int, day:int):
     """Year: e.x 2024
     Month: (starts from 0) 0 - Jan, 1 - Feb ...
     Day - (starts from 1)"""
     l = 1 if (month == 0 or month == 1) else 0
     return (
         14956 + day +
```

### Comparing `librds-1.5/librds/generator.py` & `librds-1.6/librds/generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,22 @@
-from .group import Group
-from .comfort import get_from_list
+from .datatypes import Group, GroupIdentifier
+from .comfort import get_from_list,BitProcessor
 from .af import AlternativeFrequency
 from .charset import RDSCharset
 class SegmentError(Exception): pass
 class GroupGeneratorError(Exception): pass
 
+def get_group(group:int, ab:bool=False,details:bool=False):
+    group = ((group << 4) | int(ab))
+    if not details: 
+        return (((group >> 4) & 15) << 12) | (0x800 if ab else 0)
+    else:
+        return ((group >> 4) & 15), int(ab)
+
+
 class GroupGenerator:
     def basic(pi:int, tp:bool=False, pty:int=0):
         """
         This function will generate a basic block structure which includes the PI, TP and PTY, this shouldn't be sent by itself to a decoder
         
         :param pi: The PI code, should be a 16 bit integer (for example 0x3000), pi codes are country dependent (especially for ECC), see Standart EN50067 page 70 (first byte, so 3 in 0x3555), also see page 72 for coverage code
         :param tp: Traffic Program
@@ -27,14 +35,16 @@
         :param blocks: Basic block structure, which is generated by basic()
         :param ps_text: PS Text
         :param segment: Current segment to generate (ps is segmented into four 2 character segments)
         :param ms: Music/Speech (music is True)
         :param ta: Trafic Annoucement
         :param di: Decoder Identificaton
         :param block2: Block C, you can use this to send AF
+
+        Decoder status: Decoded
         """
         if segment > 3: raise SegmentError("Segment limit")
         return Group(
             blocks.a & 0xFFFF,
             ( blocks.b | int(ta) << 4 | int(ms) << 3 | ( ( di >> (3-segment) ) << 2) | segment ) & 0xFFFF,
             (int(block2) & 0xFFFF) or AlternativeFrequency.get_no_af(),
             (RDSCharset.translate(get_from_list(ps_text,segment*2," "))<<8 | RDSCharset.translate(get_from_list(ps_text,segment*2+1," "))) & 0xFFFF, #low byte + high byte as we're using utf-8, and we conver 2 8 bit numbers to a single 16 bit one
@@ -45,110 +55,124 @@
         
         :param blocks: Basic block structure, which is generated by basic()
         :param ps_text: PS Text
         :param segment: Current segment to generate (ps is segmented into four 2 character segments)
         :param ms: Music/Speech (music is True)
         :param ta: Trafic Annoucement
         :param di: Decoder Identificaton
+
+        Decoder status: Decoded
         """
         if segment > 3: raise SegmentError("Segment limit")
         return Group(
             blocks.a & 0xFFFF,
-            ( blocks.b | int(ta) << 4 | int(ms) << 3 | ( ( di >> (3-segment) ) << 2) | segment ) & 0xFFFF,
+            ( blocks.b | get_group(0,True) | int(ta) << 4 | int(ms) << 3 | ( ( di >> (3-segment) ) << 2) | segment ) & 0xFFFF,
             blocks.a & 0xFFFF,
             (RDSCharset.translate(get_from_list(ps_text,segment*2," "))<<8 | RDSCharset.translate(get_from_list(ps_text,segment*2+1," "))) & 0xFFFF,
             True
         )
     def ecc(blocks:Group, ecc: int):
         """This function will generate a 1A group, with the ECC value
         
         :param blocks: Basic block structure, which is generated by basic()
         :param ecc: The ECC code itself, see EN50067 page 71
+
+        Decoder status: Decoded
         """
         return Group(
             blocks.a & 0xFFFF,
-            (blocks.b | 1 << 12) & 0xFFFF,
+            (blocks.b | get_group(1)) & 0xFFFF,
             (blocks.c | ecc) & 0xFFFF,
             blocks.d & 0xFFFF,
             False
         )
     def lic(blocks:Group, lic: int):
         """This function will generate a 1A group, very similiar to ECC
         
         :param blocks: Basic block structure, which is generated by basic()
         :param lic: The LIC code itself, see EN50067 page 84-85
+
+        Decoder status: Decoded
         """
         return Group(
             blocks.a & 0xFFFF,
-            (blocks.b | 1 << 12) & 0xFFFF,
+            (blocks.b | get_group(1)) & 0xFFFF,
             (blocks.c | (lic | 0x3000)) & 0xFFFF,
             blocks.d & 0xFFFF,
             False
         )
     def rt(blocks:Group,rt_text:str,segment:int,ab:bool=False):
         """This function will generate a 2A group, which includes AB the segment and 4 characters of text
         
         :param blocks: Basic block structure, which is generated by basic()
         :param rt_text: RT Text
         :param segment: Current segment to generate (2a is segmented into 16 4 character segments)
         :param ab: Switch this if RT changes
+
+        Decoder status: Decoded
         """
         if segment > 15: raise SegmentError("Segment limit")
         return Group(
             blocks.a & 0xFFFF,
-            (blocks.b | 2 << 12 | int(ab) << 4 | segment) & 0xFFFF,
+            (blocks.b | get_group(2) | int(ab) << 4 | segment) & 0xFFFF,
             (RDSCharset.translate(get_from_list(rt_text,segment*4+0," "))<<8 | RDSCharset.translate(get_from_list(rt_text,segment*4+1," "))) & 0xFFFF,
             (RDSCharset.translate(get_from_list(rt_text,segment*4+2," "))<<8 | RDSCharset.translate(get_from_list(rt_text,segment*4+3," "))) & 0xFFFF,
             False
         )
     def rt_b(blocks:Group,rt_text:str,segment:int,ab:bool=False):
         """This function will generate a 2B group, very similiar to 2A but this include only 2 characters of text
         
         :param blocks: Basic block structure, which is generated by basic()
         :param rt_text: RT Text
         :param segment: Current segment to generate (2b is segmented into 16 2 character segments)
         :param ab: Switch this if RT changes
+
+        Decoder status: Decoded
         """
         if segment > 15: raise SegmentError("Segment limit")
         return Group(
             blocks.a & 0xFFFF,
-            (0x0800 | blocks.a | 2 << 12 | int(ab) << 4 | segment) & 0xFFFF,
+            (blocks.b | get_group(2,True) | int(ab) << 4 | segment) & 0xFFFF,
             blocks.a & 0xFFFF,
             (RDSCharset.translate(get_from_list(rt_text,segment*4+0," "))<<8 | RDSCharset.translate(get_from_list(rt_text,segment*4+1," "))) & 0xFFFF,
             True
         )
     def ptyn(blocks:Group, ptyn_text:str, segment:int,ab:bool=False):
         """This function will generate a 10A group, which includes 4 characters of text
         
         :param blocks: Basic block structure, which is generated by basic()
         :param ptyn_text: PTYN Text
         :param segment: Current segment to generate (2b is segmented into 2 2 character segments)
         :param ab: Switch this if PTYN changes
+
+        Decoder status: Decoded
         """
         if segment > 1: raise SegmentError("Segment limit")
         return Group(
             blocks.a & 0xFFFF,
-            (blocks.b | 10 << 12 | (int(ab) << 4) | segment) & 0xFFFF,
+            (blocks.b | get_group(10) | (int(ab) << 4) | segment) & 0xFFFF,
             (RDSCharset.translate(get_from_list(ptyn_text,segment*4+0," "))<<8 | RDSCharset.translate(get_from_list(ptyn_text,segment*4+1," "))) & 0xFFFF,
             (RDSCharset.translate(get_from_list(ptyn_text,segment*4+2," "))<<8 | RDSCharset.translate(get_from_list(ptyn_text,segment*4+3," "))) & 0xFFFF,
             False
         )
     def ct(basic:Group, mjd: int, hour: int, minute: int, local_hour:int=None,local_minute:int=None):
         """This function generates a 4A group
         
         :param blocks: Basic block structure, which is generated by basic()
         :param mjd: The Modified Julian Day value, calculated with calculate_mjd
         :param hour: UTC Hour
         :param minute: UTC Minute
         :param local_hour: Local Hour
         :param local_minute: Local Minute
+
+        Decoder status: Decoded
         """
         group = Group(
             basic.a & 0xFFFF,
-            (basic.b | 4 << 12 | (mjd>>15)) & 0xffff,
+            (basic.b | get_group(4) | (mjd>>15)) & 0xffff,
             ((mjd<<1) | (hour >> 4)) & 0xffff,
             ((hour & 0xF)<<12 | minute << 6) & 0xffff,
             False
         )
         if local_hour and local_minute:
             offset_h = local_hour - hour
             if offset_h < 0: group.d |= (1 << 5)
@@ -163,64 +187,92 @@
             offset = int((0 + (offset_h * 60)) / 30)
             group.d |= abs(offset)
         elif local_minute:
             offset_m = local_minute - minute
             offset = int((offset_m + (0 * 60)) / 30)
             group.d |= abs(offset)
         return group
-    def tda(blocks:Group, channel:int,data:list[int],segment:int):
+    def tdc(blocks:Group, channel:int,data:list[int],segment:int):
         """This function will generate a 5A group
         
         :param blocks: Basic block structure, which is generated by basic()
-        :param channnel: TDA channel< this should stay static, shoudn't be 31 ot more (32 but it starts from 0 so 31)
-        :param data: TDA Data, should be a list of ints
-        :param segment: Segment of the TDA message
+        :param channnel: TDC channel< this should stay static, shoudn't be 31 ot more (32 but it starts from 0 so 31)
+        :param data: TDC Data, should be a list of ints
+        :param segment: Segment of the TDC message
+
+        Decoder status: Decoded
         """
-        if channel > 31: raise GroupGeneratorError("Channel bigger than 32")
+        if channel > 31: raise GroupGeneratorError("Channel bigger than 31")
         return Group(
             blocks.a & 0xFFFF,
-            (blocks.b | 5 << 12 | (channel & 0x001F)) & 0xFFFF,
+            (blocks.b | get_group(5) | (channel & 0x001F)) & 0xFFFF,
             (get_from_list(data,segment+0,0)<<8 | get_from_list(data,segment+1,0)) & 0xFFFF,
             (get_from_list(data,segment+2,0)<<8 | get_from_list(data,segment+3,0)) & 0xFFFF,
             False
         )
-    def tda_b(blocks:Group, channel:int,data:list[int],segment:int):
+    def tdc_b(blocks:Group, channel:int,data:list[int],segment:int):
         """This function will generate a 5B group
         
         :param blocks: Basic block structure, which is generated by basic()
-        :param channnel: TDA channel< this should stay static, shoudn't be 31 ot more (32 but it starts from 0 so 31)
-        :param data: TDA Data, should be a list of ints
-        :param segment: Segment of the TDA message
+        :param channnel: TDC channel< this should stay static, shoudn't be 31 ot more (32 but it starts from 0 so 31)
+        :param data: TDC Data, should be a list of ints
+        :param segment: Segment of the TDC message
+
+        Decoder status: Decoded
         """
+        if channel > 31: raise GroupGeneratorError("Channel bigger than 31")
         return Group(
             blocks.a & 0xFFFF,
-            (0x0800 | blocks.b | 5 << 12 | (channel & 0x001F)) & 0xFFFF,
+            (blocks.b | get_group(5,True) | (channel & 0x001F)) & 0xFFFF,
             blocks.a & 0xFFFF,
             (get_from_list(data,segment+0,0)<<8 | get_from_list(data,segment+1,0)) & 0xFFFF,
             True
         )
     def in_house(blocks:Group, data:list[int]):
         """This function will generate a 6A group
         
         :param blocks: Basic block structure, which is generated by basic()
         :data data: 3 byte long list of ints, but the 1st byte is not guarteed to be decoded so maybe but some unnessacy info here
+
+        Decoder status: Decoded
         """
         return Group(
             blocks.a & 0xFFFF,
-            (((blocks.b | 6 << 12) & ~0b11111) | (get_from_list(data,0,0) & 0b11111)) & 0xFFFF,
+            (((blocks.b | get_group(6)) & ~0b11111) | (get_from_list(data,0,0) & 0b11111)) & 0xFFFF,
             get_from_list(data,1,0) & 0xFFFF,
             get_from_list(data,2,0) & 0xFFFF,
             False
         )
     def in_house_b(blocks:Group, data:list[int]):
         """This function will generate a 6B group
         
         :param blocks: Basic block structure, which is generated by basic()
         :data data: 2 byte long list of ints
+
+        Decoder status: Decoded
         """
         return Group(
             blocks.a & 0xFFFF,
-            (((0x0800 | blocks.b | 6 << 12) & ~0b11111) | (get_from_list(data,0,0) & 0b11111)) & 0xFFFF,
+            (((blocks.b | get_group(6,True)) & ~0b11111) | (get_from_list(data,0,0) & 0b11111)) & 0xFFFF,
             blocks.a & 0xFFFF,
             get_from_list(data,1,0) & 0xFFFF,
             True
         )
+    def oda_aid(blocks:Group, group: GroupIdentifier, aid:int, scb:int=0):
+        """This function will generate a 3A group
+        
+        :param blocks: Basic block structure, which is generated by basic()
+        :data group: The type of group this AID is for
+        :data aid: AID
+        :data scb: 'Message bits'
+
+        Decoder status: Decoded
+        """
+        if not isinstance(group, GroupIdentifier): raise GroupGeneratorError("group should be a GroupIdentifier")
+        group_type, group_ver = get_group(group.group_number,group.group_version,True)
+        return Group(
+            blocks.a & 0xFFFF,
+            (blocks.b | 3 << 12 | (group_type << 1) | group_ver) & 0xFFFF,
+            scb & 0xFFFF,
+            aid & 0xFFFF,
+            False
+        )
```

### Comparing `librds-1.5/librds/interface.py` & `librds-1.6/librds/interface.py`

 * *Files identical despite different names*

### Comparing `librds-1.5/librds.egg-info/PKG-INFO` & `librds-1.6/librds.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librds
-Version: 1.5
+Version: 1.6
 Summary: RDS Group Generator
 Home-page: https://flerken.zapto.org:1115/kuba/librds
 Author: kuba201
 Project-URL: Source, https://flerken.zapto.org:1115/kuba/librds
 Keywords: radiodatasystem,rds,broadcast_fm
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Telecommunications Industry
@@ -36,8 +36,8 @@
     Group(a=12288, b=0, c=0, d=0, is_version_b=None)
     Group(a=12288, b=8, c=57549, d=26729, is_version_b=False)
 ```
 
 **Note** that LibRDS required Python 3.10+ to run due to its use of `match` in the character set which is required for PS, RT, PTYN and also match is used in AF
 
 # Decoder
-LibRDS also includes a simple RDS Group decoder, so you can encode with librds and then also decode it, currently librds's decoder decodes most of the stuff it can encode (without support for tdc, in_house, ct but rest are decoded okay)
+LibRDS also includes a RDS Group decoder, so you can encode with librds and then also decode it, currently librds's decoder decodes all of the groups it can encode (such as CT, IH, TDC, etc...)
```

### Comparing `librds-1.5/setup.py` & `librds-1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
         name="librds", 
-        version="1.5",
+        version="1.6",
         author="kuba201",
         description='RDS Group Generator',
         long_description=readme,
         long_description_content_type='text/markdown',
         packages=find_packages(),
         url="https://flerken.zapto.org:1115/kuba/librds",
         install_requires=[],
```

### Comparing `librds-1.5/tests/test_interfaces.py` & `librds-1.6/tests/test_interfaces.py`

 * *Files identical despite different names*

