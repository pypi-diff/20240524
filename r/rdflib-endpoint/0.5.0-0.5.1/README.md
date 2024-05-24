# Comparing `tmp/rdflib_endpoint-0.5.0.tar.gz` & `tmp/rdflib_endpoint-0.5.1.tar.gz`

## Comparing `rdflib_endpoint-0.5.0.tar` & `rdflib_endpoint-0.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/CITATION.cff
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/example/Dockerfile
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/example/README.md
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/example/docker-compose.yml
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/example/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/example/app/__init__.py
--rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/example/app/custom_eval.py
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/example/app/main.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/src/rdflib_endpoint/__init__.py
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/src/rdflib_endpoint/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/src/rdflib_endpoint/py.typed
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/src/rdflib_endpoint/sparql_endpoint.py
--rw-r--r--   0        0        0    18983 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/src/rdflib_endpoint/sparql_router.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/src/rdflib_endpoint/yasgui.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/tests/test_example_app.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/tests/test_oxrdflib.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/tests/test_parse_accept.py
--rw-r--r--   0        0        0     7384 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/tests/test_rdflib_endpoint.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/tests/test_serve_cli.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/tests/resources/another.jsonld
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/tests/resources/custom_eval_todo.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/tests/resources/test.nq
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/tests/resources/test2.ttl
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0    12657 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/README.md
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/CITATION.cff
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/example/Dockerfile
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/example/README.md
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/example/docker-compose.yml
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/example/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/example/app/__init__.py
+-rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/example/app/custom_eval.py
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/example/app/main.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/src/rdflib_endpoint/__init__.py
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/src/rdflib_endpoint/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/src/rdflib_endpoint/py.typed
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/src/rdflib_endpoint/sparql_endpoint.py
+-rw-r--r--   0        0        0    20067 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/src/rdflib_endpoint/sparql_router.py
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/src/rdflib_endpoint/yasgui.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/tests/test_example_app.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/tests/test_oxrdflib.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/tests/test_parse_accept.py
+-rw-r--r--   0        0        0     7847 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/tests/test_rdflib_endpoint.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/tests/test_serve_cli.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/tests/resources/another.jsonld
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/tests/resources/custom_eval_todo.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/tests/resources/test.nq
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/tests/resources/test2.ttl
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/LICENSE.txt
+-rw-r--r--   0        0        0    12711 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/README.md
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 rdflib_endpoint-0.5.1/PKG-INFO
```

### Comparing `rdflib_endpoint-0.5.0/.pre-commit-config.yaml` & `rdflib_endpoint-0.5.1/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -11,26 +11,23 @@
       name: " ✔️  Check YAML"
       args:
       - --unsafe
     - id: end-of-file-fixer
       name: " 🪚 Fix end of files"
     - id: trailing-whitespace
       name: " ✂️  Trim trailing whitespaces"
-  - repo: https://github.com/psf/black
-    rev: 23.11.0
-    hooks:
-      - id: black
-        name: " ✒️  Formatting code with Black"
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.1.6
+    rev: v0.4.5
     hooks:
       - id: ruff
-        name: " ⚡️ Formatting code with Ruff"
+        name: " ⚡️ Lint code with ruff"
         args:
         - --fix
+      - id: ruff-format
+        name: " ✒️  Format code with ruff"
   # Does not read the config from pyproject.toml
   # - repo: https://github.com/pre-commit/mirrors-mypy
   #   rev: v1.4.1
   #   hooks:
   #   - id: mypy
   #     name: 🔎 Check types with mypy
   #     args:
```

### Comparing `rdflib_endpoint-0.5.0/CONTRIBUTING.md` & `rdflib_endpoint-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rdflib_endpoint-0.5.0/.github/workflows/release.yml` & `rdflib_endpoint-0.5.1/.github/workflows/release.yml`

 * *Files 20% similar despite different names*

```diff
@@ -14,26 +14,22 @@
     needs: tests
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
 
     - name: Install dependencies
       run: |
         pip install build
 
