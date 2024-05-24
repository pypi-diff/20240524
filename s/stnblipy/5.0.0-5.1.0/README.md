# Comparing `tmp/stnblipy-5.0.0.tar.gz` & `tmp/stnblipy-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\stnblipy-5.0.0.tar", last modified: Tue May 14 17:44:08 2024, max compression
+gzip compressed data, was "dist\stnblipy-5.1.0.tar", last modified: Fri May 24 14:21:32 2024, max compression
```

## Comparing `stnblipy-5.0.0.tar` & `stnblipy-5.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 17:44:08.000000 stnblipy-5.0.0/
--rw-rw-rw-   0        0        0      385 2024-05-14 17:44:08.000000 stnblipy-5.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 17:44:07.000000 stnblipy-5.0.0/blipy/
--rw-rw-rw-   0        0        0        0 2022-07-22 17:59:57.000000 stnblipy-5.0.0/blipy/__init__.py
--rw-rw-rw-   0        0        0     2699 2024-05-14 17:37:14.000000 stnblipy-5.0.0/blipy/arquivo_csv.py
--rw-rw-rw-   0        0        0     2457 2024-05-14 17:37:14.000000 stnblipy-5.0.0/blipy/arquivo_posicional.py
--rw-rw-rw-   0        0        0    15272 2024-01-31 20:22:27.000000 stnblipy-5.0.0/blipy/conexao_bd.py
--rw-rw-rw-   0        0        0      335 2022-07-22 17:59:57.000000 stnblipy-5.0.0/blipy/enum_tipo_col_bd.py
--rw-rw-rw-   0        0        0     2135 2022-07-22 17:59:57.000000 stnblipy-5.0.0/blipy/erro.py
--rw-rw-rw-   0        0        0    32144 2024-05-14 17:37:14.000000 stnblipy-5.0.0/blipy/func_transformacao.py
--rw-rw-rw-   0        0        0    69255 2024-05-14 17:37:15.000000 stnblipy-5.0.0/blipy/job.py
--rw-rw-rw-   0        0        0     5673 2024-03-20 14:04:38.000000 stnblipy-5.0.0/blipy/jsonstring.py
--rw-rw-rw-   0        0        0     4799 2024-05-14 17:37:15.000000 stnblipy-5.0.0/blipy/planilha.py
--rw-rw-rw-   0        0        0     2759 2022-07-22 17:59:57.000000 stnblipy-5.0.0/blipy/profiling.py
--rw-rw-rw-   0        0        0     3982 2024-05-14 17:37:15.000000 stnblipy-5.0.0/blipy/tabela_dataframe.py
--rw-rw-rw-   0        0        0     4885 2023-09-20 15:10:58.000000 stnblipy-5.0.0/blipy/tabela_entrada.py
--rw-rw-rw-   0        0        0     1607 2024-05-14 17:37:15.000000 stnblipy-5.0.0/blipy/tabela_html.py
--rw-rw-rw-   0        0        0    13498 2024-05-14 17:37:15.000000 stnblipy-5.0.0/blipy/tabela_saida.py
--rw-rw-rw-   0        0        0     7311 2023-03-10 18:27:46.000000 stnblipy-5.0.0/blipy/utils.py
--rw-rw-rw-   0        0        0       42 2024-05-14 17:44:08.000000 stnblipy-5.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1029 2024-05-14 17:37:53.000000 stnblipy-5.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:44:07.000000 stnblipy-5.0.0/stnblipy.egg-info/
--rw-rw-rw-   0        0        0      385 2024-05-14 17:44:07.000000 stnblipy-5.0.0/stnblipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      634 2024-05-14 17:44:07.000000 stnblipy-5.0.0/stnblipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 17:44:07.000000 stnblipy-5.0.0/stnblipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      168 2024-05-14 17:44:07.000000 stnblipy-5.0.0/stnblipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-14 17:44:07.000000 stnblipy-5.0.0/stnblipy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 17:44:08.000000 stnblipy-5.0.0/test/
--rw-rw-rw-   0        0        0    32979 2024-01-31 20:22:28.000000 stnblipy-5.0.0/test/teste_conexao_json.py
--rw-rw-rw-   0        0        0     5791 2024-01-31 20:22:28.000000 stnblipy-5.0.0/test/teste_estrategias_atualizacao.py
--rw-rw-rw-   0        0        0    22197 2024-05-14 17:37:15.000000 stnblipy-5.0.0/test/teste_geral.py
--rw-rw-rw-   0        0        0    20808 2022-08-17 17:16:30.000000 stnblipy-5.0.0/test/teste_job.py
--rw-rw-rw-   0        0        0     2287 2022-07-22 17:59:57.000000 stnblipy-5.0.0/test/testes_classe_planilha.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:21:32.000000 stnblipy-5.1.0/
+-rw-rw-rw-   0        0        0      385 2024-05-24 14:21:32.000000 stnblipy-5.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-24 14:21:32.000000 stnblipy-5.1.0/blipy/
+-rw-rw-rw-   0        0        0        0 2024-05-20 13:07:02.000000 stnblipy-5.1.0/blipy/__init__.py
+-rw-rw-rw-   0        0        0     2699 2024-05-20 13:07:02.000000 stnblipy-5.1.0/blipy/arquivo_csv.py
+-rw-rw-rw-   0        0        0     2457 2024-05-20 13:07:02.000000 stnblipy-5.1.0/blipy/arquivo_posicional.py
+-rw-rw-rw-   0        0        0    15272 2024-05-20 13:07:02.000000 stnblipy-5.1.0/blipy/conexao_bd.py
+-rw-rw-rw-   0        0        0      335 2024-05-20 13:07:02.000000 stnblipy-5.1.0/blipy/enum_tipo_col_bd.py
+-rw-rw-rw-   0        0        0     2135 2024-05-20 13:07:02.000000 stnblipy-5.1.0/blipy/erro.py
+-rw-rw-rw-   0        0        0    34622 2024-05-24 13:59:45.000000 stnblipy-5.1.0/blipy/func_transformacao.py
+-rw-rw-rw-   0        0        0    69255 2024-05-20 13:07:02.000000 stnblipy-5.1.0/blipy/job.py
+-rw-rw-rw-   0        0        0     5673 2024-05-20 13:07:02.000000 stnblipy-5.1.0/blipy/jsonstring.py
+-rw-rw-rw-   0        0        0     4799 2024-05-20 13:07:02.000000 stnblipy-5.1.0/blipy/planilha.py
+-rw-rw-rw-   0        0        0     2759 2024-05-20 13:07:02.000000 stnblipy-5.1.0/blipy/profiling.py
+-rw-rw-rw-   0        0        0     3982 2024-05-20 13:07:02.000000 stnblipy-5.1.0/blipy/tabela_dataframe.py
+-rw-rw-rw-   0        0        0     4885 2024-05-20 13:07:02.000000 stnblipy-5.1.0/blipy/tabela_entrada.py
+-rw-rw-rw-   0        0        0     1607 2024-05-20 13:07:02.000000 stnblipy-5.1.0/blipy/tabela_html.py
+-rw-rw-rw-   0        0        0    13498 2024-05-20 13:07:02.000000 stnblipy-5.1.0/blipy/tabela_saida.py
+-rw-rw-rw-   0        0        0     7311 2024-05-20 13:07:02.000000 stnblipy-5.1.0/blipy/utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-24 14:21:32.000000 stnblipy-5.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1029 2024-05-24 14:01:19.000000 stnblipy-5.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:21:32.000000 stnblipy-5.1.0/stnblipy.egg-info/
+-rw-rw-rw-   0        0        0      385 2024-05-24 14:21:32.000000 stnblipy-5.1.0/stnblipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      634 2024-05-24 14:21:32.000000 stnblipy-5.1.0/stnblipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 14:21:32.000000 stnblipy-5.1.0/stnblipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      168 2024-05-24 14:21:32.000000 stnblipy-5.1.0/stnblipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-24 14:21:32.000000 stnblipy-5.1.0/stnblipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 14:21:32.000000 stnblipy-5.1.0/test/
+-rw-rw-rw-   0        0        0    32979 2024-05-20 13:07:02.000000 stnblipy-5.1.0/test/teste_conexao_json.py
+-rw-rw-rw-   0        0        0     5791 2024-05-20 13:07:02.000000 stnblipy-5.1.0/test/teste_estrategias_atualizacao.py
+-rw-rw-rw-   0        0        0    22805 2024-05-24 13:59:45.000000 stnblipy-5.1.0/test/teste_geral.py
+-rw-rw-rw-   0        0        0    20808 2024-05-20 13:07:02.000000 stnblipy-5.1.0/test/teste_job.py
+-rw-rw-rw-   0        0        0     2287 2024-05-20 13:07:02.000000 stnblipy-5.1.0/test/testes_classe_planilha.py
```

### Comparing `stnblipy-5.0.0/blipy/arquivo_csv.py` & `stnblipy-5.1.0/blipy/arquivo_csv.py`

 * *Files identical despite different names*

### Comparing `stnblipy-5.0.0/blipy/arquivo_posicional.py` & `stnblipy-5.1.0/blipy/arquivo_posicional.py`

 * *Files identical despite different names*

### Comparing `stnblipy-5.0.0/blipy/conexao_bd.py` & `stnblipy-5.1.0/blipy/conexao_bd.py`

 * *Files identical despite different names*

### Comparing `stnblipy-5.0.0/blipy/erro.py` & `stnblipy-5.1.0/blipy/erro.py`

 * *Files identical despite different names*

### Comparing `stnblipy-5.0.0/blipy/func_transformacao.py` & `stnblipy-5.1.0/blipy/func_transformacao.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 Funções de transformação a serem usadas nas cargas ("T" do ETL).
 """
 
+import os
+import hashlib
 import html
 import re
 from datetime import date, datetime
 
 
 """
 Módulo com as classes de transformação de dados ("T" do ETL)
