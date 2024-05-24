# Comparing `tmp/orinoco-1.0.9.tar.gz` & `tmp/orinoco-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orinoco-1.0.9.tar", max compression
+gzip compressed data, was "orinoco-2.0.0.tar", max compression
```

## Comparing `orinoco-1.0.9.tar` & `orinoco-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0       55 2022-12-13 10:13:01.119676 orinoco-1.0.9/orinoco/__init__.py
--rw-r--r--   0        0        0    23076 2023-03-30 12:00:15.135863 orinoco-1.0.9/orinoco/action.py
--rw-r--r--   0        0        0    19379 2023-03-28 13:34:21.396751 orinoco-1.0.9/orinoco/condition.py
--rw-r--r--   0        0        0     5167 2021-12-31 10:46:36.408869 orinoco-1.0.9/orinoco/data_source.py
--rw-r--r--   0        0        0    16877 2023-03-29 09:58:52.335343 orinoco-1.0.9/orinoco/entities.py
--rw-r--r--   0        0        0     3052 2021-12-31 10:46:36.409156 orinoco-1.0.9/orinoco/event.py
--rw-r--r--   0        0        0     1546 2023-03-30 11:15:19.669248 orinoco-1.0.9/orinoco/exceptions.py
--rw-r--r--   0        0        0     1208 2023-03-28 13:16:43.521363 orinoco-1.0.9/orinoco/helpers.py
--rw-r--r--   0        0        0    10528 2023-03-28 08:42:35.213261 orinoco-1.0.9/orinoco/loop.py
--rw-r--r--   0        0        0     2223 2021-12-31 10:46:36.409598 orinoco-1.0.9/orinoco/observers.py
--rw-r--r--   0        0        0        0 2021-12-31 10:46:36.409648 orinoco-1.0.9/orinoco/py.typed
--rw-r--r--   0        0        0     6589 2023-01-10 15:02:52.827250 orinoco-1.0.9/orinoco/retry.py
--rw-r--r--   0        0        0      252 2022-12-13 10:13:01.128251 orinoco-1.0.9/orinoco/settings.py
--rw-r--r--   0        0        0      157 2021-12-31 10:46:36.410027 orinoco-1.0.9/orinoco/tags.py
--rw-r--r--   0        0        0     3798 2023-03-28 11:55:42.999434 orinoco-1.0.9/orinoco/transformation.py
--rw-r--r--   0        0        0     9051 2023-03-29 09:56:30.787380 orinoco-1.0.9/orinoco/typed_action.py
--rw-r--r--   0        0        0     6037 2023-03-29 09:51:14.173388 orinoco-1.0.9/orinoco/types.py
--rw-r--r--   0        0        0      596 2023-03-29 10:13:16.969233 orinoco-1.0.9/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 orinoco-1.0.9/setup.py
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 orinoco-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0       55 2022-12-13 10:13:01.119676 orinoco-2.0.0/orinoco/__init__.py
+-rw-r--r--   0        0        0    20952 2024-05-24 13:21:54.289129 orinoco-2.0.0/orinoco/action.py
+-rw-r--r--   0        0        0    19369 2024-05-24 13:21:54.291002 orinoco-2.0.0/orinoco/condition.py
+-rw-r--r--   0        0        0     5167 2021-12-31 10:46:36.408869 orinoco-2.0.0/orinoco/data_source.py
+-rw-r--r--   0        0        0    16420 2024-05-24 13:21:54.293057 orinoco-2.0.0/orinoco/entities.py
+-rw-r--r--   0        0        0     3052 2021-12-31 10:46:36.409156 orinoco-2.0.0/orinoco/event.py
+-rw-r--r--   0        0        0     1303 2024-02-08 11:57:46.898940 orinoco-2.0.0/orinoco/exceptions.py
+-rw-r--r--   0        0        0     1198 2024-05-24 13:21:54.293821 orinoco-2.0.0/orinoco/helpers.py
+-rw-r--r--   0        0        0    10498 2024-05-24 13:21:54.296153 orinoco-2.0.0/orinoco/loop.py
+-rw-r--r--   0        0        0     2223 2021-12-31 10:46:36.409598 orinoco-2.0.0/orinoco/observers.py
+-rw-r--r--   0        0        0        0 2021-12-31 10:46:36.409648 orinoco-2.0.0/orinoco/py.typed
+-rw-r--r--   0        0        0     6597 2024-05-24 13:21:54.296505 orinoco-2.0.0/orinoco/retry.py
+-rw-r--r--   0        0        0      297 2024-05-24 13:21:54.300959 orinoco-2.0.0/orinoco/settings.py
+-rw-r--r--   0        0        0      157 2021-12-31 10:46:36.410027 orinoco-2.0.0/orinoco/tags.py
+-rw-r--r--   0        0        0     3798 2024-02-08 11:57:52.153567 orinoco-2.0.0/orinoco/transformation.py
+-rw-r--r--   0        0        0     9051 2024-02-08 11:57:52.154309 orinoco-2.0.0/orinoco/typed_action.py
+-rw-r--r--   0        0        0     6032 2024-05-24 13:21:54.303335 orinoco-2.0.0/orinoco/types.py
+-rw-r--r--   0        0        0      598 2024-05-24 13:21:54.303655 orinoco-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      626 1970-01-01 00:00:00.000000 orinoco-2.0.0/PKG-INFO
```

### Comparing `orinoco-1.0.9/orinoco/action.py` & `orinoco-2.0.0/orinoco/action.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,28 +14,21 @@
     AsyncContextManager,
     Tuple,
     NoReturn,
     Coroutine,
     List,
 )
 
