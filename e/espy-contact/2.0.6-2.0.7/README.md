# Comparing `tmp/espy_contact-2.0.6.tar.gz` & `tmp/espy_contact-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espy_contact-2.0.6.tar", last modified: Sat May 25 23:18:19 2024, max compression
+gzip compressed data, was "espy_contact-2.0.7.tar", last modified: Sat Jun  1 06:41:16 2024, max compression
```

## Comparing `espy_contact-2.0.6.tar` & `espy_contact-2.0.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 23:18:19.703013 espy_contact-2.0.6/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-2.0.6/LICENSE
--rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-25 23:18:19.702876 espy_contact-2.0.6/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-05-05 21:34:51.000000 espy_contact-2.0.6/README.md
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 23:18:19.694408 espy_contact-2.0.6/espy_contact/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.6/espy_contact/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 23:18:19.696627 espy_contact-2.0.6/espy_contact/model/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-2.0.6/espy_contact/model/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      558 2024-04-28 03:38:46.000000 espy_contact-2.0.6/espy_contact/model/messaging.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2692 2024-05-24 06:00:52.000000 espy_contact-2.0.6/espy_contact/model/models.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3622 2024-05-07 01:04:59.000000 espy_contact-2.0.6/espy_contact/model/reach.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1920 2024-05-24 06:56:06.000000 espy_contact-2.0.6/espy_contact/model/tranx.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 23:18:19.699916 espy_contact-2.0.6/espy_contact/schema/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 05:18:23.000000 espy_contact-2.0.6/espy_contact/schema/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1170 2024-05-18 16:51:45.000000 espy_contact-2.0.6/espy_contact/schema/blog.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2918 2024-05-24 06:48:35.000000 espy_contact-2.0.6/espy_contact/schema/campus.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-25 17:11:06.000000 espy_contact-2.0.6/espy_contact/schema/messaging.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     5759 2024-04-28 03:39:29.000000 espy_contact-2.0.6/espy_contact/schema/mgcampus.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1782 2024-05-25 22:24:50.000000 espy_contact-2.0.6/espy_contact/schema/reach.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3773 2024-05-25 23:17:03.000000 espy_contact-2.0.6/espy_contact/schema/schema.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      932 2024-04-28 03:35:00.000000 espy_contact-2.0.6/espy_contact/schema/tranx.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 23:18:19.700340 espy_contact-2.0.6/espy_contact/service/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-28 00:08:44.000000 espy_contact-2.0.6/espy_contact/service/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-2.0.6/espy_contact/service/service.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 23:18:19.701934 espy_contact-2.0.6/espy_contact/util/
--rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-2.0.6/espy_contact/util/CONSTANTS.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-2.0.6/espy_contact/util/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1055 2024-05-12 03:28:55.000000 espy_contact-2.0.6/espy_contact/util/db.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3989 2024-05-23 21:32:05.000000 espy_contact-2.0.6/espy_contact/util/enums.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      113 2024-05-20 14:38:12.000000 espy_contact-2.0.6/espy_contact/util/esread.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     4353 2024-05-24 05:29:17.000000 espy_contact-2.0.6/espy_contact/util/pg.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 23:18:19.695182 espy_contact-2.0.6/espy_contact.egg-info/
--rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-25 23:18:19.000000 espy_contact-2.0.6/espy_contact.egg-info/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      914 2024-05-25 23:18:19.000000 espy_contact-2.0.6/espy_contact.egg-info/SOURCES.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-25 23:18:19.000000 espy_contact-2.0.6/espy_contact.egg-info/dependency_links.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       77 2024-05-25 23:18:19.000000 espy_contact-2.0.6/espy_contact.egg-info/requires.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-05-25 23:18:19.000000 espy_contact-2.0.6/espy_contact.egg-info/top_level.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-25 23:18:19.703071 espy_contact-2.0.6/setup.cfg
--rw-r--r--   0 philipadigun   (501) staff       (20)      659 2024-05-25 23:18:14.000000 espy_contact-2.0.6/setup.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-25 23:18:19.702678 espy_contact-2.0.6/tests/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.6/tests/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-2.0.6/tests/test_copyright.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.6/tests/test_service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 06:41:16.790409 espy_contact-2.0.7/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-2.0.7/LICENSE
+-rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-06-01 06:41:16.790255 espy_contact-2.0.7/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-05-05 21:34:51.000000 espy_contact-2.0.7/README.md
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 06:41:16.781935 espy_contact-2.0.7/espy_contact/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.7/espy_contact/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 06:41:16.783734 espy_contact-2.0.7/espy_contact/model/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-2.0.7/espy_contact/model/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      558 2024-04-28 03:38:46.000000 espy_contact-2.0.7/espy_contact/model/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2692 2024-05-24 06:00:52.000000 espy_contact-2.0.7/espy_contact/model/models.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3622 2024-05-07 01:04:59.000000 espy_contact-2.0.7/espy_contact/model/reach.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2024 2024-06-01 05:26:10.000000 espy_contact-2.0.7/espy_contact/model/tranx.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 06:41:16.787066 espy_contact-2.0.7/espy_contact/schema/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 05:18:23.000000 espy_contact-2.0.7/espy_contact/schema/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1170 2024-05-18 16:51:45.000000 espy_contact-2.0.7/espy_contact/schema/blog.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2918 2024-05-24 06:48:35.000000 espy_contact-2.0.7/espy_contact/schema/campus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-25 17:11:06.000000 espy_contact-2.0.7/espy_contact/schema/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     5759 2024-04-28 03:39:29.000000 espy_contact-2.0.7/espy_contact/schema/mgcampus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1782 2024-05-25 22:24:50.000000 espy_contact-2.0.7/espy_contact/schema/reach.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3773 2024-05-25 23:17:03.000000 espy_contact-2.0.7/espy_contact/schema/schema.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1005 2024-06-01 06:39:37.000000 espy_contact-2.0.7/espy_contact/schema/tranx.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 06:41:16.787485 espy_contact-2.0.7/espy_contact/service/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-28 00:08:44.000000 espy_contact-2.0.7/espy_contact/service/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-2.0.7/espy_contact/service/service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 06:41:16.789159 espy_contact-2.0.7/espy_contact/util/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-2.0.7/espy_contact/util/CONSTANTS.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-2.0.7/espy_contact/util/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1055 2024-05-12 03:28:55.000000 espy_contact-2.0.7/espy_contact/util/db.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     4013 2024-06-01 06:38:48.000000 espy_contact-2.0.7/espy_contact/util/enums.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      113 2024-05-20 14:38:12.000000 espy_contact-2.0.7/espy_contact/util/esread.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     4353 2024-05-24 05:29:17.000000 espy_contact-2.0.7/espy_contact/util/pg.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 06:41:16.782512 espy_contact-2.0.7/espy_contact.egg-info/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-06-01 06:41:16.000000 espy_contact-2.0.7/espy_contact.egg-info/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      914 2024-06-01 06:41:16.000000 espy_contact-2.0.7/espy_contact.egg-info/SOURCES.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-06-01 06:41:16.000000 espy_contact-2.0.7/espy_contact.egg-info/dependency_links.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       77 2024-06-01 06:41:16.000000 espy_contact-2.0.7/espy_contact.egg-info/requires.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-06-01 06:41:16.000000 espy_contact-2.0.7/espy_contact.egg-info/top_level.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-06-01 06:41:16.790464 espy_contact-2.0.7/setup.cfg
+-rw-r--r--   0 philipadigun   (501) staff       (20)      659 2024-06-01 06:40:26.000000 espy_contact-2.0.7/setup.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 06:41:16.790069 espy_contact-2.0.7/tests/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.7/tests/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-2.0.7/tests/test_copyright.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.7/tests/test_service.py
```

### Comparing `espy_contact-2.0.6/LICENSE` & `espy_contact-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.6/espy_contact/model/messaging.py` & `espy_contact-2.0.7/espy_contact/model/messaging.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.6/espy_contact/model/models.py` & `espy_contact-2.0.7/espy_contact/model/models.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.6/espy_contact/model/reach.py` & `espy_contact-2.0.7/espy_contact/model/reach.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.6/espy_contact/model/tranx.py` & `espy_contact-2.0.7/espy_contact/model/tranx.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     amount = Column(Integer, nullable=False)
     currency = Column(String, nullable=False)
     status = Column(String, nullable=False)
     payee_id = Column(Integer, ForeignKey("appusers.id"))
     detail = Column(Text)  # Text allows for larger details if needed
     createdOn = Column(DateTime, default=datetime)
     modifiedOn = Column(DateTime, onupdate=datetime)
