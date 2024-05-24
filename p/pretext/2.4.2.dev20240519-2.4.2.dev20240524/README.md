# Comparing `tmp/pretext-2.4.2.dev20240519.tar.gz` & `tmp/pretext-2.4.2.dev20240524.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-2.4.2.dev20240519.tar", max compression
+gzip compressed data, was "pretext-2.4.2.dev20240524.tar", max compression
```

## Comparing `pretext-2.4.2.dev20240519.tar` & `pretext-2.4.2.dev20240524.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0    35148 2024-05-19 06:13:31.913748 pretext-2.4.2.dev20240519/LICENSE
--rw-r--r--   0        0        0     9936 2024-05-19 06:13:31.913748 pretext-2.4.2.dev20240519/README.md
--rw-r--r--   0        0        0     1505 2024-05-19 06:14:12.110154 pretext-2.4.2.dev20240519/pretext/__init__.py
--rw-r--r--   0        0        0       61 2024-05-19 06:13:31.913748 pretext-2.4.2.dev20240519/pretext/__main__.py
--rw-r--r--   0        0        0    31364 2024-05-19 06:13:31.913748 pretext-2.4.2.dev20240519/pretext/cli.py
--rw-r--r--   0        0        0     6149 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/codechat.py
--rw-r--r--   0        0        0     3592 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/constants.py
--rw-r--r--   0        0        0      714 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/core/__init__.py
--rw-r--r--   0        0        0   185446 2024-05-19 06:14:15.966191 pretext-2.4.2.dev20240519/pretext/core/pretext.py
--rw-r--r--   0        0        0     1848 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/core/resources.py
--rw-r--r--   0        0        0  1130204 2024-05-19 06:14:15.966191 pretext-2.4.2.dev20240519/pretext/core/resources.zip
--rw-r--r--   0        0        0      409 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Alignment.jinja2s
--rw-r--r--   0        0        0      294 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Arrays.jinja2s
--rw-r--r--   0        0        0      198 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Bibliography.jinja2s
--rw-r--r--   0        0        0      236 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Boxes.jinja2s
--rw-r--r--   0        0        0      105 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Breaking.jinja2s
--rw-r--r--   0        0        0      634 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Crossref.jinja2s
--rw-r--r--   0        0        0      344 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Floats.jinja2s
--rw-r--r--   0        0        0     1476 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/FontSelection.jinja2s
--rw-r--r--   0        0        0       93 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Footnotes.jinja2s
--rwxr-xr-x   0        0        0      197 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Index.jinja2s
--rw-r--r--   0        0        0      343 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Lists.jinja2s
--rw-r--r--   0        0        0      172 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Pictures.jinja2s
--rw-r--r--   0        0        0      147 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Quotations.jinja2s
--rw-r--r--   0        0        0     2032 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Sectioning.jinja2s
--rw-r--r--   0        0        0      493 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Sentences.jinja2s
--rw-r--r--   0        0        0      329 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Space.jinja2s
--rw-r--r--   0        0        0       90 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Tabbing.jinja2s
--rw-r--r--   0        0        0        0 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Themes/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Themes/default/__init__.py
--rw-r--r--   0        0        0       51 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Themes/default/default-layout.jinja2
--rw-r--r--   0        0        0     1049 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Themes/default/document-layout.jinja2
--rw-r--r--   0        0        0      248 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Thms.jinja2s
--rw-r--r--   0        0        0       65 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/Verbatim.jinja2s
--rw-r--r--   0        0        0     1882 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/__init__.py
--rw-r--r--   0        0        0       66 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/babel.jinja2s
--rwxr-xr-x   0        0        0      263 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/graphicx.jinja2s
--rw-r--r--   0        0        0      652 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/hyperref.jinja2s
--rwxr-xr-x   0        0        0       27 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/lipsum.jinja2s
--rw-r--r--   0        0        0      251 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/longtable.jinja2s
--rw-r--r--   0        0        0      436 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/math.jinja2s
--rw-r--r--   0        0        0        0 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/misc.jinja2s
--rw-r--r--   0        0        0      270 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/natbib.jinja2s
--rw-r--r--   0        0        0       87 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/p.jinja2s
--rw-r--r--   0        0        0      673 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/subfig.jinja2s
--rw-r--r--   0        0        0      130 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/textcomp.jinja2s
--rw-r--r--   0        0        0       95 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/tikzcd.jinja2
--rw-r--r--   0        0        0       94 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/tikzpicture.jinja2
--rw-r--r--   0        0        0      184 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/url.jinja2s
--rwxr-xr-x   0        0        0       96 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/plastex/wrapfig.jinja2s
--rw-r--r--   0        0        0    66255 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/project/__init__.py
--rw-r--r--   0        0        0     3329 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/project/xml.py
--rw-r--r--   0        0        0     1173 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/templates/__init__.py
--rw-r--r--   0        0        0     3259 2024-05-19 06:14:16.050192 pretext-2.4.2.dev20240519/pretext/templates/resources/.devcontainer.json
--rw-r--r--   0        0        0     1939 2024-05-19 06:14:16.050192 pretext-2.4.2.dev20240519/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2024-05-19 06:14:16.050192 pretext-2.4.2.dev20240519/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160389 2024-05-19 06:14:16.050192 pretext-2.4.2.dev20240519/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0    10405 2024-05-19 06:14:16.022192 pretext-2.4.2.dev20240519/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0     3028 2024-05-19 06:14:16.050192 pretext-2.4.2.dev20240519/pretext/templates/resources/codechat_config.yaml
--rw-r--r--   0        0        0   174142 2024-05-19 06:14:16.042192 pretext-2.4.2.dev20240519/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     2456 2024-05-19 06:14:16.050192 pretext-2.4.2.dev20240519/pretext/templates/resources/deploy.yml
--rw-r--r--   0        0        0     5099 2024-05-19 06:14:16.026192 pretext-2.4.2.dev20240519/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0      432 2024-05-19 06:14:16.050192 pretext-2.4.2.dev20240519/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2024-05-19 06:14:16.050192 pretext-2.4.2.dev20240519/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8939 2024-05-19 06:14:16.026192 pretext-2.4.2.dev20240519/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0     1127 2024-05-19 06:14:16.050192 pretext-2.4.2.dev20240519/pretext/templates/resources/test-build.yml
--rw-r--r--   0        0        0      183 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/types.py
--rw-r--r--   0        0        0    27082 2024-05-19 06:13:31.917748 pretext-2.4.2.dev20240519/pretext/utils.py
--rw-r--r--   0        0        0     3813 2024-05-19 06:14:12.110154 pretext-2.4.2.dev20240519/pyproject.toml
--rw-r--r--   0        0        0    11165 1970-01-01 00:00:00.000000 pretext-2.4.2.dev20240519/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-05-24 06:15:19.907834 pretext-2.4.2.dev20240524/LICENSE
+-rw-r--r--   0        0        0     9936 2024-05-24 06:15:19.907834 pretext-2.4.2.dev20240524/README.md
+-rw-r--r--   0        0        0     1505 2024-05-24 06:16:05.212154 pretext-2.4.2.dev20240524/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/__main__.py
+-rw-r--r--   0        0        0    31370 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/cli.py
+-rw-r--r--   0        0        0     6149 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/codechat.py
+-rw-r--r--   0        0        0     3592 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/constants.py
+-rw-r--r--   0        0        0      714 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/core/__init__.py
+-rw-r--r--   0        0        0   185446 2024-05-24 06:16:09.520184 pretext-2.4.2.dev20240524/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1848 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/core/resources.py
+-rw-r--r--   0        0        0  1130204 2024-05-24 06:16:09.520184 pretext-2.4.2.dev20240524/pretext/core/resources.zip
+-rw-r--r--   0        0        0      409 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Alignment.jinja2s
+-rw-r--r--   0        0        0      294 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Arrays.jinja2s
+-rw-r--r--   0        0        0      198 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Bibliography.jinja2s
+-rw-r--r--   0        0        0      236 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Boxes.jinja2s
+-rw-r--r--   0        0        0      105 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Breaking.jinja2s
+-rw-r--r--   0        0        0      634 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Crossref.jinja2s
+-rw-r--r--   0        0        0      344 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Floats.jinja2s
+-rw-r--r--   0        0        0     1476 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/FontSelection.jinja2s
+-rw-r--r--   0        0        0       93 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Footnotes.jinja2s
+-rwxr-xr-x   0        0        0      197 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Index.jinja2s
+-rw-r--r--   0        0        0      343 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Lists.jinja2s
+-rw-r--r--   0        0        0      172 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Pictures.jinja2s
+-rw-r--r--   0        0        0      147 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Quotations.jinja2s
+-rw-r--r--   0        0        0     2032 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Sectioning.jinja2s
+-rw-r--r--   0        0        0      493 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Sentences.jinja2s
+-rw-r--r--   0        0        0      329 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Space.jinja2s
+-rw-r--r--   0        0        0       90 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Tabbing.jinja2s
+-rw-r--r--   0        0        0        0 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Themes/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Themes/default/__init__.py
+-rw-r--r--   0        0        0       51 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Themes/default/default-layout.jinja2
+-rw-r--r--   0        0        0     1049 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Themes/default/document-layout.jinja2
+-rw-r--r--   0        0        0      248 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Thms.jinja2s
+-rw-r--r--   0        0        0       65 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/Verbatim.jinja2s
+-rw-r--r--   0        0        0     1882 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/__init__.py
+-rw-r--r--   0        0        0       66 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/babel.jinja2s
+-rwxr-xr-x   0        0        0      263 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/graphicx.jinja2s
+-rw-r--r--   0        0        0      652 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/hyperref.jinja2s
+-rwxr-xr-x   0        0        0       27 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/lipsum.jinja2s
+-rw-r--r--   0        0        0      251 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/longtable.jinja2s
+-rw-r--r--   0        0        0      436 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/math.jinja2s
+-rw-r--r--   0        0        0        0 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/misc.jinja2s
+-rw-r--r--   0        0        0      270 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/natbib.jinja2s
+-rw-r--r--   0        0        0       87 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/p.jinja2s
+-rw-r--r--   0        0        0      673 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/subfig.jinja2s
+-rw-r--r--   0        0        0      130 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/textcomp.jinja2s
+-rw-r--r--   0        0        0       95 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/tikzcd.jinja2
+-rw-r--r--   0        0        0       94 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/tikzpicture.jinja2
+-rw-r--r--   0        0        0      184 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/url.jinja2s
+-rwxr-xr-x   0        0        0       96 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/plastex/wrapfig.jinja2s
+-rw-r--r--   0        0        0    66489 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/project/__init__.py
+-rw-r--r--   0        0        0     3329 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/project/xml.py
+-rw-r--r--   0        0        0     1173 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     3259 2024-05-24 06:16:09.604185 pretext-2.4.2.dev20240524/pretext/templates/resources/.devcontainer.json
+-rw-r--r--   0        0        0     1939 2024-05-24 06:16:09.604185 pretext-2.4.2.dev20240524/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2024-05-24 06:16:09.604185 pretext-2.4.2.dev20240524/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160389 2024-05-24 06:16:09.604185 pretext-2.4.2.dev20240524/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0    10405 2024-05-24 06:16:09.576185 pretext-2.4.2.dev20240524/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0     3028 2024-05-24 06:16:09.604185 pretext-2.4.2.dev20240524/pretext/templates/resources/codechat_config.yaml
+-rw-r--r--   0        0        0   174142 2024-05-24 06:16:09.596185 pretext-2.4.2.dev20240524/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2456 2024-05-24 06:16:09.604185 pretext-2.4.2.dev20240524/pretext/templates/resources/deploy.yml
+-rw-r--r--   0        0        0     5099 2024-05-24 06:16:09.580185 pretext-2.4.2.dev20240524/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0      432 2024-05-24 06:16:09.604185 pretext-2.4.2.dev20240524/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2024-05-24 06:16:09.604185 pretext-2.4.2.dev20240524/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8939 2024-05-24 06:16:09.584185 pretext-2.4.2.dev20240524/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0     1127 2024-05-24 06:16:09.604185 pretext-2.4.2.dev20240524/pretext/templates/resources/test-build.yml
+-rw-r--r--   0        0        0      183 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/types.py
+-rw-r--r--   0        0        0    27543 2024-05-24 06:15:19.911834 pretext-2.4.2.dev20240524/pretext/utils.py
+-rw-r--r--   0        0        0     3813 2024-05-24 06:16:05.212154 pretext-2.4.2.dev20240524/pyproject.toml
+-rw-r--r--   0        0        0    11165 1970-01-01 00:00:00.000000 pretext-2.4.2.dev20240524/PKG-INFO
```

### Comparing `pretext-2.4.2.dev20240519/LICENSE` & `pretext-2.4.2.dev20240524/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/README.md` & `pretext-2.4.2.dev20240524/README.md`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/__init__.py` & `pretext-2.4.2.dev20240524/pretext/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/cli.py` & `pretext-2.4.2.dev20240524/pretext/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         log.info(utils.project_xml_string())
         log.info("------------------------")
 
         # Create a project from the project.ptx file
         project = Project.parse()
         project.init_core()
 
-        for exec_name in project.get_executables().dict():
+        for exec_name in project.get_executables().model_dump():
             if utils.check_executable(exec_name) is None:
                 log.warning(
                     f"Unable to locate the command for <{exec_name}> on your system."
                 )
     else:
         log.info("No project.ptx found.")
```