-from pydantic import Extra, ValidationError, BaseModel
-
 from orinoco import config
 from orinoco.entities import ActionData, Signature
-from orinoco.exceptions import (
-    ActionNotProperlyConfigured,
-    BaseActionException,
-    ActionSetInputValidationMissingValueError,
-    ActionSetInputTypeValidationError,
-)
+from orinoco.exceptions import ActionNotProperlyConfigured, BaseActionException
 from orinoco.helpers import compose
 from orinoco.observers import ActionsLog
 from orinoco.tags import SystemActionTag
-from orinoco.types import ActionT, ActionDataT, NamespacedActionT, ActionVar
+from orinoco.types import ActionT, ActionDataT, NamespacedActionT, ActionVar, SignatureT
 
 
 class _NamespacedAction(NamespacedActionT):
     """
     Wrapper class named actions. See `Action.namespaced`
     """
 
@@ -330,49 +323,49 @@
         self.renamed_inputs = renamed_inputs or {}
         self.outputs = outputs or []
         self.renamed_outputs = renamed_outputs or {}
         super().__init__(name="GuardedActionSet[{}]".format(action_set.name), description=action_set.description)
 
     def run(self, action_data: ActionDataT) -> ActionDataT:
         return compose(
-            partial(self._remove_keys, desired_keys=self._input_keys),
+            partial(self._remove_keys, keys_to_keep=self._input_keys),
             partial(self._rename_keys, keys=self.renamed_inputs),
             self.action_set.run,
-            partial(self._remove_keys, desired_keys=self._output_keys),
+            partial(self._remove_keys, keys_to_keep=self._output_keys),
             partial(self._rename_keys, keys=self.renamed_outputs),
         )(action_data)
 
     def with_inputs(self, *keys: str, **renamed_keys: str) -> "GuardedActionSet":
         self.inputs = list(keys)
         self.renamed_inputs = renamed_keys
         return self
 
     def with_outputs(self, *keys: str, **renamed_keys: str) -> "GuardedActionSet":
         self.outputs = list(keys)
         self.renamed_outputs = renamed_keys
         return self
 
     @classmethod
-    def _remove_keys(cls, action_data: ActionDataT, desired_keys: List[str]) -> ActionDataT:
-        if not desired_keys:
+    def _remove_keys(cls, action_data: ActionDataT, keys_to_keep: List[str]) -> ActionDataT:
+        if not keys_to_keep:
             return action_data.evolve_self(data=tuple())
 
         return action_data.remove_many(
-            searched_signatures=cls._get_additive_signatures(action_data, desired_keys),
+            searched_signatures=cls._get_remaining_signatures(action_data, keys_to_keep),
             exact_match=False,
             ignore_non_existent=False,
         )
 
     def _rename_keys(self, action_data: ActionDataT, keys: Dict[str, str]) -> ActionDataT:
         for new_key, key in keys.items():
             action_data = action_data.rename(key, new_key)
         return action_data
 
     @staticmethod
-    def _get_additive_signatures(action_data: ActionDataT, keys: List[str]) -> List[Signature]:
+    def _get_remaining_signatures(action_data: ActionDataT, keys: List[str]) -> List[SignatureT]:
         return [signature for signature in action_data.signatures if signature.key not in keys]
 
     @property
     def _input_keys(self) -> List[str]:
         return self.inputs + list(self.renamed_inputs.values())
 
     @property
@@ -384,100 +377,42 @@
     """
     Set of actions which are executed consequently
     """
 
     ACTIONS: Optional[Iterable[ActionT]] = None
 
     def __init__(
-        self,
-        actions: Optional[Iterable[ActionT]] = None,
-        description: Optional[str] = None,
-        name: Optional[str] = None,
-        input_validation: Optional[Union[Type, Callable[[Any], None]]] = None,
+        self, actions: Optional[Iterable[ActionT]] = None, description: Optional[str] = None, name: Optional[str] = None
     ):