@@ -888,25 +890,97 @@
         """
         
         if len(entradas) != 1:
             raise RuntimeError(
                 "Não pode haver mais de um dado de entrada para uma "
                 "inversão de sinal.")
 
-        if entradas[0] is None:
+        if entradas[0] is None or entradas[0] == "nan":
             return None
 
         if type(entradas[0]) == str:
             val = entradas[0].replace(",", ".")
             val = float(val)
         else:
             val = entradas[0]
 
         return val*(-1)
+    
+class Hash():
+    """
+    Função que retorna um hash de um valor. Utiliza o algoritmo md5. Se o
+    parâmetro salt_hash for None, será utilizado o valor padrão definido numa
+    variável de ambiente chamada SALT_HASH.
+    """
+
+    def __init__(self, salt_hash=None):
+        self.__salt_hash = salt_hash
+
+    def transforma(self, entradas):                
+        if len(entradas) != 1:
+            raise RuntimeError(
+                "Não pode haver mais de um dado de entrada para um "
+                "hash.")
+
+        if entradas[0] is None or entradas[0] == "nan":
+            return None
+
+        val = str(entradas[0])
+        salt_hash = self.__salt_hash
+
+        if salt_hash is None:
+            salt_hash = os.getenv("SALT_HASH")
+        else:
+            salt_hash = str(salt_hash)
+
+        if salt_hash is None:
+            raise RuntimeError("A variável de ambiente SALT_HASH não foi "
+                               "encontrada.")
+
+        val = (val + salt_hash).encode("utf-8")
 
+        return str.upper(hashlib.md5(val).hexdigest())
+    
+class HashCPF(Hash):
+    """
+    Função que retorna um hash de um valor de um CPF, garantindo que o hash de
+    CPFs de mesma numeração serão iguais independentemente de suas formatações.
+    Utiliza o algoritmo herdado da classe Hash. Sempre será utilizado o valor
+    padrão de salt definido numa variável de ambiente chamada SALT_HASH.
+    """
+
+    # 'None' é passado como parâmetro para o construtor da classe pai, para
+    # garantir que o valor do salt vai ser buscado da variável de ambiente
+    # SALT_HASH    
+    def __init__(self):
+        super().__init__(None)
+
+    def transforma(self, entradas):
+        if len(entradas) != 1:
+            raise RuntimeError(
+                "Não pode haver mais de um CPF de entrada para um "
+                "hash.")
+
+        if entradas[0] is None or entradas[0] == "nan":
+            return None
+        
+        # Retirando do cpf caracteres indesejados, para que ele fique apenas
+        # com números
+        cpf = str(entradas[0]).strip()
+        cpf = cpf.replace(".", "")
+        cpf = cpf.replace("-", "")
+
+        # Laço para completar o cpf com zeros, caso ele tenha menos que 11
+        # dígitos
+        while len(cpf) < 11:
+            cpf = "0" + cpf
+
+        return super().transforma([cpf])
+
+        
 # TODO: implementar classe de transformação de conversão tipo
 
 #  objetos de classes de transformação que só fazem sentido ter uma instância 
 #  (singletons). Desta forma, ao importar este módulo estes objetos já estarão
 #  instanciandos e bastará utilizá-los, sem necessidade de criar uma nova
 #  instância no código que importou este módulo
 f_copia     = Copia()
```

### Comparing `stnblipy-5.0.0/blipy/job.py` & `stnblipy-5.1.0/blipy/job.py`

 * *Files identical despite different names*

### Comparing `stnblipy-5.0.0/blipy/jsonstring.py` & `stnblipy-5.1.0/blipy/jsonstring.py`

 * *Files identical despite different names*

### Comparing `stnblipy-5.0.0/blipy/planilha.py` & `stnblipy-5.1.0/blipy/planilha.py`

 * *Files identical despite different names*

### Comparing `stnblipy-5.0.0/blipy/profiling.py` & `stnblipy-5.1.0/blipy/profiling.py`

 * *Files identical despite different names*

### Comparing `stnblipy-5.0.0/blipy/tabela_dataframe.py` & `stnblipy-5.1.0/blipy/tabela_dataframe.py`

 * *Files identical despite different names*

### Comparing `stnblipy-5.0.0/blipy/tabela_entrada.py` & `stnblipy-5.1.0/blipy/tabela_entrada.py`

 * *Files identical despite different names*

### Comparing `stnblipy-5.0.0/blipy/tabela_html.py` & `stnblipy-5.1.0/blipy/tabela_html.py`

 * *Files identical despite different names*

### Comparing `stnblipy-5.0.0/blipy/tabela_saida.py` & `stnblipy-5.1.0/blipy/tabela_saida.py`

 * *Files identical despite different names*

### Comparing `stnblipy-5.0.0/blipy/utils.py` & `stnblipy-5.1.0/blipy/utils.py`

 * *Files identical despite different names*

### Comparing `stnblipy-5.0.0/setup.py` & `stnblipy-5.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 0d0a 6672 6f6d 2073 6574 7570 746f 6f6c  ..from setuptool
 00000010: 7320 696d 706f 7274 2073 6574 7570 2c20  s import setup, 
 00000020: 6669 6e64 5f70 6163 6b61 6765 730d 0a0d  find_packages...
-00000030: 0a56 4552 5349 4f4e 203d 2027 352e 302e  .VERSION = '5.0.
+00000030: 0a56 4552 5349 4f4e 203d 2027 352e 312e  .VERSION = '5.1.
 00000040: 3027 200d 0a44 4553 4352 4950 5449 4f4e  0' ..DESCRIPTION
 00000050: 203d 2027 4672 616d 6577 6f72 6b20 7061   = 'Framework pa
 00000060: 7261 2072 6f74 696e 6173 2064 6520 4554  ra rotinas de ET
 00000070: 4c27 0d0a 4c4f 4e47 5f44 4553 4352 4950  L'..LONG_DESCRIP
 00000080: 5449 4f4e 203d 2027 4672 616d 6577 6f72  TION = 'Framewor
 00000090: 6b20 7061 7261 2073 696d 706c 6966 6963  k para simplific
 000000a0: 6172 206f 2064 6573 656e 766f 6c76 696d  ar o desenvolvim
```

### Comparing `stnblipy-5.0.0/stnblipy.egg-info/SOURCES.txt` & `stnblipy-5.1.0/stnblipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stnblipy-5.0.0/test/teste_conexao_json.py` & `stnblipy-5.1.0/test/teste_conexao_json.py`

 * *Files identical despite different names*

### Comparing `stnblipy-5.0.0/test/teste_estrategias_atualizacao.py` & `stnblipy-5.1.0/test/teste_estrategias_atualizacao.py`

 * *Files identical despite different names*

### Comparing `stnblipy-5.0.0/test/teste_geral.py` & `stnblipy-5.1.0/test/teste_geral.py`

 * *Files 2% similar despite different names*

```diff
@@ -512,83 +512,83 @@
 #         carrega_entes_arquivo(conn_stg)
 
 #     except:
 #         print("except")
 #         raise RuntimeError("Deu pau")
 
 
-class FormataNumero():
-    def transforma(self, entradas):
-        if entradas[0] is not None:
-            return entradas[0] / 100
-
-from datetime import datetime
-class StrParaData():
-    def transforma(self, entradas):
-        if entradas[0] is not None:
-            return datetime.strptime(entradas[0][:10], "%d/%m/%Y")
-        else:
-            return None
-
-class FormataData2():
-    def transforma(self, entradas):
-        if entradas[0] is not None:
-            return datetime.strptime(entradas[0], "%Y-%m-%d %H:%M:%S")
-        else:
-            return None
+# class FormataNumero():
+#     def transforma(self, entradas):
+#         if entradas[0] is not None:
+#             return entradas[0] / 100
+
+# from datetime import datetime
+# class StrParaData():
+#     def transforma(self, entradas):
+#         if entradas[0] is not None:
+#             return datetime.strptime(entradas[0][:10], "%d/%m/%Y")
+#         else:
+#             return None
+
+# class FormataData2():
+#     def transforma(self, entradas):
+#         if entradas[0] is not None:
+#             return datetime.strptime(entradas[0], "%Y-%m-%d %H:%M:%S")
+#         else:
+#             return None
  
-from blipy.enum_tipo_col_bd import TpColBD
-class StrToFloat():
-    def transforma(self, entradas):
-        if entradas[0] is not None and str(entradas[0]) != "nan":
-            return float(entradas[0])
-        else:
-            return None
-
-def carrega_arquivo_posicional(conn_stg):
-    job = Job("Carrega arquivo posicional")
-
-    cols_saida = [  
-        ["ANO", tp.NUMBER],
-        ["MES", tp.NUMBER],
-        ["NOME", tp.STRING],
-        # ["NOME", tp.STRING, StrToFloat()],
-        ["CODIGO", tp.NUMBER],
-        ["DIA", tp.DATE, StrParaData()],
-        # ["DIA", tp.DATE, FormataData2()],
-        # ["VALOR", tp.NUMBER, FormataNumero()],
-        ["VALOR", tp.NUMBER],
-        ["DATA1", tp.DATE, ft.StrParaData(ft.TpData.BR)], 
-        # ["DATA1", tp.DATE, ft.MontaDataMesAno(31, trata_ult_dia=True)], 
-        # ["DATA2", tp.DATE, ft.MontaDataMesAno(19)], 
-        ["DATA2", tp.DATE, ft.StrParaData(ft.TpData.UN)], 
-        ["DATA3", tp.DATE, ft.StrParaData(ft.TpData.UN_HF)], 
-        # ["DATA4", tp.DATE, ft.FormataData(ft.FmtDt.BR_SO_NUMEROS)], 
-        # ["DATA4", tp.DATE, ft.FormataData(ft.FmtDt.BR_SN)], 
-        # ["DATA4", tp.DATE, ft.StrParaData("%m%Y%d %H:%M:%S", ignora_horario=False)], 
-        # ["DATA4", tp.DATE, ft.StrParaData("%m%Y%d %H:%M:%S", ignora_horario=False)], 
-        ["DATA4", tp.DATE, ft.StrParaData(ft.TpData.UN_SN)], 
-    ]
-
-    job.importa_arquivo_csv(
-        conn_stg,
-        "ARQPOS",
-        cols_saida,
-        "arqpos_teste.csv",
-        decimal=",",
-        thousands=".",
-        # uso_cols=[0, 1, 2, 3, 4, 5, [1, 0], 7, 8, 9],
-        uso_cols=[0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
-        # qtd_linhas=2,
-        # header=1,
-        # engine="python",
-        # engine="c",
-        # skipfooter=None, 
-        skiprows=1,
-    )
+# from blipy.enum_tipo_col_bd import TpColBD
+# class StrToFloat():
+#     def transforma(self, entradas):
+#         if entradas[0] is not None and str(entradas[0]) != "nan":
+#             return float(entradas[0])
+#         else:
+#             return None
+
+# def carrega_arquivo_posicional(conn_stg):
+#     job = Job("Carrega arquivo posicional")
+
+#     cols_saida = [  
+#         ["ANO", tp.NUMBER],
+#         ["MES", tp.NUMBER],
+#         ["NOME", tp.STRING],
+#         # ["NOME", tp.STRING, StrToFloat()],
+#         ["CODIGO", tp.NUMBER],
+#         ["DIA", tp.DATE, StrParaData()],
+#         # ["DIA", tp.DATE, FormataData2()],
+#         # ["VALOR", tp.NUMBER, FormataNumero()],
+#         ["VALOR", tp.NUMBER],
+#         ["DATA1", tp.DATE, ft.StrParaData(ft.TpData.BR)], 
+#         # ["DATA1", tp.DATE, ft.MontaDataMesAno(31, trata_ult_dia=True)], 
+#         # ["DATA2", tp.DATE, ft.MontaDataMesAno(19)], 
+#         ["DATA2", tp.DATE, ft.StrParaData(ft.TpData.UN)], 
+#         ["DATA3", tp.DATE, ft.StrParaData(ft.TpData.UN_HF)], 
+#         # ["DATA4", tp.DATE, ft.FormataData(ft.FmtDt.BR_SO_NUMEROS)], 
+#         # ["DATA4", tp.DATE, ft.FormataData(ft.FmtDt.BR_SN)], 
+#         # ["DATA4", tp.DATE, ft.StrParaData("%m%Y%d %H:%M:%S", ignora_horario=False)], 
+#         # ["DATA4", tp.DATE, ft.StrParaData("%m%Y%d %H:%M:%S", ignora_horario=False)], 
+#         ["DATA4", tp.DATE, ft.StrParaData(ft.TpData.UN_SN)], 
+#     ]
+
+#     job.importa_arquivo_csv(
+#         conn_stg,
+#         "ARQPOS",
+#         cols_saida,
+#         "arqpos_teste.csv",
+#         decimal=",",
+#         thousands=".",
+#         # uso_cols=[0, 1, 2, 3, 4, 5, [1, 0], 7, 8, 9],
+#         uso_cols=[0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
+#         # qtd_linhas=2,
+#         # header=1,
+#         # engine="python",
+#         # engine="c",
+#         # skipfooter=None, 
+#         skiprows=1,
+#     )
 
     # tp_cols_entrada = [
     #     TpColBD.NUMBER, 
     #     TpColBD.NUMBER,
     #     TpColBD.NUMBER,
     #     TpColBD.NUMBER
     # ]
@@ -627,20 +627,44 @@
     #     # decimal=",",
     #     # cols=[0, 1, 2, 3],
     #     # ordem_uso_cols=[1, 1, 2, 3],
     #     # tp_cols_entrada=tp_cols_entrada,
     #     # estrategia=TpEstrategia.UPDATE_INSERT,
     #     # cols_chave_update=["ANO", "MES"]
     # )
-    
+
+def hash(conn_stg):
+    job = Job("Aplica hash")
+
+    cols_entrada = [
+        "ID_ABRANG",
+        "NO_ABRANG"
+    ]
+
+    cols_saida = [  
+        ["ID_ABRANG", tp.NUMBER],
+        ["NO_ABRANG_HASH", tp.STRING, ft.HashCPF()]
+    ]
+
+    job.importa_tabela_por_nome(
+        conn_stg,
+        conn_stg,
+        "ZZ_TESTE_HASH",
+        "ZZ_TESTE_HASH",
+        cols_entrada,
+        cols_saida,
+        estrategia=TpEstrategia.UPDATE,
+        cols_chave_update=["ID_ABRANG"]
+    )
+   
 
 if __name__ == "__main__":
     try:
         conn_stg, = ConexaoBD.from_json()
 
-        carrega_arquivo_posicional(conn_stg)
+        hash(conn_stg)
 
     except:
         print("except")
         raise RuntimeError("Deu pau")
         sys.exit(1)
```

### Comparing `stnblipy-5.0.0/test/teste_job.py` & `stnblipy-5.1.0/test/teste_job.py`

 * *Files identical despite different names*

### Comparing `stnblipy-5.0.0/test/testes_classe_planilha.py` & `stnblipy-5.1.0/test/testes_classe_planilha.py`

 * *Files identical despite different names*