### Comparing `pretext-2.4.2.dev20240519/pretext/codechat.py` & `pretext-2.4.2.dev20240524/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/constants.py` & `pretext-2.4.2.dev20240524/pretext/constants.py`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/core/__init__.py` & `pretext-2.4.2.dev20240524/pretext/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/core/pretext.py` & `pretext-2.4.2.dev20240524/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/core/resources.py` & `pretext-2.4.2.dev20240524/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/core/resources.zip` & `pretext-2.4.2.dev20240524/pretext/core/resources.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,196 +1,196 @@
 Zip file size: 1130204 bytes, number of entries: 194
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 css/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 js/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 js_lib/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 script/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 xsl/utilities/
--rw-r--r--  2.0 unx   552864 b- defN 24-May-19 06:14 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     1768 b- defN 24-May-19 06:14 xsl/README.md
--rw-r--r--  2.0 unx    17295 b- defN 24-May-19 06:14 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   608800 b- defN 24-May-19 06:14 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx    44062 b- defN 24-May-19 06:14 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    42242 b- defN 24-May-19 06:14 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx    11766 b- defN 24-May-19 06:14 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx    21086 b- defN 24-May-19 06:14 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx    40230 b- defN 24-May-19 06:14 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx     2601 b- defN 24-May-19 06:14 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx     8130 b- defN 24-May-19 06:14 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx     9787 b- defN 24-May-19 06:14 xsl/entities.ent
--rw-r--r--  2.0 unx     2847 b- defN 24-May-19 06:14 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx     6066 b- defN 24-May-19 06:14 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx     8134 b- defN 24-May-19 06:14 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx    22094 b- defN 24-May-19 06:14 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx     2597 b- defN 24-May-19 06:14 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx    12084 b- defN 24-May-19 06:14 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx     2248 b- defN 24-May-19 06:14 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx   132279 b- defN 24-May-19 06:14 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     2734 b- defN 24-May-19 06:14 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx    19092 b- defN 24-May-19 06:14 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx   120688 b- defN 24-May-19 06:14 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx     8783 b- defN 24-May-19 06:14 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     3239 b- defN 24-May-19 06:14 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx     3560 b- defN 24-May-19 06:14 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx    13037 b- defN 24-May-19 06:14 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx    95377 b- defN 24-May-19 06:14 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx    41730 b- defN 24-May-19 06:14 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx   551514 b- defN 24-May-19 06:14 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx    67630 b- defN 24-May-19 06:14 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx     2709 b- defN 24-May-19 06:14 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx    10708 b- defN 24-May-19 06:14 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx    13189 b- defN 24-May-19 06:14 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx   235477 b- defN 24-May-19 06:14 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   138087 b- defN 24-May-19 06:14 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx     2740 b- defN 24-May-19 06:14 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx     6281 b- defN 24-May-19 06:14 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     4571 b- defN 24-May-19 06:14 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx   173803 b- defN 24-May-19 06:14 xsl/html-symbols.xsl
--rw-r--r--  2.0 unx     4299 b- defN 24-May-19 06:14 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx     1810 b- defN 24-May-19 06:14 xsl/utilities/README.md
--rw-r--r--  2.0 unx      513 b- defN 24-May-19 06:14 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx    30257 b- defN 24-May-19 06:14 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4926 b- defN 24-May-19 06:14 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx      787 b- defN 24-May-19 06:14 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx     7277 b- defN 24-May-19 06:14 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 24-May-19 06:14 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     5135 b- defN 24-May-19 06:14 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx    14322 b- defN 24-May-19 06:14 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     2261 b- defN 24-May-19 06:14 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx     4810 b- defN 24-May-19 06:14 xsl/localizations/README.md
--rw-r--r--  2.0 unx    16904 b- defN 24-May-19 06:14 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    17122 b- defN 24-May-19 06:14 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    16378 b- defN 24-May-19 06:14 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    19453 b- defN 24-May-19 06:14 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    17297 b- defN 24-May-19 06:14 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16318 b- defN 24-May-19 06:14 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    19251 b- defN 24-May-19 06:14 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx     2347 b- defN 24-May-19 06:14 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    15648 b- defN 24-May-19 06:14 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    15924 b- defN 24-May-19 06:14 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16600 b- defN 24-May-19 06:14 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    16151 b- defN 24-May-19 06:14 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    17147 b- defN 24-May-19 06:14 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    16415 b- defN 24-May-19 06:14 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    19076 b- defN 24-May-19 06:14 xsl/localizations/zh-HANS.xml
--rw-r--r--  2.0 unx    20546 b- defN 24-May-19 06:14 xsl/localizations/ku-CKB.xml
--rw-r--r--  2.0 unx    16566 b- defN 24-May-19 06:14 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17368 b- defN 24-May-19 06:14 xsl/localizations/fi-FI.xml
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 xsl/support/play-button/
--rw-r--r--  2.0 unx      504 b- defN 24-May-19 06:14 xsl/support/README.md
--rw-r--r--  2.0 unx     5241 b- defN 24-May-19 06:14 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx     5879 b- defN 24-May-19 06:14 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx    10300 b- defN 24-May-19 06:14 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5800 b- defN 24-May-19 06:14 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx      522 b- defN 24-May-19 06:14 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5061 b- defN 24-May-19 06:14 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx     2657 b- defN 24-May-19 06:14 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx      722 b- defN 24-May-19 06:14 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     6621 b- defN 24-May-19 06:14 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx     1362 b- defN 24-May-19 06:14 css/epub.css
--rw-r--r--  2.0 unx    10602 b- defN 24-May-19 06:14 css/edit.css
--rw-r--r--  2.0 unx    14207 b- defN 24-May-19 06:14 css/setcolors.css
--rw-r--r--  2.0 unx     4308 b- defN 24-May-19 06:14 css/colors_blue_green.css
--rw-r--r--  2.0 unx      533 b- defN 24-May-19 06:14 css/toc_wide.css
--rw-r--r--  2.0 unx     2720 b- defN 24-May-19 06:14 css/pretext_search.css
--rw-r--r--  2.0 unx      691 b- defN 24-May-19 06:14 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx    74934 b- defN 24-May-19 06:14 css/pretext_add_on.css
--rw-r--r--  2.0 unx     1280 b- defN 24-May-19 06:14 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     3757 b- defN 24-May-19 06:14 css/colors_blue_red_dark.css
--rw-r--r--  2.0 unx     5875 b- defN 24-May-19 06:14 css/banner_crc.css
--rw-r--r--  2.0 unx     3769 b- defN 24-May-19 06:14 css/navbar_default.css
--rw-r--r--  2.0 unx     3818 b- defN 24-May-19 06:14 css/toc_min.css
--rw-r--r--  2.0 unx     1255 b- defN 24-May-19 06:14 css/colors_focused_gray_aqua.css
--rw-r--r--  2.0 unx      679 b- defN 24-May-19 06:14 css/navbar_wide.css
--rw-r--r--  2.0 unx     4236 b- defN 24-May-19 06:14 css/style_wide.css
--rw-r--r--  2.0 unx     3240 b- defN 24-May-19 06:14 css/banner_default.css
--rw-r--r--  2.0 unx    24707 b- defN 24-May-19 06:14 css/pretext.css
--rw-r--r--  2.0 unx     8496 b- defN 24-May-19 06:14 css/shell_crc.css
--rw-r--r--  2.0 unx     8179 b- defN 24-May-19 06:14 css/style_default.css
--rw-r--r--  2.0 unx     2438 b- defN 24-May-19 06:14 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2397 b- defN 24-May-19 06:14 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx     7521 b- defN 24-May-19 06:14 css/shell_wide.css
--rw-r--r--  2.0 unx     5836 b- defN 24-May-19 06:14 css/shell_min.css
--rw-r--r--  2.0 unx     2781 b- defN 24-May-19 06:14 css/colors_default.css
--rw-r--r--  2.0 unx     2397 b- defN 24-May-19 06:14 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     2397 b- defN 24-May-19 06:14 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2446 b- defN 24-May-19 06:14 css/colors_martiansands.css
--rw-r--r--  2.0 unx     9821 b- defN 24-May-19 06:14 css/toc_default.css
--rw-r--r--  2.0 unx     1102 b- defN 24-May-19 06:14 css/webwork.css
--rw-r--r--  2.0 unx     3473 b- defN 24-May-19 06:14 css/style_soundwriting.css
--rw-r--r--  2.0 unx     2441 b- defN 24-May-19 06:14 css/kindle.css
--rw-r--r--  2.0 unx     2397 b- defN 24-May-19 06:14 css/colors_orange_navy.css
--rw-r--r--  2.0 unx     4348 b- defN 24-May-19 06:14 css/colors_bluegreen_grey.css
--rw-r--r--  2.0 unx    13638 b- defN 24-May-19 06:14 css/style_oscarlevin.css
--rw-r--r--  2.0 unx     2397 b- defN 24-May-19 06:14 css/colors_green_blue.css
--rw-r--r--  2.0 unx     1207 b- defN 24-May-19 06:14 css/colors_focused_light.css
--rw-r--r--  2.0 unx     8096 b- defN 24-May-19 06:14 css/toc_crc.css
--rw-r--r--  2.0 unx     1338 b- defN 24-May-19 06:14 css/colors_red_blue.css
--rw-r--r--  2.0 unx     2397 b- defN 24-May-19 06:14 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     1804 b- defN 24-May-19 06:14 css/knowls_default.css
--rw-r--r--  2.0 unx     6966 b- defN 24-May-19 06:14 css/navbar_crc.css
--rw-r--r--  2.0 unx     1330 b- defN 24-May-19 06:14 css/reveal.css
--rw-r--r--  2.0 unx     2446 b- defN 24-May-19 06:14 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     5374 b- defN 24-May-19 06:14 css/shell_default.css
--rw-r--r--  2.0 unx     1276 b- defN 24-May-19 06:14 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx     6012 b- defN 24-May-19 06:14 css/features.css
--rw-r--r--  2.0 unx     1683 b- defN 24-May-19 06:14 css/catalog.css
--rw-r--r--  2.0 unx     2397 b- defN 24-May-19 06:14 css/colors_blue_red.css
--rw-r--r--  2.0 unx      389 b- defN 24-May-19 06:14 css/banner_wide.css
--rw-r--r--  2.0 unx    36176 b- defN 24-May-19 06:14 pretext/braille_format.py
--rw-r--r--  2.0 unx     1367 b- defN 24-May-19 06:14 pretext/README.md
--rw-r--r--  2.0 unx     2566 b- defN 24-May-19 06:14 pretext/pretext.cfg
--rw-r--r--  2.0 unx        0 b- defN 24-May-19 06:14 pretext/__init__.py
--rw-r--r--  2.0 unx    30970 b- defN 24-May-19 06:14 pretext/pretext
--rw-r--r--  2.0 unx     1955 b- defN 24-May-19 06:14 pretext/module-test.py
--rw-r--r--  2.0 unx   185446 b- defN 24-May-19 06:14 pretext/pretext.py
--rw-r--r--  2.0 unx      215 b- defN 24-May-19 06:14 pretext/requirements.txt
--rw-r--r--  2.0 unx    86927 b- defN 24-May-19 06:14 js_lib/jquery.min.js
--rw-r--r--  2.0 unx     6674 b- defN 24-May-19 06:14 js_lib/jquery.espy.min.js
--rw-r--r--  2.0 unx     5275 b- defN 24-May-19 06:14 js_lib/jquery.sticky.js
--rw-r--r--  2.0 unx    12611 b- defN 24-May-19 06:14 js_lib/knowl.js
--rw-r--r--  2.0 unx     1390 b- defN 24-May-19 06:14 js_lib/mathjaxknowl3.js
--rw-r--r--  2.0 unx     3177 b- defN 24-May-19 06:14 js_lib/mathjaxknowl.js
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 24-May-19 06:14 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 24-May-19 06:14 script/mbx
--rw-r--r--  2.0 unx      481 b- defN 24-May-19 06:14 script/mjsre/README.md
--rw-r--r--  2.0 unx      116 b- defN 24-May-19 06:14 script/mjsre/package.json
--rw-r--r--  2.0 unx       92 b- defN 24-May-19 06:14 script/mjsre/update-sre
--rw-r--r--  2.0 unx     9251 b- defN 24-May-19 06:14 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx     3135 b- defN 24-May-19 06:14 schema/build.sh
--rw-r--r--  2.0 unx     1180 b- defN 24-May-19 06:14 schema/README.md
--rw-r--r--  2.0 unx      326 b- defN 24-May-19 06:14 schema/xml.xsd
--rw-r--r--  2.0 unx   140214 b- defN 24-May-19 06:14 schema/pretext.xml
--rw-r--r--  2.0 unx    21415 b- defN 24-May-19 06:14 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx    60821 b- defN 24-May-19 06:14 schema/pretext.rnc
--rw-r--r--  2.0 unx   107306 b- defN 24-May-19 06:14 schema/pretext.rng
--rw-r--r--  2.0 unx      162 b- defN 24-May-19 06:14 schema/publication.xml
--rw-r--r--  2.0 unx   129207 b- defN 24-May-19 06:14 schema/pretext.xsd
--rw-r--r--  2.0 unx    39988 b- defN 24-May-19 06:14 schema/pretext-dev.rng
--rw-r--r--  2.0 unx    18421 b- defN 24-May-19 06:14 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx    25870 b- defN 24-May-19 06:14 schema/pretext-validation-plus.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 js/pretext-webwork/
--rw-r--r--  2.0 unx     3693 b- defN 24-May-19 06:14 js/ptx_search.js
--rw-r--r--  2.0 unx     5318 b- defN 24-May-19 06:14 js/instructor.js
--rw-r--r--  2.0 unx    42973 b- defN 24-May-19 06:14 js/pretext_add_on.js
--rw-r--r--  2.0 unx    10957 b- defN 24-May-19 06:14 js/login.js
--rw-r--r--  2.0 unx    23560 b- defN 24-May-19 06:14 js/highlight.js
--rw-r--r--  2.0 unx   228054 b- defN 24-May-19 06:14 js/edit.js
--rw-r--r--  2.0 unx    20911 b- defN 24-May-19 06:14 js/user_preferences.js
--rw-r--r--  2.0 unx    12113 b- defN 24-May-19 06:14 js/pretext_search.js
--rw-r--r--  2.0 unx    25633 b- defN 24-May-19 06:14 js/answer.js
--rw-r--r--  2.0 unx     6810 b- defN 24-May-19 06:14 js/pretext.js
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 js/pretext-webwork/2.16/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 js/pretext-webwork/2.17/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 js/pretext-webwork/2.18/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:14 js/pretext-webwork/2.19/
--rw-r--r--  2.0 unx    44152 b- defN 24-May-19 06:14 js/pretext-webwork/2.17/pretext-webwork.js
--rw-r--r--  2.0 unx    32570 b- defN 24-May-19 06:14 js/pretext-webwork/2.19/pretext-webwork.js
--rw-r--r--  2.0 unx    44152 b- defN 24-May-19 06:14 js/pretext-webwork/2.18/pretext-webwork.js
--rw-r--r--  2.0 unx    37123 b- defN 24-May-19 06:14 js/pretext-webwork/2.16/pretext-webwork.js
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 css/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 js/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 js_lib/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 script/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 xsl/utilities/
+-rw-r--r--  2.0 unx   552864 b- defN 24-May-24 06:16 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 24-May-24 06:16 xsl/README.md
+-rw-r--r--  2.0 unx    17295 b- defN 24-May-24 06:16 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   608800 b- defN 24-May-24 06:16 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx    44062 b- defN 24-May-24 06:16 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    42242 b- defN 24-May-24 06:16 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 24-May-24 06:16 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 24-May-24 06:16 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 24-May-24 06:16 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 24-May-24 06:16 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 24-May-24 06:16 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 24-May-24 06:16 xsl/entities.ent
+-rw-r--r--  2.0 unx     2847 b- defN 24-May-24 06:16 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 24-May-24 06:16 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx     8134 b- defN 24-May-24 06:16 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx    22094 b- defN 24-May-24 06:16 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 24-May-24 06:16 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 24-May-24 06:16 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 24-May-24 06:16 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx   132279 b- defN 24-May-24 06:16 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     2734 b- defN 24-May-24 06:16 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx    19092 b- defN 24-May-24 06:16 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx   120688 b- defN 24-May-24 06:16 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx     8783 b- defN 24-May-24 06:16 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 24-May-24 06:16 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 24-May-24 06:16 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 24-May-24 06:16 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx    95377 b- defN 24-May-24 06:16 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 24-May-24 06:16 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx   551514 b- defN 24-May-24 06:16 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx    67630 b- defN 24-May-24 06:16 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 24-May-24 06:16 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 24-May-24 06:16 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx    13189 b- defN 24-May-24 06:16 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx   235477 b- defN 24-May-24 06:16 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx   138087 b- defN 24-May-24 06:16 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 24-May-24 06:16 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 24-May-24 06:16 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 24-May-24 06:16 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx   173803 b- defN 24-May-24 06:16 xsl/html-symbols.xsl
+-rw-r--r--  2.0 unx     4299 b- defN 24-May-24 06:16 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx     1810 b- defN 24-May-24 06:16 xsl/utilities/README.md
+-rw-r--r--  2.0 unx      513 b- defN 24-May-24 06:16 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx    30257 b- defN 24-May-24 06:16 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 24-May-24 06:16 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx      787 b- defN 24-May-24 06:16 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx     7277 b- defN 24-May-24 06:16 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 24-May-24 06:16 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 24-May-24 06:16 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx    14322 b- defN 24-May-24 06:16 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 24-May-24 06:16 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx     4810 b- defN 24-May-24 06:16 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    16904 b- defN 24-May-24 06:16 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    17122 b- defN 24-May-24 06:16 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    16378 b- defN 24-May-24 06:16 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    19453 b- defN 24-May-24 06:16 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    17297 b- defN 24-May-24 06:16 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16318 b- defN 24-May-24 06:16 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    19251 b- defN 24-May-24 06:16 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx     2347 b- defN 24-May-24 06:16 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    15648 b- defN 24-May-24 06:16 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    15924 b- defN 24-May-24 06:16 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16600 b- defN 24-May-24 06:16 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    16151 b- defN 24-May-24 06:16 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    17147 b- defN 24-May-24 06:16 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    16415 b- defN 24-May-24 06:16 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    19076 b- defN 24-May-24 06:16 xsl/localizations/zh-HANS.xml
+-rw-r--r--  2.0 unx    20546 b- defN 24-May-24 06:16 xsl/localizations/ku-CKB.xml
+-rw-r--r--  2.0 unx    16566 b- defN 24-May-24 06:16 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17368 b- defN 24-May-24 06:16 xsl/localizations/fi-FI.xml
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 xsl/support/play-button/
+-rw-r--r--  2.0 unx      504 b- defN 24-May-24 06:16 xsl/support/README.md
+-rw-r--r--  2.0 unx     5241 b- defN 24-May-24 06:16 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 24-May-24 06:16 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx    10300 b- defN 24-May-24 06:16 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5800 b- defN 24-May-24 06:16 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx      522 b- defN 24-May-24 06:16 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5061 b- defN 24-May-24 06:16 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx     2657 b- defN 24-May-24 06:16 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx      722 b- defN 24-May-24 06:16 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     6621 b- defN 24-May-24 06:16 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx     1362 b- defN 24-May-24 06:16 css/epub.css
+-rw-r--r--  2.0 unx    10602 b- defN 24-May-24 06:16 css/edit.css
+-rw-r--r--  2.0 unx    14207 b- defN 24-May-24 06:16 css/setcolors.css
+-rw-r--r--  2.0 unx     4308 b- defN 24-May-24 06:16 css/colors_blue_green.css
+-rw-r--r--  2.0 unx      533 b- defN 24-May-24 06:16 css/toc_wide.css
+-rw-r--r--  2.0 unx     2720 b- defN 24-May-24 06:16 css/pretext_search.css
+-rw-r--r--  2.0 unx      691 b- defN 24-May-24 06:16 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx    74934 b- defN 24-May-24 06:16 css/pretext_add_on.css
+-rw-r--r--  2.0 unx     1280 b- defN 24-May-24 06:16 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     3757 b- defN 24-May-24 06:16 css/colors_blue_red_dark.css
+-rw-r--r--  2.0 unx     5875 b- defN 24-May-24 06:16 css/banner_crc.css
+-rw-r--r--  2.0 unx     3769 b- defN 24-May-24 06:16 css/navbar_default.css
+-rw-r--r--  2.0 unx     3818 b- defN 24-May-24 06:16 css/toc_min.css
+-rw-r--r--  2.0 unx     1255 b- defN 24-May-24 06:16 css/colors_focused_gray_aqua.css
+-rw-r--r--  2.0 unx      679 b- defN 24-May-24 06:16 css/navbar_wide.css
+-rw-r--r--  2.0 unx     4236 b- defN 24-May-24 06:16 css/style_wide.css
+-rw-r--r--  2.0 unx     3240 b- defN 24-May-24 06:16 css/banner_default.css
+-rw-r--r--  2.0 unx    24707 b- defN 24-May-24 06:16 css/pretext.css
+-rw-r--r--  2.0 unx     8496 b- defN 24-May-24 06:16 css/shell_crc.css
+-rw-r--r--  2.0 unx     8179 b- defN 24-May-24 06:16 css/style_default.css
+-rw-r--r--  2.0 unx     2438 b- defN 24-May-24 06:16 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-May-24 06:16 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx     7521 b- defN 24-May-24 06:16 css/shell_wide.css
+-rw-r--r--  2.0 unx     5836 b- defN 24-May-24 06:16 css/shell_min.css
+-rw-r--r--  2.0 unx     2781 b- defN 24-May-24 06:16 css/colors_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-May-24 06:16 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-May-24 06:16 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     2446 b- defN 24-May-24 06:16 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     9821 b- defN 24-May-24 06:16 css/toc_default.css
+-rw-r--r--  2.0 unx     1102 b- defN 24-May-24 06:16 css/webwork.css
+-rw-r--r--  2.0 unx     3473 b- defN 24-May-24 06:16 css/style_soundwriting.css
+-rw-r--r--  2.0 unx     2441 b- defN 24-May-24 06:16 css/kindle.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-May-24 06:16 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx     4348 b- defN 24-May-24 06:16 css/colors_bluegreen_grey.css
+-rw-r--r--  2.0 unx    13638 b- defN 24-May-24 06:16 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-May-24 06:16 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     1207 b- defN 24-May-24 06:16 css/colors_focused_light.css
+-rw-r--r--  2.0 unx     8096 b- defN 24-May-24 06:16 css/toc_crc.css
+-rw-r--r--  2.0 unx     1338 b- defN 24-May-24 06:16 css/colors_red_blue.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-May-24 06:16 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     1804 b- defN 24-May-24 06:16 css/knowls_default.css
+-rw-r--r--  2.0 unx     6966 b- defN 24-May-24 06:16 css/navbar_crc.css
+-rw-r--r--  2.0 unx     1330 b- defN 24-May-24 06:16 css/reveal.css
+-rw-r--r--  2.0 unx     2446 b- defN 24-May-24 06:16 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     5374 b- defN 24-May-24 06:16 css/shell_default.css
+-rw-r--r--  2.0 unx     1276 b- defN 24-May-24 06:16 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx     6012 b- defN 24-May-24 06:16 css/features.css
+-rw-r--r--  2.0 unx     1683 b- defN 24-May-24 06:16 css/catalog.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-May-24 06:16 css/colors_blue_red.css
+-rw-r--r--  2.0 unx      389 b- defN 24-May-24 06:16 css/banner_wide.css
+-rw-r--r--  2.0 unx    36176 b- defN 24-May-24 06:16 pretext/braille_format.py
+-rw-r--r--  2.0 unx     1367 b- defN 24-May-24 06:16 pretext/README.md
+-rw-r--r--  2.0 unx     2566 b- defN 24-May-24 06:16 pretext/pretext.cfg
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 06:16 pretext/__init__.py
+-rw-r--r--  2.0 unx    30970 b- defN 24-May-24 06:16 pretext/pretext
+-rw-r--r--  2.0 unx     1955 b- defN 24-May-24 06:16 pretext/module-test.py
+-rw-r--r--  2.0 unx   185446 b- defN 24-May-24 06:16 pretext/pretext.py
+-rw-r--r--  2.0 unx      215 b- defN 24-May-24 06:16 pretext/requirements.txt
+-rw-r--r--  2.0 unx    86927 b- defN 24-May-24 06:16 js_lib/jquery.min.js
+-rw-r--r--  2.0 unx     6674 b- defN 24-May-24 06:16 js_lib/jquery.espy.min.js
+-rw-r--r--  2.0 unx     5275 b- defN 24-May-24 06:16 js_lib/jquery.sticky.js
+-rw-r--r--  2.0 unx    12611 b- defN 24-May-24 06:16 js_lib/knowl.js
+-rw-r--r--  2.0 unx     1390 b- defN 24-May-24 06:16 js_lib/mathjaxknowl3.js
+-rw-r--r--  2.0 unx     3177 b- defN 24-May-24 06:16 js_lib/mathjaxknowl.js
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 24-May-24 06:16 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 24-May-24 06:16 script/mbx
+-rw-r--r--  2.0 unx      481 b- defN 24-May-24 06:16 script/mjsre/README.md
+-rw-r--r--  2.0 unx      116 b- defN 24-May-24 06:16 script/mjsre/package.json
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 06:16 script/mjsre/update-sre
+-rw-r--r--  2.0 unx     9251 b- defN 24-May-24 06:16 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx     3135 b- defN 24-May-24 06:16 schema/build.sh
+-rw-r--r--  2.0 unx     1180 b- defN 24-May-24 06:16 schema/README.md
+-rw-r--r--  2.0 unx      326 b- defN 24-May-24 06:16 schema/xml.xsd
+-rw-r--r--  2.0 unx   140214 b- defN 24-May-24 06:16 schema/pretext.xml
+-rw-r--r--  2.0 unx    21415 b- defN 24-May-24 06:16 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx    60821 b- defN 24-May-24 06:16 schema/pretext.rnc
+-rw-r--r--  2.0 unx   107306 b- defN 24-May-24 06:16 schema/pretext.rng
+-rw-r--r--  2.0 unx      162 b- defN 24-May-24 06:16 schema/publication.xml
+-rw-r--r--  2.0 unx   129207 b- defN 24-May-24 06:16 schema/pretext.xsd
+-rw-r--r--  2.0 unx    39988 b- defN 24-May-24 06:16 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx    18421 b- defN 24-May-24 06:16 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx    25870 b- defN 24-May-24 06:16 schema/pretext-validation-plus.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 js/pretext-webwork/
+-rw-r--r--  2.0 unx     3693 b- defN 24-May-24 06:16 js/ptx_search.js
+-rw-r--r--  2.0 unx     5318 b- defN 24-May-24 06:16 js/instructor.js
+-rw-r--r--  2.0 unx    42973 b- defN 24-May-24 06:16 js/pretext_add_on.js
+-rw-r--r--  2.0 unx    10957 b- defN 24-May-24 06:16 js/login.js
+-rw-r--r--  2.0 unx    23560 b- defN 24-May-24 06:16 js/highlight.js
+-rw-r--r--  2.0 unx   228054 b- defN 24-May-24 06:16 js/edit.js
+-rw-r--r--  2.0 unx    20911 b- defN 24-May-24 06:16 js/user_preferences.js
+-rw-r--r--  2.0 unx    12113 b- defN 24-May-24 06:16 js/pretext_search.js
+-rw-r--r--  2.0 unx    25633 b- defN 24-May-24 06:16 js/answer.js
+-rw-r--r--  2.0 unx     6810 b- defN 24-May-24 06:16 js/pretext.js
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 js/pretext-webwork/2.16/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 js/pretext-webwork/2.17/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 js/pretext-webwork/2.18/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:16 js/pretext-webwork/2.19/
+-rw-r--r--  2.0 unx    44152 b- defN 24-May-24 06:16 js/pretext-webwork/2.17/pretext-webwork.js
+-rw-r--r--  2.0 unx    32570 b- defN 24-May-24 06:16 js/pretext-webwork/2.19/pretext-webwork.js
+-rw-r--r--  2.0 unx    44152 b- defN 24-May-24 06:16 js/pretext-webwork/2.18/pretext-webwork.js
+-rw-r--r--  2.0 unx    37123 b- defN 24-May-24 06:16 js/pretext-webwork/2.16/pretext-webwork.js
 194 files, 5246038 bytes uncompressed, 1106506 bytes compressed:  78.9%