-        """
-        :input_validation: Dataclass/pydantic base model or callable which validates input data. It will be used for
-        validation of input data before action execution. Note that it needs to be able to handle extra kwargs.
-        """
         super().__init__(description=description, name=name)
         self.actions = actions or self.ACTIONS or []
-        self.input_validation = input_validation or self._construct_inner_input_dataclass()
 
     @record_action
     @verbose_action_exception
     def run(self, action_data: ActionDataT) -> ActionDataT:
-        self._validate_input(action_data)
-
         for action in self.actions:
             if action_data.skip_processing:
                 return action_data
 
             action_data = action.run(action_data)
         return action_data
 
     @async_record_action
     @async_verbose_action_exception
     async def async_run(self, action_data: ActionDataT) -> ActionDataT:
-        self._validate_input(action_data)
-
         for action in self.actions:
             if action_data.skip_processing:
                 return action_data
 
             action_data = await action.async_run(action_data)
         return action_data
 
     def as_guarded(self) -> GuardedActionSet:
         return GuardedActionSet(action_set=self)
 
-    def get_input_validation_cls(self) -> Optional[BaseModel]:
-        if isinstance(self.input_validation, BaseModel):
-            return self.input_validation
-
-    def as_atomic(self, atomic_context_manager) -> "AtomicActionSet":
-        return AtomicActionSet(
-            actions=self.actions,
-            description=self.description,
-            name=self.name,
-            atomic_context_manager=atomic_context_manager,
-        )
-
-    def as_async_atomic(self, atomic_context_manager) -> "AsyncAtomicActionSet":
-        return AsyncAtomicActionSet(
-            actions=self.actions,
-            description=self.description,
-            name=self.name,
-            atomic_context_manager=atomic_context_manager,
-        )
-
-    def _validate_input(self, action_data: ActionDataT) -> None:
-        if self.input_validation:
-            try:
-                self.input_validation(**action_data.as_keyed_dict())
-            except TypeError as err:
-                raise ActionSetInputValidationMissingValueError(
-                    f"Missing key in action data for action set {self.name}: {err}"
-                ) from err
-            except ValidationError as err:
-                raise ActionSetInputTypeValidationError(
-                    f"Type validation failed for action set {self.name}: {err}"
-                ) from err
-
-    @classmethod
-    def _construct_inner_input_dataclass(cls) -> Optional[Type[BaseModel]]:
-        if hasattr(cls, "Input"):
-            if issubclass(cls.Input, BaseModel):
-                return cls.Input
-
-            class Config:
-                extra = Extra.allow
-                arbitrary_types_allowed = True
-
-            return type("Input", (BaseModel,), {"Config": Config, "__annotations__": cls.Input.__annotations__})
-
 
 class AtomicActionSet(ActionSet, SystemActionTag):
     """
     Set of actions which are executed in a context manager
     """
 
     def __init__(
@@ -490,37 +425,47 @@
         super().__init__(actions=actions, description=description, name=name)
         self.atomic_context_manager = atomic_context_manager
 
     @record_action
     @verbose_action_exception
     def run(self, action_data: ActionDataT) -> ActionDataT:
         with self.atomic_context_manager():
-            return super().run(action_data)
+            for action in self.actions:
+                if action_data.skip_processing:
+                    return action_data
+
+                action_data = action.run(action_data)
+            return action_data
 
 
 class AsyncAtomicActionSet(ActionSet, SystemActionTag):
     """
     Async version of :class:`AtomicActionSet`.
     """
 
     def __init__(
         self,
+        actions: Iterable[ActionT],
         atomic_context_manager: Callable[[], AsyncContextManager[None]],
-        actions: Optional[Iterable[ActionT]] = None,
         description: Optional[str] = None,
         name: Optional[str] = None,
     ):
         super().__init__(actions=actions, description=description, name=name)
         self.atomic_context_manager = atomic_context_manager
 
     @async_record_action
     @async_verbose_action_exception
     async def async_run(self, action_data: ActionDataT) -> ActionDataT:
         async with self.atomic_context_manager():
-            return await super().async_run(action_data)
+            for action in self.actions:
+                if action_data.skip_processing:
+                    return action_data
+
+                action_data = await action.async_run(action_data)
+            return action_data
 
 
 class Then(ActionSet, SystemActionTag):
     """
     Syntactics sugar for :class:`ActionSet`. See :class:`~orinoco.condition.Switch` docs for usage
     """
```

### Comparing `orinoco-1.0.9/orinoco/condition.py` & `orinoco-2.0.0/orinoco/condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 class PropertyCondition(Condition):
     """
     Generic condition which evaluates property of an object in the dataset
     """
 
     PROPERTY_OBJECT: Optional[str] = None
     ATTRIBUTE: Optional[str] = None
-    EQUAL_TO: Optional[Any] = True
+    EQUAL_TO: Any = True
 
     SOMETHING: Any = object
 
     attribute: str
 
     def __init__(
         self,
```

### Comparing `orinoco-1.0.9/orinoco/data_source.py` & `orinoco-2.0.0/orinoco/data_source.py`

 * *Files identical despite different names*

### Comparing `orinoco-1.0.9/orinoco/entities.py` & `orinoco-2.0.0/orinoco/entities.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,19 @@
     ObserverVar,
     ImmutableEvolvableModelT,
 )
 
 
 class ImmutableEvolvableModel(ImmutableEvolvableModelT, abc.ABC):
     def evolve_self(self: BaseModelT, **kwargs: Any) -> BaseModelT:
-        return self.copy(update=kwargs)
+        return self.model_copy(update=kwargs)
 
 
-class Signature(Generic[T], ImmutableEvolvableModel, SignatureT[T]):
-    type_: Optional[Any] = None
+class Signature(ImmutableEvolvableModel, SignatureT[T], Generic[T]):
     tags: Set[str] = Field(default_factory=set)
-    key: Optional[str] = None
 
     def match(self, other_signature: "SignatureT[T]") -> bool:
         """
         Match with another signature. Note that matching with for ``tags`` set is done as "is subset"
         """
         if (
             other_signature.type_ is not None
@@ -44,43 +42,35 @@
         if len(other_signature.tags) > 0 and not other_signature.tags.issubset(self.tags):
             return False
 
         if other_signature.key is not None and other_signature.key != self.key:
             return False
         return True
 
-    def __class_getitem__(cls: T, _: Any) -> T:
-        # Fix for pydantic to support generic types (expressions like `SignatureT[bool]`)
-        return cls
-
 
 class SignatureWithDefaultValue(Signature[T]):
     default_value: T
 
 
-class ActionConfig(Generic[T], ImmutableEvolvableModel, ActionConfigT[T]):
-    INPUT: Optional[Dict[str, SignatureT[Any]]] = None
+class ActionConfig(ImmutableEvolvableModel, ActionConfigT[T], Generic[T]):
+    INPUT: Optional[Dict[str, SignatureT]] = None
     OUTPUT: Optional[SignatureT[T]] = None
 
     @classmethod
     def create_strict(
         cls,
-        input_: Optional[Dict[str, Type[Any]]] = None,
+        input_: Optional[Dict[str, Type]] = None,
         output_type: Optional[Type[T]] = None,
         output_name: Optional[str] = None,
     ) -> "ActionConfig[T]":
         return cls(
             INPUT=({name: Signature(type_=type_, key=name) for name, type_ in input_.items()}) if input_ else None,
             OUTPUT=Signature(type_=output_type, key=output_name),
         )
 
-    def __class_getitem__(cls: T, _: Any) -> T:
-        # Fix for pydantic to support generic types (expressions like `SignatureT[bool]`)
-        return cls
-
 
 class ActionData(ImmutableEvolvableModel, ActionDataT):
     """
     Fundamental data structure which is both input and output of actions.
 
     Virtual keys: To save a memory some data are not stored directly, but just a method how to get them from other
     data stored in `ActionData`.
@@ -90,16 +80,16 @@
 
     History of all actions done on the dataset are recorded in `ActionData.actions_done`.
     """
 
     NOT_FOUND: ClassVar = object()
     DEFAULT_OBSERVERS_CLASSES: ClassVar = (ExecutionTimeObserver, ActionsLog)
 
-    data: Tuple[Tuple[SignatureT[Any], Any], ...] = Field(default_factory=tuple)
-    futures: List[Awaitable[Any]] = Field(default_factory=list)
+    data: Tuple[Tuple[SignatureT, Any], ...] = Field(default_factory=tuple)
+    futures: List[Awaitable] = Field(default_factory=list)
     observers: List[ObserverT] = Field(default_factory=partial(initialize, DEFAULT_OBSERVERS_CLASSES))
 
     skip_processing: bool = False
 
     # Shortcuts
     def __getitem__(self, searched_signature: SignatureT[T]) -> T:
         return self.get_by_signature(searched_signature)
@@ -127,24 +117,24 @@
                 [(signature, entity) for signature, entity in self.data if signature == searched_signature]
             )
         except SearchError as err:
             raise SearchError(
                 "Failed to find {}\nPresent signatures: {}".format(searched_signature, self.signatures)
             ) from err
 
-    def get_or_default(self, key: str, default: Optional[Any] = None) -> Any:
+    def get_or_default(self, key: str, default: Any = None) -> Any:
         """
         Get data by key or return a default value
         """
         try:
             return self.get_by_signature(Signature(key=key))
         except (NothingFound, SearchError):
             return default
 
-    def find_or_default(self, key: str, default: Optional[Any] = None) -> Any:
+    def find_or_default(self, key: str, default: Any = None) -> Any:
         """
         Find a single value with matching or default
         """
         try:
             return self.find_one(Signature(key=key))
         except NothingFound:
             return default
@@ -225,15 +215,15 @@
 
         Already registered data with signatures with keys matching the new will be removed and replaced by the new ones
         """
         # TODO: Can be optimized
         existing = {}
         for key in data.keys():
             try:
-                signature: SignatureT[Any] = self._ensure_one(self.find_with_signature(Signature(key=key)))[0]
+                signature: SignatureT = self._ensure_one(self.find_with_signature(Signature(key=key)))[0]
                 existing[key] = signature
 
             except SearchError:
                 pass
 
         return self.remove_many(searched_signatures=list(existing.values()), ignore_non_existent=True).register_many(
             [(existing.get(key, Signature(key=key, type_=type(value))), value) for key, value in data.items()]
@@ -278,15 +268,15 @@
         """
         instance = self
         for signature, entity in data:
             instance = self.register(signature=signature, entity=entity, check_if_exists=check_if_exists)
         return instance
 
     def remove(
-        self, searched_signature: SignatureT[Any], ignore_non_existent: bool = False, exact_match: bool = True
+        self, searched_signature: SignatureT, ignore_non_existent: bool = False, exact_match: bool = True
     ) -> "ActionData":
         """
         Remove a value matching the signature
         :param searched_signature: Looked up signature
         :param ignore_non_existent: Controls whether the method raises an exception if a value with
         the ``signature`` wasn't found
         :param exact_match: Controls whether exact signature should be found
@@ -302,15 +292,15 @@
                 raise
             return self.evolve_self()
 
         return self.evolve_self(data=tuple(filter(lambda signature_value: signature_value[0] != to_remove, self.data)))
 
     def remove_many(
         self,
-        searched_signatures: Sequence[SignatureT[Any]],
+        searched_signatures: Sequence[SignatureT],
         ignore_non_existent: bool = False,
         exact_match: bool = True,
     ) -> "ActionData":
         """
         Remove values matching the signatures
         :param searched_signatures: Looked up signatures
         :param ignore_non_existent: Controls whether the method raises an exception if a value with
@@ -330,15 +320,15 @@
         """
         Clean all metadata from the previous execution. Note that observers will be created from the default classes
 
         :return: Copy of self with only :attrs:`ActionData.data` preserved
         """
         return ActionData(data=self.data)
 
-    def with_future(self, future: Awaitable[Any]) -> "ActionData":
+    def with_future(self, future: Awaitable) -> "ActionData":
         """
         Log futures references
         """
         return self.evolve_self(futures=self.futures + [future])
 
     def record_start(self, action: ActionT) -> "ActionData":
         """
@@ -381,15 +371,15 @@
         """
         :param data: New data to be appended
         :return: Copy with new data
         """
         return self.evolve_self(data=self._keyed_dict_as_values_with_signatures(data))
 
     @property
-    def signatures(self) -> List[SignatureT[Any]]:
+    def signatures(self) -> List[SignatureT]:
         """
         List registered signatures
         """
         return [reg[0] for reg in self.data]
 
     def is_in(self, key: str) -> bool:
         """
@@ -397,15 +387,15 @@
         """
         try:
             self.get_by_key(key)
             return True
         except NothingFound:
             return False
 
-    def signature_is_in(self, searched_signature: SignatureT[Any]) -> bool:
+    def signature_is_in(self, searched_signature: SignatureT) -> bool:
         """
         Find if the signature is in the data
         """
         try:
             self.get_by_signature(searched_signature)
             return True
         except NothingFound:
@@ -424,15 +414,15 @@
             if signature.key == key:
                 new_data.append((signature.evolve_self(key=new_key), value))
             else:
                 new_data.append((signature, value))
         return self.evolve_self(data=tuple(new_data))
 
     @classmethod
-    def _get_from_nested(cls, key: str, data: Dict[str, Any], default: Optional[Any] = None) -> Any:
+    def _get_from_nested(cls, key: str, data: Dict[str, Any], default: Any = None) -> Any:
         first_dot_index = key.find(".")
         if first_dot_index > 0:
             if key[:first_dot_index] not in data:
                 return default
 
             return cls._get_from_nested(key[first_dot_index + 1 :], data[key[:first_dot_index]])
         return data.get(key, default)
@@ -450,9 +440,9 @@
         first_value = matched[0]
         for value in matched[1:]:
             if value != first_value:
                 raise FoundMoreThanOne("Expected one, but found {}".format(n_matched))
         return first_value
 
     @staticmethod
-    def _keyed_dict_as_values_with_signatures(data: Dict[str, Any]) -> Tuple[Tuple[SignatureT[Any], Any], ...]:
+    def _keyed_dict_as_values_with_signatures(data: Dict[str, Any]) -> Tuple[Tuple[SignatureT, Any], ...]:
         return tuple((Signature(key=key, type_=type(value)), value) for key, value in data.items())
```

### Comparing `orinoco-1.0.9/orinoco/event.py` & `orinoco-2.0.0/orinoco/event.py`

 * *Files identical despite different names*

### Comparing `orinoco-1.0.9/orinoco/exceptions.py` & `orinoco-2.0.0/orinoco/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,19 +59,7 @@
 
 class RunnableOnlyInAsyncContext(BaseActionException):
     pass
 
 
 class RetryError(BaseActionException):
     pass
-
-
-class ActionSetInputValidationError(BaseActionException):
-    pass
-
-
-class ActionSetInputValidationMissingValueError(ActionSetInputValidationError):
-    pass
-
-
-class ActionSetInputTypeValidationError(ActionSetInputValidationError):
-    pass
```

### Comparing `orinoco-1.0.9/orinoco/helpers.py` & `orinoco-2.0.0/orinoco/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Iterable, Type, List, Any, NoReturn, Union, Optional, Tuple, Set
 
 from typing_extensions import Annotated, get_origin, get_args
 
 from orinoco.types import TypeT, AnnotationNameT
 
 
-def initialize(classes: Iterable[Type[Any]]) -> List[Any]:
+def initialize(classes: Iterable[Type]) -> List:
     return [cls_object() for cls_object in classes]
 
 
 def raise_not_provided_field(field_name: str) -> NoReturn:
     raise ValueError("Field {} has to be provided".format(field_name))
```

### Comparing `orinoco-1.0.9/orinoco/loop.py` & `orinoco-2.0.0/orinoco/loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         return action_data
 
     def _get_data_generator(self, action_data: ActionDataT) -> Iterable[ActionDataT]:
         for value in self._get_generator(action_data):
             yield action_data.evolve(**{self.iterating_key: value})
 
     @abstractmethod
-    def _get_generator(self, action_data: ActionDataT) -> Iterable[Any]:
+    def _get_generator(self, action_data: ActionDataT) -> Iterable:
         """
         :param action_data: Data container passed by actions
         :return: Iterable which provides the value which is set to the :class:`~orinoco.entities.ActionData`
         in each of the iterations
         """
         pass
 
@@ -81,15 +81,15 @@
 
         ForSideEffects("event", lambda action_data: action_data.get_or_default("event_log", [])).do(GetNotification())
 
     Then `GetNotification` has access to `event` via action data in each of the iterations
     which comes from the iterable "event_log"
     """
 
-    def __init__(self, iterating_key: str, method: Callable[[ActionDataT], Iterable[Any]]):
+    def __init__(self, iterating_key: str, method: Callable[[ActionDataT], Iterable]):
         """
         :param iterating_key: Key which will be propagated into the `ActionData` with the new value
         :param method: Method which returns the iterable to iterate over
         """
         super().__init__(iterating_key=iterating_key)
         self.method = method
 
@@ -110,15 +110,15 @@
         .run_with_data(values=[10, 40, 60])
         .get("doubled_list")
     """
 
     def __init__(
         self,
         iterating_key: str,
-        method: Callable[[ActionDataT], Iterable[Any]],
+        method: Callable[[ActionDataT], Iterable],
         aggregated_field: Optional[str] = None,
         aggregated_field_new_name: Optional[str] = None,
         skip_none_for_aggregated_field: bool = False,
     ):
         """
         :param iterating_key: Key which will be propagated into the `ActionData` with the new value
         :param method: Method which returns the iterable to iterate over
@@ -179,15 +179,15 @@
         return action_data
 
     async def _get_async_data_generator(self, action_data: ActionDataT) -> AsyncIterable[ActionDataT]:
         async for value in self._get_generator(action_data):
             yield action_data.evolve(**{self.iterating_key: value})
 
     @abstractmethod
-    def _get_generator(self, action_data: ActionDataT) -> AsyncIterable[Any]:
+    def _get_generator(self, action_data: ActionDataT) -> AsyncIterable:
         """
         :param action_data: Data container passed by actions
         :return: Iterable which provides the value which is set to the :class:`~orinoco.entities.ActionData`
         in each of the iterations
         """
         pass
 
@@ -202,15 +202,15 @@
 
         For("event", lambda action_data: action_data.get_or_default("event_log", [])).do(GetNotification())
 
     Then `GetNotification` has access to `event` via action data in each of the iterations
     which comes from the async iterable "event_log"
     """
 
-    def __init__(self, iterating_key: str, method: Callable[[ActionDataT], AsyncIterable[Any]]):
+    def __init__(self, iterating_key: str, method: Callable[[ActionDataT], AsyncIterable]):
         """
         :param iterating_key: Key which will be propagated into the `ActionData` with the new value
         :param method: Method which returns the iterable to iterate over
         """
         super().__init__(iterating_key=iterating_key)
         self.method = method
 
@@ -221,15 +221,15 @@
 class AsyncFor(BaseLoop):
     def run(self, action_data: ActionDataT) -> ActionDataT:
         raise RunnableOnlyInAsyncContext()
 
     def __init__(
         self,
         iterating_key: str,
-        method: Callable[[ActionDataT], AsyncIterable[Any]],
+        method: Callable[[ActionDataT], AsyncIterable],
         aggregated_field: Optional[str] = None,
         aggregated_field_new_name: Optional[str] = None,
         skip_none_for_aggregated_field: bool = False,
     ):
         """
         :param iterating_key: Key which will be propagated into the `ActionData` with the new value
         :param method: Method which returns the iterable to iterate over
```

### Comparing `orinoco-1.0.9/orinoco/observers.py` & `orinoco-2.0.0/orinoco/observers.py`

 * *Files identical despite different names*

### Comparing `orinoco-1.0.9/orinoco/retry.py` & `orinoco-2.0.0/orinoco/retry.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import abc
 import time
 from datetime import datetime
 from enum import Enum, auto
 from typing import Any, Callable, Type, Generic, Optional, cast
 
-from pydantic import BaseModel, Field
+from pydantic import ConfigDict, BaseModel, Field
 from returns import pipeline
 
 from returns.result import Failure, Result, Success
 
 from orinoco.action import record_action, verbose_action_exception, Action
 from orinoco.exceptions import RetryError, ConditionNotMet, BaseActionException
 from orinoco.types import ActionT, ActionDataT, ErrorT
@@ -26,18 +26,15 @@
     max_retries: int
     retry_delay: float
     retry_count: int = 0
     status: RetryStatus = RetryStatus.STARTED
 
     started: datetime = Field(default_factory=datetime.now)
     finished: Optional[datetime] = None
-
-    class Config:
-        arbitrary_types_allowed = False
-        allow_mutation = False
+    model_config = ConfigDict(frozen=True, arbitrary_types_allowed=False)
 
 
 class AbstractRetry(Generic[ErrorT], Action, abc.ABC):
     def __init__(self, action: ActionT, max_retries: int = 10, retry_delay: float = 10):
         super().__init__(name=f"<{self.__class__.__name__}: {action.name} every {retry_delay}s (max {max_retries})>")
         self.action = action
         self.max_retries = max_retries
@@ -62,17 +59,17 @@
                 )
 
             time.sleep(self.retry_delay)
         raise RetryError("{} failed after {} retries. Info: {}".format(self.name, self.max_retries, retry_info))
 
     def _get_new_retry_info(self, is_successful: bool, retry_counter: int, previous_retry_info: RetryInfo) -> RetryInfo:
         retry_status = self._get_retry_status(is_successful, retry_counter)