-    # - name: Bump version to ${{github.ref_name}}
-    #   run: |
-    #     hatch version "${{github.ref_name}}"
-
     - name: Build package
       run: python -m build
 
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
```

### Comparing `rdflib_endpoint-0.5.0/example/README.md` & `rdflib_endpoint-0.5.1/example/README.md`

 * *Files identical despite different names*

### Comparing `rdflib_endpoint-0.5.0/example/app/custom_eval.py` & `rdflib_endpoint-0.5.1/example/app/custom_eval.py`

 * *Files identical despite different names*

### Comparing `rdflib_endpoint-0.5.0/example/app/main.py` & `rdflib_endpoint-0.5.1/example/app/main.py`

 * *Files identical despite different names*

### Comparing `rdflib_endpoint-0.5.0/src/rdflib_endpoint/__main__.py` & `rdflib_endpoint-0.5.1/src/rdflib_endpoint/__main__.py`

 * *Files identical despite different names*

### Comparing `rdflib_endpoint-0.5.0/src/rdflib_endpoint/sparql_endpoint.py` & `rdflib_endpoint-0.5.1/src/rdflib_endpoint/sparql_endpoint.py`

 * *Files identical despite different names*

### Comparing `rdflib_endpoint-0.5.0/src/rdflib_endpoint/sparql_router.py` & `rdflib_endpoint-0.5.1/src/rdflib_endpoint/sparql_router.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,17 +62,33 @@
     200: {
         "description": "SPARQL query results",
         "content": {
             "application/sparql-results+json": {"example": {"results": {"bindings": []}, "head": {"vars": []}}},
             "application/json": {"example": {"results": {"bindings": []}, "head": {"vars": []}}},
             "text/csv": {"example": "s,p,o"},
             "application/sparql-results+csv": {"example": "s,p,o"},
-            "text/turtle": {"example": "service description"},
             "application/sparql-results+xml": {"example": "<root></root>"},
             "application/xml": {"example": "<root></root>"},
+            "text/turtle": {"example": "<http://subject> <http://predicate> <http://object> ."},
+            "application/n-triples": {"example": "<http://subject> <http://predicate> <http://object> ."},
+            "text/n3": {"example": "<http://subject> <http://predicate> <http://object> ."},
+            "application/n-quads": {"example": "<http://subject> <http://predicate> <http://object> <http://graph> ."},
+            "application/trig": {
+                "example": "GRAPH <http://graph> {<http://subject> <http://predicate> <http://object> .}"
+            },
+            "application/trix": {"example": "<xml></xml>"},
+            "application/ld+json": {
+                "example": [
+                    {
+                        "@id": "http://subject",
+                        "@type": ["http://object"],
+                        "http://www.w3.org/2000/01/rdf-schema#label": [{"@value": "foo"}],
+                    }
+                ]
+            },
             # "application/rdf+xml": {
             #     "example": '<?xml version="1.0" encoding="UTF-8"?> <rdf:RDF xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"></rdf:RDF>'
             # },
         },
     },
     400: {
         "description": "Bad Request",
@@ -96,19 +112,26 @@
     "application/json": "json",
     "text/json": "json",
     # https://www.w3.org/TR/rdf-sparql-XMLres/
     "application/sparql-results+xml": "xml",
     "application/xml": "xml",  # for compatibility
     "application/rdf+xml": "xml",  # for compatibility
     "text/xml": "xml",  # not standard
+    "application/ld+json": "json-ld",
     # https://www.w3.org/TR/sparql11-results-csv-tsv/
     "application/sparql-results+csv": "csv",
     "text/csv": "csv",  # for compatibility
     # Extras
     "text/turtle": "ttl",
+    "text/n3": "n3",
+    "application/n-triples": "nt",
+    "text/plain": "nt",
+    "application/trig": "trig",
+    "application/trix": "trix",
+    "application/n-quads": "nquads",
 }
 
 
 def parse_accept_header(accept: str) -> List[str]:
     """
     Given an accept header string, return a list of media types in order of preference.
 
@@ -253,25 +276,25 @@
                             # Use the first mime_type that matches
                             break
 
                     query_operation = re.sub(r"(\w)([A-Z])", r"\1 \2", parsed_query.algebra.name)
 
                     # Handle mime type for construct queries
                     if query_operation == "Construct Query":
-                        if output_mime_type in {"application/json", "text/csv"}:
+                        if output_mime_type == "text/csv":
                             output_mime_type = "text/turtle"
-                            # TODO: support JSON-LD for construct query?
-                            # g.serialize(format='json-ld', indent=4)
+                        elif output_mime_type == "application/json":
+                            output_mime_type = "application/ld+json"
                         elif output_mime_type == "application/xml":
                             output_mime_type = "application/rdf+xml"
                         else:
-                            pass  # TODO what happens here?
+                            pass
 
                     try:
-                        rdflib_format = CONTENT_TYPE_TO_RDFLIB_FORMAT[output_mime_type]
+                        rdflib_format = CONTENT_TYPE_TO_RDFLIB_FORMAT.get(output_mime_type, output_mime_type)
                         response = Response(
                             query_results.serialize(format=rdflib_format),
                             media_type=output_mime_type,
                         )
                     except Exception as e:
                         logging.error(f"Error serializing the SPARQL query results with RDFLib: {e}")
                         return JSONResponse(
@@ -406,15 +429,15 @@
         html_str = html_str.replace("$TITLE", self.title)
         html_str = html_str.replace("$DESCRIPTION", self.description)
         html_str = html_str.replace("$FAVICON", self.favicon)
         html_str = html_str.replace("$EXAMPLE_QUERY", self.example_query)
         html_str = html_str.replace("$EXAMPLE_QUERIES", json.dumps(self.example_queries))
         return Response(content=html_str, media_type="text/html")
 
-    def get_service_graph(self) -> rdflib.Graph:
+    def get_service_graph(self) -> Graph:
         # Service description returned when no query provided
         service_description_ttl = SERVICE_DESCRIPTION_TTL_FMT.format(
             public_url=self.public_url,
             title=self.title,
             description=self.description.replace("\n", ""),
         )
         graph = Graph()
```

### Comparing `rdflib_endpoint-0.5.0/src/rdflib_endpoint/yasgui.html` & `rdflib_endpoint-0.5.1/src/rdflib_endpoint/yasgui.html`

 * *Files identical despite different names*

### Comparing `rdflib_endpoint-0.5.0/tests/test_example_app.py` & `rdflib_endpoint-0.5.1/tests/test_example_app.py`

 * *Files identical despite different names*

### Comparing `rdflib_endpoint-0.5.0/tests/test_oxrdflib.py` & `rdflib_endpoint-0.5.1/tests/test_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `rdflib_endpoint-0.5.0/tests/test_parse_accept.py` & `rdflib_endpoint-0.5.1/tests/test_parse_accept.py`

 * *Files identical despite different names*

### Comparing `rdflib_endpoint-0.5.0/tests/test_rdflib_endpoint.py` & `rdflib_endpoint-0.5.1/tests/test_rdflib_endpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 )
 
 endpoint = TestClient(app)
 
 
 def test_service_description():
     response = endpoint.get("/", headers={"accept": "text/turtle"})
-    # print(response.text.strip())
     assert response.status_code == 200
     assert response.text.strip() == service_description
 
     response = endpoint.post("/", headers={"accept": "text/turtle"})
     assert response.status_code == 200
     assert response.text.strip() == service_description
 
@@ -59,14 +58,15 @@
     assert response.status_code == 200
     assert response.json()["results"]["bindings"][0]["concat"]["value"] == "Firstlast"
 
 
 def test_select_noaccept_xml():
     response = endpoint.post("/", data={"query": concat_select})
     assert response.status_code == 200
+    assert response.text.startswith("<?xml ")
 
 
 def test_select_csv():
     response = endpoint.post("/", data={"query": concat_select}, headers={"accept": "text/csv"})
     assert response.status_code == 200
 
 
@@ -136,36 +136,55 @@
     assert response.status_code == 200
     assert response.json()["results"]["bindings"][0]["concat"]["value"] == "Firstlast"
 
 
 def test_fail_select_turtle():
     response = endpoint.post("/", data={"query": concat_select}, headers={"accept": "text/turtle"})
     assert response.status_code == 422
-    # assert response.json()['results']['bindings'][0]['concat']['value'] == "Firstlast"
 
 
 def test_concat_construct_turtle():
-    # expected to return turtle
+    response = endpoint.post(
+        "/",
+        data={"query": custom_concat_construct},
+        headers={"accept": "text/turtle"},
+    )
+    assert response.status_code == 200
+    assert response.text.startswith("@prefix ")
+
+
+def test_concat_construct_csv():
+    response = endpoint.post(
+        "/",
+        data={"query": custom_concat_construct},
+        headers={"accept": "text/csv"},
+    )
+    assert response.status_code == 200
+    assert response.text.startswith("@prefix ")
+
+
+def test_concat_construct_jsonld():
     response = endpoint.post(
         "/",
         data={"query": custom_concat_construct},
         headers={"accept": "application/json"},
     )
     assert response.status_code == 200
-    # assert response.json()['results']['bindings'][0]['concat']['value'] == "Firstlast"
+    assert response.json()[0]["@id"] == "http://example.com/test"
 
 
 def test_concat_construct_xml():
     # expected to return turtle
     response = endpoint.post(
         "/",
         data={"query": custom_concat_construct},
         headers={"accept": "application/xml"},
     )
     assert response.status_code == 200
+    assert response.text.startswith("<?xml ")
 
 
 def test_yasgui():
     # expected to return turtle
     response = endpoint.get(
         "/",
         headers={"accept": "text/html"},
@@ -182,15 +201,15 @@
 SELECT ?concat ?concatLength WHERE {
     BIND("First" AS ?first)
     BIND(myfunctions:custom_concat(?first, "last") AS ?concat)
 }"""
 
 custom_concat_construct = """PREFIX myfunctions: <https://w3id.org/um/sparql-functions/>
 CONSTRUCT {
-    <http://test> <http://concat> ?concat, ?concatLength .
+    <http://example.com/test> <http://example.com/concat> ?concat, ?concatLength .
 } WHERE {
     BIND("First" AS ?first)
     BIND(myfunctions:custom_concat(?first, "last") AS ?concat)
 }"""
 
 service_description = """@prefix dc: <http://purl.org/dc/elements/1.1/> .
 @prefix ent: <http://www.w3.org/ns/entailment/> .
```

### Comparing `rdflib_endpoint-0.5.0/tests/test_serve_cli.py` & `rdflib_endpoint-0.5.1/tests/test_serve_cli.py`

 * *Files identical despite different names*

### Comparing `rdflib_endpoint-0.5.0/tests/resources/custom_eval_todo.py` & `rdflib_endpoint-0.5.1/tests/resources/custom_eval_todo.py`

 * *Files identical despite different names*

### Comparing `rdflib_endpoint-0.5.0/LICENSE.txt` & `rdflib_endpoint-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rdflib_endpoint-0.5.0/README.md` & `rdflib_endpoint-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,21 +44,21 @@
 ```bash
 pip install "rdflib-endpoint[web]"
 ```
 
 If you want to use `rdlib-endpoint` as a CLI you can install with the optional dependency `cli`:
 
 ```bash
-pip install "rdflib-endpoint[cli]"
+pip install "rdflib-endpoint[web,cli]"
 ```
 
 If you want to use [oxigraph](https://github.com/oxigraph/oxigraph) as backend triplestore you can install with the optional dependency `oxigraph`:
 
 ```bash
-pip install "rdflib-endpoint[oxigraph,cli]"
+pip install "rdflib-endpoint[web,cli,oxigraph]"
 ```
 
 > [!WARNING]
 > Oxigraph and `oxrdflib` do not support custom functions, so it can be only used to deploy graphs without custom functions.
 
 ## ⌨️ Use the CLI
 
@@ -171,14 +171,16 @@
     public_url='https://your-endpoint-url/',
 )
 
 app = FastAPI()
 app.include_router(sparql_router)
 ```
 
+> TODO: add docs to integrate to a Flask app
+
 ### 📝 Define custom SPARQL functions
 
 This option makes it easier to define functions in your SPARQL endpoint, e.g. `BIND(myfunction:custom_concat("start", "end") AS ?concat)`. It can be used with the `SparqlEndpoint` and `SparqlRouter` classes.
 
 Create a `app/main.py` file in your project folder with your custom SPARQL functions, and endpoint parameters:
 
 ````python
```

### Comparing `rdflib_endpoint-0.5.0/pyproject.toml` & `rdflib_endpoint-0.5.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -108,14 +108,17 @@
 
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 
 # TOOLS
+[tool.hatch.build.targets.wheel]
+packages = ["src/rdflib_endpoint"]
+
 [tool.hatch.version]
 path = "src/rdflib_endpoint/__init__.py"
 
 
 [tool.coverage.run]
 source = ["src/rdflib_endpoint"]
 branch = false
@@ -153,27 +156,21 @@
 warn_no_return = true
 warn_unused_ignores = true
 warn_redundant_casts = true
 disallow_untyped_defs = true
 disallow_any_generics = true
 disallow_untyped_calls = false # needed due to _eval() not being typed in rdflib
 
-
-[tool.black]
-color = true
-line-length = 120
-target-version = ['py38']
-skip-string-normalization = false
-
-
-# https://beta.ruff.rs/docs/rules
+# https://docs.astral.sh/ruff/rules/
 [tool.ruff]
 src = ["src", "tests"]
 target-version = "py38"
 line-length = 120
+
+[tool.ruff.lint]
 select = [
     "I",     # isort
     "N",     # pep8-naming
     "S",     # bandit
     "A",     # flake8-builtins
     "YTT",   # flake8-2020
     "B",     # flake8-bugbear
@@ -199,13 +196,13 @@
     "B008", # do not perform function calls in argument defaults (required for FastAPI afaik)
     "E501", # line too long
     "C901", # too complex
     "S101", # Use of `assert` detected
     "T201", "T203", # remove print and pprint
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["I", "F401"] # module imported but unused
 
 
 # [tool.hatch.build]
 # sources = ["src"]
```

### Comparing `rdflib_endpoint-0.5.0/PKG-INFO` & `rdflib_endpoint-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: rdflib-endpoint
-Version: 0.5.0
+Version: 0.5.1
 Summary: A package to deploy SPARQL endpoint to serve local RDF files, machine learning models, or any other logic implemented in Python, using RDFLib and FastAPI.
 Project-URL: Homepage, https://github.com/vemonet/rdflib-endpoint
 Project-URL: Documentation, https://github.com/vemonet/rdflib-endpoint
 Project-URL: History, https://github.com/vemonet/rdflib-endpoint/releases
 Project-URL: Tracker, https://github.com/vemonet/rdflib-endpoint/issues
 Project-URL: Source, https://github.com/vemonet/rdflib-endpoint
 Author-email: Vincent Emonet <vincent.emonet@gmail.com>
@@ -110,21 +110,21 @@
 ```bash
 pip install "rdflib-endpoint[web]"
 ```
 
 If you want to use `rdlib-endpoint` as a CLI you can install with the optional dependency `cli`:
 
 ```bash
-pip install "rdflib-endpoint[cli]"
+pip install "rdflib-endpoint[web,cli]"
 ```
 
 If you want to use [oxigraph](https://github.com/oxigraph/oxigraph) as backend triplestore you can install with the optional dependency `oxigraph`:
 
 ```bash
-pip install "rdflib-endpoint[oxigraph,cli]"
+pip install "rdflib-endpoint[web,cli,oxigraph]"
 ```
 
 > [!WARNING]
 > Oxigraph and `oxrdflib` do not support custom functions, so it can be only used to deploy graphs without custom functions.
 
 ## ⌨️ Use the CLI
 
@@ -237,14 +237,16 @@
     public_url='https://your-endpoint-url/',
 )
 
 app = FastAPI()
 app.include_router(sparql_router)
 ```
 
+> TODO: add docs to integrate to a Flask app
+
 ### 📝 Define custom SPARQL functions
 
 This option makes it easier to define functions in your SPARQL endpoint, e.g. `BIND(myfunction:custom_concat("start", "end") AS ?concat)`. It can be used with the `SparqlEndpoint` and `SparqlRouter` classes.
 
 Create a `app/main.py` file in your project folder with your custom SPARQL functions, and endpoint parameters:
 
 ````python
```