```

### Comparing `pretext-2.4.2.dev20240519/pretext/plastex/Crossref.jinja2s` & `pretext-2.4.2.dev20240524/pretext/plastex/Crossref.jinja2s`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/plastex/FontSelection.jinja2s` & `pretext-2.4.2.dev20240524/pretext/plastex/FontSelection.jinja2s`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/plastex/Sectioning.jinja2s` & `pretext-2.4.2.dev20240524/pretext/plastex/Sectioning.jinja2s`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/plastex/Themes/default/document-layout.jinja2` & `pretext-2.4.2.dev20240524/pretext/plastex/Themes/default/document-layout.jinja2`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/plastex/__init__.py` & `pretext-2.4.2.dev20240524/pretext/plastex/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/plastex/hyperref.jinja2s` & `pretext-2.4.2.dev20240524/pretext/plastex/hyperref.jinja2s`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/plastex/subfig.jinja2s` & `pretext-2.4.2.dev20240524/pretext/plastex/subfig.jinja2s`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/project/__init__.py` & `pretext-2.4.2.dev20240524/pretext/project/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1266,15 +1266,21 @@
             args=[self.abspath(), access, port],
         )
 
     def get_executables(self) -> Executables:
         return self._executables
 
     def init_core(self) -> None:
-        core.set_executables(self._executables.model_dump())
+        # core does not support None as an executable value, so we must
+        # adjust accordingly
+        exec_dict = self._executables.model_dump()
+        for k in exec_dict:
+            if exec_dict[k] is None:
+                exec_dict[k] = "None"
+        core.set_executables(exec_dict)
 
     def deploy_targets(self) -> t.List[Target]:
         return [target for target in self.targets if target.deploy_dir is not None]
 
     def stage_deployment(self) -> None:
         # Ensure stage directory exists
         self.stage_abspath().mkdir(parents=True, exist_ok=True)