-        retry_info = previous_retry_info.copy(update={"status": retry_status, "retry_count": retry_counter})
+        retry_info = previous_retry_info.model_copy(update={"status": retry_status, "retry_count": retry_counter})
         if retry_status is RetryStatus.SUCCESSFUL:
-            return retry_info.copy(update={"finished": datetime.utcnow()})
+            return retry_info.model_copy(update={"finished": datetime.utcnow()})
 
         return retry_info
 
     def _get_retry_status(self, is_successful: bool, retry_counter: int) -> RetryStatus:
         if is_successful:
             return RetryStatus.SUCCESSFUL
         elif retry_counter > self.max_retries:
```

### Comparing `orinoco-1.0.9/orinoco/transformation.py` & `orinoco-2.0.0/orinoco/transformation.py`

 * *Files identical despite different names*

### Comparing `orinoco-1.0.9/orinoco/typed_action.py` & `orinoco-2.0.0/orinoco/typed_action.py`

 * *Files identical despite different names*

### Comparing `orinoco-1.0.9/orinoco/types.py` & `orinoco-2.0.0/orinoco/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import Dict, Any, TypeVar, Optional, Type, List, Tuple, Sequence, ClassVar, Set, Generic
 
-from pydantic import BaseModel
+from pydantic import ConfigDict, BaseModel
 
 
 T = TypeVar("T")
 BaseModelT = TypeVar("BaseModelT", bound=BaseModel)
 
 
 class NamespacedActionT:
@@ -13,37 +13,35 @@
 
     @abstractmethod
     def __getattr__(self, _: Any) -> Type["ActionT"]:
         pass
 
 
 class ImmutableEvolvableModelT(BaseModel, ABC):
-    class Config:
-        allow_mutation = False
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(frozen=True, arbitrary_types_allowed=True)
 
     @abstractmethod
     def evolve_self(self: T, **kwargs: Any) -> T:
         pass
 
 
-class SignatureT(Generic[T], ImmutableEvolvableModelT, ABC):
-    type_: Optional[Type[T]]
+class SignatureT(ImmutableEvolvableModelT, Generic[T], ABC):
+    type_: Optional[Type[T]] = None
     tags: Set[str]
-    key: Optional[str]
-    default_value: Any
+    key: Optional[str] = None
+    default_value: Any = None
 
     @abstractmethod
     def match(self, other_signature: "SignatureT[T]") -> bool:
         pass
 
 
-class ActionConfigT(Generic[T], ImmutableEvolvableModelT, ABC):
-    INPUT: Optional[Dict[str, SignatureT[Any]]]
-    OUTPUT: Optional[SignatureT[T]]
+class ActionConfigT(ImmutableEvolvableModelT, Generic[T], ABC):
+    INPUT: Optional[Dict[str, SignatureT]] = None
+    OUTPUT: Optional[SignatureT[T]] = None
 
 
 class ObserverT(ABC):
     @abstractmethod
     def should_record_action(self, action: "ActionT") -> bool:
         pass
 