+    raw_json = Column(Text)  # This can be used to store the raw json response from the payment gateway
 
     payee = relationship("Appuser", backref="transactions")
 
 
 class Account(Base):
     __tablename__ = "accounts"
```

### Comparing `espy_contact-2.0.6/espy_contact/schema/blog.py` & `espy_contact-2.0.7/espy_contact/schema/blog.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.6/espy_contact/schema/campus.py` & `espy_contact-2.0.7/espy_contact/schema/campus.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.6/espy_contact/schema/mgcampus.py` & `espy_contact-2.0.7/espy_contact/schema/mgcampus.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.6/espy_contact/schema/reach.py` & `espy_contact-2.0.7/espy_contact/schema/reach.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.6/espy_contact/schema/schema.py` & `espy_contact-2.0.7/espy_contact/schema/schema.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.6/espy_contact/schema/tranx.py` & `espy_contact-2.0.7/espy_contact/schema/tranx.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from pydantic import BaseModel
 from espy_contact.util.enums import StatusEnum, NigerianBank
 
 
 class TranxDto(BaseModel):
     id: Optional[int] = None
     ref: str
-    stripeId: str
+    stripeId: Optional[str] = None
     amount: float
-    currency: str
-    status: StatusEnum
-    payee_id: Optional[str]  # Assuming Appuser has an ID field
-    detail: Optional[Union[dict, str]]  # Can be dict or string for flexibility
+    currency: Optional[str] = "NGN"
+    status: Optional[StatusEnum] = StatusEnum.PENDING
+    payee_id: Optional[int]  # Assuming Appuser has an ID field
+    detail: Optional[Union[dict, str]] = None  # Can be dict or string for flexibility
     createdOn: Optional[datetime]
     modifiedOn: Optional[datetime]
 
 
 class AccountDto(BaseModel):
     id: Optional[int] = None
     bank: NigerianBank