```

### Comparing `pretext-2.4.2.dev20240519/pretext/project/xml.py` & `pretext-2.4.2.dev20240524/pretext/project/xml.py`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/templates/__init__.py` & `pretext-2.4.2.dev20240524/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/templates/resources/.devcontainer.json` & `pretext-2.4.2.dev20240524/pretext/templates/resources/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/templates/resources/.gitignore` & `pretext-2.4.2.dev20240524/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/templates/resources/article.zip` & `pretext-2.4.2.dev20240524/pretext/templates/resources/article.zip`

 * *Files 3% similar despite different names*

#### zipinfo {}

```diff
@@ -1,15 +1,15 @@
 Zip file size: 160389 bytes, number of entries: 13
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:13 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:13 source/
--rw-r--r--  2.0 unx       86 b- defN 24-May-19 06:13 README.md
--rw-r--r--  2.0 unx     1939 b- defN 24-May-19 06:14 .gitignore
--rw-r--r--  2.0 unx     3259 b- defN 24-May-19 06:14 .devcontainer.json
--rw-r--r--  2.0 unx      432 b- defN 24-May-19 06:14 project.ptx
--rw-r--r--  2.0 unx     3028 b- defN 24-May-19 06:14 codechat_config.yaml
--rw-r--r--  2.0 unx      242 b- defN 24-May-19 06:13 publication/publication.ptx
--rw-r--r--  2.0 unx      430 b- defN 24-May-19 06:13 source/main.ptx
--rw-r--r--  2.0 unx      765 b- defN 24-May-19 06:13 source/section-2.ptx
--rw-r--r--  2.0 unx      576 b- defN 24-May-19 06:13 source/section-1.ptx
--rw-r--r--  2.0 unx   154806 b- defN 24-May-19 06:13 assets/frog.jpg
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:15 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:15 source/
+-rw-r--r--  2.0 unx       86 b- defN 24-May-24 06:15 README.md
+-rw-r--r--  2.0 unx     1939 b- defN 24-May-24 06:16 .gitignore
+-rw-r--r--  2.0 unx     3259 b- defN 24-May-24 06:16 .devcontainer.json
+-rw-r--r--  2.0 unx      432 b- defN 24-May-24 06:16 project.ptx
+-rw-r--r--  2.0 unx     3028 b- defN 24-May-24 06:16 codechat_config.yaml
+-rw-r--r--  2.0 unx      242 b- defN 24-May-24 06:15 publication/publication.ptx
+-rw-r--r--  2.0 unx      430 b- defN 24-May-24 06:15 source/main.ptx
+-rw-r--r--  2.0 unx      765 b- defN 24-May-24 06:15 source/section-2.ptx
+-rw-r--r--  2.0 unx      576 b- defN 24-May-24 06:15 source/section-1.ptx
+-rw-r--r--  2.0 unx   154806 b- defN 24-May-24 06:15 assets/frog.jpg
 13 files, 165563 bytes uncompressed, 158997 bytes compressed:  4.0%
```