@@ -57,22 +55,22 @@
 
 
 class ActionDataT(ImmutableEvolvableModelT, ABC):
 
     NOT_FOUND: ClassVar = object()
 
     # data: List[Tuple[SignatureT[Any], Any]]
-    data: Tuple[Tuple[SignatureT[Any], Any], ...]
-    futures: List[Any]
+    data: Tuple[Tuple[SignatureT, Any], ...]
+    futures: List
     observers: List[ObserverT]
     skip_processing: bool
 
+    @property
     @abstractmethod
-    # @property
-    def signatures(self) -> List[SignatureT[Any]]:
+    def signatures(self) -> List[SignatureT]:
         pass
 
     @abstractmethod
     def __getitem__(self, searched_signature: SignatureT[T]) -> T:
         pass
 
     @abstractmethod
@@ -84,19 +82,19 @@
         pass
 
     @abstractmethod
     def get_with_signature(self, searched_signature: SignatureT[T]) -> Tuple[SignatureT[T], T]:
         pass
 
     @abstractmethod
-    def get_or_default(self, key: str, default: Optional[Any] = None) -> Any:
+    def get_or_default(self, key: str, default: Any = None) -> Any:
         pass
 
     @abstractmethod
-    def find_or_default(self, key: str, default: Optional[Any] = None) -> Any:
+    def find_or_default(self, key: str, default: Any = None) -> Any:
         pass
 
     @abstractmethod
     def get_by_key(self, name: str, default: Any = NOT_FOUND) -> Any:
         pass
 
     @abstractmethod
