# Comparing `tmp/espy_contact-0.9.tar.gz` & `tmp/espy_contact-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espy_contact-0.9.tar", last modified: Mon May  6 02:35:40 2024, max compression
+gzip compressed data, was "espy_contact-2.0.0.tar", last modified: Fri May 24 06:42:12 2024, max compression
```

## Comparing `espy_contact-0.9.tar` & `espy_contact-2.0.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 02:35:40.628529 espy_contact-0.9/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-0.9/LICENSE
--rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-05-06 02:35:40.628401 espy_contact-0.9/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-05-05 21:34:51.000000 espy_contact-0.9/README.md
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 02:35:40.621308 espy_contact-0.9/espy_contact/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.9/espy_contact/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 02:35:40.623600 espy_contact-0.9/espy_contact/model/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-0.9/espy_contact/model/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     9835 2024-04-28 04:32:29.000000 espy_contact-0.9/espy_contact/model/campus.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      558 2024-04-28 03:38:46.000000 espy_contact-0.9/espy_contact/model/messaging.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2616 2024-05-04 04:42:58.000000 espy_contact-0.9/espy_contact/model/models.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2870 2024-05-06 02:29:42.000000 espy_contact-0.9/espy_contact/model/reach.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1821 2024-04-28 03:38:03.000000 espy_contact-0.9/espy_contact/model/tranx.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 02:35:40.625909 espy_contact-0.9/espy_contact/schema/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 05:18:23.000000 espy_contact-0.9/espy_contact/schema/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2200 2024-04-28 03:20:57.000000 espy_contact-0.9/espy_contact/schema/campus.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      295 2024-04-28 00:12:40.000000 espy_contact-0.9/espy_contact/schema/messaging.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     5759 2024-04-28 03:39:29.000000 espy_contact-0.9/espy_contact/schema/mgcampus.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      984 2024-05-05 22:52:13.000000 espy_contact-0.9/espy_contact/schema/reach.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3204 2024-04-28 03:14:05.000000 espy_contact-0.9/espy_contact/schema/schema.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      932 2024-04-28 03:35:00.000000 espy_contact-0.9/espy_contact/schema/tranx.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 02:35:40.626334 espy_contact-0.9/espy_contact/service/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-28 00:08:44.000000 espy_contact-0.9/espy_contact/service/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-0.9/espy_contact/service/service.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 02:35:40.627440 espy_contact-0.9/espy_contact/util/
--rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-0.9/espy_contact/util/CONSTANTS.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-0.9/espy_contact/util/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      184 2024-04-28 03:04:46.000000 espy_contact-0.9/espy_contact/util/db.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3797 2024-05-04 04:43:43.000000 espy_contact-0.9/espy_contact/util/enums.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     4356 2024-05-04 17:13:08.000000 espy_contact-0.9/espy_contact/util/pg.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 02:35:40.621894 espy_contact-0.9/espy_contact.egg-info/
--rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-05-06 02:35:40.000000 espy_contact-0.9/espy_contact.egg-info/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      887 2024-05-06 02:35:40.000000 espy_contact-0.9/espy_contact.egg-info/SOURCES.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-06 02:35:40.000000 espy_contact-0.9/espy_contact.egg-info/dependency_links.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       76 2024-05-06 02:35:40.000000 espy_contact-0.9/espy_contact.egg-info/requires.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-05-06 02:35:40.000000 espy_contact-0.9/espy_contact.egg-info/top_level.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-06 02:35:40.628576 espy_contact-0.9/setup.cfg
--rw-r--r--   0 philipadigun   (501) staff       (20)      655 2024-05-06 02:35:35.000000 espy_contact-0.9/setup.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 02:35:40.628239 espy_contact-0.9/tests/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.9/tests/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-0.9/tests/test_copyright.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.9/tests/test_service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:42:12.124818 espy_contact-2.0.0/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-2.0.0/LICENSE
+-rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-24 06:42:12.124540 espy_contact-2.0.0/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-05-05 21:34:51.000000 espy_contact-2.0.0/README.md
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:42:12.115104 espy_contact-2.0.0/espy_contact/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.0/espy_contact/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:42:12.117613 espy_contact-2.0.0/espy_contact/model/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-2.0.0/espy_contact/model/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      558 2024-04-28 03:38:46.000000 espy_contact-2.0.0/espy_contact/model/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2692 2024-05-24 06:00:52.000000 espy_contact-2.0.0/espy_contact/model/models.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3622 2024-05-07 01:04:59.000000 espy_contact-2.0.0/espy_contact/model/reach.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1821 2024-04-28 03:38:03.000000 espy_contact-2.0.0/espy_contact/model/tranx.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:42:12.120658 espy_contact-2.0.0/espy_contact/schema/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 05:18:23.000000 espy_contact-2.0.0/espy_contact/schema/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1170 2024-05-18 16:51:45.000000 espy_contact-2.0.0/espy_contact/schema/blog.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2967 2024-05-24 06:12:34.000000 espy_contact-2.0.0/espy_contact/schema/campus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      295 2024-04-28 00:12:40.000000 espy_contact-2.0.0/espy_contact/schema/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     5759 2024-04-28 03:39:29.000000 espy_contact-2.0.0/espy_contact/schema/mgcampus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1741 2024-05-09 02:58:06.000000 espy_contact-2.0.0/espy_contact/schema/reach.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3395 2024-05-24 05:51:09.000000 espy_contact-2.0.0/espy_contact/schema/schema.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      932 2024-04-28 03:35:00.000000 espy_contact-2.0.0/espy_contact/schema/tranx.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:42:12.121123 espy_contact-2.0.0/espy_contact/service/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-28 00:08:44.000000 espy_contact-2.0.0/espy_contact/service/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-2.0.0/espy_contact/service/service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:42:12.123290 espy_contact-2.0.0/espy_contact/util/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-2.0.0/espy_contact/util/CONSTANTS.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-2.0.0/espy_contact/util/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1055 2024-05-12 03:28:55.000000 espy_contact-2.0.0/espy_contact/util/db.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3989 2024-05-23 21:32:05.000000 espy_contact-2.0.0/espy_contact/util/enums.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      113 2024-05-20 14:38:12.000000 espy_contact-2.0.0/espy_contact/util/esread.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     4353 2024-05-24 05:29:17.000000 espy_contact-2.0.0/espy_contact/util/pg.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:42:12.115742 espy_contact-2.0.0/espy_contact.egg-info/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      350 2024-05-24 06:42:12.000000 espy_contact-2.0.0/espy_contact.egg-info/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      914 2024-05-24 06:42:12.000000 espy_contact-2.0.0/espy_contact.egg-info/SOURCES.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-24 06:42:12.000000 espy_contact-2.0.0/espy_contact.egg-info/dependency_links.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       77 2024-05-24 06:42:12.000000 espy_contact-2.0.0/espy_contact.egg-info/requires.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-05-24 06:42:12.000000 espy_contact-2.0.0/espy_contact.egg-info/top_level.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-24 06:42:12.124929 espy_contact-2.0.0/setup.cfg
+-rw-r--r--   0 philipadigun   (501) staff       (20)      659 2024-05-24 06:40:00.000000 espy_contact-2.0.0/setup.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-24 06:42:12.124258 espy_contact-2.0.0/tests/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.0/tests/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-2.0.0/tests/test_copyright.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-2.0.0/tests/test_service.py
```

### Comparing `espy_contact-0.9/LICENSE` & `espy_contact-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `espy_contact-0.9/espy_contact/model/messaging.py` & `espy_contact-2.0.0/espy_contact/model/messaging.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.9/espy_contact/model/models.py` & `espy_contact-2.0.0/espy_contact/model/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,50 +11,52 @@
 """
 import uuid
 from sqlalchemy import Column, DateTime, ForeignKey, Enum
 from sqlalchemy.sql import func
 from sqlalchemy.sql.sqltypes import Integer,String,Boolean
 from sqlalchemy.dialects.postgresql import ARRAY
 from sqlalchemy.orm import relationship
-from espy_contact.util.enums import AccessRoleEnum,StatusEnum
+from espy_contact.util.enums import AccessRoleEnum,StatusEnum,GenderEnum
 from espy_contact.util.db import Base
 
 class Webbuilder(Base):
     __tablename__ = "webbuilder"
-    id = Column(String, primary_key=True, index=True)
+    id = Column(Integer, primary_key=True, index=True, autoincrement=True)
     content = Column(String)
     product_id = Column(Integer)
     is_live = Column(Boolean, default=False)
     timestamp = Column(DateTime(), server_default=func.now())
 
 class Address(Base):
     __tablename__ = "addresses"
-    id = Column(String, primary_key=True, index=True, default=lambda: str(uuid.uuid4()))
+    id = Column(Integer, primary_key=True, index=True, autoincrement=True)
     street = Column(String)
     city = Column(String)
     state = Column(String)
     zip_code = Column(Integer)
     email = Column(String)
     phone_number = Column(String)
     country = Column(String)
 
 
 class Appuser(Base):
     __tablename__ = "appusers"
-    id = Column(String, primary_key=True, index=True, default=lambda: str(uuid.uuid4()))
+    id = Column(Integer, primary_key=True, index=True, autoincrement=True)
     timestamp = Column(DateTime(), server_default=func.now())
     first_name = Column(String)
     last_name = Column(String)
     country = Column(String)
     email = Column(String, nullable=False, unique=True)
     password = Column(String)
     token = Column(String)
     dp = Column(String)
     is_active = Column(Boolean)
     roles = Column(ARRAY(Enum(AccessRoleEnum)))
     status = Column(Enum(StatusEnum))
+    gender = Column(Enum(GenderEnum))
+    socialmedia = Column(String)
     address_id = Column(
-        String, ForeignKey("addresses.id"), nullable=True
+        Integer, ForeignKey("addresses.id"), nullable=True
     )  # Add foreign key
     address = relationship(
         "Address", uselist=False, backref="user"
     )  # One-to-one relationship
```