### Comparing `pretext-2.4.2.dev20240519/pretext/templates/resources/book.zip` & `pretext-2.4.2.dev20240524/pretext/templates/resources/book.zip`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 10405 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:13 source/
--rw-r--r--  2.0 unx       82 b- defN 24-May-19 06:13 README.md
--rw-r--r--  2.0 unx     1939 b- defN 24-May-19 06:14 .gitignore
--rw-r--r--  2.0 unx     3259 b- defN 24-May-19 06:14 .devcontainer.json
--rw-r--r--  2.0 unx      432 b- defN 24-May-19 06:14 project.ptx
--rw-r--r--  2.0 unx     3028 b- defN 24-May-19 06:14 codechat_config.yaml
--rw-r--r--  2.0 unx     6207 b- defN 24-May-19 06:13 publication/publication.ptx
--rw-r--r--  2.0 unx     2131 b- defN 24-May-19 06:13 source/docinfo.ptx
--rw-r--r--  2.0 unx      597 b- defN 24-May-19 06:13 source/main.ptx
--rw-r--r--  2.0 unx      873 b- defN 24-May-19 06:13 source/backmatter.ptx
--rw-r--r--  2.0 unx      315 b- defN 24-May-19 06:13 source/ch-chapter-title.ptx
--rw-r--r--  2.0 unx      190 b- defN 24-May-19 06:13 source/sec-section-name.ptx
--rw-r--r--  2.0 unx     1047 b- defN 24-May-19 06:13 source/frontmatter.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:15 source/
+-rw-r--r--  2.0 unx       82 b- defN 24-May-24 06:15 README.md
+-rw-r--r--  2.0 unx     1939 b- defN 24-May-24 06:16 .gitignore
+-rw-r--r--  2.0 unx     3259 b- defN 24-May-24 06:16 .devcontainer.json
+-rw-r--r--  2.0 unx      432 b- defN 24-May-24 06:16 project.ptx
+-rw-r--r--  2.0 unx     3028 b- defN 24-May-24 06:16 codechat_config.yaml
+-rw-r--r--  2.0 unx     6207 b- defN 24-May-24 06:15 publication/publication.ptx
+-rw-r--r--  2.0 unx     2131 b- defN 24-May-24 06:15 source/docinfo.ptx
+-rw-r--r--  2.0 unx      597 b- defN 24-May-24 06:15 source/main.ptx
+-rw-r--r--  2.0 unx      873 b- defN 24-May-24 06:15 source/backmatter.ptx
+-rw-r--r--  2.0 unx      315 b- defN 24-May-24 06:15 source/ch-chapter-title.ptx
+-rw-r--r--  2.0 unx      190 b- defN 24-May-24 06:15 source/sec-section-name.ptx
+-rw-r--r--  2.0 unx     1047 b- defN 24-May-24 06:15 source/frontmatter.ptx
 14 files, 20100 bytes uncompressed, 8831 bytes compressed:  56.1%