@@ -129,22 +127,22 @@
 
     @abstractmethod
     def register_many(self, data: Sequence[Tuple[SignatureT[T], T]], check_if_exists: bool = True) -> "ActionDataT":
         pass
 
     @abstractmethod
     def remove(
-        self, searched_signature: SignatureT[Any], ignore_non_existent: bool = False, exact_match: bool = True
+        self, searched_signature: SignatureT, ignore_non_existent: bool = False, exact_match: bool = True
     ) -> "ActionDataT":
         pass
 
     @abstractmethod
     def remove_many(
         self,
-        searched_signatures: Sequence[SignatureT[Any]],
+        searched_signatures: Sequence[SignatureT],
         ignore_non_existent: bool = False,
         exact_match: bool = True,
     ) -> "ActionDataT":
         pass
 
     @abstractmethod
     def with_future(self, future: Any) -> "ActionDataT":
@@ -172,15 +170,15 @@
         pass
 
     @abstractmethod
     def is_in(self, key: str) -> bool:
         pass
 
     @abstractmethod
-    def signature_is_in(self, searched_signature: SignatureT[Any]) -> bool:
+    def signature_is_in(self, searched_signature: SignatureT) -> bool:
         pass
 
     @abstractmethod
     def get_observer(self, observer_cls: Type["ObserverVar"]) -> "ObserverVar":
         pass
 
     @abstractmethod
@@ -198,14 +196,15 @@
     NAME: str
 
     description: str
     name: str
 
     # @abstractmethod
     @property
+    @abstractmethod
     def action_name(self) -> str:
         pass
 
     @abstractmethod
     def then(self, another_action: "ActionT") -> "ActionT":
         pass
```

