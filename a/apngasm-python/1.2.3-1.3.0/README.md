# Comparing `tmp/apngasm_python-1.2.3.tar.gz` & `tmp/apngasm_python-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apngasm_python-1.2.3.tar", last modified: Wed Feb  7 02:09:34 2024, max compression
+gzip compressed data, was "apngasm_python-1.3.0.tar", last modified: Fri May 24 02:41:40 2024, max compression
```

## Comparing `apngasm_python-1.2.3.tar` & `apngasm_python-1.3.0.tar`

### file list

```diff
@@ -1,264 +1,263 @@
--rw-r--r--   0        0        0     4486 2024-02-07 02:09:20.576291 apngasm_python-1.2.3/CMakeLists.txt
--rw-r--r--   0        0        0    26526 2024-02-07 02:09:20.576291 apngasm_python-1.2.3/LICENSE
--rw-r--r--   0        0        0     5330 2024-02-07 02:09:20.576291 apngasm_python-1.2.3/README.md
--rw-r--r--   0        0        0       32 2024-02-07 02:09:21.108287 apngasm_python-1.2.3/apngasm/.git
--rw-r--r--   0        0        0     3136 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/.github/workflows/build.yml
--rw-r--r--   0        0        0      624 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/.gitignore
--rw-r--r--   0        0        0    18247 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/BACKERS.txt
--rw-r--r--   0        0        0     1049 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/CMakeLists.txt
--rw-r--r--   0        0        0      861 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/LICENSE.txt
--rw-r--r--   0        0        0     4764 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/README.md
--rw-r--r--   0        0        0     2742 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/cli/CMakeLists.txt
--rw-r--r--   0        0        0      462 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/cli/DESCRIPTION.txt
--rw-r--r--   0        0        0      861 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/cli/LICENSE.txt
--rw-r--r--   0        0        0     1559 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/cli/package/CMakeLists.txt.in
--rw-r--r--   0        0        0      217 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/cli/src/apngasm-cli-version.h.in
--rw-r--r--   0        0        0      440 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/cli/src/apngasm-cli.cpp
--rw-r--r--   0        0        0     7896 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/cli/src/cli.cpp
--rw-r--r--   0        0        0      840 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/cli/src/cli.h
--rw-r--r--   0        0        0     8306 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/cli/src/options.cpp
--rw-r--r--   0        0        0     1385 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/cli/src/options.h
--rw-r--r--   0        0        0       10 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/debian/apngasm.install
--rw-r--r--   0        0        0       19 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/debian/apngasm.manpages
--rw-r--r--   0        0        0     2798 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/debian/changelog
--rw-r--r--   0        0        0        2 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/debian/compat
--rw-r--r--   0        0        0     2174 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/debian/control
--rw-r--r--   0        0        0      310 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/debian/copyright
--rw-r--r--   0        0        0       24 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/debian/libapngasm.install
--rw-r--r--   0        0        0       33 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/debian/libapngasm.postinst
--rwxr-xr-x   0        0        0      119 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/debian/rules
--rw-r--r--   0        0        0       13 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/debian/source/format
--rw-r--r--   0        0        0     4598 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/docs/building/win/instructions.md
--rw-r--r--   0        0        0    80561 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/docs/doxygen-config
--rw-r--r--   0        0        0     6589 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/docs/html/annotated.html
--rw-r--r--   0        0        0     7686 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/docs/html/apngasm-conf_8h_source.html
--rw-r--r--   0        0        0    28772 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/docs/html/apngasm_8h_source.html
--rw-r--r--   0        0        0    20111 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/docs/html/apngframe_8h_source.html
--rw-r--r--   0        0        0      676 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/docs/html/bc_s.png
--rw-r--r--   0        0        0      147 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/docs/html/bdwn.png
--rw-r--r--   0        0        0     9746 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/docs/html/classapngasm_1_1APNGAsm-members.html
--rw-r--r--   0        0        0    32579 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/docs/html/classapngasm_1_1APNGAsm.html
--rw-r--r--   0        0        0    13499 2024-02-07 02:09:21.472284 apngasm_python-1.2.3/apngasm/docs/html/classapngasm_1_1APNGFrame-members.html
--rw-r--r--   0        0        0    29090 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/classapngasm_1_1APNGFrame.html
--rw-r--r--   0        0        0     5841 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/classes.html
--rw-r--r--   0        0        0      132 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/closed.png
--rw-r--r--   0        0        0     4718 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/dir_97aefd0d527b934f1d99a682da8fe6a9.html
--rw-r--r--   0        0        0     6033 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/dir_a065c5f60305fee3569f887679366939.html
--rw-r--r--   0        0        0    23935 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/doxygen.css
--rw-r--r--   0        0        0     3779 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/doxygen.png
--rw-r--r--   0        0        0     2983 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/dynsections.js
--rw-r--r--   0        0        0       86 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/ftv2blank.png
--rw-r--r--   0        0        0      453 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/ftv2cl.png
--rw-r--r--   0        0        0      746 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/ftv2doc.png
--rw-r--r--   0        0        0      616 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/ftv2folderclosed.png
--rw-r--r--   0        0        0      597 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/ftv2folderopen.png
--rw-r--r--   0        0        0       86 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/ftv2lastnode.png
--rw-r--r--   0        0        0      746 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/ftv2link.png
--rw-r--r--   0        0        0      246 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/ftv2mlastnode.png
--rw-r--r--   0        0        0      246 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/ftv2mnode.png
--rw-r--r--   0        0        0      403 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/ftv2mo.png
--rw-r--r--   0        0        0       86 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/ftv2node.png
--rw-r--r--   0        0        0      388 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/ftv2ns.png
--rw-r--r--   0        0        0      229 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/ftv2plastnode.png
--rw-r--r--   0        0        0      229 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/ftv2pnode.png
--rw-r--r--   0        0        0      314 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/ftv2splitbar.png
--rw-r--r--   0        0        0       86 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/ftv2vertline.png
--rw-r--r--   0        0        0     6831 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/functions.html
--rw-r--r--   0        0        0     6719 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/functions_func.html
--rw-r--r--   0        0        0     4058 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/index.html
--rw-r--r--   0        0        0   104693 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/jquery.js
--rw-r--r--   0        0        0     9397 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/namespaceapngasm.html
--rw-r--r--   0        0        0     4831 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/namespacemembers.html
--rw-r--r--   0        0        0     4713 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/namespacemembers_vars.html
--rw-r--r--   0        0        0     4822 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/namespaces.html
--rw-r--r--   0        0        0      153 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/nav_f.png
--rw-r--r--   0        0        0       95 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/nav_g.png
--rw-r--r--   0        0        0       98 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/nav_h.png
--rw-r--r--   0        0        0      123 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/open.png
--rw-r--r--   0        0        0     1011 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_0.html
--rw-r--r--   0        0        0     2133 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_0.js
--rw-r--r--   0        0        0     1011 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_1.html
--rw-r--r--   0        0        0      426 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_1.js
--rw-r--r--   0        0        0     1011 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_2.html
--rw-r--r--   0        0        0      144 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_2.js
--rw-r--r--   0        0        0     1011 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_3.html
--rw-r--r--   0        0        0      142 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_3.js
--rw-r--r--   0        0        0     1011 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_4.html
--rw-r--r--   0        0        0      158 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_4.js
--rw-r--r--   0        0        0     1011 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_5.html
--rw-r--r--   0        0        0      154 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_5.js
--rw-r--r--   0        0        0     1011 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_6.html
--rw-r--r--   0        0        0      265 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_6.js
--rw-r--r--   0        0        0     1012 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_61.html
--rw-r--r--   0        0        0      176 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_61.js
--rw-r--r--   0        0        0     1011 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_7.html
--rw-r--r--   0        0        0      634 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_7.js
--rw-r--r--   0        0        0     1012 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_72.html
--rw-r--r--   0        0        0      151 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_72.js
--rw-r--r--   0        0        0     1011 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_8.html
--rw-r--r--   0        0        0      138 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_8.js
--rw-r--r--   0        0        0     1011 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_9.html
--rw-r--r--   0        0        0      142 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/all_9.js
--rw-r--r--   0        0        0     1015 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/classes_0.html
--rw-r--r--   0        0        0      176 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/classes_0.js
--rw-r--r--   0        0        0     1015 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/classes_1.html
--rw-r--r--   0        0        0      151 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/classes_1.js
--rw-r--r--   0        0        0     1016 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/classes_61.html
--rw-r--r--   0        0        0      176 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/classes_61.js
--rw-r--r--   0        0        0     1016 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/classes_72.html
--rw-r--r--   0        0        0      151 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/classes_72.js
--rw-r--r--   0        0        0      273 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/close.png
--rw-r--r--   0        0        0     1017 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_0.html
--rw-r--r--   0        0        0     1936 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_0.js
--rw-r--r--   0        0        0     1017 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_1.html
--rw-r--r--   0        0        0      146 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_1.js
--rw-r--r--   0        0        0     1017 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_2.html
--rw-r--r--   0        0        0      144 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_2.js
--rw-r--r--   0        0        0     1017 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_3.html
--rw-r--r--   0        0        0      142 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_3.js
--rw-r--r--   0        0        0     1017 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_4.html
--rw-r--r--   0        0        0      158 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_4.js
--rw-r--r--   0        0        0     1017 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_5.html
--rw-r--r--   0        0        0      154 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_5.js
--rw-r--r--   0        0        0     1017 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_6.html
--rw-r--r--   0        0        0      134 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_6.js
--rw-r--r--   0        0        0     1017 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_7.html
--rw-r--r--   0        0        0      634 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_7.js
--rw-r--r--   0        0        0     1017 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_8.html
--rw-r--r--   0        0        0      138 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_8.js
--rw-r--r--   0        0        0     1017 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_9.html
--rw-r--r--   0        0        0      142 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/functions_9.js
--rw-r--r--   0        0        0      563 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/mag_sel.png
--rw-r--r--   0        0        0     1018 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/namespaces_0.html
--rw-r--r--   0        0        0       81 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/namespaces_0.js
--rw-r--r--   0        0        0      461 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/nomatches.html
--rw-r--r--   0        0        0     4461 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/search.css
--rw-r--r--   0        0        0    22150 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/search.js
--rw-r--r--   0        0        0      604 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/search_l.png
--rw-r--r--   0        0        0      158 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/search_m.png
--rw-r--r--   0        0        0      612 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/search_r.png
--rw-r--r--   0        0        0     1017 2024-02-07 02:09:21.476284 apngasm_python-1.2.3/apngasm/docs/html/search/variables_0.html
--rw-r--r--   0        0        0      300 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/html/search/variables_0.js
--rw-r--r--   0        0        0     5527 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/html/structapngasm_1_1rgb-members.html
--rw-r--r--   0        0        0     5994 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/html/structapngasm_1_1rgb.html
--rw-r--r--   0        0        0     5795 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/html/structapngasm_1_1rgba-members.html
--rw-r--r--   0        0        0     6360 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/html/structapngasm_1_1rgba.html
--rw-r--r--   0        0        0      853 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/html/sync_off.png
--rw-r--r--   0        0        0      845 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/html/sync_on.png
--rw-r--r--   0        0        0      142 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/html/tab_a.png
--rw-r--r--   0        0        0      169 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/html/tab_b.png
--rw-r--r--   0        0        0      177 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/html/tab_h.png
--rw-r--r--   0        0        0      184 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/html/tab_s.png
--rw-r--r--   0        0        0     1163 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/html/tabs.css
--rw-r--r--   0        0        0      508 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/latex/Makefile
--rw-r--r--   0        0        0      779 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/latex/annotated.tex
--rw-r--r--   0        0        0    19499 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/latex/classapngasm_1_1APNGAsm.tex
--rw-r--r--   0        0        0    15351 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/latex/classapngasm_1_1APNGFrame.tex
--rw-r--r--   0        0        0      434 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/latex/dir_97aefd0d527b934f1d99a682da8fe6a9.tex
--rw-r--r--   0        0        0      692 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/latex/dir_a065c5f60305fee3569f887679366939.tex
--rw-r--r--   0        0        0    10548 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/latex/doxygen.sty
--rw-r--r--   0        0        0     2400 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/latex/namespaceapngasm.tex
--rw-r--r--   0        0        0      302 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/latex/namespaces.tex
--rw-r--r--   0        0        0     3458 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/latex/refman.tex
--rw-r--r--   0        0        0      624 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/latex/structapngasm_1_1CHUNK.tex
--rw-r--r--   0        0        0     1525 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/latex/structapngasm_1_1OP.tex
--rw-r--r--   0        0        0      737 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/latex/structapngasm_1_1rgb.tex
--rw-r--r--   0        0        0      918 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/latex/structapngasm_1_1rgba.tex
--rw-r--r--   0        0        0     1798 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/docs/man/apngasm.1
--rw-r--r--   0        0        0     5015 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/CMakeLists.txt
--rw-r--r--   0        0        0      587 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/DESCRIPTION.txt
--rw-r--r--   0        0        0      861 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/LICENSE.txt
--rw-r--r--   0        0        0     2594 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/interfaces/java/CMakeLists.txt
--rw-r--r--   0        0        0     1192 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/interfaces/java/NativeLibLoader.java.in
--rw-r--r--   0        0        0      958 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/interfaces/ruby/CMakeLists.txt
--rw-r--r--   0        0        0      278 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/libapngasm.pc.in
--rw-r--r--   0        0        0       49 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/manifest.txt.in
--rw-r--r--   0        0        0     1432 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/package/CMakeLists.txt.in
--rw-r--r--   0        0        0     6175 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/src/apng.i
--rw-r--r--   0        0        0      381 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/src/apngasm-conf.h
--rw-r--r--   0        0        0      193 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/src/apngasm-version.h.in
--rw-r--r--   0        0        0    60869 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/src/apngasm.cpp
--rw-r--r--   0        0        0    10766 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/src/apngasm.h
--rw-r--r--   0        0        0     9217 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/src/apngframe.cpp
--rw-r--r--   0        0        0     4392 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/src/apngframe.h
--rw-r--r--   0        0        0     1702 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/src/listener/apngasmlistener.cpp
--rw-r--r--   0        0        0     2473 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/src/listener/apngasmlistener.h
--rw-r--r--   0        0        0     8685 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/src/spec/priv/specreaderimpl.cpp
--rw-r--r--   0        0        0     2439 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/src/spec/priv/specreaderimpl.h
--rw-r--r--   0        0        0     3705 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/src/spec/priv/specwriterimpl.cpp
--rw-r--r--   0        0        0     2058 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/src/spec/priv/specwriterimpl.h
--rw-r--r--   0        0        0     1923 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/src/spec/specreader.cpp
--rw-r--r--   0        0        0      522 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/src/spec/specreader.h
--rw-r--r--   0        0        0     3690 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/src/spec/specwriter.cpp
--rw-r--r--   0        0        0      899 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/lib/src/spec/specwriter.h
--rw-r--r--   0        0        0     2864 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/00.png
--rw-r--r--   0        0        0     2864 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/01.png
--rw-r--r--   0        0        0     2864 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/02.png
--rw-r--r--   0        0        0     2864 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/03.png
--rw-r--r--   0        0        0     2864 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/04.png
--rw-r--r--   0        0        0     2864 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/05.png
--rw-r--r--   0        0        0     2864 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/06.png
--rw-r--r--   0        0        0     2864 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/07.png
--rw-r--r--   0        0        0     2864 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/08.png
--rw-r--r--   0        0        0     2864 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/09.png
--rw-r--r--   0        0        0     2864 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/10.png
--rw-r--r--   0        0        0     2864 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/11.png
--rw-r--r--   0        0        0     2864 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/12.png
--rw-r--r--   0        0        0     3015 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/13.png
--rw-r--r--   0        0        0     3160 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/14.png
--rw-r--r--   0        0        0     3133 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/15.png
--rw-r--r--   0        0        0     2992 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/16.png
--rw-r--r--   0        0        0     2907 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/17.png
--rw-r--r--   0        0        0     2821 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/18.png
--rw-r--r--   0        0        0     2609 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/19.png
--rw-r--r--   0        0        0     2179 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/20.png
--rw-r--r--   0        0        0     1796 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/21.png
--rw-r--r--   0        0        0      977 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/22.png
--rw-r--r--   0        0        0      114 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/23.png
--rw-r--r--   0        0        0      977 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/24.png
--rw-r--r--   0        0        0     1796 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/25.png
--rw-r--r--   0        0        0     2179 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/26.png
--rw-r--r--   0        0        0     2609 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/27.png
--rw-r--r--   0        0        0     2821 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/28.png
--rw-r--r--   0        0        0     2907 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/29.png
--rw-r--r--   0        0        0     2992 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/30.png
--rw-r--r--   0        0        0     3133 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/31.png
--rw-r--r--   0        0        0     3160 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/32.png
--rw-r--r--   0        0        0     3015 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm/33.png
--rw-r--r--   0        0        0    32557 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/apngasm.png
--rw-r--r--   0        0        0      347 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/test.json
--rw-r--r--   0        0        0      361 2024-02-07 02:09:21.480284 apngasm_python-1.2.3/apngasm/resources/images/test.xml
--rw-r--r--   0        0        0     2981 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/test/CMakeLists.txt
--rwxr-xr-x   0        0        0     1392 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/test/cli/delay-test.sh
--rwxr-xr-x   0        0        0      311 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/test/cli/disassemble-test.sh
--rwxr-xr-x   0        0        0      253 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/test/cli/json-test.sh
--rwxr-xr-x   0        0        0      265 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/test/cli/logo-test.sh
--rwxr-xr-x   0        0        0      251 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/test/cli/xml-test.sh
--rw-r--r--   0        0        0     6212 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/test/cpp/apngasm-test.cpp
--rw-r--r--   0        0        0     8753 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/test/samples/clk-first.png
--rw-r--r--   0        0        0     4254 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/test/samples/clock1.png
--rw-r--r--   0        0        0     4203 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/test/samples/clock2.png
--rw-r--r--   0        0        0     4283 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/test/samples/clock3.png
--rw-r--r--   0        0        0     4197 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/test/samples/clock4.png
--rw-r--r--   0        0        0   112705 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/test/samples/gold01.png
--rw-r--r--   0        0        0   112734 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/test/samples/gold02.png
--rw-r--r--   0        0        0   112645 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/test/samples/gold03.png
--rw-r--r--   0        0        0     5753 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/test/samples/penguins.png
--rw-r--r--   0        0        0      224 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/windows/compile.bat
--rw-r--r--   0        0        0     1066 2024-02-07 02:09:21.484284 apngasm_python-1.2.3/apngasm/windows/compile_deps.bat
--rw-r--r--   0        0        0      721 2024-02-07 02:09:20.576291 apngasm_python-1.2.3/cmake/NanobindStubgen.cmake
--rw-r--r--   0        0        0     5108 2024-02-07 02:09:20.576291 apngasm_python-1.2.3/cmake/QueryPythonForNanobind.cmake
--rw-r--r--   0        0        0     1125 2024-02-07 02:09:20.576291 apngasm_python-1.2.3/conanfile.py
--rw-r--r--   0        0        0     2198 2024-02-07 02:09:20.584291 apngasm_python-1.2.3/pyproject.toml
--rwxr-xr-x   0        0        0      891 2024-02-07 02:09:20.584291 apngasm_python-1.2.3/scripts/get_arch.py
--rwxr-xr-x   0        0        0     3094 2024-02-07 02:09:20.584291 apngasm_python-1.2.3/scripts/get_deps.py
--rwxr-xr-x   0        0        0      714 2024-02-07 02:09:20.584291 apngasm_python-1.2.3/scripts/patch_stub.py
--rwxr-xr-x   0        0        0     1185 2024-02-07 02:09:20.584291 apngasm_python-1.2.3/scripts/update_stub.py
--rw-r--r--   0        0        0    26699 2024-02-07 02:09:20.584291 apngasm_python-1.2.3/src/apngasm_python.cpp
--rwxr-xr-x   0        0        0       66 2024-02-07 02:09:20.584291 apngasm_python-1.2.3/src-python/apngasm_python/__init__.py
--rw-r--r--   0        0        0       17 2024-02-07 02:09:20.584291 apngasm_python-1.2.3/src-python/apngasm_python/__init__.pyi
--rw-r--r--   0        0        0    20572 2024-02-07 02:09:20.584291 apngasm_python-1.2.3/src-python/apngasm_python/_apngasm_python/__init__.pyi
--rwxr-xr-x   0        0        0    20676 2024-02-07 02:09:20.584291 apngasm_python-1.2.3/src-python/apngasm_python/apngasm.py
--rw-r--r--   0        0        0     3302 2024-02-07 02:09:20.584291 apngasm_python-1.2.3/src-python/apngasm_python/apngasm.pyi
--rw-r--r--   0        0        0        0 2024-02-07 02:09:20.584291 apngasm_python-1.2.3/src-python/apngasm_python/py.typed
--rw-r--r--   0        0        0    36449 1970-01-01 00:00:00.000000 apngasm_python-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     4521 2024-05-24 02:41:29.927460 apngasm_python-1.3.0/CMakeLists.txt
+-rw-r--r--   0        0        0    26526 2024-05-24 02:41:29.927460 apngasm_python-1.3.0/LICENSE
+-rw-r--r--   0        0        0      386 2024-05-24 02:41:29.927460 apngasm_python-1.3.0/PreLoad.cmake
+-rw-r--r--   0        0        0     5713 2024-05-24 02:41:29.927460 apngasm_python-1.3.0/README.md
+-rw-r--r--   0        0        0       32 2024-05-24 02:41:30.207457 apngasm_python-1.3.0/apngasm/.git
+-rw-r--r--   0        0        0     4761 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/.github/workflows/build.yml
+-rw-r--r--   0        0        0      624 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/.gitignore
+-rw-r--r--   0        0        0    18247 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/BACKERS.txt
+-rw-r--r--   0        0        0     1079 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/CMakeLists.txt
+-rw-r--r--   0        0        0      861 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/LICENSE.txt
+-rw-r--r--   0        0        0     4764 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/README.md
+-rw-r--r--   0        0        0     2735 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/cli/CMakeLists.txt
+-rw-r--r--   0        0        0      462 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/cli/DESCRIPTION.txt
+-rw-r--r--   0        0        0      861 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/cli/LICENSE.txt
+-rw-r--r--   0        0        0     1559 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/cli/package/CMakeLists.txt.in
+-rw-r--r--   0        0        0      217 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/cli/src/apngasm-cli-version.h.in
+-rw-r--r--   0        0        0      440 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/cli/src/apngasm-cli.cpp
+-rw-r--r--   0        0        0     7945 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/cli/src/cli.cpp
+-rw-r--r--   0        0        0      840 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/cli/src/cli.h
+-rw-r--r--   0        0        0     8306 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/cli/src/options.cpp
+-rw-r--r--   0        0        0     1385 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/cli/src/options.h
+-rw-r--r--   0        0        0       10 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/debian/apngasm.install
+-rw-r--r--   0        0        0       19 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/debian/apngasm.manpages
+-rw-r--r--   0        0        0     2798 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/debian/changelog
+-rw-r--r--   0        0        0        2 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/debian/compat
+-rw-r--r--   0        0        0     2174 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/debian/control
+-rw-r--r--   0        0        0      310 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/debian/copyright
+-rw-r--r--   0        0        0       24 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/debian/libapngasm.install
+-rw-r--r--   0        0        0       33 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/debian/libapngasm.postinst
+-rwxr-xr-x   0        0        0      119 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/debian/rules
+-rw-r--r--   0        0        0       13 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/debian/source/format
+-rw-r--r--   0        0        0     4598 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/building/win/instructions.md
+-rw-r--r--   0        0        0    80561 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/doxygen-config
+-rw-r--r--   0        0        0     6589 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/annotated.html
+-rw-r--r--   0        0        0     7686 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/apngasm-conf_8h_source.html
+-rw-r--r--   0        0        0    28772 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/apngasm_8h_source.html
+-rw-r--r--   0        0        0    20111 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/apngframe_8h_source.html
+-rw-r--r--   0        0        0      676 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/bc_s.png
+-rw-r--r--   0        0        0      147 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/bdwn.png
+-rw-r--r--   0        0        0     9746 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/classapngasm_1_1APNGAsm-members.html
+-rw-r--r--   0        0        0    32579 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/classapngasm_1_1APNGAsm.html
+-rw-r--r--   0        0        0    13499 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/classapngasm_1_1APNGFrame-members.html
+-rw-r--r--   0        0        0    29090 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/classapngasm_1_1APNGFrame.html
+-rw-r--r--   0        0        0     5841 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/classes.html
+-rw-r--r--   0        0        0      132 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/closed.png
+-rw-r--r--   0        0        0     4718 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/dir_97aefd0d527b934f1d99a682da8fe6a9.html
+-rw-r--r--   0        0        0     6033 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/dir_a065c5f60305fee3569f887679366939.html
+-rw-r--r--   0        0        0    23935 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/doxygen.css
+-rw-r--r--   0        0        0     3779 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/doxygen.png
+-rw-r--r--   0        0        0     2983 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/dynsections.js
+-rw-r--r--   0        0        0       86 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/ftv2blank.png
+-rw-r--r--   0        0        0      453 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/ftv2cl.png
+-rw-r--r--   0        0        0      746 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/ftv2doc.png
+-rw-r--r--   0        0        0      616 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/ftv2folderclosed.png
+-rw-r--r--   0        0        0      597 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/ftv2folderopen.png
+-rw-r--r--   0        0        0       86 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/ftv2lastnode.png
+-rw-r--r--   0        0        0      746 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/ftv2link.png
+-rw-r--r--   0        0        0      246 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/ftv2mlastnode.png
+-rw-r--r--   0        0        0      246 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/ftv2mnode.png
+-rw-r--r--   0        0        0      403 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/ftv2mo.png
+-rw-r--r--   0        0        0       86 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/ftv2node.png
+-rw-r--r--   0        0        0      388 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/ftv2ns.png
+-rw-r--r--   0        0        0      229 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/ftv2plastnode.png
+-rw-r--r--   0        0        0      229 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/ftv2pnode.png
+-rw-r--r--   0        0        0      314 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/ftv2splitbar.png
+-rw-r--r--   0        0        0       86 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/ftv2vertline.png
+-rw-r--r--   0        0        0     6831 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/functions.html
+-rw-r--r--   0        0        0     6719 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/functions_func.html
+-rw-r--r--   0        0        0     4058 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/index.html
+-rw-r--r--   0        0        0   104693 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/jquery.js
+-rw-r--r--   0        0        0     9397 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/namespaceapngasm.html
+-rw-r--r--   0        0        0     4831 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/namespacemembers.html
+-rw-r--r--   0        0        0     4713 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/namespacemembers_vars.html
+-rw-r--r--   0        0        0     4822 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/namespaces.html
+-rw-r--r--   0        0        0      153 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/nav_f.png
+-rw-r--r--   0        0        0       95 2024-05-24 02:41:30.795450 apngasm_python-1.3.0/apngasm/docs/html/nav_g.png
+-rw-r--r--   0        0        0       98 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/nav_h.png
+-rw-r--r--   0        0        0      123 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/open.png
+-rw-r--r--   0        0        0     1011 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_0.html
+-rw-r--r--   0        0        0     2133 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_0.js
+-rw-r--r--   0        0        0     1011 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_1.html
+-rw-r--r--   0        0        0      426 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_1.js
+-rw-r--r--   0        0        0     1011 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_2.html
+-rw-r--r--   0        0        0      144 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_2.js
+-rw-r--r--   0        0        0     1011 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_3.html
+-rw-r--r--   0        0        0      142 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_3.js
+-rw-r--r--   0        0        0     1011 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_4.html
+-rw-r--r--   0        0        0      158 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_4.js
+-rw-r--r--   0        0        0     1011 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_5.html
+-rw-r--r--   0        0        0      154 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_5.js
+-rw-r--r--   0        0        0     1011 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_6.html
+-rw-r--r--   0        0        0      265 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_6.js
+-rw-r--r--   0        0        0     1012 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_61.html
+-rw-r--r--   0        0        0      176 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_61.js
+-rw-r--r--   0        0        0     1011 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_7.html
+-rw-r--r--   0        0        0      634 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_7.js
+-rw-r--r--   0        0        0     1012 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_72.html
+-rw-r--r--   0        0        0      151 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_72.js
+-rw-r--r--   0        0        0     1011 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_8.html
+-rw-r--r--   0        0        0      138 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_8.js
+-rw-r--r--   0        0        0     1011 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_9.html
+-rw-r--r--   0        0        0      142 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/all_9.js
+-rw-r--r--   0        0        0     1015 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/classes_0.html
+-rw-r--r--   0        0        0      176 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/classes_0.js
+-rw-r--r--   0        0        0     1015 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/classes_1.html
+-rw-r--r--   0        0        0      151 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/classes_1.js
+-rw-r--r--   0        0        0     1016 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/classes_61.html
+-rw-r--r--   0        0        0      176 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/classes_61.js
+-rw-r--r--   0        0        0     1016 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/classes_72.html
+-rw-r--r--   0        0        0      151 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/classes_72.js
+-rw-r--r--   0        0        0      273 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/close.png
+-rw-r--r--   0        0        0     1017 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_0.html
+-rw-r--r--   0        0        0     1936 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_0.js
+-rw-r--r--   0        0        0     1017 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_1.html
+-rw-r--r--   0        0        0      146 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_1.js
+-rw-r--r--   0        0        0     1017 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_2.html
+-rw-r--r--   0        0        0      144 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_2.js
+-rw-r--r--   0        0        0     1017 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_3.html
+-rw-r--r--   0        0        0      142 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_3.js
+-rw-r--r--   0        0        0     1017 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_4.html
+-rw-r--r--   0        0        0      158 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_4.js
+-rw-r--r--   0        0        0     1017 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_5.html
+-rw-r--r--   0        0        0      154 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_5.js
+-rw-r--r--   0        0        0     1017 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_6.html
+-rw-r--r--   0        0        0      134 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_6.js
+-rw-r--r--   0        0        0     1017 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_7.html
+-rw-r--r--   0        0        0      634 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_7.js
+-rw-r--r--   0        0        0     1017 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_8.html
+-rw-r--r--   0        0        0      138 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_8.js
+-rw-r--r--   0        0        0     1017 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_9.html
+-rw-r--r--   0        0        0      142 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/functions_9.js
+-rw-r--r--   0        0        0      563 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/mag_sel.png
+-rw-r--r--   0        0        0     1018 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/namespaces_0.html
+-rw-r--r--   0        0        0       81 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/namespaces_0.js
+-rw-r--r--   0        0        0      461 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/nomatches.html
+-rw-r--r--   0        0        0     4461 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/search.css
+-rw-r--r--   0        0        0    22150 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/search.js
+-rw-r--r--   0        0        0      604 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/search_l.png
+-rw-r--r--   0        0        0      158 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/search_m.png
+-rw-r--r--   0        0        0      612 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/search_r.png
+-rw-r--r--   0        0        0     1017 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/variables_0.html
+-rw-r--r--   0        0        0      300 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/search/variables_0.js
+-rw-r--r--   0        0        0     5527 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/structapngasm_1_1rgb-members.html
+-rw-r--r--   0        0        0     5994 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/structapngasm_1_1rgb.html
+-rw-r--r--   0        0        0     5795 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/structapngasm_1_1rgba-members.html
+-rw-r--r--   0        0        0     6360 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/structapngasm_1_1rgba.html
+-rw-r--r--   0        0        0      853 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/sync_off.png
+-rw-r--r--   0        0        0      845 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/sync_on.png
+-rw-r--r--   0        0        0      142 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/tab_a.png
+-rw-r--r--   0        0        0      169 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/tab_b.png
+-rw-r--r--   0        0        0      177 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/tab_h.png
+-rw-r--r--   0        0        0      184 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/tab_s.png
+-rw-r--r--   0        0        0     1163 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/html/tabs.css
+-rw-r--r--   0        0        0      508 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/latex/Makefile
+-rw-r--r--   0        0        0      779 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/latex/annotated.tex
+-rw-r--r--   0        0        0    19499 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/latex/classapngasm_1_1APNGAsm.tex
+-rw-r--r--   0        0        0    15351 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/latex/classapngasm_1_1APNGFrame.tex
+-rw-r--r--   0        0        0      434 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/latex/dir_97aefd0d527b934f1d99a682da8fe6a9.tex
+-rw-r--r--   0        0        0      692 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/latex/dir_a065c5f60305fee3569f887679366939.tex
+-rw-r--r--   0        0        0    10548 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/latex/doxygen.sty
+-rw-r--r--   0        0        0     2400 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/latex/namespaceapngasm.tex
+-rw-r--r--   0        0        0      302 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/latex/namespaces.tex
+-rw-r--r--   0        0        0     3458 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/latex/refman.tex
+-rw-r--r--   0        0        0      624 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/latex/structapngasm_1_1CHUNK.tex
+-rw-r--r--   0        0        0     1525 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/latex/structapngasm_1_1OP.tex
+-rw-r--r--   0        0        0      737 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/latex/structapngasm_1_1rgb.tex
+-rw-r--r--   0        0        0      918 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/latex/structapngasm_1_1rgba.tex
+-rw-r--r--   0        0        0     1798 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/docs/man/apngasm.1
+-rw-r--r--   0        0        0     4990 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/CMakeLists.txt
+-rw-r--r--   0        0        0      587 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/DESCRIPTION.txt
+-rw-r--r--   0        0        0      861 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/LICENSE.txt
+-rw-r--r--   0        0        0     2594 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/interfaces/java/CMakeLists.txt
+-rw-r--r--   0        0        0     1192 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/interfaces/java/NativeLibLoader.java.in
+-rw-r--r--   0        0        0      958 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/interfaces/ruby/CMakeLists.txt
+-rw-r--r--   0        0        0      278 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/libapngasm.pc.in
+-rw-r--r--   0        0        0       49 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/manifest.txt.in
+-rw-r--r--   0        0        0     1432 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/package/CMakeLists.txt.in
+-rw-r--r--   0        0        0     6175 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/src/apng.i
+-rw-r--r--   0        0        0      381 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/src/apngasm-conf.h
+-rw-r--r--   0        0        0      193 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/src/apngasm-version.h.in
+-rw-r--r--   0        0        0    60906 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/src/apngasm.cpp
+-rw-r--r--   0        0        0    10766 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/src/apngasm.h
+-rw-r--r--   0        0        0     9217 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/src/apngframe.cpp
+-rw-r--r--   0        0        0     4392 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/src/apngframe.h
+-rw-r--r--   0        0        0     1725 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/src/listener/apngasmlistener.cpp
+-rw-r--r--   0        0        0     2473 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/src/listener/apngasmlistener.h
+-rw-r--r--   0        0        0     8734 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/src/spec/priv/specreaderimpl.cpp
+-rw-r--r--   0        0        0     2439 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/src/spec/priv/specreaderimpl.h
+-rw-r--r--   0        0        0     3705 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/src/spec/priv/specwriterimpl.cpp
+-rw-r--r--   0        0        0     2058 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/src/spec/priv/specwriterimpl.h
+-rw-r--r--   0        0        0     1923 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/src/spec/specreader.cpp
+-rw-r--r--   0        0        0      522 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/src/spec/specreader.h
+-rw-r--r--   0        0        0     3731 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/src/spec/specwriter.cpp
+-rw-r--r--   0        0        0      899 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/lib/src/spec/specwriter.h
+-rw-r--r--   0        0        0      304 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/macos/x64-osx-10-9.cmake
+-rw-r--r--   0        0        0     2864 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/00.png
+-rw-r--r--   0        0        0     2864 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/01.png
+-rw-r--r--   0        0        0     2864 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/02.png
+-rw-r--r--   0        0        0     2864 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/03.png
+-rw-r--r--   0        0        0     2864 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/04.png
+-rw-r--r--   0        0        0     2864 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/05.png
+-rw-r--r--   0        0        0     2864 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/06.png
+-rw-r--r--   0        0        0     2864 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/07.png
+-rw-r--r--   0        0        0     2864 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/08.png
+-rw-r--r--   0        0        0     2864 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/09.png
+-rw-r--r--   0        0        0     2864 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/10.png
+-rw-r--r--   0        0        0     2864 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/11.png
+-rw-r--r--   0        0        0     2864 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/12.png
+-rw-r--r--   0        0        0     3015 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/13.png
+-rw-r--r--   0        0        0     3160 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/14.png
+-rw-r--r--   0        0        0     3133 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/15.png
+-rw-r--r--   0        0        0     2992 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/16.png
+-rw-r--r--   0        0        0     2907 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/17.png
+-rw-r--r--   0        0        0     2821 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/18.png
+-rw-r--r--   0        0        0     2609 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/19.png
+-rw-r--r--   0        0        0     2179 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/20.png
+-rw-r--r--   0        0        0     1796 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/21.png
+-rw-r--r--   0        0        0      977 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/22.png
+-rw-r--r--   0        0        0      114 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/23.png
+-rw-r--r--   0        0        0      977 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/24.png
+-rw-r--r--   0        0        0     1796 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/25.png
+-rw-r--r--   0        0        0     2179 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/26.png
+-rw-r--r--   0        0        0     2609 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/27.png
+-rw-r--r--   0        0        0     2821 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/28.png
+-rw-r--r--   0        0        0     2907 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/29.png
+-rw-r--r--   0        0        0     2992 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/30.png
+-rw-r--r--   0        0        0     3133 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/31.png
+-rw-r--r--   0        0        0     3160 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/32.png
+-rw-r--r--   0        0        0     3015 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm/33.png
+-rw-r--r--   0        0        0    32557 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/apngasm.png
+-rw-r--r--   0        0        0      347 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/test.json
+-rw-r--r--   0        0        0      361 2024-05-24 02:41:30.799450 apngasm_python-1.3.0/apngasm/resources/images/test.xml
+-rw-r--r--   0        0        0     2963 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/test/CMakeLists.txt
+-rwxr-xr-x   0        0        0     1392 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/test/cli/delay-test.sh
+-rwxr-xr-x   0        0        0      311 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/test/cli/disassemble-test.sh
+-rwxr-xr-x   0        0        0      253 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/test/cli/json-test.sh
+-rwxr-xr-x   0        0        0      265 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/test/cli/logo-test.sh
+-rwxr-xr-x   0        0        0      251 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/test/cli/xml-test.sh
+-rw-r--r--   0        0        0     6212 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/test/cpp/apngasm-test.cpp
+-rw-r--r--   0        0        0     8753 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/test/samples/clk-first.png
+-rw-r--r--   0        0        0     4254 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/test/samples/clock1.png
+-rw-r--r--   0        0        0     4203 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/test/samples/clock2.png
+-rw-r--r--   0        0        0     4283 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/test/samples/clock3.png
+-rw-r--r--   0        0        0     4197 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/test/samples/clock4.png
+-rw-r--r--   0        0        0   112705 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/test/samples/gold01.png
+-rw-r--r--   0        0        0   112734 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/test/samples/gold02.png
+-rw-r--r--   0        0        0   112645 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/test/samples/gold03.png
+-rw-r--r--   0        0        0     5753 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/test/samples/penguins.png
+-rw-r--r--   0        0        0      224 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/windows/compile.bat
+-rw-r--r--   0        0        0     1084 2024-05-24 02:41:30.803450 apngasm_python-1.3.0/apngasm/windows/compile_deps.bat
+-rw-r--r--   0        0        0     5108 2024-05-24 02:41:29.927460 apngasm_python-1.3.0/cmake/QueryPythonForNanobind.cmake
+-rw-r--r--   0        0        0      999 2024-05-24 02:41:29.927460 apngasm_python-1.3.0/conanfile.py
+-rw-r--r--   0        0        0     2213 2024-05-24 02:41:30.807450 apngasm_python-1.3.0/lipo-dir-merge/lipo-dir-merge.py
+-rw-r--r--   0        0        0     2418 2024-05-24 02:41:29.927460 apngasm_python-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-24 02:41:29.931460 apngasm_python-1.3.0/scripts/__init__.py
+-rwxr-xr-x   0        0        0      927 2024-05-24 02:41:29.931460 apngasm_python-1.3.0/scripts/get_arch.py
+-rwxr-xr-x   0        0        0     5815 2024-05-24 02:41:29.931460 apngasm_python-1.3.0/scripts/get_deps.py
+-rw-r--r--   0        0        0    26697 2024-05-24 02:41:29.931460 apngasm_python-1.3.0/src/apngasm_python.cpp
+-rwxr-xr-x   0        0        0       67 2024-05-24 02:41:29.931460 apngasm_python-1.3.0/src-python/apngasm_python/__init__.py
+-rw-r--r--   0        0        0    17725 2024-05-24 02:41:29.931460 apngasm_python-1.3.0/src-python/apngasm_python/_apngasm_python.pyi
+-rwxr-xr-x   0        0        0    20648 2024-05-24 02:41:29.931460 apngasm_python-1.3.0/src-python/apngasm_python/apngasm.py
+-rw-r--r--   0        0        0        0 2024-05-24 02:41:29.931460 apngasm_python-1.3.0/src-python/apngasm_python/py.typed
+-rw-r--r--   0        0        0    37202 1970-01-01 00:00:00.000000 apngasm_python-1.3.0/PKG-INFO
```

### Comparing `apngasm_python-1.2.3/CMakeLists.txt` & `apngasm_python-1.3.0/CMakeLists.txt`

 * *Files 19% similar despite different names*

```diff
@@ -18,51 +18,54 @@
 message(STATUS "Executing get_deps.py")
 execute_process(
     WORKING_DIRECTORY ${CMAKE_SOURCE_DIR}
     COMMAND ${GET_DEPS_CMD}
 )
 message(STATUS "Finished get_deps.py")
 