```

### Comparing `pretext-2.4.2.dev20240519/pretext/templates/resources/codechat_config.yaml` & `pretext-2.4.2.dev20240524/pretext/templates/resources/codechat_config.yaml`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/templates/resources/demo.zip` & `pretext-2.4.2.dev20240524/pretext/templates/resources/demo.zip`

 * *Files 6% similar despite different names*

#### zipinfo {}

```diff
@@ -1,36 +1,36 @@
 Zip file size: 174142 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:13 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:13 source/
--rw-r--r--  2.0 unx       82 b- defN 24-May-19 06:13 README.md
--rw-r--r--  2.0 unx     1939 b- defN 24-May-19 06:14 .gitignore
--rw-r--r--  2.0 unx     3259 b- defN 24-May-19 06:14 .devcontainer.json
--rw-r--r--  2.0 unx      432 b- defN 24-May-19 06:14 project.ptx
--rw-r--r--  2.0 unx     3028 b- defN 24-May-19 06:14 codechat_config.yaml
--rw-r--r--  2.0 unx     6092 b- defN 24-May-19 06:13 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:13 source/images/
--rw-r--r--  2.0 unx     2427 b- defN 24-May-19 06:13 source/docinfo.ptx
--rw-r--r--  2.0 unx      375 b- defN 24-May-19 06:13 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx     2428 b- defN 24-May-19 06:13 source/main.ptx
--rw-r--r--  2.0 unx      777 b- defN 24-May-19 06:13 source/ww.ptx
--rw-r--r--  2.0 unx      339 b- defN 24-May-19 06:13 source/ch-features.ptx
--rw-r--r--  2.0 unx      229 b- defN 24-May-19 06:13 source/ch-empty.ptx
--rw-r--r--  2.0 unx      411 b- defN 24-May-19 06:13 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx      885 b- defN 24-May-19 06:13 source/backmatter.ptx
--rw-r--r--  2.0 unx      847 b- defN 24-May-19 06:13 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx     2531 b- defN 24-May-19 06:13 source/ch-generate.ptx
--rw-r--r--  2.0 unx      335 b- defN 24-May-19 06:13 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx     1697 b- defN 24-May-19 06:13 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      381 b- defN 24-May-19 06:13 source/fig-tikz.ptx
--rw-r--r--  2.0 unx     1515 b- defN 24-May-19 06:13 source/ex-first.ptx
--rw-r--r--  2.0 unx     1115 b- defN 24-May-19 06:13 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx     2050 b- defN 24-May-19 06:13 source/frontmatter.ptx
--rw-r--r--  2.0 unx      867 b- defN 24-May-19 06:13 source/sec-features.ptx
--rw-r--r--  2.0 unx      357 b- defN 24-May-19 06:13 source/images/tikz.tex
--rw-r--r--  2.0 unx       93 b- defN 24-May-19 06:13 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx       10 b- defN 24-May-19 06:13 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx      835 b- defN 24-May-19 06:13 source/images/cflag.asy
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:13 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 24-May-19 06:13 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 24-May-19 06:13 assets/jsxgraph/infinity.js
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:15 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:15 source/
+-rw-r--r--  2.0 unx       82 b- defN 24-May-24 06:15 README.md
+-rw-r--r--  2.0 unx     1939 b- defN 24-May-24 06:16 .gitignore
+-rw-r--r--  2.0 unx     3259 b- defN 24-May-24 06:16 .devcontainer.json
+-rw-r--r--  2.0 unx      432 b- defN 24-May-24 06:16 project.ptx
+-rw-r--r--  2.0 unx     3028 b- defN 24-May-24 06:16 codechat_config.yaml
+-rw-r--r--  2.0 unx     6092 b- defN 24-May-24 06:15 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:15 source/images/
+-rw-r--r--  2.0 unx     2427 b- defN 24-May-24 06:15 source/docinfo.ptx
+-rw-r--r--  2.0 unx      375 b- defN 24-May-24 06:15 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx     2428 b- defN 24-May-24 06:15 source/main.ptx
+-rw-r--r--  2.0 unx      777 b- defN 24-May-24 06:15 source/ww.ptx
+-rw-r--r--  2.0 unx      339 b- defN 24-May-24 06:15 source/ch-features.ptx
+-rw-r--r--  2.0 unx      229 b- defN 24-May-24 06:15 source/ch-empty.ptx
+-rw-r--r--  2.0 unx      411 b- defN 24-May-24 06:15 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx      885 b- defN 24-May-24 06:15 source/backmatter.ptx
+-rw-r--r--  2.0 unx      847 b- defN 24-May-24 06:15 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx     2531 b- defN 24-May-24 06:15 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      335 b- defN 24-May-24 06:15 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 24-May-24 06:15 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      381 b- defN 24-May-24 06:15 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 24-May-24 06:15 source/ex-first.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 24-May-24 06:15 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx     2050 b- defN 24-May-24 06:15 source/frontmatter.ptx
+-rw-r--r--  2.0 unx      867 b- defN 24-May-24 06:15 source/sec-features.ptx
+-rw-r--r--  2.0 unx      357 b- defN 24-May-24 06:15 source/images/tikz.tex
+-rw-r--r--  2.0 unx       93 b- defN 24-May-24 06:15 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx       10 b- defN 24-May-24 06:15 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx      835 b- defN 24-May-24 06:15 source/images/cflag.asy
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:15 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 24-May-24 06:15 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-24 06:15 assets/jsxgraph/infinity.js
 34 files, 191879 bytes uncompressed, 170214 bytes compressed:  11.3%
```