### Comparing `espy_contact-0.9/espy_contact/model/tranx.py` & `espy_contact-2.0.0/espy_contact/model/tranx.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.9/espy_contact/schema/mgcampus.py` & `espy_contact-2.0.0/espy_contact/schema/mgcampus.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.9/espy_contact/schema/schema.py` & `espy_contact-2.0.0/espy_contact/schema/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 office@myeverlasting.net
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 """
 from datetime import datetime, date
 from pydantic import BaseModel, EmailStr,Field
-from espy_contact.util.enums import AccessRoleEnum, StatusEnum
+from espy_contact.util.enums import AccessRoleEnum, StatusEnum,GenderEnum
 from typing import List, Optional, Union
 import uuid
 class ReachBase(BaseModel):
     id: str
     timestamp: datetime
 class SeoRequest(BaseModel):
     url: str = Field(min_length=4, description="Your website url")
@@ -28,29 +28,31 @@
     id: Optional[Union[str, int]] = str(uuid.uuid4())
     timestamp: Optional[datetime] = None
     first_name: str
     last_name: str
     email: EmailStr
     is_active: bool = False
     status: StatusEnum = StatusEnum.NEW
-    role: List[AccessRoleEnum]
+    roles: List[AccessRoleEnum]
+    socialmedia: Optional[str] = None # comma separated string
+    gender: Optional[GenderEnum]
 class AddressDto(BaseModel):
     id: Optional[str] = None
     street: str
     city: str
     state: str
     zip_code: int
     email: Optional[EmailStr] = None
     phone_number: Optional[str] = None
     country: str
 
 
 class AppuserDto(UserResponse):
     password: str
-    address: AddressDto
+    address: Optional[AddressDto] = None
 
     class Config:
         from_attributes = True
 
 
 class EnrollmentDto(UserResponse):
     dob: date
@@ -100,8 +102,12 @@
     grade_level: str
     reason_for_leaving: str
     classroom: str  # ForeignKey to Classroom or String
     owner: AppuserDto  # ForeignKey to StudentProfile or None
 
     # teacher: Teacher  # Optional ForeignKey to Teacher (null allowed) or None
     class Config:
-        from_attributes = True
+        from_attributes = True
+
+class GenDto(BaseModel):
+    start_date: date
+    end_date: date
```

### Comparing `espy_contact-0.9/espy_contact/schema/tranx.py` & `espy_contact-2.0.0/espy_contact/schema/tranx.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.9/espy_contact/service/service.py` & `espy_contact-2.0.0/espy_contact/service/service.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.9/espy_contact/util/CONSTANTS.py` & `espy_contact-2.0.0/espy_contact/util/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.9/espy_contact/util/enums.py` & `espy_contact-2.0.0/espy_contact/util/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,7 +104,15 @@
     STERLING_BANK = "Sterling Bank"
     SUNTRUST_BANK_NIGERIA = "Suntrust Bank Nigeria"
     UNION_BANK_OF_NIGERIA = "Union Bank of Nigeria"
     UNITED_BANK_FOR_AFRICA = "United Bank for Africa"
     UNITY_BANK_PLC = "Unity Bank Plc"
     WEMA_BANK = "Wema Bank"
     ZENITH_BANK = "Zenith Bank"
+class Appname(enum.Enum):
+    aefinance= 'aefinance'
+    essl='essl'
+    harmonypflege='harmonypflege'
+class GenderEnum(enum.Enum):
+    MALE = "Male"
+    FEMALE = "Female"
+    OTHER = "Other"
```

### Comparing `espy_contact-0.9/espy_contact/util/pg.py` & `espy_contact-2.0.0/espy_contact/util/pg.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 """
 from typing import Type
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.orm import Session
 