-if (WIN32)
+if (MSVC)
     set(CMAKE_MSVC_RUNTIME_LIBRARY "MultiThreaded$<$<CONFIG:Debug>:Debug>")
     set(CMAKE_CXX_FLAGS_RELEASE "${CMAKE_CXX_FLAGS_RELEASE} /MT")
     set(CMAKE_CXX_FLAGS_DEBUG "${CMAKE_CXX_FLAGS_DEBUG} /MTd")
+    set(CMAKE_CXX_FLAGS_RELWITHDEBINFO "${CMAKE_CXX_FLAGS_RELWITHDEBINFO} /Zi /Ob0 /Od /RTC1")
 elseif (LINUX)
     set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fPIC")
 elseif (APPLE)
-    if(${APNGASM_COMPILE_TARGET} STREQUAL "x86_64")
+    if(${APNGASM_COMPILE_TARGET} STREQUAL "armv8")
         set(CMAKE_OSX_DEPLOYMENT_TARGET "11.0")
     else()
-        set(CMAKE_OSX_DEPLOYMENT_TARGET "10.15")
+        set(CMAKE_OSX_DEPLOYMENT_TARGET "10.9")
+        set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++0x -stdlib=libc++ -fno-aligned-allocation")
     endif()
 endif()
 
 set(ZLIB_USE_STATIC_LIBS ON)
 set(PNG_USE_STATIC_LIBS ON)
 set(Boost_USE_STATIC_LIBS ON)