### Comparing `pretext-2.4.2.dev20240519/pretext/templates/resources/deploy.yml` & `pretext-2.4.2.dev20240524/pretext/templates/resources/deploy.yml`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/templates/resources/hello.zip` & `pretext-2.4.2.dev20240524/pretext/templates/resources/hello.zip`

 * *Files 17% similar despite different names*

#### zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 5099 bytes, number of entries: 9
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:13 source/
--rw-r--r--  2.0 unx       69 b- defN 24-May-19 06:13 README.md
--rw-r--r--  2.0 unx     1939 b- defN 24-May-19 06:14 .gitignore
--rw-r--r--  2.0 unx     3259 b- defN 24-May-19 06:14 .devcontainer.json
--rw-r--r--  2.0 unx      432 b- defN 24-May-19 06:14 project.ptx
--rw-r--r--  2.0 unx     3028 b- defN 24-May-19 06:14 codechat_config.yaml
--rw-r--r--  2.0 unx      242 b- defN 24-May-19 06:13 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 24-May-19 06:13 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:15 source/
+-rw-r--r--  2.0 unx       69 b- defN 24-May-24 06:15 README.md
+-rw-r--r--  2.0 unx     1939 b- defN 24-May-24 06:16 .gitignore
+-rw-r--r--  2.0 unx     3259 b- defN 24-May-24 06:16 .devcontainer.json
+-rw-r--r--  2.0 unx      432 b- defN 24-May-24 06:16 project.ptx
+-rw-r--r--  2.0 unx     3028 b- defN 24-May-24 06:16 codechat_config.yaml
+-rw-r--r--  2.0 unx      242 b- defN 24-May-24 06:15 publication/publication.ptx
+-rw-r--r--  2.0 unx      156 b- defN 24-May-24 06:15 source/main.ptx
 9 files, 9125 bytes uncompressed, 4135 bytes compressed:  54.7%