```

### Comparing `espy_contact-2.0.6/espy_contact/service/service.py` & `espy_contact-2.0.7/espy_contact/service/service.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.6/espy_contact/util/CONSTANTS.py` & `espy_contact-2.0.7/espy_contact/util/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.6/espy_contact/util/db.py` & `espy_contact-2.0.7/espy_contact/util/db.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.6/espy_contact/util/enums.py` & `espy_contact-2.0.7/espy_contact/util/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     NEW = "New"
     ENROLLED = "Enrolled"
     ADMITTED = "Admitted"
     DEBTOR = "Debtor"
     DELETED = "Deleted"
     SUSPENDED = "Suspended"
     EXPELLED = "Expelled"
+    PENDING = "Pending"
 
 
 class NigerianBank(enum.Enum):
     ACCESS_BANK = "Access Bank"
     CITIBANK = "Citibank"
     DIAMOND_BANK = "Diamond Bank"
     ECOBANK_NIGERIA = "Ecobank Nigeria"
```

### Comparing `espy_contact-2.0.6/espy_contact/util/pg.py` & `espy_contact-2.0.7/espy_contact/util/pg.py`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.6/espy_contact.egg-info/SOURCES.txt` & `espy_contact-2.0.7/espy_contact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `espy_contact-2.0.6/setup.py` & `espy_contact-2.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 VERSION = '0.0.4'
 DESCRIPTION = 'ESSL users management'
 LONG_DESCRIPTION = 'Internal helper package for ESSL users management'
 setup(
     name='espy_contact',
-    version='2.0.6',
+    version='2.0.7',
     packages=find_packages(),
     install_requires=[
         'bcrypt==4.1.2',
         'pytest==8.1.1',
         'pydantic==2.7.1',
         'sqlalchemy==2.0.29',
         'PyYAML ==6.0.1'
```

### Comparing `espy_contact-2.0.6/tests/test_copyright.py` & `espy_contact-2.0.7/tests/test_copyright.py`

 * *Files identical despite different names*