-if (WIN32)
+if (MSVC)
     set(Boost_USE_MULTITHREADED ON)
     set(Boost_USE_STATIC_RUNTIME ON)
 endif()
 
 # Add conan packages
-if ("${APNGASM_COMPILE_TARGET}" STREQUAL "universal2")
-    # x86_64 Contians static libraries that are universal2
+if ("${APNGASM_COMPILE_TARGET}" STREQUAL "universal2_x86_64")
     set(CONAN_TOOLCHAIN ${CMAKE_SOURCE_DIR}/conan_output/x86_64/conan_toolchain.cmake)
+elseif ("${APNGASM_COMPILE_TARGET}" STREQUAL "universal2_armv8")
+    set(CONAN_TOOLCHAIN ${CMAKE_SOURCE_DIR}/conan_output/armv8/conan_toolchain.cmake)
 else()
     set(CONAN_TOOLCHAIN ${CMAKE_SOURCE_DIR}/conan_output/${APNGASM_COMPILE_TARGET}/conan_toolchain.cmake)
 endif()
 
 if (EXISTS ${CONAN_TOOLCHAIN})
     include(${CONAN_TOOLCHAIN})
 else()
     message(FATAL_ERROR "The conan_toolchain file could not be found: ${CONAN_TOOLCHAIN}")
 endif()
 
-project(apngasm-python VERSION 1.2.3)
+project(apngasm-python VERSION 1.3.0)
 set(PY_VERSION_SUFFIX "")
 set(PY_FULL_VERSION ${PROJECT_VERSION}${PY_VERSION_SUFFIX})
 
 # Make sure that the Python and CMake versions match
 if (DEFINED PY_BUILD_CMAKE_PACKAGE_VERSION)
     if (NOT "${PY_BUILD_CMAKE_PACKAGE_VERSION}" MATCHES "^${PY_FULL_VERSION}$")
         message(FATAL_ERROR "Version number does not match "
@@ -72,15 +75,15 @@
 
 # Find the nanobind package
 include(cmake/QueryPythonForNanobind.cmake)
 find_nanobind_python_first()
 
 # Compile the Python module
 nanobind_add_module(_apngasm_python "src/apngasm_python.cpp" NB_STATIC STABLE_ABI)
-if (WIN32)
+if (MSVC)
     nanobind_compile_options(_apngasm_python "/MT /MP /bigobj")
 endif()
 target_compile_definitions(_apngasm_python PRIVATE _apngasm_python_EXPORTS)
 target_compile_definitions(_apngasm_python PRIVATE apngasm_EXPORTS)
 
 # Static linking
 add_subdirectory(apngasm)
@@ -97,31 +100,30 @@
 )
 
 # Hide all symbols by default (including external libraries on Linux)
 set_target_properties(_apngasm_python PROPERTIES
     CXX_VISIBILITY_PRESET "hidden"
     VISIBILITY_INLINES_HIDDEN true
     POSITION_INDEPENDENT_CODE true)
-if (WIN32)
+if (MSVC)
     set_target_properties(_apngasm_python PROPERTIES LINK_FALGS_RELEASE "/WHOLEARCHIVE:MNN")
 elseif (LINUX)
     target_link_options(_apngasm_python PRIVATE "LINKER:--exclude-libs,ALL")
 endif()
 
 # Install the module
 install(TARGETS _apngasm_python
         EXCLUDE_FROM_ALL
         DESTINATION ${PY_BUILD_CMAKE_MODULE_NAME}
         COMPONENT python_modules)
 
 # Generate stubs for the Python module
-option(WITH_PY_STUBS
-    "Generate Python stub files (.pyi) for the Python module." On)
-if (WITH_PY_STUBS AND NOT CMAKE_CROSSCOMPILING)
-    include(cmake/NanobindStubgen.cmake)
-    nanobind_stubgen(_apngasm_python)
-    add_custom_command(TARGET _apngasm_python POST_BUILD
-        COMMAND ${PYTHON_EXECUTABLE} patch_stub.py $<TARGET_FILE_DIR:_apngasm_python>/_apngasm_python.pyi
-        WORKING_DIRECTORY ${CMAKE_SOURCE_DIR}/scripts
-        USES_TERMINAL)
-    nanobind_stubgen_install(_apngasm_python ${PY_BUILD_CMAKE_MODULE_NAME})
-endif()
+nanobind_add_stub(
+    apngasm_python_stub
+    INSTALL_TIME
+    MODULE apngasm_python._apngasm_python
+    OUTPUT "${PY_BUILD_CMAKE_MODULE_NAME}/_apngasm_python.pyi"
+    MARKER_FILE "${PY_BUILD_CMAKE_MODULE_NAME}/py.typed"
+    COMPONENT python_modules
+    EXCLUDE_FROM_ALL
+    VERBOSE
+)
```

### Comparing `apngasm_python-1.2.3/LICENSE` & `apngasm_python-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/README.md` & `apngasm_python-1.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,128 +1,137 @@
 # apngasm-python
 