```

### Comparing `pretext-2.4.2.dev20240519/pretext/templates/resources/slideshow.zip` & `pretext-2.4.2.dev20240524/pretext/templates/resources/slideshow.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 8939 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:13 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:13 source/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-19 06:13 xsl/
--rw-r--r--  2.0 unx     1939 b- defN 24-May-19 06:14 .gitignore
--rw-r--r--  2.0 unx     3259 b- defN 24-May-19 06:14 .devcontainer.json
--rw-r--r--  2.0 unx      480 b- defN 24-May-19 06:13 project.ptx
--rw-r--r--  2.0 unx     3028 b- defN 24-May-19 06:14 codechat_config.yaml
--rw-r--r--  2.0 unx      190 b- defN 24-May-19 06:13 xsl/slides.xsl
--rw-r--r--  2.0 unx     2097 b- defN 24-May-19 06:13 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 24-May-19 06:13 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:15 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:15 source/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-24 06:15 xsl/
+-rw-r--r--  2.0 unx     1939 b- defN 24-May-24 06:16 .gitignore
+-rw-r--r--  2.0 unx     3259 b- defN 24-May-24 06:16 .devcontainer.json
+-rw-r--r--  2.0 unx      480 b- defN 24-May-24 06:15 project.ptx
+-rw-r--r--  2.0 unx     3028 b- defN 24-May-24 06:16 codechat_config.yaml
+-rw-r--r--  2.0 unx      190 b- defN 24-May-24 06:15 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2097 b- defN 24-May-24 06:15 publication/publication.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 24-May-24 06:15 source/main.ptx
 10 files, 22193 bytes uncompressed, 7881 bytes compressed:  64.5%
```

### Comparing `pretext-2.4.2.dev20240519/pretext/templates/resources/test-build.yml` & `pretext-2.4.2.dev20240524/pretext/templates/resources/test-build.yml`

 * *Files identical despite different names*

### Comparing `pretext-2.4.2.dev20240519/pretext/utils.py` & `pretext-2.4.2.dev20240524/pretext/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -574,23 +574,34 @@
         log.info("")
         log.info(
             "And if you haven't already, create a remote GitHub repository for this project at:"
         )
         log.info("    https://github.com/new")
         log.info('(Do NOT check any "initialize" options.)')
         log.info(
-            'On the next page, copy the URL in the "Quick Setup" section (use HTTPS unless you have SSH setup already).'
+            'On the next page, copy the "HTTPS" version of the URL in the "Quick Setup" section.'
         )
         log.info("")
-        repourl = input("Paste url here: ").strip()
-        repo.create_remote("origin", url=repourl)
-        origin = repo.remotes.origin
+        repourl = input("Paste url here: ")
+        username = repourl.split("/")[-2]
+        reponame = repourl.split("/")[-1]
+        log.info("")
+        log.info("Next, set up a GitHub personal access token. Instructions:")
+        log.info(
+            "    https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#creating-a-personal-access-token-classic"
+        )
         log.info(
-            "\nFor information about authentication options for github, see: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/about-authentication-to-github\n"
+            "Be sure to check the `repo` and `workflow` scopes when generating this token."
         )
+        log.info("")
+        pat = input("Paste your personal access token (`ghp_RANDOMCHARCTERS`): ")
+        log.info("")
+        repourl = f"https://{username}:{pat}@github.com/{username}/{reponame}"
+        repo.create_remote("origin", url=repourl)
+        origin = repo.remotes.origin
     log.info("Committing your latest build to the `gh-pages` branch.")
     log.info("")
     ghp_import.ghp_import(
         directory,
         mesg="Latest build deployed.",
         nojekyll=True,
     )
```

### Comparing `pretext-2.4.2.dev20240519/pyproject.toml` & `pretext-2.4.2.dev20240524/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # See https://python-poetry.org/docs/dependency-specification/ to get an understanding of
 # how poetry specifies dependencies.
 #
 # Project metadata
 # ----------------
 [tool.poetry]
 name = "pretext"
-version = "2.4.2.dev20240519"
+version = "2.4.2.dev20240524"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-2.4.2.dev20240519/PKG-INFO` & `pretext-2.4.2.dev20240524/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 2.4.2.dev20240519
+Version: 2.4.2.dev20240524
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