-def add_model(model_class: Type, db: Session, **kwargs) -> bool:
+def add_model(model_class: Type, db: Session, **kwargs):
     """
     Persist a SQLAlchemy model to the database.
 
     Args:
     - model_class (Type): The SQLAlchemy model class to be persisted.
     - db (Session): The database session to use for persistence.
     - **kwargs: Keyword arguments to pass to the model constructor.
@@ -29,15 +29,15 @@
     - IntegrityError: If the model cannot be persisted due to an integrity error.
     """
     try:
         new_model = model_class(**kwargs)
         db.add(new_model)
         db.commit()
         db.refresh(new_model)
-        return True
+        return new_model
     except IntegrityError:
         db.rollback()
         return False
 def update_model(model_class: Type, db: Session, id: int, **kwargs) -> bool:
     """
     Update a SQLAlchemy model in the database.
```

### Comparing `espy_contact-0.9/espy_contact.egg-info/SOURCES.txt` & `espy_contact-2.0.0/espy_contact.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 espy_contact/__init__.py
 espy_contact.egg-info/PKG-INFO
 espy_contact.egg-info/SOURCES.txt
 espy_contact.egg-info/dependency_links.txt
 espy_contact.egg-info/requires.txt
 espy_contact.egg-info/top_level.txt
 espy_contact/model/__init__.py
-espy_contact/model/campus.py
 espy_contact/model/messaging.py
 espy_contact/model/models.py
 espy_contact/model/reach.py
 espy_contact/model/tranx.py
 espy_contact/schema/__init__.py
+espy_contact/schema/blog.py
 espy_contact/schema/campus.py
 espy_contact/schema/messaging.py
 espy_contact/schema/mgcampus.py
 espy_contact/schema/reach.py
 espy_contact/schema/schema.py
 espy_contact/schema/tranx.py
 espy_contact/service/__init__.py
 espy_contact/service/service.py
 espy_contact/util/CONSTANTS.py
 espy_contact/util/__init__.py
 espy_contact/util/db.py
 espy_contact/util/enums.py
+espy_contact/util/esread.py
 espy_contact/util/pg.py
 tests/__init__.py
 tests/test_copyright.py
 tests/test_service.py
```

### Comparing `espy_contact-0.9/setup.py` & `espy_contact-2.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.4'
 DESCRIPTION = 'ESSL users management'
 LONG_DESCRIPTION = 'Internal helper package for ESSL users management'
 setup(
     name='espy_contact',
-    version='0.9',
+    version='2.0.0',
     packages=find_packages(),
     install_requires=[
         'bcrypt==4.1.2',
         'pytest==8.1.1',
         'pydantic==2.7.1',
         'sqlalchemy==2.0.29',
-        'bson==0.5.10'
+        'PyYAML ==6.0.1'
         ],
     author='Femi Adigun',
     author_email='femi.adigun@myeverlasting.net',
     description=DESCRIPTION,
     long_description_content_type='text/markdown',
     long_description=LONG_DESCRIPTION,
     keywords=['fastapi','ESSL','ReachAI']
```

### Comparing `espy_contact-0.9/tests/test_copyright.py` & `espy_contact-2.0.0/tests/test_copyright.py`

 * *Files identical despite different names*