-A nanobind API for [apngasm](https://github.com/apngasm/apngasm), a tool/library for APNG assembly/disassembly.
+A nanobind API for [apngasm](https://github.com/apngasm/apngasm), which is a
+tool/library for APNG assembly & disassembly with compression support.
 
-apngasm is originally a CLI program for quickly assembling PNG images into animated PNG (APNG). It also supports creating compressed APNG.
+apngasm is originally a CLI program for quickly assembling PNG images into 
+animated PNG (APNG). It also supports creating compressed APNG.
 
-apngasm-python is a binding for apngasm using nanobind, allowing you to use apngasm without calling it using commands.
+apngasm-python is a binding for apngasm using nanobind, allowing you to use apngasm 
+without calling it using commands.
 
-With this module, you can even create APNG using images inside memory (No need to write them out as file and call apngasm! This is about 2 times faster from testing.)
+With this module, you can even create APNG using images inside memory (No need to write 
+them out as file and call apngasm! This is about 2 times faster from testing.)
 
-A similar python module is https://github.com/eight04/pyAPNG , which handles APNG files with python natively and does not support compression.
+A similar python module is https://github.com/eight04/pyAPNG , which handles APNG files 
+with python natively and does not support compression.
 
-For convenience, prebuilt library is packaged with this module, so you need not download apngasm.
+For convenience, prebuilt library is packaged with this module, so you need not 
+download apngasm.
 
 Documentations: https://apngasm-python.readthedocs.io/en/latest/
 
 ## Install
-```
+```bash
 pip install apngasm-python
 ```
 
-Optionally, you can also install `Pillow` and `numpy`
-```
-pip install Pillow numpy
+`Pillow` and `numpy` are optional dependencies. Without them,
+some functions are not usable. To also install them:
+```bash
+pip install apngasm-python[full]
 ```
 
 ## Example usage
-The recommended usage is to `from apngasm_python.apngasm import APNGAsmBinder`, see [example/example_binder.py](example/example_binder.py)
+The recommended usage is to `from apngasm_python.apngasm import APNGAsmBinder`, see 
+[example/example_binder.py](example/example_binder.py)
 ```python
 from apngasm_python.apngasm import APNGAsmBinder
 import numpy as np
 from PIL import Image
 import os
 
 apngasm = APNGAsmBinder()
 
 # From file
-for file_name in sorted(os.listdir('frames')):
+for file_name in sorted(os.listdir("samples/frames")):
     # To adjust frame duration, set delay_num and delay_den
     # The frame duration will be (delay_num / delay_den) seconds
-    apngasm.add_frame_from_file(file_path=os.path.join('frames', file_name), delay_num=100, delay_den=1000)
+    apngasm.add_frame_from_file(file_path=os.path.join("samples/frames", file_name), delay_num=100, delay_den=1000)
     
 # Default value of loops is 0, which is infinite looping of APNG animation
 # This sets the APNG animation to loop for 3 times before stopping
 apngasm.set_loops(3)
-apng.assemble('result-from-file.apng')
+apng.assemble("samples/result-from-file.apng")
 apngasm.reset()
 
 # From Pillow
-for file_name in sorted(os.listdir('frames')):
-    image = Image.open(os.path.join('frames', file_name)).convert('RGBA')
+for file_name in sorted(os.listdir("samples/frames")):
+    image = Image.open(os.path.join("samples/frames", file_name)).convert("RGBA")
     frame = apngasm.add_frame_from_pillow(image, delay_num=50, delay_den=1000)
-apngasm.assemble('result-from-pillow.apng')
+apngasm.assemble("result-from-pillow.apng")
 apngasm.reset()
 
 # Disassemble and get pillow image of one frame
 # You can use with statement to avoid calling reset()
 with APNGAsmBinder() as apng:
-    frames = apng.disassemble_as_pillow('input/ball.apng')
+    frames = apng.disassemble_as_pillow("samples/input/ball.apng")
     frame = frames[0]
-    frame.save('output/ball0.png')
+    frame.save("samples/output/ball0.png")
 
 # Disassemble all APNG into PNGs
-apngasm.save_pngs('output')
+apngasm.save_pngs("samples/output")
 ```
 
-Alternatively, you can reduce overhead and do advanced tasks by calling methods directly, see [example/example_direct.py](example/example_direct.py)
+Alternatively, you can reduce overhead and do advanced tasks by calling methods 
+directly, see [example/example_direct.py](example/example_direct.py)
 ```python
 from apngasm_python._apngasm_python import APNGAsm, APNGFrame, create_frame_from_rgb, create_frame_from_rgba
 import numpy as np
 from PIL import Image
 import os
 
 apngasm = APNGAsm()
 
 # From file
-for file_name in sorted(os.listdir('frames')):
+for file_name in sorted(os.listdir("samples/frames")):
     # To adjust frame duration, set delay_num and delay_den
     # The frame duration will be (delay_num / delay_den) seconds
-    apngasm.add_frame_from_file(file_path=os.path.join('frames', file_name), delay_num=100, delay_den=1000)
+    apngasm.add_frame_from_file(file_path=os.path.join("samples/frames", file_name), delay_num=100, delay_den=1000)
     
 # Default value of loops is 0, which is infinite looping of APNG animation
 # This sets the APNG animation to loop for 3 times before stopping
 apngasm.set_loops(3)
-apng.assemble('result-from-file.apng')
+apng.assemble("samples/result-from-file.apng")
 
 # From Pillow
 apngasm.reset()
-for file_name in sorted(os.listdir('frames')):
-    image = Image.open(os.path.join('frames', file_name)).convert('RGBA')
+for file_name in sorted(os.listdir("samples/frames")):
+    image = Image.open(os.path.join("samples/frames", file_name)).convert("RGBA")
     frame = create_frame_from_rgba(np.array(image), image.width, image.height)
     frame.delay_num = 50
     frame.delay_den = 1000
     apngasm.add_frame(frame)
-apngasm.assemble('result-from-pillow.apng')
+apngasm.assemble("samples/result-from-pillow.apng")
 
 # Disassemble and get pillow image of one frame
 apngasm.reset()
-frames = apngasm.disassemble('input/ball.apng')
+frames = apngasm.disassemble("samples/input/ball.apng")
 frame = frames[0]
 im = Image.frombytes(mode, (frame.width, frame.height), frame.pixels)
-im.save('output/ball0.png')
+im.save("samples/output/ball0.png")
 
 # Disassemble all APNG into PNGs
-apngasm.save_pngs('output')
+apngasm.save_pngs("samples/output")
 ```
 
-The methods are based on [apngasm.h](https://github.com/apngasm/apngasm/blob/master/lib/src/apngasm.h) and [apngframe.h](https://github.com/apngasm/apngasm/blob/master/lib/src/apngframe.h)
+The methods are based on [apngasm.h](https://github.com/apngasm/apngasm/blob/master/lib/src/apngasm.h) 
+and [apngframe.h](https://github.com/apngasm/apngasm/blob/master/lib/src/apngframe.h)
 
 You can get more info about the binding from [src/apngasm_python.cpp](src/apngasm_python.cpp), or by...
 
 ```python
 from apngasm_python import _apngasm_python
 help(_apngasm_python)
 ```
 
 ## Building from source
 ```bash
-git clone https://github.com/laggykiller/apngasm-python.git
+git clone --recursive https://github.com/laggykiller/apngasm-python.git
 cd apngasm-python
-git submodule update --init --recursive
 
 # To build wheel
 python3 -m build .
 
 # To install directly
 pip3 install .
 ```
@@ -140,14 +149,30 @@
 export APNGASM_COMPILE_TARGET=x64
 export APNGASM_COMPILE_TARGET=x86
 export APNGASM_COMPILE_TARGET=armv8
 export APNGASM_COMPILE_TARGET=ppc64le
 export APNGASM_COMPILE_TARGET=s390x
 ```
 
+## Development
+To run tests:
+```bash
+pip install pytest
+pytest
+```
+
+To lint:
+```bash
+pip install ruff mypy isort
+mypy
+isort .
+ruff check
+ruff format
+```
+
 ## Credits
 - apngasm: https://github.com/apngasm/apngasm
 - Packaging: https://github.com/tttapa/py-build-cmake
 - Example files:
     - https://apng.onevcat.com/demo/
     - https://commons.wikimedia.org/wiki/File:Animated_PNG_example_bouncing_beach_ball.png
     - https://commons.wikimedia.org/wiki/File:Grayscale_8bits_palette_sample_image.png
```

### Comparing `apngasm_python-1.2.3/apngasm/.gitignore` & `apngasm_python-1.3.0/apngasm/.gitignore`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/BACKERS.txt` & `apngasm_python-1.3.0/apngasm/BACKERS.txt`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/CMakeLists.txt` & `apngasm_python-1.3.0/apngasm/CMakeLists.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 cmake_minimum_required(VERSION 3.13)
+cmake_policy(SET CMP0074 NEW)
 
 project(APNGASM)
 
 # If BUILD_SHARED_LIBS was set to OFF, prepare for static linking
 if (DEFINED BUILD_SHARED_LIBS AND NOT BUILD_SHARED_LIBS)
   set(Boost_USE_STATIC_LIBS ON)
   if (MSVC)
```

### Comparing `apngasm_python-1.2.3/apngasm/LICENSE.txt` & `apngasm_python-1.3.0/apngasm/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/README.md` & `apngasm_python-1.3.0/apngasm/README.md`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/cli/CMakeLists.txt` & `apngasm_python-1.3.0/apngasm/cli/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,30 +27,29 @@
 if (MSYS)
   include_directories("/mingw64/include")
   link_directories("/mingw64/lib")
   set(Boost_ROOT "/mingw64")
 endif ()
 
 # Search and prepare Boost
-find_package(Boost REQUIRED COMPONENTS program_options regex system)
+find_package(Boost REQUIRED COMPONENTS program_options regex filesystem system)
 include_directories(${Boost_INCLUDE_DIRS})
 
 find_package(PNG REQUIRED)
 include_directories(${PNG_INCLUDE_DIRS})
 
 # Generate executable
 add_executable(apngasm-cli
   ${PROJECT_SOURCE_DIR}/src/apngasm-cli.cpp
   ${PROJECT_SOURCE_DIR}/src/options.cpp
   ${PROJECT_SOURCE_DIR}/src/cli.cpp
 )
 set_target_properties(apngasm-cli
   PROPERTIES 
   OUTPUT_NAME apngasm
-  CXX_STANDARD 20
 )
 
 # Link to built apngasm library
 target_link_libraries(apngasm-cli
   apngasm
   ${Boost_LIBRARIES}
 )
```

### Comparing `apngasm_python-1.2.3/apngasm/cli/LICENSE.txt` & `apngasm_python-1.3.0/apngasm/cli/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/cli/package/CMakeLists.txt.in` & `apngasm_python-1.3.0/apngasm/cli/package/CMakeLists.txt.in`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/cli/src/cli.cpp` & `apngasm_python-1.3.0/apngasm/cli/src/cli.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #include "cli.h"
 #include "apngasm-cli-version.h"
 #include "listener/apngasmlistener.h"
 #include <boost/algorithm/string.hpp>
 #include <boost/regex.hpp>
-#include <filesystem>
+#include <boost/filesystem/operations.hpp>
 #include <iostream>
 
 namespace {
-const char separator = std::filesystem::path::preferred_separator;
+const char separator = boost::filesystem::path::preferred_separator;
 
 bool isNumber(const std::string s) {
   std::string::const_iterator it = s.begin();
   while (it != s.end() && std::isdigit(*it))
     ++it;
   return !s.empty() && it == s.end();
 }
@@ -70,15 +70,15 @@
     using namespace std;
     using namespace boost;
 
     if (_overwriteMode == apngasm_cli::Options::OVERWRITE_FORCE) {
       createParentDirs(filePath);
       return true;
     }
-    if (!filesystem::exists(filesystem::path(filePath))) {
+    if (!boost::filesystem::exists(boost::filesystem::path(filePath))) {
       createParentDirs(filePath);
       return true;
     }
     cout << "The file '" << filePath << "' already exists.";
     if (_overwriteMode == apngasm_cli::Options::OVERWRITE_INTERACTIVE) {
       cout << " Overwrite? [y/N]: ";
       string reply;
@@ -110,20 +110,20 @@
 
 private:
   const apngasm::APNGAsm *const _apngasm;
   const int _overwriteMode;
 
   // Return true if create succeeded.
   bool createParentDirs(const std::string &filePath) const {
-    std::filesystem::path path = filePath;
-    std::filesystem::path parent = path.parent_path();
+    boost::filesystem::path path = filePath;
+    boost::filesystem::path parent = path.parent_path();
     if (parent == "") {
       return true;
     }
-    return std::filesystem::create_directories(parent);
+    return boost::filesystem::create_directories(parent);
   }
 }; // class CustomAPNGAsmListener
 
 } // unnamed namespace
 
 namespace apngasm_cli {
 const std::string CLI::VERSION = APNGASM_CLI_VERSION;
@@ -236,33 +236,33 @@
   // Dissassemble apng file.
   std::vector<apngasm::APNGFrame> frames = assembler.disassemble(src);
   std::cout << frames.size() << " Frames" << std::endl;
 
   // Output png image files.
   std::string outdir;
   if (!options.outputFile(outdir)) {
-    std::filesystem::path path = src;
+    boost::filesystem::path path = src;
     outdir = path.replace_extension("").string();
   }
   if (!assembler.savePNGs(outdir))
     return 1;
 
   // Output json spec files.
   std::string outSpecFile;
   if (options.outputJSONFile(outSpecFile)) {
-    std::filesystem::path path = outSpecFile;
+    boost::filesystem::path path = outSpecFile;
     if (path.is_relative())
       outSpecFile = outdir + separator + outSpecFile;
 
     assembler.saveJSON(outSpecFile, outdir);
   }
 
   // Output XML spec files.
   if (options.outputXMLFile(outSpecFile)) {
-    std::filesystem::path path = outSpecFile;
+    boost::filesystem::path path = outSpecFile;
     if (path.is_relative())
       outSpecFile = outdir + separator + outSpecFile;
 
     assembler.saveXML(outSpecFile, outdir);
   }
 
   return 0;
```

### Comparing `apngasm_python-1.2.3/apngasm/cli/src/cli.h` & `apngasm_python-1.3.0/apngasm/cli/src/cli.h`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/cli/src/options.cpp` & `apngasm_python-1.3.0/apngasm/cli/src/options.cpp`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/cli/src/options.h` & `apngasm_python-1.3.0/apngasm/cli/src/options.h`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/debian/changelog` & `apngasm_python-1.3.0/apngasm/debian/changelog`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/debian/control` & `apngasm_python-1.3.0/apngasm/debian/control`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/building/win/instructions.md` & `apngasm_python-1.3.0/apngasm/docs/building/win/instructions.md`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/doxygen-config` & `apngasm_python-1.3.0/apngasm/docs/doxygen-config`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/annotated.html` & `apngasm_python-1.3.0/apngasm/docs/html/annotated.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/apngasm-conf_8h_source.html` & `apngasm_python-1.3.0/apngasm/docs/html/apngasm-conf_8h_source.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/apngasm_8h_source.html` & `apngasm_python-1.3.0/apngasm/docs/html/apngasm_8h_source.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/apngframe_8h_source.html` & `apngasm_python-1.3.0/apngasm/docs/html/apngframe_8h_source.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/bc_s.png` & `apngasm_python-1.3.0/apngasm/docs/html/bc_s.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/classapngasm_1_1APNGAsm-members.html` & `apngasm_python-1.3.0/apngasm/docs/html/classapngasm_1_1APNGAsm-members.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/classapngasm_1_1APNGAsm.html` & `apngasm_python-1.3.0/apngasm/docs/html/classapngasm_1_1APNGAsm.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/classapngasm_1_1APNGFrame-members.html` & `apngasm_python-1.3.0/apngasm/docs/html/classapngasm_1_1APNGFrame-members.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/classapngasm_1_1APNGFrame.html` & `apngasm_python-1.3.0/apngasm/docs/html/classapngasm_1_1APNGFrame.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/classes.html` & `apngasm_python-1.3.0/apngasm/docs/html/classes.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/dir_97aefd0d527b934f1d99a682da8fe6a9.html` & `apngasm_python-1.3.0/apngasm/docs/html/dir_97aefd0d527b934f1d99a682da8fe6a9.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/dir_a065c5f60305fee3569f887679366939.html` & `apngasm_python-1.3.0/apngasm/docs/html/dir_a065c5f60305fee3569f887679366939.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/doxygen.css` & `apngasm_python-1.3.0/apngasm/docs/html/doxygen.css`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/doxygen.png` & `apngasm_python-1.3.0/apngasm/docs/html/doxygen.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/dynsections.js` & `apngasm_python-1.3.0/apngasm/docs/html/dynsections.js`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/ftv2doc.png` & `apngasm_python-1.3.0/apngasm/docs/html/ftv2doc.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/ftv2folderclosed.png` & `apngasm_python-1.3.0/apngasm/docs/html/ftv2folderclosed.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/ftv2folderopen.png` & `apngasm_python-1.3.0/apngasm/docs/html/ftv2folderopen.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/ftv2link.png` & `apngasm_python-1.3.0/apngasm/docs/html/ftv2link.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/functions.html` & `apngasm_python-1.3.0/apngasm/docs/html/functions.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/functions_func.html` & `apngasm_python-1.3.0/apngasm/docs/html/functions_func.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/index.html` & `apngasm_python-1.3.0/apngasm/docs/html/index.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/jquery.js` & `apngasm_python-1.3.0/apngasm/docs/html/jquery.js`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/namespaceapngasm.html` & `apngasm_python-1.3.0/apngasm/docs/html/namespaceapngasm.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/namespacemembers.html` & `apngasm_python-1.3.0/apngasm/docs/html/namespacemembers.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/namespacemembers_vars.html` & `apngasm_python-1.3.0/apngasm/docs/html/namespacemembers_vars.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/namespaces.html` & `apngasm_python-1.3.0/apngasm/docs/html/namespaces.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/all_0.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/all_0.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/all_0.js` & `apngasm_python-1.3.0/apngasm/docs/html/search/all_0.js`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/all_1.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/all_1.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/all_2.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/all_2.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/all_3.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/all_3.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/all_4.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/all_4.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/all_5.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/all_5.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/all_6.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/all_6.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/all_61.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/all_61.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/all_7.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/all_7.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/all_7.js` & `apngasm_python-1.3.0/apngasm/docs/html/search/all_7.js`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/all_72.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/all_72.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/all_8.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/all_8.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/all_9.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/all_9.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/classes_0.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/classes_0.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/classes_1.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/classes_1.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/classes_61.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/classes_61.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/classes_72.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/classes_72.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/functions_0.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/functions_0.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/functions_0.js` & `apngasm_python-1.3.0/apngasm/docs/html/search/functions_0.js`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/functions_1.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/functions_1.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/functions_2.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/functions_2.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/functions_3.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/functions_3.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/functions_4.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/functions_4.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/functions_5.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/functions_5.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/functions_6.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/functions_6.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/functions_7.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/functions_7.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/functions_7.js` & `apngasm_python-1.3.0/apngasm/docs/html/search/functions_7.js`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/functions_8.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/functions_8.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/functions_9.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/functions_9.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/mag_sel.png` & `apngasm_python-1.3.0/apngasm/docs/html/search/mag_sel.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/namespaces_0.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/namespaces_0.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/search.css` & `apngasm_python-1.3.0/apngasm/docs/html/search/search.css`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/search.js` & `apngasm_python-1.3.0/apngasm/docs/html/search/search.js`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/search_l.png` & `apngasm_python-1.3.0/apngasm/docs/html/search/search_l.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/search_r.png` & `apngasm_python-1.3.0/apngasm/docs/html/search/search_r.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/search/variables_0.html` & `apngasm_python-1.3.0/apngasm/docs/html/search/variables_0.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/structapngasm_1_1rgb-members.html` & `apngasm_python-1.3.0/apngasm/docs/html/structapngasm_1_1rgb-members.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/structapngasm_1_1rgb.html` & `apngasm_python-1.3.0/apngasm/docs/html/structapngasm_1_1rgb.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/structapngasm_1_1rgba-members.html` & `apngasm_python-1.3.0/apngasm/docs/html/structapngasm_1_1rgba-members.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/structapngasm_1_1rgba.html` & `apngasm_python-1.3.0/apngasm/docs/html/structapngasm_1_1rgba.html`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/sync_off.png` & `apngasm_python-1.3.0/apngasm/docs/html/sync_off.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/sync_on.png` & `apngasm_python-1.3.0/apngasm/docs/html/sync_on.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/html/tabs.css` & `apngasm_python-1.3.0/apngasm/docs/html/tabs.css`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/latex/annotated.tex` & `apngasm_python-1.3.0/apngasm/docs/latex/annotated.tex`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/latex/classapngasm_1_1APNGAsm.tex` & `apngasm_python-1.3.0/apngasm/docs/latex/classapngasm_1_1APNGAsm.tex`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/latex/classapngasm_1_1APNGFrame.tex` & `apngasm_python-1.3.0/apngasm/docs/latex/classapngasm_1_1APNGFrame.tex`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/latex/dir_a065c5f60305fee3569f887679366939.tex` & `apngasm_python-1.3.0/apngasm/docs/latex/dir_a065c5f60305fee3569f887679366939.tex`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/latex/doxygen.sty` & `apngasm_python-1.3.0/apngasm/docs/latex/doxygen.sty`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/latex/namespaceapngasm.tex` & `apngasm_python-1.3.0/apngasm/docs/latex/namespaceapngasm.tex`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/latex/refman.tex` & `apngasm_python-1.3.0/apngasm/docs/latex/refman.tex`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/latex/structapngasm_1_1CHUNK.tex` & `apngasm_python-1.3.0/apngasm/docs/latex/structapngasm_1_1CHUNK.tex`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/latex/structapngasm_1_1OP.tex` & `apngasm_python-1.3.0/apngasm/docs/latex/structapngasm_1_1OP.tex`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/latex/structapngasm_1_1rgb.tex` & `apngasm_python-1.3.0/apngasm/docs/latex/structapngasm_1_1rgb.tex`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/latex/structapngasm_1_1rgba.tex` & `apngasm_python-1.3.0/apngasm/docs/latex/structapngasm_1_1rgba.tex`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/docs/man/apngasm.1` & `apngasm_python-1.3.0/apngasm/docs/man/apngasm.1`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/lib/CMakeLists.txt` & `apngasm_python-1.3.0/apngasm/lib/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -48,27 +48,25 @@
 add_library(${APNGASM_DYNAMIC_LIB_TARGET} SHARED
   ${APNGASM_SOURCES}
 )
 set_target_properties(${APNGASM_DYNAMIC_LIB_TARGET}
   PROPERTIES
   POSITION_INDEPENDENT_CODE TRUE
   OUTPUT_NAME apngasm
-  CXX_STANDARD 20
 )
 
 # Add the static library/archive
 set(APNGASM_STATIC_LIB_TARGET apngasm-static)
 add_library(${APNGASM_STATIC_LIB_TARGET}
   ${APNGASM_SOURCES}
 )
 set_target_properties(${APNGASM_STATIC_LIB_TARGET}
   PROPERTIES
   POSITION_INDEPENDENT_CODE TRUE
   OUTPUT_NAME apngasm
-  CXX_STANDARD 20
 )
 
 # Add libraries/includes
 #target_link_libraries(${APNGASM_DYNAMIC_LIB_TARGET} stdc++fs)
 #target_link_libraries(${APNGASM_STATIC_LIB_TARGET} stdc++fs)
 
 find_package(ZLIB REQUIRED)
@@ -79,15 +77,15 @@
 find_package(PNG REQUIRED)
 include_directories(${PNG_INCLUDE_DIR})
 target_link_libraries(${APNGASM_DYNAMIC_LIB_TARGET} ${PNG_LIBRARIES})
 target_link_libraries(${APNGASM_STATIC_LIB_TARGET} ${PNG_LIBRARIES})
 message(${PNG_VERSION_STRING})
 
 #SET(CMAKE_FIND_LIBRARY_SUFFIXES .dll.a .a .lib ${CMAKE_FIND_LIBRARY_SUFFIXES})
-find_package(Boost REQUIRED COMPONENTS program_options regex system)
+find_package(Boost REQUIRED COMPONENTS program_options regex system filesystem)
 include_directories(SYSTEM ${Boost_INCLUDE_DIRS})
 target_link_libraries(${APNGASM_DYNAMIC_LIB_TARGET} ${Boost_LIBRARIES})
 target_link_libraries(${APNGASM_STATIC_LIB_TARGET} ${Boost_LIBRARIES})
 
 get_target_property(APNGASM_DYNAMIC_LIB_TARGET_NAME ${APNGASM_DYNAMIC_LIB_TARGET} OUTPUT_NAME)
 get_target_property(APNGASM_STATIC_LIB_TARGET_NAME ${APNGASM_STATIC_LIB_TARGET} OUTPUT_NAME)
 set(APNGASM_LIBRARIES
```

### Comparing `apngasm_python-1.2.3/apngasm/lib/DESCRIPTION.txt` & `apngasm_python-1.3.0/apngasm/lib/DESCRIPTION.txt`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/lib/LICENSE.txt` & `apngasm_python-1.3.0/apngasm/lib/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/lib/interfaces/java/CMakeLists.txt` & `apngasm_python-1.3.0/apngasm/lib/interfaces/java/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/lib/interfaces/java/NativeLibLoader.java.in` & `apngasm_python-1.3.0/apngasm/lib/interfaces/java/NativeLibLoader.java.in`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/lib/interfaces/ruby/CMakeLists.txt` & `apngasm_python-1.3.0/apngasm/lib/interfaces/ruby/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/lib/package/CMakeLists.txt.in` & `apngasm_python-1.3.0/apngasm/lib/package/CMakeLists.txt.in`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/lib/src/apng.i` & `apngasm_python-1.3.0/apngasm/lib/src/apng.i`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/lib/src/apngasm.cpp` & `apngasm_python-1.3.0/apngasm/lib/src/apngasm.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #include "apngasm.h"
 #include <cstdlib>
-#include <filesystem>
 #include <png.h>
 #include <zlib.h>
 #include <boost/algorithm/string/predicate.hpp>
+#include <boost/filesystem/operations.hpp>
 #include <boost/regex.hpp>
 #include <boost/range/algorithm.hpp>
 #ifdef APNG_SPECS_SUPPORTED
 #include "spec/specreader.h"
 #include "spec/specwriter.h"
 #endif
 #include "listener/apngasmlistener.h"
@@ -52,61 +52,61 @@
   {
 
     // Get file path vector.
     const std::vector<std::string>& getFiles(const std::string& filepath)
     {
       static std::vector<std::string> files;
 
-      std::filesystem::path nativePath(filepath);
+      boost::filesystem::path nativePath(filepath);
       nativePath.make_preferred();
 
       // filepath is current directory.
       if( !nativePath.has_parent_path() )
       {
-        const std::string currentDirPath = "." + std::string(1, std::filesystem::path::preferred_separator);
+        const std::string currentDirPath = "." + std::string(1, boost::filesystem::path::preferred_separator);
         nativePath = currentDirPath + nativePath.string();
       }
 
       // Clear temporary vector.
       files.clear();
 
       // File is unique.
       if (nativePath.string().find('*', 0) == std::string::npos)
       {
         // Add extension
         if (!boost::algorithm::iends_with(nativePath.string(), ".png"))
           nativePath = nativePath.string() + ".png";
 
-        if (std::filesystem::exists(nativePath))
+        if (boost::filesystem::exists(nativePath))
           files.push_back(nativePath.string());
       }
 
       // File path has wildcard.
       else
       {
-        const std::filesystem::path &parentPath = nativePath.parent_path();
+        const boost::filesystem::path &parentPath = nativePath.parent_path();
 
         // Convert filepath.
         static const boost::regex escape("[\\^\\.\\$\\|\\(\\)\\[\\]\\+\\?\\\\]");
         static const boost::regex wildcard("\\*");
 
         nativePath = boost::regex_replace(nativePath.string(), escape, "\\\\$0");
         nativePath = boost::regex_replace(nativePath.string(), wildcard, ".*");
 
         // Skip if directory is not found.
-        if (!std::filesystem::exists(parentPath))
+        if (!boost::filesystem::exists(parentPath))
           return files;
 
         // Search files.
         const boost::regex filter(nativePath.string());
-        const std::filesystem::directory_iterator itEnd;
-        for (std::filesystem::directory_iterator itCur(parentPath); itCur != itEnd; ++itCur)
+        const boost::filesystem::directory_iterator itEnd;
+        for (boost::filesystem::directory_iterator itCur(parentPath); itCur != itEnd; ++itCur)
         {
           // Skip if not a file.
-          if (!std::filesystem::is_regular_file(itCur->status()))
+          if (!boost::filesystem::is_regular_file(itCur->status()))
             continue;
 
           // Skip if no match.
           const std::string& curFilePath = itCur->path().string();
           if (!boost::regex_match(curFilePath, filter))
             continue;
```

### Comparing `apngasm_python-1.2.3/apngasm/lib/src/apngasm.h` & `apngasm_python-1.3.0/apngasm/lib/src/apngasm.h`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/lib/src/apngframe.cpp` & `apngasm_python-1.3.0/apngasm/lib/src/apngframe.cpp`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/lib/src/apngframe.h` & `apngasm_python-1.3.0/apngasm/lib/src/apngframe.h`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/lib/src/listener/apngasmlistener.cpp` & `apngasm_python-1.3.0/apngasm/lib/src/listener/apngasmlistener.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #include "apngasmlistener.h"
-#include <filesystem>
 #include <sstream>
+#include <boost/filesystem/operations.hpp>
 
 namespace apngasm {
 namespace listener {
 
 // Called before add frame.
 // Return true if can add.
 bool APNGAsmListener::onPreAddFrame(const std::string &filePath,
@@ -42,15 +42,15 @@
   // nop
 }
 
 // Called when create output path of png file.
 // Return output path.
 const std::string APNGAsmListener::onCreatePngPath(const std::string &outputDir,
                                                    int index) const {
-  const char separator = std::filesystem::path::preferred_separator;
+  const char separator = boost::filesystem::path::preferred_separator;
   const std::string separatorStr =
       (outputDir.empty() || *outputDir.rbegin() == separator)
           ? ""
           : std::string(1, separator);
   std::ostringstream result;
   result << outputDir << separatorStr << index << ".png";
   return result.str();
```

### Comparing `apngasm_python-1.2.3/apngasm/lib/src/listener/apngasmlistener.h` & `apngasm_python-1.3.0/apngasm/lib/src/listener/apngasmlistener.h`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/lib/src/spec/priv/specreaderimpl.cpp` & `apngasm_python-1.3.0/apngasm/lib/src/spec/priv/specreaderimpl.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #include "specreaderimpl.h"
 #include "../../apngframe.h"  // DEFAULT_FRAME_NUMERATOR, DEFAULT_FRAME_DENOMINATOR
-#include <filesystem>
+#include <boost/filesystem/operations.hpp>
 #include <boost/property_tree/json_parser.hpp>
 #include <boost/property_tree/xml_parser.hpp>
 #include <boost/lexical_cast.hpp>
 #include <boost/foreach.hpp>
 
 namespace apngasm {
   namespace spec {
@@ -100,18 +100,18 @@
       bool JSONSpecReaderImpl::read(const std::string& filePath)
       {
         // Read JSON file.
         boost::property_tree::ptree root;
         boost::property_tree::read_json(filePath, root);
 
         // Set current directory.
-        const std::filesystem::path oldPath = std::filesystem::current_path();
-        const std::filesystem::path currentPath = std::filesystem::path(filePath);
+        const boost::filesystem::path oldPath = boost::filesystem::current_path();
+        const boost::filesystem::path currentPath = boost::filesystem::path(filePath);
         if(currentPath.has_parent_path())
-          std::filesystem::current_path(currentPath.parent_path());
+          boost::filesystem::current_path(currentPath.parent_path());
 
         // Read fields.
         // name
         if( boost::optional<std::string> value = root.get_optional<std::string>("name") )
         {
           _name = value.get();
         }
@@ -177,40 +177,40 @@
               const boost::property_tree::ptree::value_type& value = frame.front();
               file = value.first;
               if( !str2delay(value.second.data(), &delay) )
                 delay = defaultDelay;
             }
 
             // Add frame informations.
-            const FrameInfo frameInfo = { std::filesystem::absolute(file).string(), delay };
+            const FrameInfo frameInfo = { boost::filesystem::absolute(file).string(), delay };
             _frameInfos.push_back(frameInfo);
 
             ++delayIndex;
           }
         }
 
         // Reset current directory.
-        std::filesystem::current_path(oldPath);
+        boost::filesystem::current_path(oldPath);
 
         return true;
       }
       
       // Read parameter from spec file.
       // Return true if read succeeded.
       bool XMLSpecReaderImpl::read(const std::string& filePath)
       {
         // Read XML file.
         boost::property_tree::ptree root;
         boost::property_tree::read_xml(filePath, root);
 
         // Set current directory.
-        const std::filesystem::path oldPath = std::filesystem::current_path();
-        const std::filesystem::path currentPath = std::filesystem::path(filePath);
+        const boost::filesystem::path oldPath = boost::filesystem::current_path();
+        const boost::filesystem::path currentPath = boost::filesystem::path(filePath);
         if(currentPath.has_parent_path())
-          std::filesystem::current_path(currentPath.parent_path());
+          boost::filesystem::current_path(currentPath.parent_path());
 
         // Read fields.
         // name
         if( boost::optional<std::string> value = root.get_optional<std::string>("animation.<xmlattr>.name") )
         {
           _name = value.get();
         }
@@ -263,21 +263,21 @@
             }
             else
             {
               delay = defaultDelay;
             }
 
             // Add frame informations.
-            const FrameInfo frameInfo = { std::filesystem::absolute(file).string(), delay };
+            const FrameInfo frameInfo = { boost::filesystem::absolute(file).string(), delay };
             _frameInfos.push_back(frameInfo);
           }
         }
 
         // Reset current directory.
-        std::filesystem::current_path(oldPath);
+        boost::filesystem::current_path(oldPath);
 
         return true;
       }
 
     } // namespace priv
   } // namespace spec
 } // namespace apngasm
```

### Comparing `apngasm_python-1.2.3/apngasm/lib/src/spec/priv/specreaderimpl.h` & `apngasm_python-1.3.0/apngasm/lib/src/spec/priv/specreaderimpl.h`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/lib/src/spec/priv/specwriterimpl.cpp` & `apngasm_python-1.3.0/apngasm/lib/src/spec/priv/specwriterimpl.cpp`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/lib/src/spec/priv/specwriterimpl.h` & `apngasm_python-1.3.0/apngasm/lib/src/spec/priv/specwriterimpl.h`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/lib/src/spec/specreader.cpp` & `apngasm_python-1.3.0/apngasm/lib/src/spec/specreader.cpp`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/lib/src/spec/specreader.h` & `apngasm_python-1.3.0/apngasm/lib/src/spec/specreader.h`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/lib/src/spec/specwriter.cpp` & `apngasm_python-1.3.0/apngasm/lib/src/spec/specwriter.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #include "specwriter.h"
 #include "priv/specwriterimpl.h"
 #include "../apngasm.h"
-#include <filesystem>
+#include <boost/filesystem/operations.hpp>
 
 namespace apngasm {
   namespace spec {
 
     namespace {
-      const char separator = std::filesystem::path::preferred_separator;
+      const char separator = boost::filesystem::path::preferred_separator;
 
-      const std::filesystem::path createAbsolutePath(const std::string& path)
+      const boost::filesystem::path createAbsolutePath(const std::string& path)
       {
-        const std::filesystem::path oldPath = std::filesystem::current_path();
-        std::filesystem::path result = path;
-        std::filesystem::current_path(result.parent_path());
-        result = std::filesystem::current_path();
-        std::filesystem::current_path(oldPath);
+        const boost::filesystem::path oldPath = boost::filesystem::current_path();
+        boost::filesystem::path result = path;
+        boost::filesystem::current_path(result.parent_path());
+        result = boost::filesystem::current_path();
+        boost::filesystem::current_path(oldPath);
         return result;
       }
 
       const std::string createRelativeDir(const std::string& from, const std::string& to)
       {
-        std::filesystem::path fromPath = createAbsolutePath(from);
-        std::filesystem::path toPath = createAbsolutePath(to);
+        boost::filesystem::path fromPath = createAbsolutePath(from);
+        boost::filesystem::path toPath = createAbsolutePath(to);
         const std::string separatorStr = std::string(1, separator);
 
         // Convert path to native.
         fromPath.make_preferred();
         toPath.make_preferred();
         if (*fromPath.string().rbegin() != separator)
           fromPath /= separatorStr;
```

### Comparing `apngasm_python-1.2.3/apngasm/lib/src/spec/specwriter.h` & `apngasm_python-1.3.0/apngasm/lib/src/spec/specwriter.h`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/00.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/00.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/01.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/01.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/02.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/02.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/03.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/03.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/04.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/04.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/05.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/05.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/06.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/06.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/07.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/07.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/08.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/08.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/09.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/09.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/10.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/10.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/11.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/11.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/12.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/12.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/13.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/13.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/14.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/14.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/15.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/15.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/16.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/16.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/17.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/17.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/18.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/18.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/19.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/19.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/20.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/20.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/21.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/21.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/22.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/22.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/24.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/24.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/25.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/25.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/26.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/26.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/27.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/27.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/28.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/28.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/29.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/29.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/30.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/30.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/31.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/31.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/32.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/32.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm/33.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm/33.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/resources/images/apngasm.png` & `apngasm_python-1.3.0/apngasm/resources/images/apngasm.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/test/CMakeLists.txt` & `apngasm_python-1.3.0/apngasm/test/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
   EXCLUDE_FROM_ALL
   ${PROJECT_SOURCE_DIR}/cpp/apngasm-test.cpp
 )
 
 set_target_properties(apngasm-cpp-test
   PROPERTIES
   OUTPUT_NAME apngasm-cpp-test
-  CXX_STANDARD 20
 )
 
 link_directories(${PROJECT_BINARY_DIR}/lib)
 include_directories(
   ${PROJECT_SOURCE_DIR}/../lib/src
   ${CMAKE_BINARY_DIR}/lib/src
 )
```

### Comparing `apngasm_python-1.2.3/apngasm/test/cli/delay-test.sh` & `apngasm_python-1.3.0/apngasm/test/cli/delay-test.sh`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/test/cpp/apngasm-test.cpp` & `apngasm_python-1.3.0/apngasm/test/cpp/apngasm-test.cpp`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/test/samples/clk-first.png` & `apngasm_python-1.3.0/apngasm/test/samples/clk-first.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/test/samples/clock1.png` & `apngasm_python-1.3.0/apngasm/test/samples/clock1.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/test/samples/clock2.png` & `apngasm_python-1.3.0/apngasm/test/samples/clock2.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/test/samples/clock3.png` & `apngasm_python-1.3.0/apngasm/test/samples/clock3.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/test/samples/clock4.png` & `apngasm_python-1.3.0/apngasm/test/samples/clock4.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/test/samples/gold01.png` & `apngasm_python-1.3.0/apngasm/test/samples/gold01.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/test/samples/gold02.png` & `apngasm_python-1.3.0/apngasm/test/samples/gold02.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/test/samples/gold03.png` & `apngasm_python-1.3.0/apngasm/test/samples/gold03.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/test/samples/penguins.png` & `apngasm_python-1.3.0/apngasm/test/samples/penguins.png`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/apngasm/windows/compile_deps.bat` & `apngasm_python-1.3.0/apngasm/windows/compile_deps.bat`

 * *Files 8% similar despite different names*

```diff
@@ -20,11 +20,11 @@
 cd %APNGASM_BUILD_PATH%
 curl -O -L "https://boostorg.jfrog.io/artifactory/main/release/1.82.0/source/boost_1_82_0.zip"
 tar -xf boost_1_82_0.zip
 del boost_1_82_0.zip
 move boost_1_82_0 boost
 cd boost
 call bootstrap.bat --prefix=.
-b2.exe install --build-dir=tmp --prefix=. --build-type=complete --with-program_options --with-regex --with-system -j4 msvc stage
+b2.exe install --build-dir=tmp --prefix=. --build-type=complete --with-program_options --with-regex --with-system --with-filesystem -j4 msvc stage
 robocopy include\boost-1_82\boost include\boost /E
 
 exit 0
```

### Comparing `apngasm_python-1.2.3/cmake/QueryPythonForNanobind.cmake` & `apngasm_python-1.3.0/cmake/QueryPythonForNanobind.cmake`

 * *Files identical despite different names*

### Comparing `apngasm_python-1.2.3/conanfile.py` & `apngasm_python-1.3.0/conanfile.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from conan import ConanFile
+#!/usr/bin/env python3
+# type: ignore
 import shutil
-from scripts.get_arch import get_arch
-from conan.tools.cmake import CMake, CMakeToolchain, CMakeDeps, cmake_layout
+
+from conan import ConanFile
 from conan.tools.apple import is_apple_os
+from conan.tools.cmake import CMakeDeps, CMakeToolchain
+
+from scripts.get_arch import get_arch
 
 
 class ApngasmRecipe(ConanFile):
     settings = "os", "compiler", "build_type", "arch"
 
     def requirements(self):
-        self.requires("zlib/1.2.13") # type: ignore
-        self.requires("libpng/1.6.40") # type: ignore
-        self.requires(
-            "boost/1.75.0" # type: ignore
-        )  # https://github.com/conan-io/conan-center-index/issues/19704
+        self.requires("zlib/1.3.1")
+        self.requires("libpng/1.6.42")
+        self.requires("boost/1.84.0")
 
     def build_requirements(self):
-        self.build_requires("b2/4.10.1") # type: ignore
+        self.build_requires("b2/4.10.1")
         if not shutil.which("cmake"):
-            self.tool_requires("cmake/[>=3.27]") # type: ignore
+            self.tool_requires("cmake/[>=3.27]")
 
     def build(self):
-        build_type = "Release"
+        build_type = "Release"  # noqa: F841
 
     def generate(self):
         tc = CMakeToolchain(self)
         cmake = CMakeDeps(self)
         if is_apple_os(self) and get_arch() == "universal2":
-            tc.blocks["apple_system"].values[
-                "cmake_osx_architectures"
-            ] = "x86_64; arm64"
+            tc.blocks["apple_system"].values["cmake_osx_architectures"] = (
+                "x86_64; arm64"
+            )
         tc.generate()
         cmake.generate()
```

### Comparing `apngasm_python-1.2.3/pyproject.toml` & `apngasm_python-1.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,77 +1,100 @@
 [project] # Project metadata
 name = "apngasm-python"
-description = "A nanobind API for apngasm, a tool/library for APNG assembly/disassembly."
+description = "A nanobind python API for apngasm, a tool/library for APNG assembly & disassembly with compression support."
 requires-python = ">=3.8"
 readme = "README.md"
 license = { "file" = "LICENSE" }
 authors = [{ "name" = "chaudominic", "email" = "chaudominic2@gmail.com" }]
 keywords = ["apng", "png", "nanobind", "pybind11"]
 classifiers = ["Topic :: Multimedia :: Graphics"]
 dependencies = []
 dynamic = ["version"]
 
 [project.urls]
 Repository = "https://github.com/laggykiller/apngasm-python"
 Documentation = "https://apngasm-python.readthedocs.io/en/latest/"
 Tracker = "https://github.com/laggykiller/apngasm-python/issues"
 
+[project.optional-dependencies]
+full = [
+    "Pillow",
+    "numpy",
+]
+
+test = [
+    "pytest",
+]
+
+lint = [
+    "ruff",
+    "mypy",
+    "isort",
+    "types-Pillow",
+]
+
 [build-system] # How pip and other frontends should build this project
 requires = [
-    "py-build-cmake==0.2.0a7",
-    "nanobind~=1.8.0",
-    "nanobind-stubgen==0.1.3",
-    "conan>=2.0",
-    "wheel"
+    "py-build-cmake==0.2.0a12",
+    "nanobind>=2.0.0",
+    "conan>=2.0"
 ]
 build-backend = "py_build_cmake.build"
 
 [tool.py-build-cmake.module] # Where to find the Python module to package
 name = "apngasm_python"
 directory = "src-python"
 
 [tool.py-build-cmake.sdist] # What to include in source distributions
 include = [
     "CMakeLists.txt",
+    "PreLoad.cmake",
     "cmake/*.cmake",
     "src/*",
     "src-python/*",
     "scripts/*",
     "conanfile.py",
-    "apngasm/*"
+    "apngasm/*",
+    "lipo-dir-merge/*.py"
 ]
 
 [tool.py-build-cmake.cmake] # How to build the CMake project
 build_type = "Release"
 source_path = "."
-options = { "WITH_PY_STUBS:BOOL" = "On" }
 args = ["-Wdev"]
 find_python3 = false
 find_python = true
 build_args = ["-j", "--verbose"]
 build_tool_args = []
 install_args = ["--verbose"]
 install_components = ["python_modules"]
 env = {}
 python_abi = 'abi3'
 abi3_minimum_cpython_version = 312
 
 [tool.py-build-cmake.linux.cmake] # Linux-specific options
-generator = "Ninja Multi-Config"
 config = "Release"
 env = { "CMAKE_PREFIX_PATH" = "${HOME}/.local" }
 
 [tool.py-build-cmake.mac.cmake] # macOS-specific options
-generator = "Ninja Multi-Config"
 config = "Release"
 
 [tool.py-build-cmake.windows.cmake] # Windows-specific options
 config = "Release"
-[tool.py-build-cmake.windows.cmake.options]
-CMAKE_CXX_FLAGS_RELWITHDEBINFO = "/Zi /Ob0 /Od /RTC1"
-
-[tool.py-build-cmake.stubgen]
-args = ["-v"]
 
 [tool.cibuildwheel]
 build-verbosity = 1
-environment = { PY_BUILD_CMAKE_VERBOSE="1" }
+environment = { PY_BUILD_CMAKE_VERBOSE="1" }
+
+[tool.pyright]
+include = ["src-python", "scripts", "tests", "example"]
+strict = ["*"]
+
+[tool.mypy]
+python_version = "3.9"
+files = ["src-python", "scripts", "tests", "example"]
+
+[tool.isort]
+extend_skip = ["lipo-dir-merge"]
+
+[tool.ruff]
+exclude = ["lipo-dir-merge"]
```

### Comparing `apngasm_python-1.2.3/src/apngasm_python.cpp` & `apngasm_python-1.3.0/src/apngasm_python.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#ifdef _WINDOWS
+#if defined(_WIN32) && !defined(__GNUC__)
 #  ifdef _apngasm_python_EXPORTS
 #    define APNGASM_PY_DECLSPEC __declspec(dllexport)
 #  else
 #    define APNGASM_PY_DECLSPEC __declspec(dllimport)
 #  endif
 #else
 #  define APNGASM_PY_DECLSPEC __attribute__ ((visibility("default")))
@@ -33,15 +33,15 @@
 };
 
 NB_MODULE(MODULE_NAME, m) {
     m.doc() = "A nanobind API for apngasm, a tool/library for APNG assembly/disassembly";
     m.attr("__version__") = VERSION_INFO;
 
     m.def("create_frame_from_rgb", [](
-        nb::ndarray<unsigned char, nb::shape<nb::any, nb::any, 3>> *pixels,
+        nb::ndarray<unsigned char, nb::shape<-1, -1, 3>> *pixels,
         unsigned int width, unsigned int height,
         unsigned delayNum = apngasm::DEFAULT_FRAME_NUMERATOR,
         unsigned delayDen = apngasm::DEFAULT_FRAME_DENOMINATOR
     ) APNGASM_PY_DECLSPEC {
         apngasm::rgb *pixelsNew = new apngasm::rgb[pixels->shape(0)*pixels->shape(1)];
         unsigned char *pixels_ptr = pixels->data();
 
@@ -68,15 +68,15 @@
     :param int delay_den: The delay denominator for this frame (defaults to DEFAULT_FRAME_DENMINATOR).
     
     :return: A APNGFrame object.
     :rtype: apngasm_python._apngasm_python.APNGFrame
     )pbdoc");
 
     m.def("create_frame_from_rgb_trns", [](
-        nb::ndarray<unsigned char, nb::shape<nb::any, nb::any, 3>> *pixels,
+        nb::ndarray<unsigned char, nb::shape<-1, -1, 3>> *pixels,
         unsigned int width, unsigned int height,
         nb::ndarray<unsigned char, nb::shape<3>> *trns_color,
         unsigned delayNum = apngasm::DEFAULT_FRAME_NUMERATOR,
         unsigned delayDen = apngasm::DEFAULT_FRAME_DENOMINATOR
     ) APNGASM_PY_DECLSPEC {
         apngasm::rgb *pixelsNew = new apngasm::rgb[pixels->shape(0)*pixels->shape(1)];
         unsigned char *pixels_ptr = pixels->data();
@@ -113,15 +113,15 @@
     :param int delay_den: The delay denominator for this frame (defaults to DEFAULT_FRAME_DENMINATOR).
     
     :return: A APNGFrame object.
     :rtype: apngasm_python._apngasm_python.APNGFrame
     )pbdoc");
     
     m.def("create_frame_from_rgba", [](
-        nb::ndarray<unsigned char, nb::shape<nb::any, nb::any, 4>> *pixels,
+        nb::ndarray<unsigned char, nb::shape<-1, -1, 4>> *pixels,
         unsigned int width, unsigned int height,
         unsigned delayNum = apngasm::DEFAULT_FRAME_NUMERATOR,
         unsigned delayDen = apngasm::DEFAULT_FRAME_DENOMINATOR
     ) APNGASM_PY_DECLSPEC {
         apngasm::rgba *pixelsNew = new apngasm::rgba[pixels->shape(0)*pixels->shape(1)];
         unsigned char *pixels_ptr = pixels->data();
 
@@ -253,17 +253,17 @@
         :rtype: bool
         )pbdoc")
 
         .def_prop_rw("pixels", 
         [](apngasm::APNGFrame &t) APNGASM_PY_DECLSPEC {
             size_t rowbytes = rowbytesMap[t._colorType];
             size_t shape[3] = { t._height, t._width, rowbytes };
-            return nb::ndarray<nb::numpy, unsigned char, nb::shape<nb::any, nb::any, nb::any>>(t._pixels, 3, shape);
+            return nb::ndarray<nb::numpy, unsigned char, nb::shape<-1, -1, -1>>(t._pixels, 3, shape, nb::handle());
         },
-        [](apngasm::APNGFrame &t, nb::ndarray<unsigned char, nb::shape<nb::any, nb::any, nb::any>> *v) APNGASM_PY_DECLSPEC {
+        [](apngasm::APNGFrame &t, nb::ndarray<unsigned char, nb::shape<-1, -1, -1>> *v) APNGASM_PY_DECLSPEC {
             size_t rowbytes = rowbytesMap[t._colorType];
             unsigned char *pixelsNew = new unsigned char[v->size()];
             unsigned char *v_ptr = v->data();
 
             for (int i = 0; i < v->size(); ++i) {
                 pixelsNew[i] = v_ptr[i];
             }
@@ -312,15 +312,15 @@
             unsigned char paletteView[256][3];
             for (int i = 0; i < 256; ++i) {
                 paletteView[i][0] = t._palette[i].r;
                 paletteView[i][1] = t._palette[i].g;
                 paletteView[i][2] = t._palette[i].b;
             }
             size_t shape[2] = { 256, 3 };
-            return nb::ndarray<nb::numpy, unsigned char, nb::shape<256, 3>>(paletteView, 2, shape); 
+            return nb::ndarray<nb::numpy, unsigned char, nb::shape<256, 3>>(paletteView, 2, shape, nb::handle()); 
         },
         [](apngasm::APNGFrame &t, nb::ndarray<unsigned char, nb::shape<256, 3>> *v) APNGASM_PY_DECLSPEC {
             unsigned char *v_ptr = v->data();
             for (int i = 0; i < 256; ++i) {
                 t._palette[i].r = v_ptr[0];
                 t._palette[i].g = v_ptr[1];
                 t._palette[i].b = v_ptr[2];
@@ -331,17 +331,17 @@
         The palette data of frame. Only applies to 'P' mode Image (i.e. Not RGB, RGBA).
         Expressed as 2D numpy array in format of [[r0, g0, b0], [r1, g1, b1], ..., [r255, g255, b255]] in Python.
         )pbdoc")
 
         .def_prop_rw("transparency", 
         [](apngasm::APNGFrame &t) APNGASM_PY_DECLSPEC {
             size_t shape[1] = { static_cast<size_t>(t._transparencySize) };
-            return nb::ndarray<nb::numpy, unsigned char, nb::shape<nb::any>>(t._transparency, 1, shape); 
+            return nb::ndarray<nb::numpy, unsigned char, nb::shape<-1>>(t._transparency, 1, shape, nb::handle()); 
         },
-        [](apngasm::APNGFrame &t, nb::ndarray<unsigned char, nb::shape<nb::any>> *v) APNGASM_PY_DECLSPEC {
+        [](apngasm::APNGFrame &t, nb::ndarray<unsigned char, nb::shape<-1>> *v) APNGASM_PY_DECLSPEC {
             unsigned char *v_ptr = v->data();
             for (int i = 0; i < v->shape(0); ++i) {
                 t._transparency[i] = *v_ptr;
                 ++v_ptr;
             }
         },
         R"pbdoc(
@@ -419,15 +419,15 @@
         :param int delay_den: The delay denominator for this frame (defaults to DEFAULT_FRAME_DENMINATOR).
 
         :return: The new number of frames/the number of this frame on the frame vector.
         :rtype: int
         )pbdoc")
 
         .def("add_frame_from_rgb", nb::overload_cast<apngasm::rgb *, unsigned int, unsigned int, apngasm::rgb *, unsigned, unsigned>(&apngasm::APNGAsm::addFrame),
-        "pixels_rgb"_a, "width"_a, "height"_a, "trns_color"_a = NULL, "delay_num"_a = apngasm::DEFAULT_FRAME_NUMERATOR, "delay_den"_a = apngasm::DEFAULT_FRAME_DENOMINATOR,
+        "pixels_rgb"_a, "width"_a, "height"_a, "trns_color"_a.none(), "delay_num"_a = apngasm::DEFAULT_FRAME_NUMERATOR, "delay_den"_a = apngasm::DEFAULT_FRAME_DENOMINATOR,
         R"pbdoc(
         Adds an APNGFrame object to the vector.
         Not possible to use in Python. As alternative,
         Use create_frame_from_rgb() or create_frame_from_rgba(). Or manually,
         First create an empty APNGFrame with frame = APNGFrame(),
         then set frame.width, frame.height, frame.color_type, frame.pixels,
         frame.palette, frame.delay_num, frame.delay_den manually.
```

### Comparing `apngasm_python-1.2.3/src-python/apngasm_python/_apngasm_python/__init__.pyi` & `apngasm_python-1.3.0/src-python/apngasm_python/_apngasm_python.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,605 +1,482 @@
-from __future__ import annotations
-import numpy.typing
-from typing import Any, Optional, overload, Typing, Sequence
-from enum import Enum
-from . import _apngasm_python
+from collections.abc import Sequence
+from typing import Annotated, Optional, overload
+
+from numpy.typing import ArrayLike
+
 
 class APNGAsm:
-    """
-    Class representing APNG file, storing APNGFrame(s) and other metadata.
-    """
+    """Class representing APNG file, storing APNGFrame(s) and other metadata."""
 
-    def __init__(self, frames: list[_apngasm_python.APNGFrame]) -> None:
-        """
-        Construct APNGAsm object from an existing vector of apngasm frames.
-        
-        :param list[apngasm_python._apngasm_python.APNGFrame] frames: A list of APNGFrame objects.
-        """
-        ...
-    
     @overload
     def __init__(self) -> None:
+        """Construct an empty APNGAsm object."""
+
+    @overload
+    def __init__(self, frames: Sequence[APNGFrame]) -> None:
         """
-        Construct an empty APNGAsm object.
+        Construct APNGAsm object from an existing vector of apngasm frames.
+
+        :param list[apngasm_python._apngasm_python.APNGFrame] frames: A list of APNGFrame objects.
         """
-        ...
-    
-    def add_frame(self, frame: _apngasm_python.APNGFrame) -> int:
+
+    def add_frame(self, frame: APNGFrame) -> int:
         """
         Adds an APNGFrame object to the frame vector.
-        
+
         :param frame: The APNGFrame object to be added.
         :type frame: apngasm_python._apngasm_python.APNGFrame
-        
+
         :return: The new number of frames/the number of this frame on the frame vector.
         :rtype: int
         """
-        ...
-    
+
     def add_frame_from_file(self, file_path: str, delay_num: int = 100, delay_den: int = 1000) -> int:
         """
         Adds a frame from a PNG file or frames from a APNG file to the frame vector.
-        
+
         :param str file_path: The relative or absolute path to an image file.
         :param int delay_num: The delay numerator for this frame (defaults to DEFAULT_FRAME_NUMERATOR).
         :param int delay_den: The delay denominator for this frame (defaults to DEFAULT_FRAME_DENMINATOR).
-        
+
         :return: The new number of frames/the number of this frame on the frame vector.
         :rtype: int
         """
-        ...
-    
-    def add_frame_from_rgb(self, pixels_rgb: _apngasm_python.rgb, width: int, height: int, trns_color: _apngasm_python.rgb = 0, delay_num: int = 100, delay_den: int = 1000) -> int:
+
+    def add_frame_from_rgb(self, pixels_rgb: rgb, width: int, height: int, trns_color: Optional[rgb], delay_num: int = 100, delay_den: int = 1000) -> int:
         """
         Adds an APNGFrame object to the vector.
         Not possible to use in Python. As alternative,
         Use create_frame_from_rgb() or create_frame_from_rgba(). Or manually,
         First create an empty APNGFrame with frame = APNGFrame(),
         then set frame.width, frame.height, frame.color_type, frame.pixels,
         frame.palette, frame.delay_num, frame.delay_den manually.
-        
+
         :param apngasm_python._apngasm_python.rgb pixels_rgb: The RGB pixel data.
         :param int width: The width of the pixel data.
         :param int height: The height of the pixel data.
         :param apngasm_python._apngasm_python.rgb trns_color: The color [r, g, b] to be treated as transparent.
         :param int delay_num: The delay numerator for this frame (defaults to DEFAULT_FRAME_NUMERATOR).
         :param int delay_den: The delay denominator for this frame (defaults to DEFAULT_FRAME_DENMINATOR).
-        
+
         :return: The new number of frames/the number of this frame on the frame vector.
         :rtype: int
         """
-        ...
-    
-    def add_frame_from_rgba(self, pixels_rgba: _apngasm_python.rgba, width: int, height: int, delay_num: int = 100, delay_den: int = 1000) -> int:
+
+    def add_frame_from_rgba(self, pixels_rgba: rgba, width: int, height: int, delay_num: int = 100, delay_den: int = 1000) -> int:
         """
         Adds an APNGFrame object to the vector.
         Not possible to use in Python. As alternative,
         Use create_frame_from_rgb() or create_frame_from_rgba(). Or manually,
         First create an empty APNGFrame with frame = APNGFrame(),
         then set frame.width, frame.height, frame.color_type, frame.pixels,
         frame.palette, frame.delay_num, frame.delay_den manually.
-        
+
         :param apngasm_python._apngasm_python.rgba pixels_rgba: The RGBA pixel data.
         :param int width: The width of the pixel data.
         :param int height: The height of the pixel data.
         :param int delay_num: The delay numerator for this frame (defaults to DEFAULT_FRAME_NUMERATOR).
         :param int delay_den: The delay denominator for this frame (defaults to DEFAULT_FRAME_DENMINATOR).
-        
+
         :return: The new number of frames/the number of this frame on the frame vector.
         :rtype: int
         """
-        ...
-    
+
     def assemble(self, output_path: str) -> bool:
         """
         Assembles and outputs an APNG file.
-        
+
         :param str output_path: The output file path.
-        
+
         :return: true if assemble completed succesfully.
         :rtype: bool
         """
-        ...
-    
-    def disassemble(self, file_path: str) -> list[_apngasm_python.APNGFrame]:
+
+    def disassemble(self, file_path: str) -> list[APNGFrame]:
         """
         Disassembles an APNG file.
-        
+
         :param str file_path: The file path to the PNG image to be disassembled.
-        
+
         :return: A vector containing the frames of the disassembled PNG.
         :rtype: list[apngasm_python._apngasm_python.APNGFrame]
         """
-        ...
-    
-    def frame_count(self) -> int:
-        """
-        Returns the number of frames.
-        
-        :return: number of frames.
-        :rtype: int
-        """
-        ...
-    
-    def get_frames(self) -> list[_apngasm_python.APNGFrame]:
-        """
-        Returns the frame vector.
-        
-        :return: frame vector.
-        :rtype: list[apngasm_python._apngasm_python.APNGFrame]
-        """
-        ...
-    
-    def get_loops(self) -> int:
-        """
-        Returns the loop count.
-        
-        :return: loop count.
-        :rtype: int
-        """
-        ...
-    
-    def is_skip_first(self) -> bool:
+
+    def save_pngs(self, output_dir: str) -> bool:
         """
-        Returns the flag of skip first frame.
-        
-        :return: flag of skip first frame.
+        Saves individual PNG files of the frames in the frame vector.
+
+        :param str output_dir: The directory where the PNG fils will be saved.
+
+        :return: true if all files were saved successfully.
         :rtype: bool
         """
-        ...
-    
-    def load_animation_spec(self, file_path: str) -> list[_apngasm_python.APNGFrame]:
+
+    def load_animation_spec(self, file_path: str) -> list[APNGFrame]:
         """
         Loads an animation spec from JSON or XML.
         Loaded frames are added to the end of the frame vector.
         For more details on animation specs see:
         https://github.com/Genshin/PhantomStandards
-        
+
         :param str file_path: The path of JSON or XML file.
-        
+
         :return: A vector containing the frames
         :rtype: list[apngasm_python._apngasm_python.APNGFrame]
         """
-        ...
-    
-    def reset(self) -> int:
-        """
-        Destroy all frames in memory/dispose of the frame vector.
-        Leaves the apngasm object in a clean state.
-        Returns number of frames disposed of.
-        
-        :return: number of frames disposed of.
-        :rtype: int
-        """
-        ...
-    
+
     def save_json(self, output_path: str, image_dir: str) -> bool:
         """
         Saves a JSON animation spec file.
-        
+
         :param str output_path: Path to save the file to.
         :param str image_dir: Directory where frame files are to be saved if not the same path as the animation spec.
-        
+
         :return: true if save was successful.
         :rtype: bool
         """
-        ...
-    
-    def save_pngs(self, output_dir: str) -> bool:
-        """
-        Saves individual PNG files of the frames in the frame vector.
-        
-        :param str output_dir: The directory where the PNG fils will be saved.
-        
-        :return: true if all files were saved successfully.
-        :rtype: bool
-        """
-        ...
-    
+
     def save_xml(self, output_path: str, image_dir: str) -> bool:
         """
         Saves an XML animation spec file.
-        
+
         :param str file_path: Path to save the file to.
         :param str image_dir: Directory where frame files are to be saved if not the same path as the animation spec.
-        
+
         :return: true if save was successful.
         :rtype: bool
         """
-        ...
-    
-    def set_apngasm_listener(self, listener: Optional[_apngasm_python.IAPNGAsmListener] = None) -> None:
+
+    def set_apngasm_listener(self, listener: Optional[IAPNGAsmListener] = None) -> None:
         """
         Sets a listener.
-        
+
         :param Optional[apngasm_python._apngasm_python.IAPNGAsmListener] listener: A pointer to the listener object. If the argument is NULL a default APNGAsmListener will be created and assigned.
         """
-        ...
-    
+
     def set_loops(self, loops: int = 0) -> None:
         """
         Set loop count of animation.
-        
+
         :param int loops: Loop count of animation. If the argument is 0 a loop count is infinity.
         """
-        ...
-    
+
     def set_skip_first(self, skip_first: bool) -> None:
         """
         Set flag of skip first frame.
-        
+
         :param int skip_first: Flag of skip first frame.
         """
-        ...
-    
+
+    def get_frames(self) -> list[APNGFrame]:
+        """
+        Returns the frame vector.
+
+        :return: frame vector.
+        :rtype: list[apngasm_python._apngasm_python.APNGFrame]
+        """
+
+    def get_loops(self) -> int:
+        """
+        Returns the loop count.
+
+        :return: loop count.
+        :rtype: int
+        """
+
+    def is_skip_first(self) -> bool:
+        """
+        Returns the flag of skip first frame.
+
+        :return: flag of skip first frame.
+        :rtype: bool
+        """
+
+    def frame_count(self) -> int:
+        """
+        Returns the number of frames.
+
+        :return: number of frames.
+        :rtype: int
+        """
+
+    def reset(self) -> int:
+        """
+        Destroy all frames in memory/dispose of the frame vector.
+        Leaves the apngasm object in a clean state.
+        Returns number of frames disposed of.
+
+        :return: number of frames disposed of.
+        :rtype: int
+        """
+
     def version(self) -> str:
         """
         Returns the version of APNGAsm.
-        
+
         :return: the version of APNGAsm.
         :rtype: str
         """
-        ...
-    
+
 class APNGFrame:
-    """
-    Class representing a frame in APNG.
-    """
+    """Class representing a frame in APNG."""
 
-    def __init__(self, pixels: _apngasm_python.rgba, width: int, height: int, delay_num: int = 100, delay_den: int = 1000) -> None:
-        """
-        Creates an APNGFrame from a bitmapped array of RBGA pixel data.
-        Not possible to use in Python. To create APNGFrame from pixel data in memory,
-        Use create_frame_from_rgb() or create_frame_from_rgba(). Or manually,
-        First create an empty APNGFrame with frame = APNGFrame(),
-        then set frame.width, frame.height, frame.color_type, frame.pixels,
-        frame.palette, frame.delay_num, frame.delay_den manually.
-        
-        :param apngasm_python._apngasm_python.rgba pixels: The RGBA pixel data.
-        :param int width: The width of the pixel data.
-        :param int height: The height of the pixel data.
-        :param int delay_num: The delay numerator for this frame (defaults to DEFAULT_FRAME_NUMERATOR).
-        :param int delay_den: The delay denominator for this frame (defaults to DEFAULT_FRAME_DENMINATOR).
-        """
-        ...
-    
     @overload
     def __init__(self) -> None:
-        """
-        Creates an empty APNGFrame.
-        """
-        ...
-    
+        """Creates an empty APNGFrame."""
+
     @overload
     def __init__(self, file_path: str, delay_num: int = 100, delay_den: int = 1000) -> None:
         """
         Creates an APNGFrame from a PNG file.
-        
+
         :param str file_path: The relative or absolute path to an image file.
         :param int delay_num: The delay numerator for this frame (defaults to DEFAULT_FRAME_NUMERATOR).
         :param int delay_den: The delay denominator for this frame (defaults to DEFAULT_FRAME_DENMINATOR).
         """
-        ...
-    
+
     @overload
-    def __init__(self, pixels: _apngasm_python.rgb, width: int, height: int, trns_color: _apngasm_python.rgb, delay_num: int = 100, delay_den: int = 1000) -> None:
+    def __init__(self, pixels: rgb, width: int, height: int, trns_color: rgb, delay_num: int = 100, delay_den: int = 1000) -> None:
         """
         Creates an APNGFrame from a bitmapped array of RBG pixel data.
         Not possible to use in Python. To create APNGFrame from pixel data in memory,
         Use create_frame_from_rgb() or create_frame_from_rgba(). Or manually,
         First create an empty APNGFrame with frame = APNGFrame(),
         then set frame.width, frame.height, frame.color_type, frame.pixels,
         frame.palette, frame.delay_num, frame.delay_den manually.
-        
+
         :param apngasm_python._apngasm_python.rgb pixels: The RGB pixel data.
         :param int width: The width of the pixel data.
         :param int height: The height of the pixel data.
         :param apngasm_python._apngasm_python.rgb trns_color: The color [r, g, b] to be treated as transparent.
         :param int delay_num: The delay numerator for this frame (defaults to DEFAULT_FRAME_NUMERATOR).
         :param int delay_den: The delay denominator for this frame (defaults to DEFAULT_FRAME_DENMINATOR).
         """
-        ...
-    
-    @property
-    def color_type(self) -> int:
+
+    @overload
+    def __init__(self, pixels: rgba, width: int, height: int, delay_num: int = 100, delay_den: int = 1000) -> None:
         """
-        The color_type of the frame.
-        
-        0: Grayscale (Pillow mode='L')
-        2: RGB (Pillow mode='RGB')
-        3: Palette (Pillow mode='P')
-        4: Grayscale + Alpha (Pillow mode='LA')
-        6: RGBA (Pillow mode='RGBA')
+        Creates an APNGFrame from a bitmapped array of RBGA pixel data.
+        Not possible to use in Python. To create APNGFrame from pixel data in memory,
+        Use create_frame_from_rgb() or create_frame_from_rgba(). Or manually,
+        First create an empty APNGFrame with frame = APNGFrame(),
+        then set frame.width, frame.height, frame.color_type, frame.pixels,
+        frame.palette, frame.delay_num, frame.delay_den manually.
+
+        :param apngasm_python._apngasm_python.rgba pixels: The RGBA pixel data.
+        :param int width: The width of the pixel data.
+        :param int height: The height of the pixel data.
+        :param int delay_num: The delay numerator for this frame (defaults to DEFAULT_FRAME_NUMERATOR).
+        :param int delay_den: The delay denominator for this frame (defaults to DEFAULT_FRAME_DENMINATOR).
         """
-        ...
-    @color_type.setter
-    def color_type(self, arg: int, /) -> None:
+
+    def save(self, out_path: str) -> bool:
         """
-        The color_type of the frame.
-        
-        0: Grayscale (Pillow mode='L')
-        2: RGB (Pillow mode='RGB')
-        3: Palette (Pillow mode='P')
-        4: Grayscale + Alpha (Pillow mode='LA')
-        6: RGBA (Pillow mode='RGBA')
+        Saves this frame as a single PNG file.
+
+        :param str out_path: The relative or absolute path to save the image file to.
+
+        :return: true if save was successful.
+        :rtype: bool
         """
-        ...
-    
+
     @property
-    def delay_den(self) -> int:
+    def pixels(self) -> Annotated[ArrayLike, dict(dtype='uint8', shape=(None, None, None))]:
         """
-        The denominator of the duration of frame. Duration of time is delay_num / delay_den seconds.
-        """
-        ...
-    @delay_den.setter
-    def delay_den(self, arg: int, /) -> None:
-        """
-        The denominator of the duration of frame. Duration of time is delay_num / delay_den seconds.
+        The raw pixel data of frame, expressed as a 3D numpy array in Python.
+        Note that setting this value will also set the variable 'rows' internally.
+        This should be set AFTER you set the width, height and color_type.
         """
-        ...
-    
+
+    @pixels.setter
+    def pixels(self, arg: Annotated[ArrayLike, dict(dtype='uint8', shape=(None, None, None))], /) -> None: ...
+
     @property
-    def delay_num(self) -> int:
-        """
-        The nominator of the duration of frame. Duration of time is delay_num / delay_den seconds.
-        """
-        ...
-    @delay_num.setter
-    def delay_num(self, arg: int, /) -> None:
-        """
-        The nominator of the duration of frame. Duration of time is delay_num / delay_den seconds.
-        """
-        ...
-    
+    def width(self) -> int:
+        """The width of frame."""
+
+    @width.setter
+    def width(self, arg: int, /) -> None: ...
+
     @property
     def height(self) -> int:
-        """
-        The height of frame.
-        """
-        ...
+        """The height of frame."""
+
     @height.setter
-    def height(self, arg: int, /) -> None:
+    def height(self, arg: int, /) -> None: ...
+
+    @property
+    def color_type(self) -> int:
         """
-        The height of frame.
+        The color_type of the frame.
+
+        0: Grayscale (Pillow mode='L')
+        2: RGB (Pillow mode='RGB')
+        3: Palette (Pillow mode='P')
+        4: Grayscale + Alpha (Pillow mode='LA')
+        6: RGBA (Pillow mode='RGBA')
         """
-        ...
-    
+
+    @color_type.setter
+    def color_type(self, arg: int, /) -> None: ...
+
     @property
-    def palette(self) -> numpy.typing.NDArray:
+    def palette(self) -> Annotated[ArrayLike, dict(dtype='uint8', shape=(256, 3))]:
         """
         The palette data of frame. Only applies to 'P' mode Image (i.e. Not RGB, RGBA).
         Expressed as 2D numpy array in format of [[r0, g0, b0], [r1, g1, b1], ..., [r255, g255, b255]] in Python.
         """
-        ...
+
     @palette.setter
-    def palette(self, arg: numpy.typing.NDArray, /) -> None:
-        """
-        The palette data of frame. Only applies to 'P' mode Image (i.e. Not RGB, RGBA).
-        Expressed as 2D numpy array in format of [[r0, g0, b0], [r1, g1, b1], ..., [r255, g255, b255]] in Python.
-        """
-        ...
-    
-    @property
-    def palette_size(self) -> int:
-        """
-        The palette data size of frame.
-        """
-        ...
-    @palette_size.setter
-    def palette_size(self, arg: int, /) -> None:
-        """
-        The palette data size of frame.
-        """
-        ...
-    
-    @property
-    def pixels(self) -> numpy.typing.NDArray:
-        """
-        The raw pixel data of frame, expressed as a 3D numpy array in Python.
-        Note that setting this value will also set the variable 'rows' internally.
-        This should be set AFTER you set the width, height and color_type.
-        """
-        ...
-    @pixels.setter
-    def pixels(self, arg: numpy.typing.NDArray, /) -> None:
-        """
-        The raw pixel data of frame, expressed as a 3D numpy array in Python.
-        Note that setting this value will also set the variable 'rows' internally.
-        This should be set AFTER you set the width, height and color_type.
-        """
-        ...
-    
-    def save(self, out_path: str) -> bool:
-        """
-        Saves this frame as a single PNG file.
-        
-        :param str out_path: The relative or absolute path to save the image file to.
-        
-        :return: true if save was successful.
-        :rtype: bool
-        """
-        ...
-    
+    def palette(self, arg: Annotated[ArrayLike, dict(dtype='uint8', shape=(256, 3))], /) -> None: ...
+
     @property
-    def transparency(self) -> numpy.typing.NDArray:
+    def transparency(self) -> Annotated[ArrayLike, dict(dtype='uint8', shape=(None))]:
         """
         The transparency color of frame that is treated as transparent, expressed as 1D numpy array.
         For more info, refer to 'tRNS Transparency' in http://www.libpng.org/pub/png/spec/1.2/PNG-Chunks.html
         """
-        ...
+
     @transparency.setter
-    def transparency(self, arg: numpy.typing.NDArray, /) -> None:
-        """
-        The transparency color of frame that is treated as transparent, expressed as 1D numpy array.
-        For more info, refer to 'tRNS Transparency' in http://www.libpng.org/pub/png/spec/1.2/PNG-Chunks.html
-        """
-        ...
-    
+    def transparency(self, arg: Annotated[ArrayLike, dict(dtype='uint8', shape=(None))], /) -> None: ...
+
+    @property
+    def palette_size(self) -> int:
+        """The palette data size of frame."""
+
+    @palette_size.setter
+    def palette_size(self, arg: int, /) -> None: ...
+
     @property
     def transparency_size(self) -> int:
-        """
-        The transparency data size of frame.
-        """
-        ...
+        """The transparency data size of frame."""
+
     @transparency_size.setter
-    def transparency_size(self, arg: int, /) -> None:
-        """
-        The transparency data size of frame.
-        """
-        ...
-    
+    def transparency_size(self, arg: int, /) -> None: ...
+
     @property
-    def width(self) -> int:
+    def delay_num(self) -> int:
         """
-        The width of frame.
+        The nominator of the duration of frame. Duration of time is delay_num / delay_den seconds.
         """
-        ...
-    @width.setter
-    def width(self, arg: int, /) -> None:
+
+    @delay_num.setter
+    def delay_num(self, arg: int, /) -> None: ...
+
+    @property
+    def delay_den(self) -> int:
         """
-        The width of frame.
+        The denominator of the duration of frame. Duration of time is delay_num / delay_den seconds.
         """
-        ...
-    
+
+    @delay_den.setter
+    def delay_den(self, arg: int, /) -> None: ...
+
 class IAPNGAsmListener:
-    """
-    Class for APNGAsmListener. Meant to be used internally.
-    """
+    """Class for APNGAsmListener. Meant to be used internally."""
 
-    def __init__(*args, **kwargs):
-        """
-        Initialize self.  See help(type(self)) for accurate signature.
-        """
-        ...
-    
-def create_frame_from_rgb(pixels: numpy.typing.NDArray, width: int, height: int, delay_num: int = 100, delay_den: int = 1000) -> _apngasm_python.APNGFrame:
+def create_frame_from_rgb(pixels: Annotated[ArrayLike, dict(dtype='uint8', shape=(None, None, 3))], width: int, height: int, delay_num: int = 100, delay_den: int = 1000) -> APNGFrame:
     """
     Creates an APNGFrame from a bitmapped array of RBG pixel data.
-    
+
     :param numpy.typing.NDArray pixels: The RGB pixel data, expressed as 3D numpy array.
     :param int width: The width of the pixel data.
     :param int height: The height of the pixel data.
     :param int delay_num: The delay numerator for this frame (defaults to DEFAULT_FRAME_NUMERATOR).
     :param int delay_den: The delay denominator for this frame (defaults to DEFAULT_FRAME_DENMINATOR).
-    
+
     :return: A APNGFrame object.
     :rtype: apngasm_python._apngasm_python.APNGFrame
     """
-    ...
 
-def create_frame_from_rgb_trns(pixels: numpy.typing.NDArray, width: int, height: int, trns_color: numpy.typing.NDArray, delay_num: int = 100, delay_den: int = 1000) -> _apngasm_python.APNGFrame:
+def create_frame_from_rgb_trns(pixels: Annotated[ArrayLike, dict(dtype='uint8', shape=(None, None, 3))], width: int, height: int, trns_color: Annotated[ArrayLike, dict(dtype='uint8', shape=(3))], delay_num: int = 100, delay_den: int = 1000) -> APNGFrame:
     """
     Creates an APNGFrame from a bitmapped array of RBG pixel data, with one color treated as transparent.
-    
+
     :param numpy.typing.NDArray pixels: The RGB pixel data, expressed as 3D numpy array.
     :param int width: The width of the pixel data.
     :param int height: The height of the pixel data.
     :param numpy.typing.NDArray trns_color: The color [r, g, b] to be treated as transparent, expressed as 1D numpy array.
     :param int delay_num: The delay numerator for this frame (defaults to DEFAULT_FRAME_NUMERATOR).
     :param int delay_den: The delay denominator for this frame (defaults to DEFAULT_FRAME_DENMINATOR).
-    
+
     :return: A APNGFrame object.
     :rtype: apngasm_python._apngasm_python.APNGFrame
     """
-    ...
 
-def create_frame_from_rgba(pixels: numpy.typing.NDArray, width: int, height: int, delay_num: int = 100, delay_den: int = 1000) -> _apngasm_python.APNGFrame:
+def create_frame_from_rgba(pixels: Annotated[ArrayLike, dict(dtype='uint8', shape=(None, None, 4))], width: int, height: int, delay_num: int = 100, delay_den: int = 1000) -> APNGFrame:
     """
     Creates an APNGFrame from a bitmapped array of RBGA pixel data.
-    
+
     :param numpy.typing.NDArray pixels: The RGBA pixel data, expressed as 3D numpy array.
     :param int width: The width of the pixel data.
     :param int height: The height of the pixel data.
     :param int delay_num: The delay numerator for this frame (defaults to DEFAULT_FRAME_NUMERATOR)
     :param int delay_den: The delay denominator for this frame (defaults to DEFAULT_FRAME_DENMINATOR)
-    
+
     :return: A APNGFrame object.
     :rtype: apngasm_python._apngasm_python.APNGFrame
     """
-    ...
 
 class rgb:
-    """
-    Class for RGB object. Meant to be used internally.
-    """
+    """Class for RGB object. Meant to be used internally."""
 
-    def __init__(self, arg0: int, arg1: int, arg2: int, /) -> None:
-        """
-        Create a RGB object. Meant to be used internally.
-        """
-        ...
-    
     @overload
     def __init__(self) -> None:
-        """
-        Create an empty RGB object. Meant to be used internally.
-        """
-        ...
-    
+        """Create an empty RGB object. Meant to be used internally."""
+
+    @overload
+    def __init__(self, arg0: int, arg1: int, arg2: int, /) -> None:
+        """Create a RGB object. Meant to be used internally."""
+
     @property
-    def b(self) -> int:
-        ...
-    @b.setter
-    def b(self, arg: int, /) -> None:
-        ...
-    
+    def r(self) -> int: ...
+
+    @r.setter
+    def r(self, arg: int, /) -> None: ...
+
     @property
-    def g(self) -> int:
-        ...
+    def g(self) -> int: ...
+
     @g.setter
-    def g(self, arg: int, /) -> None:
-        ...
-    
+    def g(self, arg: int, /) -> None: ...
+
     @property
-    def r(self) -> int:
-        ...
-    @r.setter
-    def r(self, arg: int, /) -> None:
-        ...
-    
+    def b(self) -> int: ...
+
+    @b.setter
+    def b(self, arg: int, /) -> None: ...
+
 class rgba:
-    """
-    Class for RGBA object. Meant to be used internally.
-    """
+    """Class for RGBA object. Meant to be used internally."""
 
-    def __init__(self, arg0: int, arg1: int, arg2: int, arg3: int, /) -> None:
-        """
-        Create a RGBA object. Meant to be used internally.
-        """
-        ...
-    
     @overload
     def __init__(self) -> None:
-        """
-        Create an empty RGBA object. Meant to be used internally.
-        """
-        ...
-    
-    @property
-    def a(self) -> int:
-        ...
-    @a.setter
-    def a(self, arg: int, /) -> None:
-        ...
-    
+        """Create an empty RGBA object. Meant to be used internally."""
+
+    @overload
+    def __init__(self, arg0: int, arg1: int, arg2: int, arg3: int, /) -> None:
+        """Create a RGBA object. Meant to be used internally."""
+
     @property
-    def b(self) -> int:
-        ...
-    @b.setter
-    def b(self, arg: int, /) -> None:
-        ...
-    
+    def r(self) -> int: ...
+
+    @r.setter
+    def r(self, arg: int, /) -> None: ...
+
     @property
-    def g(self) -> int:
-        ...
+    def g(self) -> int: ...
+
     @g.setter
-    def g(self, arg: int, /) -> None:
-        ...
-    
+    def g(self, arg: int, /) -> None: ...
+
     @property
-    def r(self) -> int:
-        ...
-    @r.setter
-    def r(self, arg: int, /) -> None:
-        ...
-    
+    def b(self) -> int: ...
+
+    @b.setter
+    def b(self, arg: int, /) -> None: ...
+
+    @property
+    def a(self) -> int: ...
+
+    @a.setter
+    def a(self, arg: int, /) -> None: ...
```

### Comparing `apngasm_python-1.2.3/src-python/apngasm_python/apngasm.py` & `apngasm_python-1.3.0/src-python/apngasm_python/apngasm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,20 @@
 #!/usr/bin/env python3
 from __future__ import annotations
-from ._apngasm_python import (
-    APNGAsm,
-    APNGFrame,
-    IAPNGAsmListener,
-    create_frame_from_rgb,
-    create_frame_from_rgb_trns,
-    create_frame_from_rgba,
-)
-from ._apngasm_python import __version__ # type: ignore
-
-try:
-    import numpy
-    import numpy.typing
-
-    NUMPY_LOADED = True
-except ModuleNotFoundError:
-    NUMPY_LOADED = False
 
-try:
-    from PIL import Image
+from typing import TYPE_CHECKING, Any, Optional
 
-    PILLOW_LOADED = True
-except ModuleNotFoundError:
-    PILLOW_LOADED = False
+if TYPE_CHECKING:
+    from numpy.typing import NDArray
+    from PIL import Image
 
-from typing import Optional
+from ._apngasm_python import APNGFrame  # type: ignore
+from ._apngasm_python import (APNGAsm, IAPNGAsmListener, create_frame_from_rgb,
+                              create_frame_from_rgb_trns,
+                              create_frame_from_rgba)
 
 
 class APNGAsmBinder:
     """
     Python class for binding apngasm library
     """
 
@@ -38,80 +23,85 @@
 
     def __init__(self):
         self.apngasm = APNGAsm()
 
     def __enter__(self):
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
+    def __exit__(self, exc_type, exc_val, exc_tb):  # type: ignore
         self.apngasm.reset()
 
-    if PILLOW_LOADED:
+    def frame_pixels_as_pillow(
+        self, frame: int, new_value: Optional[Image.Image] = None
+    ) -> Optional[Image.Image]:
+        """
+        Get/Set the raw pixel data of frame, expressed as a Pillow object.
+        This should be set AFTER you set the width, height and color_type.
 
-        def frame_pixels_as_pillow(
-            self, frame: int, new_value: Optional[Image.Image] = None
-        ) -> Optional[Image.Image]:
-            """
-            Get/Set the raw pixel data of frame, expressed as a Pillow object.
-            This should be set AFTER you set the width, height and color_type.
-
-            :param int frame: Target frame number.
-            :param Optional[PIL.Image.Image] new_value: If set, then the raw pixel data of frame
-                is set with this value.
-
-            :return: Pillow image object of the frame (get) or None (set)
-            :rtype: Optional[PIL.Image.Image]
-            """
-            if new_value:
-                self.apngasm.get_frames()[frame].pixels = numpy.array(new_value)
-            else:
-                mode = self.color_type_dict[self.apngasm.get_frames()[frame].color_type]
-                return Image.frombytes(
-                    mode,
-                    (
-                        self.apngasm.get_frames()[frame].width,
-                        self.apngasm.get_frames()[frame].height,
-                    ),
-                    self.apngasm.get_frames()[frame].pixels,
-                )
+        :param int frame: Target frame number.
+        :param Optional[PIL.Image.Image] new_value: If set, then the raw pixel data of
+            frame is set with this value.
 
-    if NUMPY_LOADED:
+        :return: Pillow image object of the frame (get) or None (set)
+        :rtype: Optional[PIL.Image.Image]
+        """
+        from numpy import array
+        from PIL import Image
 
-        def frame_pixels_as_numpy(
-            self, frame: int, new_value: Optional[numpy.typing.NDArray] = None
-        ) -> Optional[numpy.typing.NDArray]:
-            """
-            Get/Set the raw pixel data of frame, expressed as a 3D numpy array.
-            This should be set AFTER you set the width, height and color_type.
-
-            :param int frame: Target frame number.
-            :param Optional[numpy.typing.NDArray] new_value: If set, then the raw pixel data of frame
-                is set with this value.
-
-            :return: 3D numpy array representation of raw pixel data of frame (get) or None (set)
-            :rtype: Optional[numpy.typing.NDArray]
-            """
-            if new_value:
-                self.apngasm.get_frames()[frame].pixels = new_value
-            else:
-                return self.apngasm.get_frames()[frame].pixels
+        if new_value:
+            self.apngasm.get_frames()[frame].pixels = array(new_value)
+            return None
+        else:
+            mode = self.color_type_dict[self.apngasm.get_frames()[frame].color_type]
+            return Image.frombytes(  # type: ignore
+                mode,
+                (
+                    self.apngasm.get_frames()[frame].width,
+                    self.apngasm.get_frames()[frame].height,
+                ),
+                self.apngasm.get_frames()[frame].pixels,
+            )
+
+    def frame_pixels_as_numpy(
+        self, frame: int, new_value: Optional[NDArray[Any]] = None
+    ) -> Optional[NDArray[Any]]:
+        """
+        Get/Set the raw pixel data of frame, expressed as a 3D numpy array.
+        This should be set AFTER you set the width, height and color_type.
+
+        :param int frame: Target frame number.
+        :param Optional[numpy.typing.NDArray[Any]] new_value: If set, then the
+            raw pixel  data of frame is set with this value.
+
+        :return: 3D numpy array representation of
+            raw pixel data of frame (get) or None (set)
+        :rtype: Optional[numpy.typing.NDArray[Any]]
+        """
+        from numpy import array
+
+        if new_value:
+            self.apngasm.get_frames()[frame].pixels = new_value
+            return None
+        else:
+            return array(self.apngasm.get_frames()[frame].pixels)
 
     def frame_width(self, frame: int, new_value: Optional[int] = None) -> Optional[int]:
         """
         Get/Set the width of frame.
 
         :param int frame: Target frame number.
         :param Optional[int] new_value: If set, then the width of frame
             is set with this value.
 
         :return: width (get) or None (set)
         :rtype: Optional[int]
         """
         if new_value:
             self.apngasm.get_frames()[frame].width = new_value
+            return None
         else:
             return self.apngasm.get_frames()[frame].width
 
     def frame_height(
         self, frame: int, new_value: Optional[int] = None
     ) -> Optional[int]:
         """
@@ -122,14 +112,15 @@
             is set with this value.
 
         :return: height (get) or None (set)
         :rtype: Optional[int]
         """
         if new_value:
             self.apngasm.get_frames()[frame].height = new_value
+            return None
         else:
             return self.apngasm.get_frames()[frame].height
 
     def frame_color_type(
         self, frame: int, new_value: Optional[int] = None
     ) -> Optional[int]:
         """
@@ -146,57 +137,67 @@
             is set with this value.
 
         :return: color_type of frame (get) or None (set)
         :rtype: Optional[int]
         """
         if new_value:
             self.apngasm.get_frames()[frame].color_type = new_value
+            return None
         else:
             return self.apngasm.get_frames()[frame].color_type
 
-    if NUMPY_LOADED:
+    def frame_palette(
+        self, frame: int, new_value: Optional[NDArray[Any]] = None
+    ) -> Optional[NDArray[Any]]:
+        """
+        Get/Set the palette data of frame.
+        Only applies to 'P' mode Image (i.e. Not RGB, RGBA).
+        Expressed as 2D numpy array
+        in format of [[r0, g0, b0], [r1, g1, b1], ..., [r255, g255, b255]]
 
-        def frame_palette(
-            self, frame: int, new_value: Optional[numpy.typing.NDArray] = None
-        ) -> Optional[numpy.typing.NDArray]:
-            """
-            Get/Set the palette data of frame. Only applies to 'P' mode Image (i.e. Not RGB, RGBA)
-            Expressed as 2D numpy array in format of [[r0, g0, b0], [r1, g1, b1], ..., [r255, g255, b255]]
-
-            :param int frame: Target frame number.
-            :param Optional[numpy.typing.NDArray] new_value: If set, then the palette data of frame
-                is set with this value.
-
-            :return: 2D numpy array representation of palette data of frame (get) or None (set)
-            :rtype: Optional[numpy.typing.NDArray]
-            """
-            if new_value:
-                self.apngasm.get_frames()[frame].palette = new_value
-            else:
-                return self.apngasm.get_frames()[frame].palette
+        :param int frame: Target frame number.
+        :param Optional[numpy.typing.NDArray[Any]] new_value: If set, then
+            the palette data of frame is set with this value.
 
-        def frame_transparency(
-            self, frame: int, new_value: Optional[numpy.typing.NDArray] = None
-        ) -> Optional[numpy.typing.NDArray]:
-            """
-            Get/Set the color [r, g, b] to be treated as transparent in the frame, expressed as 1D numpy array.
-            For more info, refer to 'tRNS Transparency' in
-            http://www.libpng.org/pub/png/spec/1.2/PNG-Chunks.html
-
-            :param int frame: Target frame number.
-            :param Optional[numpy.typing.NDArray] new_value: If set, then the transparency of frame
-                is set with this value.
-
-            :return: The color [r, g, b] to be treated as transparent in the frame (get) or None (set)
-            :rtype: Optional[numpy.typing.NDArray]
-            """
-            if new_value:
-                self.apngasm.get_frames()[frame].transparency = new_value
-            else:
-                return self.apngasm.get_frames()[frame].transparency
+        :return: 2D numpy array representation of
+            palette data of frame (get) or None (set)
+        :rtype: Optional[numpy.typing.NDArray[Any]]
+        """
+        from numpy import array
+
+        if new_value:
+            self.apngasm.get_frames()[frame].palette = new_value
+            return None
+        else:
+            return array(self.apngasm.get_frames()[frame].palette)
+
+    def frame_transparency(
+        self, frame: int, new_value: Optional[NDArray[Any]] = None
+    ) -> Optional[NDArray[Any]]:
+        """
+        Get/Set the color [r, g, b] to be treated as transparent in the frame,
+        expressed as 1D numpy array.
+        For more info, refer to 'tRNS Transparency' in
+        http://www.libpng.org/pub/png/spec/1.2/PNG-Chunks.html
+
+        :param int frame: Target frame number.
+        :param Optional[numpy.typing.NDArray[Any]] new_value: If set, then the
+            transparency of frame is set with this value.
+
+        :return: The color [r, g, b] to be treated as transparent
+            in the frame (get) or None (set)
+        :rtype: Optional[numpy.typing.NDArray[Any]]
+        """
+        from numpy import array
+
+        if new_value:
+            self.apngasm.get_frames()[frame].transparency = new_value
+            return None
+        else:
+            return array(self.apngasm.get_frames()[frame].transparency)
 
     def frame_palette_size(
         self, frame: int, new_value: Optional[int] = None
     ) -> Optional[int]:
         """
         Get/Set the palette data size of frame.
 
@@ -205,14 +206,15 @@
             is set with this value.
 
         :return: Palette data size of frame (get) or None (set)
         :rtype: Optional[int]
         """
         if new_value:
             self.apngasm.get_frames()[frame].palette_size = new_value
+            return None
         else:
             return self.apngasm.get_frames()[frame].palette_size
 
     def frame_transparency_size(
         self, frame: int, new_value: Optional[int] = None
     ) -> Optional[int]:
         """
@@ -223,52 +225,55 @@
             is set with this value.
 
         :return: Transparency data size of frame (get) or None (set)
         :rtype: Optional[int]
         """
         if new_value:
             self.apngasm.get_frames()[frame].transparency_size = new_value
+            return None
         else:
             return self.apngasm.get_frames()[frame].transparency_size
 
     def frame_delay_num(
         self, frame: int, new_value: Optional[int] = None
     ) -> Optional[int]:
         """
         Get/Set the nominator of the duration of frame.
         Duration of time is delay_num / delay_den seconds.
 
         :param int frame: Target frame number.
-        :param Optional[int] new_value: If set, then the nominator of the duration of frame
-            is set with this value.
+        :param Optional[int] new_value: If set, then the nominator of the
+            duration of frame is set with this value.
 
         :return: Nominator of the duration of frame.
         :rtype: Optional[int]
         """
         if new_value:
             self.apngasm.get_frames()[frame].delay_num = new_value
+            return None
         else:
             return self.apngasm.get_frames()[frame].delay_num
 
     def frame_delay_den(
         self, frame: int, new_value: Optional[int] = None
     ) -> Optional[int]:
         """
         Get/Set the denominator of the duration of frame.
         Duration of time is delay_num / delay_den seconds.
 
         :param int frame: Target frame number.
-        :param Optional[int] new_value: If set, then the denominator of the duration of frame
-            is set with this value.
+        :param Optional[int] new_value: If set, then the denominator of the
+            duration of frame is set with this value.
 
         :return: Denominator of the duration of frame.
         :rtype: Optional[int]
         """
         if new_value:
             self.apngasm.get_frames()[frame].delay_den = new_value
+            return None
         else:
             return self.apngasm.get_frames()[frame].delay_den
 
     def add_frame_from_file(
         self, file_path: str, delay_num: int = 100, delay_den: int = 1000
     ) -> int:
         """
@@ -281,160 +286,174 @@
         :return: The new number of frames.
         :rtype: int
         """
         return self.apngasm.add_frame_from_file(
             file_path=file_path, delay_num=delay_num, delay_den=delay_den
         )
 
-    if PILLOW_LOADED:
+    def add_frame_from_pillow(
+        self, pillow_image: Image.Image, delay_num: int = 100, delay_den: int = 1000
+    ) -> int:
+        """
+        Add a frame from Pillow image.
+        The frame duration is equal to delay_num / delay_den seconds.
+        Default frame duration is 100/1000 second, or 0.1 second.
 
-        def add_frame_from_pillow(
-            self, pillow_image: Image.Image, delay_num: int = 100, delay_den: int = 1000
-        ) -> int:
-            """
-            Add a frame from Pillow image.
-            The frame duration is equal to delay_num / delay_den seconds.
-            Default frame duration is 100/1000 second, or 0.1 second.
-
-            :param PIL.Image.Image pillow_image: Pillow image object.
-            :param int delay_num: The delay numerator for this frame (defaults to 100).
-            :param int delay_den: The delay denominator for this frame (defaults to 1000).
-
-            :return: The new number of frames.
-            :rtype: int
-            """
-            if pillow_image.mode not in ("RGB", "RGBA"):
-                pillow_image = pillow_image.convert("RGBA")
-            return self.add_frame_from_numpy(
-                numpy_data=numpy.array(pillow_image),
-                width=pillow_image.width,
-                height=pillow_image.height,
-                mode=pillow_image.mode,
-                delay_num=delay_num,
-                delay_den=delay_den,
-            )
+        :param PIL.Image.Image pillow_image: Pillow image object.
+        :param int delay_num: The delay numerator for this frame (defaults to 100).
+        :param int delay_den: The delay denominator for this frame (defaults to 1000).
+
+        :return: The new number of frames.
+        :rtype: int
+        """
+        from numpy import array
+
+        if pillow_image.mode not in ("RGB", "RGBA"):
+            pillow_image = pillow_image.convert("RGBA")
+        return self.add_frame_from_numpy(
+            numpy_data=array(pillow_image),
+            width=pillow_image.width,
+            height=pillow_image.height,
+            mode=pillow_image.mode,
+            delay_num=delay_num,
+            delay_den=delay_den,
+        )
 
-    if NUMPY_LOADED:
+    def add_frame_from_numpy(
+        self,
+        numpy_data: NDArray[Any],
+        width: Optional[int] = None,
+        height: Optional[int] = None,
+        trns_color: Optional[NDArray[Any]] = None,
+        mode: Optional[str] = None,
+        delay_num: int = 100,
+        delay_den: int = 1000,
+    ) -> int:
+        """
+        Add frame from numpy array.
+        The frame duration is equal to delay_num / delay_den seconds.
+        Default frame duration is 100/1000 second, or 0.1 second.
+
+        :param numpy.typing.NDArray[Any] numpy_data: The pixel data, expressed as
+            3D numpy array.
+        :param Optional[int] width: The width of the pixel data.
+            If not given, the 2nd dimension size of numpy_data is used.
+        :param Optional[int] height: The height of the pixel data.
+            If not given, the 1st dimension size of numpy_data is used.
+        :param Optional[str] mode: The color mode of data. Possible values are
+            RGB or RGBA. If not given, it is determined using the 3rd dimension size
+            of numpy_data.
+        :param Optional[numpy.typing.NDArray[Any]] trns_color: The color [r, g, b] to
+            be treated as transparent, expressed as 1D numpy array.
+            Only use if RGB mode.
+        :param int delay_num: The delay numerator for this frame (defaults to 100).
+        :param int delay_den: The delay denominator for this frame (defaults to 1000).
+
+        :return: The new number of frames.
+        :rtype: int
+        """
+        from numpy import ndarray, shape
 
-        def add_frame_from_numpy(
-            self,
-            numpy_data: numpy.typing.NDArray,
-            width: Optional[int] = None,
-            height: Optional[int] = None,
-            trns_color: Optional[numpy.typing.NDArray] = None,
-            mode: Optional[str] = None,
-            delay_num: int = 100,
-            delay_den: int = 1000,
-        ) -> int:
-            """
-            Add frame from numpy array.
-            The frame duration is equal to delay_num / delay_den seconds.
-            Default frame duration is 100/1000 second, or 0.1 second.
-
-            :param numpy.typing.NDArray numpy_data: The pixel data, expressed as 3D numpy array.
-            :param Optional[int] width: The width of the pixel data.
-                If not given, the 2nd dimension size of numpy_data is used.
-            :param Optional[int] height: The height of the pixel data.
-                If not given, the 1st dimension size of numpy_data is used.
-            :param Optional[str] mode: The color mode of data. Possible values are RGB or RGBA.
-                If not given, it is determined using the 3rd dimension size of numpy_data.
-            :param Optional[numpy.typing.NDArray] trns_color: The color [r, g, b] to be treated as transparent, expressed as 1D numpy array.
-                Only use if RGB mode.
-            :param int delay_num: The delay numerator for this frame (defaults to 100).
-            :param int delay_den: The delay denominator for this frame (defaults to 1000).
-
-            :return: The new number of frames.
-            :rtype: int
-            """
-            width = width if width else numpy.shape(numpy_data)[1]
-            height = height if height else numpy.shape(numpy_data)[0]
+        width = width if width else shape(numpy_data)[1]
+        height = height if height else shape(numpy_data)[0]
 
-            if not mode:
-                if numpy.shape(numpy_data)[2] == 3:
+        if not mode:
+            if len(shape(numpy_data)) == 3:
+                if shape(numpy_data)[2] == 3:
                     mode = "RGB"
-                elif numpy.shape(numpy_data)[2] == 4:
+                elif shape(numpy_data)[2] == 4:
                     mode = "RGBA"
-                else:
-                    raise TypeError(
-                        "Cannot determine mode from numpy_data. "
-                        "expected 3rd dimension size to be 3 (RGB) or 4 (RGBA). "
-                        f"The given numpy_data 3rd dimension size was {numpy.shape(numpy_data)[2]}."
-                    )
-
-            if mode == "RGB":
-                if type(trns_color) == numpy.typing.NDArray:
-                    frame = create_frame_from_rgb_trns(
-                        pixels=numpy_data,
-                        width=width,
-                        height=height,
-                        trns_color=trns_color,
-                        delay_num=delay_num,
-                        delay_den=delay_den,
-                    )
-                else:
-                    frame = create_frame_from_rgb(
-                        pixels=numpy_data,
-                        width=width,
-                        height=height,
-                        delay_num=delay_num,
-                        delay_den=delay_den,
-                    )
-            elif mode == "RGBA":
-                if type(trns_color) == numpy.typing.NDArray:
-                    raise TypeError(
-                        "Cannot set trns_color on RGBA mode Pillow object. Must be RGB."
-                    )
-                frame = create_frame_from_rgba(
+            else:
+                raise TypeError(
+                    "Cannot determine mode from numpy_data. "
+                    "expected 3rd dimension size to be 3 (RGB) or 4 (RGBA). "
+                    "The given numpy_data shape was "
+                    f"{shape(numpy_data)}."
+                )
+
+        if mode == "RGB":
+            if isinstance(trns_color, ndarray):
+                frame = create_frame_from_rgb_trns(
                     pixels=numpy_data,
                     width=width,
                     height=height,
+                    trns_color=trns_color,
                     delay_num=delay_num,
                     delay_den=delay_den,
                 )
             else:
-                raise TypeError(f"Invalid mode: {mode}. Must be RGB or RGBA.")
+                frame = create_frame_from_rgb(
+                    pixels=numpy_data,
+                    width=width,
+                    height=height,
+                    delay_num=delay_num,
+                    delay_den=delay_den,
+                )
+        elif mode == "RGBA":
+            if isinstance(trns_color, ndarray):
+                raise TypeError(
+                    "Cannot set trns_color on RGBA mode Pillow object. Must be RGB."
+                )
+            frame = create_frame_from_rgba(
+                pixels=numpy_data,
+                width=width,
+                height=height,
+                delay_num=delay_num,
+                delay_den=delay_den,
+            )
+        else:
+            raise TypeError(f"Invalid mode: {mode}. Must be RGB or RGBA.")
 
-            return self.apngasm.add_frame(frame)
+        return self.apngasm.add_frame(frame)
 
     def assemble(self, output_path: str) -> bool:
         """
         Assembles and outputs an APNG file.
 
         :param str output_path: The output file path.
 
         :return: true if assemble completed succesfully.
         :rtype: bool
         """
         return self.apngasm.assemble(output_path)
 
-    def disassemble_as_numpy(self, file_path: str) -> list[APNGFrame]:
+    def disassemble_as_numpy(self, file_path: str) -> list[NDArray[Any]]:
         """
         Disassembles an APNG file to a list of frames, expressed as 3D numpy array.
 
         :param str file_path: The file path to the PNG image to be disassembled.
 
         :return: A list containing the frames of the disassembled PNG.
-        :rtype: list[apngasm_python._apngasm_python.APNGFrame]
+        :rtype: list[numpy.typing.NDArray[Any]]
         """
-        return self.apngasm.disassemble(file_path)
+        from numpy import array
+
+        frames = self.apngasm.disassemble(file_path)
+        frames_numpy: list[NDArray[Any]] = []
+        for frame in frames:
+            frames_numpy.append(array(frame.pixels))
+
+        return frames_numpy
 
-    def disassemble_as_pillow(self, file_path: str) -> list[APNGFrame]:
+    def disassemble_as_pillow(self, file_path: str) -> list[Image.Image]:
         """
         Disassembles an APNG file to a list of frames, expressed as Pillow images.
 
         :param str file_path: The file path to the PNG image to be disassembled.
 
         :return: A list containing the frames of the disassembled PNG.
-        :rtype: list[apngasm_python._apngasm_python.APNGFrame]
+        :rtype: list[PIL.Image.Image]
         """
-        frames_numpy = self.apngasm.disassemble(file_path)
-        frames_pillow = []
-        for frame in frames_numpy:
+        from PIL import Image
+
+        frames = self.apngasm.disassemble(file_path)
+        frames_pillow: list[Image.Image] = []
+        for frame in frames:
             mode = self.color_type_dict[frame.color_type]
-            frame_pillow = Image.frombytes(
+            frame_pillow = Image.frombytes(  # type: ignore
                 mode, (frame.width, frame.height), frame.pixels
             )
             frames_pillow.append(frame_pillow)
 
         return frames_pillow
 
     def save_pngs(self, output_dir: str) -> bool:
@@ -486,31 +505,32 @@
             if not the same path as the animation spec.
 
         :return: true if save was successful.
         :rtype: bool
         """
         return self.apngasm.save_xml(output_path, image_dir)
 
-    def set_apng_asm_listener(self, listener: Optional[IAPNGAsmListener] = None):
+    def set_apngasm_listener(self, listener: Optional[IAPNGAsmListener] = None):  # type: ignore
         """
         Sets a listener.
         You probably won't need to use this function.
 
-        :param Optional[apngasm_python._apngasm_python.IAPNGAsmListener] listener: A pointer to the listener object.
-            If the argument is None,
+        :param Optional[apngasm_python._apngasm_python.IAPNGAsmListener] listener:
+            A pointer to the listener object. If the argument is None,
             a default APNGAsmListener will be created and assigned.
         """
-        raise NotImplementedError("set_apng_asm_listener is not implemented")
-        # return self.apngasm.set_apng_asm_listener(listener)
+        raise NotImplementedError("set_apngasm_listener is not implemented")
+        # return self.apngasm.set_apngasm_listener(listener)
 
     def set_loops(self, loops: int = 0):
         """
         Set loop count of animation.
 
-        :param int loops: Loop count of animation. If the argument is 0 a loop count is infinity.
+        :param int loops: Loop count of animation. If the argument is 0
+            a loop count is infinity.
         """
         return self.apngasm.set_loops(loops)
 
     def set_skip_first(self, skip_first: bool):
         """
         Set flag of skip first frame.
 
@@ -532,22 +552,22 @@
         Returns the loop count.
 
         :return: loop count.
         :rtype: int
         """
         return self.apngasm.get_loops()
 
-    def is_skip_first(self) -> int:
+    def is_skip_first(self) -> bool:
         """
         Returns the flag of skip first frame.
 
         :return: flag of skip first frame.
-        :rtype: int
+        :rtype: bool
         """
-        return self.apngasm.get_loops()
+        return self.apngasm.is_skip_first()
 
     def frame_count(self) -> int:
         """
         Returns the number of frames.
 
         :return: number of frames.
         :rtype: int
```

### Comparing `apngasm_python-1.2.3/PKG-INFO` & `apngasm_python-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: apngasm-python
-Version: 1.2.3
-Summary: A nanobind API for apngasm, a tool/library for APNG assembly/disassembly.
+Version: 1.3.0
+Summary: A nanobind python API for apngasm, a tool/library for APNG assembly & disassembly with compression support.
 Keywords: apng png nanobind pybind11
 Author-Email: chaudominic <chaudominic2@gmail.com>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
@@ -509,137 +509,156 @@
         
         That's all there is to it!
 Classifier: Topic :: Multimedia :: Graphics
 Project-URL: Repository, https://github.com/laggykiller/apngasm-python
 Project-URL: Documentation, https://apngasm-python.readthedocs.io/en/latest/
 Project-URL: Tracker, https://github.com/laggykiller/apngasm-python/issues
 Requires-Python: >=3.8
+Provides-Extra: full
+Provides-Extra: test
+Provides-Extra: lint
+Requires-Dist: Pillow; extra == "full"
+Requires-Dist: numpy; extra == "full"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: ruff; extra == "lint"
+Requires-Dist: mypy; extra == "lint"
+Requires-Dist: isort; extra == "lint"
+Requires-Dist: types-Pillow; extra == "lint"
 Description-Content-Type: text/markdown
 
 # apngasm-python
 
-A nanobind API for [apngasm](https://github.com/apngasm/apngasm), a tool/library for APNG assembly/disassembly.
+A nanobind API for [apngasm](https://github.com/apngasm/apngasm), which is a
+tool/library for APNG assembly & disassembly with compression support.
 
-apngasm is originally a CLI program for quickly assembling PNG images into animated PNG (APNG). It also supports creating compressed APNG.
+apngasm is originally a CLI program for quickly assembling PNG images into 
+animated PNG (APNG). It also supports creating compressed APNG.
 
-apngasm-python is a binding for apngasm using nanobind, allowing you to use apngasm without calling it using commands.
+apngasm-python is a binding for apngasm using nanobind, allowing you to use apngasm 
+without calling it using commands.
 
-With this module, you can even create APNG using images inside memory (No need to write them out as file and call apngasm! This is about 2 times faster from testing.)
+With this module, you can even create APNG using images inside memory (No need to write 
+them out as file and call apngasm! This is about 2 times faster from testing.)
 
-A similar python module is https://github.com/eight04/pyAPNG , which handles APNG files with python natively and does not support compression.
+A similar python module is https://github.com/eight04/pyAPNG , which handles APNG files 
+with python natively and does not support compression.
 
-For convenience, prebuilt library is packaged with this module, so you need not download apngasm.
+For convenience, prebuilt library is packaged with this module, so you need not 
+download apngasm.
 
 Documentations: https://apngasm-python.readthedocs.io/en/latest/
 
 ## Install
-```
+```bash
 pip install apngasm-python
 ```
 
-Optionally, you can also install `Pillow` and `numpy`
-```
-pip install Pillow numpy
+`Pillow` and `numpy` are optional dependencies. Without them,
+some functions are not usable. To also install them:
+```bash
+pip install apngasm-python[full]
 ```
 
 ## Example usage
-The recommended usage is to `from apngasm_python.apngasm import APNGAsmBinder`, see [example/example_binder.py](example/example_binder.py)
+The recommended usage is to `from apngasm_python.apngasm import APNGAsmBinder`, see 
+[example/example_binder.py](example/example_binder.py)
 ```python
 from apngasm_python.apngasm import APNGAsmBinder
 import numpy as np
 from PIL import Image
 import os
 
 apngasm = APNGAsmBinder()
 
 # From file
-for file_name in sorted(os.listdir('frames')):
+for file_name in sorted(os.listdir("samples/frames")):
     # To adjust frame duration, set delay_num and delay_den
     # The frame duration will be (delay_num / delay_den) seconds
-    apngasm.add_frame_from_file(file_path=os.path.join('frames', file_name), delay_num=100, delay_den=1000)
+    apngasm.add_frame_from_file(file_path=os.path.join("samples/frames", file_name), delay_num=100, delay_den=1000)
     
 # Default value of loops is 0, which is infinite looping of APNG animation
 # This sets the APNG animation to loop for 3 times before stopping
 apngasm.set_loops(3)
-apng.assemble('result-from-file.apng')
+apng.assemble("samples/result-from-file.apng")
 apngasm.reset()
 
 # From Pillow
-for file_name in sorted(os.listdir('frames')):
-    image = Image.open(os.path.join('frames', file_name)).convert('RGBA')
+for file_name in sorted(os.listdir("samples/frames")):
+    image = Image.open(os.path.join("samples/frames", file_name)).convert("RGBA")
     frame = apngasm.add_frame_from_pillow(image, delay_num=50, delay_den=1000)
-apngasm.assemble('result-from-pillow.apng')
+apngasm.assemble("result-from-pillow.apng")
 apngasm.reset()
 
 # Disassemble and get pillow image of one frame
 # You can use with statement to avoid calling reset()
 with APNGAsmBinder() as apng:
-    frames = apng.disassemble_as_pillow('input/ball.apng')
+    frames = apng.disassemble_as_pillow("samples/input/ball.apng")
     frame = frames[0]
-    frame.save('output/ball0.png')
+    frame.save("samples/output/ball0.png")
 
 # Disassemble all APNG into PNGs
-apngasm.save_pngs('output')
+apngasm.save_pngs("samples/output")
 ```
 
-Alternatively, you can reduce overhead and do advanced tasks by calling methods directly, see [example/example_direct.py](example/example_direct.py)
+Alternatively, you can reduce overhead and do advanced tasks by calling methods 
+directly, see [example/example_direct.py](example/example_direct.py)
 ```python
 from apngasm_python._apngasm_python import APNGAsm, APNGFrame, create_frame_from_rgb, create_frame_from_rgba
 import numpy as np
 from PIL import Image
 import os
 
 apngasm = APNGAsm()
 
 # From file
-for file_name in sorted(os.listdir('frames')):
+for file_name in sorted(os.listdir("samples/frames")):
     # To adjust frame duration, set delay_num and delay_den
     # The frame duration will be (delay_num / delay_den) seconds
-    apngasm.add_frame_from_file(file_path=os.path.join('frames', file_name), delay_num=100, delay_den=1000)
+    apngasm.add_frame_from_file(file_path=os.path.join("samples/frames", file_name), delay_num=100, delay_den=1000)
     
 # Default value of loops is 0, which is infinite looping of APNG animation
 # This sets the APNG animation to loop for 3 times before stopping
 apngasm.set_loops(3)
-apng.assemble('result-from-file.apng')
+apng.assemble("samples/result-from-file.apng")
 
 # From Pillow
 apngasm.reset()
-for file_name in sorted(os.listdir('frames')):
-    image = Image.open(os.path.join('frames', file_name)).convert('RGBA')
+for file_name in sorted(os.listdir("samples/frames")):
+    image = Image.open(os.path.join("samples/frames", file_name)).convert("RGBA")
     frame = create_frame_from_rgba(np.array(image), image.width, image.height)
     frame.delay_num = 50
     frame.delay_den = 1000
     apngasm.add_frame(frame)
-apngasm.assemble('result-from-pillow.apng')
+apngasm.assemble("samples/result-from-pillow.apng")
 
 # Disassemble and get pillow image of one frame
 apngasm.reset()
-frames = apngasm.disassemble('input/ball.apng')
+frames = apngasm.disassemble("samples/input/ball.apng")
 frame = frames[0]
 im = Image.frombytes(mode, (frame.width, frame.height), frame.pixels)
-im.save('output/ball0.png')
+im.save("samples/output/ball0.png")
 
 # Disassemble all APNG into PNGs
-apngasm.save_pngs('output')
+apngasm.save_pngs("samples/output")
 ```
 
-The methods are based on [apngasm.h](https://github.com/apngasm/apngasm/blob/master/lib/src/apngasm.h) and [apngframe.h](https://github.com/apngasm/apngasm/blob/master/lib/src/apngframe.h)
+The methods are based on [apngasm.h](https://github.com/apngasm/apngasm/blob/master/lib/src/apngasm.h) 
+and [apngframe.h](https://github.com/apngasm/apngasm/blob/master/lib/src/apngframe.h)
 
 You can get more info about the binding from [src/apngasm_python.cpp](src/apngasm_python.cpp), or by...
 
 ```python
 from apngasm_python import _apngasm_python
 help(_apngasm_python)
 ```
 
 ## Building from source
 ```bash
-git clone https://github.com/laggykiller/apngasm-python.git
+git clone --recursive https://github.com/laggykiller/apngasm-python.git
 cd apngasm-python
-git submodule update --init --recursive
 
 # To build wheel
 python3 -m build .
 
 # To install directly
 pip3 install .
 ```
@@ -657,14 +676,30 @@
 export APNGASM_COMPILE_TARGET=x64
 export APNGASM_COMPILE_TARGET=x86
 export APNGASM_COMPILE_TARGET=armv8
 export APNGASM_COMPILE_TARGET=ppc64le
 export APNGASM_COMPILE_TARGET=s390x
 ```
 
+## Development
+To run tests:
+```bash
+pip install pytest
+pytest
+```
+
+To lint:
+```bash
+pip install ruff mypy isort
+mypy
+isort .
+ruff check
+ruff format
+```
+
 ## Credits
 - apngasm: https://github.com/apngasm/apngasm
 - Packaging: https://github.com/tttapa/py-build-cmake
 - Example files:
     - https://apng.onevcat.com/demo/
     - https://commons.wikimedia.org/wiki/File:Animated_PNG_example_bouncing_beach_ball.png
     - https://commons.wikimedia.org/wiki/File:Grayscale_8bits_palette_sample_image.png
```

