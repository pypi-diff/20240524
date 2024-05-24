# Comparing `tmp/lungo_cli-0.4.1.tar.gz` & `tmp/lungo_cli-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lungo_cli-0.4.1.tar", max compression
+gzip compressed data, was "lungo_cli-0.4.2.tar", max compression
```

## Comparing `lungo_cli-0.4.1.tar` & `lungo_cli-0.4.2.tar`

### file list

```diff
@@ -1,296 +1,296 @@
--rw-r--r--   0        0        0     1075 2024-05-16 06:37:13.733848 lungo_cli-0.4.1/LICENSE
--rw-r--r--   0        0        0     2410 2024-05-16 06:37:13.733848 lungo_cli-0.4.1/README.md
--rw-r--r--   0        0        0     1116 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/app/__init__.py
--rw-r--r--   0        0        0     1264 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/app/main.py
--rw-r--r--   0        0        0     1562 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/app/state.py
--rw-r--r--   0        0        0        0 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/commands/__init__.py
--rw-r--r--   0        0        0      743 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/commands/base.py
--rw-r--r--   0        0        0      478 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/commands/check.py
--rw-r--r--   0        0        0      922 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/commands/down.py
--rw-r--r--   0        0        0     1246 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/commands/install.py
--rw-r--r--   0        0        0     3387 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/commands/list.py
--rw-r--r--   0        0        0     1243 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/commands/uninstall.py
--rw-r--r--   0        0        0     2188 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/commands/up.py
--rw-r--r--   0        0        0        0 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/core/__init__.py
--rw-r--r--   0        0        0    12557 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/core/app.py
--rw-r--r--   0        0        0     5973 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/core/console.py
--rw-r--r--   0        0        0     1042 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/core/constants.py
--rw-r--r--   0        0        0     7390 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/core/container.py
--rw-r--r--   0        0        0     4559 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/core/context.py
--rw-r--r--   0        0        0    10356 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/core/database.py
--rw-r--r--   0        0        0     5978 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/core/file.py
--rw-r--r--   0        0        0     2599 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/core/network.py
--rw-r--r--   0        0        0    17104 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/core/plugin.py
--rw-r--r--   0        0        0     2315 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/core/renderer.py
--rw-r--r--   0        0        0     6583 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/core/storage.py
--rw-r--r--   0        0        0        0 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/helpers/__init__.py
--rw-r--r--   0        0        0     1275 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/helpers/common.py
--rw-r--r--   0        0        0     2494 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/helpers/crypto.py
--rw-r--r--   0        0        0     1077 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/helpers/format.py
--rw-r--r--   0        0        0        0 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/models/__init__.py
--rw-r--r--   0        0        0     1108 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/models/base.py
--rw-r--r--   0        0        0     2876 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/models/config.py
--rw-r--r--   0        0        0      676 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/models/context.py
--rw-r--r--   0        0        0     2964 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/models/plugin.py
--rw-r--r--   0        0        0     1865 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/models/users.py
--rw-r--r--   0        0        0        0 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/plugins/__init__.py
--rw-r--r--   0        0        0      660 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/Dockerfile.jinja
--rw-r--r--   0        0        0      280 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/README.md
--rw-r--r--   0        0        0     2037 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/compose/compose.yaml.jinja
--rw-r--r--   0        0        0     1236 2024-05-16 06:37:13.737848 lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/config/config_export.yaml.jinja
--rw-r--r--   0        0        0      195 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/config/settings.yaml.jinja
--rw-r--r--   0        0        0     1258 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/config/users_export.yaml.jinja
--rw-r--r--   0        0        0     1300 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/nginx/site.conf.jinja
--rw-r--r--   0        0        0      928 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/oathkeeper/access_rules.yaml.jinja
--rw-r--r--   0        0        0      813 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/plugin.py
--rw-r--r--   0        0        0      792 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderOutline.svelte
--rw-r--r--   0        0        0      734 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderSolid.svelte
--rw-r--r--   0        0        0      136 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/web/lib/icons/index.ts
--rw-r--r--   0        0        0      100 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/web/routes/[...url]/+page.svelte
--rw-r--r--   0        0        0     1100 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/Dockerfile.jinja
--rw-r--r--   0        0        0      427 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/README.md
--rw-r--r--   0        0        0     1544 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/compose/compose.yaml.jinja
--rw-r--r--   0        0        0     2774 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/config/config.py.jinja
--rw-r--r--   0        0        0     1218 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/nginx/site.conf.jinja
--rw-r--r--   0        0        0     1799 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/plugin.py
--rw-r--r--   0        0        0       20 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/web/dependencies.txt
--rw-r--r--   0        0        0     2025 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/web/lib/icons/Jupyter.svelte
--rw-r--r--   0        0        0       58 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/web/lib/icons/index.ts
--rw-r--r--   0        0        0      116 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/web/lib/server/constants.server.ts
--rw-r--r--   0        0        0      207 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/web/lib/server/constants.server.ts.jinja
--rw-r--r--   0        0        0     1336 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/web/routes/+layout.server.ts
--rw-r--r--   0        0        0      100 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/web/routes/[...url]/+page.svelte
--rw-r--r--   0        0        0      366 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/Dockerfile.jinja
--rw-r--r--   0        0        0      275 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/README.md
--rw-r--r--   0        0        0      573 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/compose/compose.yaml.jinja
--rw-r--r--   0        0        0     7494 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/config/conf.php.jinja
--rw-r--r--   0        0        0      829 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/config/site.conf.jinja
--rw-r--r--   0        0        0     1159 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/nginx/site.conf.jinja
--rw-r--r--   0        0        0      933 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/oathkeeper/access_rules.yaml.jinja
--rw-r--r--   0        0        0     1030 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/plugin.py
--rw-r--r--   0        0        0      700 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteOutline.svelte
--rw-r--r--   0        0        0      672 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteSolid.svelte
--rw-r--r--   0        0        0      128 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/web/lib/icons/index.ts
--rw-r--r--   0        0        0      100 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/web/routes/[...url]/+page.svelte
--rw-r--r--   0        0        0      919 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/Dockerfile.jinja
--rw-r--r--   0        0        0      418 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/README.md
--rw-r--r--   0        0        0     1416 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/compose/compose.yaml.jinja
--rw-r--r--   0        0        0      135 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/config/rserver.conf.jinja
--rw-r--r--   0        0        0       30 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/config/rsession.conf
--rw-r--r--   0        0        0     1432 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/nginx/site.conf.jinja
--rw-r--r--   0        0        0     1435 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/plugin.py
--rw-r--r--   0        0        0       20 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/web/dependencies.txt
--rw-r--r--   0        0        0     1820 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioOutline.svelte
--rw-r--r--   0        0        0     1563 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioSolid.svelte
--rw-r--r--   0        0        0      140 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/web/lib/icons/index.ts
--rw-r--r--   0        0        0      107 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/web/lib/server/constants.server.ts
--rw-r--r--   0        0        0      195 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/web/lib/server/constants.server.ts.jinja
--rw-r--r--   0        0        0     2216 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/web/routes/+layout.server.ts
--rw-r--r--   0        0        0      100 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/web/routes/[...url]/+page.svelte
--rw-r--r--   0        0        0      269 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rustdesk/README.md
--rw-r--r--   0        0        0      875 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rustdesk/compose/compose.yaml.jinja
--rw-r--r--   0        0        0     1817 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rustdesk/plugin.py
--rw-r--r--   0        0        0     1246 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rustdesk/web/lib/icons/Rustdesk.svelte
--rw-r--r--   0        0        0     1257 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rustdesk/web/lib/icons/ScreenCast.svelte
--rw-r--r--   0        0        0      124 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rustdesk/web/lib/icons/index.ts
--rw-r--r--   0        0        0       74 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rustdesk/web/lib/server/constants.server.ts
--rw-r--r--   0        0        0      127 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rustdesk/web/lib/server/constants.server.ts.jinja
--rw-r--r--   0        0        0      248 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rustdesk/web/routes/+page.server.ts
--rw-r--r--   0        0        0     1586 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/rustdesk/web/routes/+page.svelte
--rw-r--r--   0        0        0      118 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/stirlingpdf/Dockerfile.jinja
--rw-r--r--   0        0        0      280 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/stirlingpdf/README.md
--rw-r--r--   0        0        0      651 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/stirlingpdf/compose/compose.yaml.jinja
--rw-r--r--   0        0        0      295 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/stirlingpdf/config/settings.yaml
--rw-r--r--   0        0        0     1013 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/stirlingpdf/nginx/site.conf.jinja
--rw-r--r--   0        0        0      888 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/stirlingpdf/plugin.py
--rw-r--r--   0        0        0     1444 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/stirlingpdf/web/lib/icons/StirlingPdf.svelte
--rw-r--r--   0        0        0       66 2024-05-16 06:37:13.741848 lungo_cli-0.4.1/src/lungo_cli/plugins/stirlingpdf/web/lib/icons/index.ts
--rw-r--r--   0        0        0      100 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/plugins/stirlingpdf/web/routes/[...url]/+page.svelte
--rw-r--r--   0        0        0      991 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/plugins/xray/README.md
--rw-r--r--   0        0        0      599 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/plugins/xray/compose/compose.yaml.jinja
--rw-r--r--   0        0        0     1234 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/plugins/xray/config/config.json.jinja
--rw-r--r--   0        0        0      423 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/plugins/xray/nginx/site.conf.jinja
--rw-r--r--   0        0        0     1692 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/plugins/xray/plugin.py
--rw-r--r--   0        0        0       33 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/plugins/xray/web/dependencies.txt
--rw-r--r--   0        0        0     1594 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/plugins/xray/web/lib/components/CodeBlock.svelte
--rw-r--r--   0        0        0       58 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/plugins/xray/web/lib/components/index.ts
--rw-r--r--   0        0        0     2133 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/plugins/xray/web/lib/icons/NetworkLock.svelte
--rw-r--r--   0        0        0     1897 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/plugins/xray/web/lib/icons/ProxyOutline.svelte
--rw-r--r--   0        0        0     1808 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/plugins/xray/web/lib/icons/ProxySolid.svelte
--rw-r--r--   0        0        0      198 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/plugins/xray/web/lib/icons/index.ts
--rw-r--r--   0        0        0      239 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/plugins/xray/web/lib/server/constants.server.ts
--rw-r--r--   0        0        0      508 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/plugins/xray/web/lib/server/constants.server.ts.jinja
--rw-r--r--   0        0        0      836 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/plugins/xray/web/routes/+page.server.ts
--rw-r--r--   0        0        0     6645 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/plugins/xray/web/routes/+page.svelte
--rw-r--r--   0        0        0        0 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/__init__.py
--rw-r--r--   0        0        0     5623 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/assets/config_references/config.yaml
--rw-r--r--   0        0        0     1995 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/assets/config_references/users.yaml
--rw-r--r--   0        0        0     6754 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/compose.yaml.jinja
--rw-r--r--   0        0        0      363 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/keto/config.yaml.jinja
--rw-r--r--   0        0        0     2116 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/kratos/config.yaml.jinja
--rw-r--r--   0        0        0    14236 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.body.gotmpl.jinja
--rw-r--r--   0        0        0      408 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.body.plaintext.gotmpl.jinja
--rw-r--r--   0        0        0       51 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.subject.gotmpl.jinja
--rw-r--r--   0        0        0    14238 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.gotmpl.jinja
--rw-r--r--   0        0        0      410 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.plaintext.gotmpl.jinja
--rw-r--r--   0        0        0       50 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.subject.gotmpl.jinja
--rw-r--r--   0        0        0     2801 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/kratos/user.schema.json
--rw-r--r--   0        0        0     1281 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx/conf.d/default.conf.jinja
--rw-r--r--   0        0        0       92 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx/custom.d/jit.conf
--rw-r--r--   0        0        0      207 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx/sites/apps.conf.jinja
--rw-r--r--   0        0        0      834 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx/sites/oathkeeper.conf
--rw-r--r--   0        0        0      712 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx/snippets/auth.conf
--rw-r--r--   0        0        0      527 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx/snippets/proxy.conf
--rw-r--r--   0        0        0      558 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx/snippets/upstreams.conf.jinja
--rw-r--r--   0        0        0     2257 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx_gateway/conf.d/default.conf.jinja
--rw-r--r--   0        0        0       92 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx_gateway/custom.d/jit.conf
--rw-r--r--   0        0        0       90 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx_gateway/snippets/certificate.conf
--rw-r--r--   0        0        0     1547 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx_gateway/snippets/proxy.conf.jinja
--rw-r--r--   0        0        0     1609 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx_gateway/snippets/rate_limiting.conf.jinja
--rw-r--r--   0        0        0     1423 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/oathkeeper/access_rules.yaml.jinja
--rw-r--r--   0        0        0     1634 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/config/oathkeeper/config.yaml.jinja
--rw-r--r--   0        0        0      456 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/dockerfiles/keto_admin/compose.yaml.jinja
--rw-r--r--   0        0        0      802 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/dockerfiles/kratos_admin/compose.yaml.jinja
--rw-r--r--   0        0        0      832 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/dockerfiles/nginx.Dockerfile.jinja
--rw-r--r--   0        0        0       82 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/excluded/kratos/secrets.yaml.jinja
--rw-r--r--   0        0        0      426 2024-05-16 06:37:15.525859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/.editorconfig
--rw-r--r--   0        0        0       93 2024-05-16 06:37:14.361852 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/.git
--rw-r--r--   0        0        0      519 2024-05-16 06:37:15.525859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/.gitattributes
--rw-r--r--   0        0        0      128 2024-05-16 06:37:15.525859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CODEOWNERS
--rw-r--r--   0        0        0      121 2024-05-16 06:37:15.525859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     5476 2024-05-16 06:37:15.525859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      323 2024-05-16 06:37:15.525859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/.github/FUNDING.yml
--rw-r--r--   0        0        0      105 2024-05-16 06:37:15.525859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/.github/dependabot.yml
--rw-r--r--   0        0        0      958 2024-05-16 06:37:15.525859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/auto-merge.yml
--rw-r--r--   0        0        0      322 2024-05-16 06:37:15.525859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1284 2024-05-16 06:37:15.525859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/server.yml
--rw-r--r--   0        0        0       91 2024-05-16 06:37:15.525859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/.gitignore
--rw-r--r--   0        0        0    41306 2024-05-16 06:37:15.525859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/CHANGELOG.md
--rw-r--r--   0        0        0     1043 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/LICENSE.txt
--rw-r--r--   0        0        0     4817 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/README.md
--rw-r--r--   0        0        0      763 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/.default.conf
--rw-r--r--   0        0        0      932 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/no-ssl.default.conf
--rw-r--r--   0        0        0     1434 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/example.com.conf
--rw-r--r--   0        0        0     1133 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/no-ssl.example.com.conf
--rw-r--r--   0        0        0      314 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/basic.conf
--rw-r--r--   0        0        0      739 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/requests.conf
--rw-r--r--   0        0        0      761 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/resource_timing.conf
--rw-r--r--   0        0        0      385 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/errors/custom_errors.conf
--rw-r--r--   0        0        0     1706 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/security_file_access.conf
--rw-r--r--   0        0        0      701 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_filename-based_cache_busting.conf
--rw-r--r--   0        0        0      685 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_svgz-compression.conf
--rw-r--r--   0        0        0     1029 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/character_encodings.conf
--rw-r--r--   0        0        0      650 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/media_types.conf
--rw-r--r--   0        0        0     1198 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/content-security-policy.conf
--rw-r--r--   0        0        0     2102 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/cross-origin-policy.conf
--rw-r--r--   0        0        0     1121 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/permissions-policy.conf
--rw-r--r--   0        0        0     1135 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/referrer-policy.conf
--rw-r--r--   0        0        0      396 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/server_software_information.conf
--rw-r--r--   0        0        0     2008 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/strict-transport-security.conf
--rw-r--r--   0        0        0      871 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-content-type-options.conf
--rw-r--r--   0        0        0     1800 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-frame-options.conf
--rw-r--r--   0        0        0     1136 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/certificate_files.conf
--rw-r--r--   0        0        0     1235 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ocsp_stapling.conf
--rw-r--r--   0        0        0      797 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_balanced.conf
--rw-r--r--   0        0        0     1818 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_strict.conf
--rw-r--r--   0        0        0     1880 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ssl_engine.conf
--rw-r--r--   0        0        0     2202 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-control.conf
--rw-r--r--   0        0        0     1484 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-file-descriptors.conf
--rw-r--r--   0        0        0     2220 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache_expiration.conf
--rw-r--r--   0        0        0     2049 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/compression.conf
--rw-r--r--   0        0        0     1435 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/content_transformation.conf
--rw-r--r--   0        0        0      732 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_brotli.conf
--rw-r--r--   0        0        0      572 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_gzip.conf
--rw-r--r--   0        0        0     5775 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/mime.types
--rw-r--r--   0        0        0     7293 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/nginx.conf
--rw-r--r--   0        0        0      399 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/default.conf
--rw-r--r--   0        0        0      678 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/secure.server.localhost.conf
--rw-r--r--   0        0        0      782 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/server.localhost.conf
--rw-r--r--   0        0        0      126 2024-05-16 06:37:15.529859 lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/www-server.localhost.conf
--rw-r--r--   0        0        0      161 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/web/.dockerignore
--rw-r--r--   0        0        0      160 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/web/.eslintignore
--rw-r--r--   0        0        0      702 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/web/.eslintrc.cjs
--rw-r--r--   0        0        0       19 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/web/.npmrc
--rw-r--r--   0        0        0      160 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/web/.prettierignore
--rw-r--r--   0        0        0      351 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/web/.prettierrc
--rw-r--r--   0        0        0      763 2024-05-16 06:37:13.745848 lungo_cli-0.4.1/src/lungo_cli/resources/web/Dockerfile.jinja
--rw-r--r--   0        0        0    40573 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/assets/schemas/keto.openapi.json
--rw-r--r--   0        0        0   300951 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/assets/schemas/kratos.openapi.json
--rw-r--r--   0        0        0     1729 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/package.json
--rw-r--r--   0        0        0   120480 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/pnpm-lock.yaml
--rw-r--r--   0        0        0      264 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/postcss.config.cjs
--rw-r--r--   0        0        0      304 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/app.d.ts
--rw-r--r--   0        0        0      352 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/app.html
--rw-r--r--   0        0        0     1736 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/app.pcss
--rw-r--r--   0        0        0      248 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/hooks.server.ts
--rw-r--r--   0        0        0     3137 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/actions.ts
--rw-r--r--   0        0        0   146031 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/assets/cover.jpg
--rw-r--r--   0        0        0     1713 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/AccountDropdown.svelte
--rw-r--r--   0        0        0     5068 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/AppShell.svelte
--rw-r--r--   0        0        0     7325 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/FormBuilder.svelte
--rw-r--r--   0        0        0      556 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/HeroFrame.svelte
--rw-r--r--   0        0        0      618 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/LoadingIndicator.svelte
--rw-r--r--   0        0        0     1525 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/NavRail.svelte
--rw-r--r--   0        0        0      887 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/PasswordInput.svelte
--rw-r--r--   0        0        0     6343 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/PatchedIFrame.svelte
--rw-r--r--   0        0        0      608 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/SwappableIcon.svelte
--rw-r--r--   0        0        0     1691 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/ThemeSelector.svelte
--rw-r--r--   0        0        0     1719 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/ThemeSelectorDropdown.svelte
--rw-r--r--   0        0        0      566 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/index.ts
--rw-r--r--   0        0        0      237 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/constants.ts
--rw-r--r--   0        0        0     2166 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/Account.svelte
--rw-r--r--   0        0        0      414 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/BaseIcon.svelte
--rw-r--r--   0        0        0      432 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/Check.svelte
--rw-r--r--   0        0        0     1031 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/Close.svelte
--rw-r--r--   0        0        0     1337 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/DarkMode.svelte
--rw-r--r--   0        0        0      427 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/Expand.svelte
--rw-r--r--   0        0        0      522 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/Fullscreen.svelte
--rw-r--r--   0        0        0     3326 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/LightMode.svelte
--rw-r--r--   0        0        0      617 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/Logout.svelte
--rw-r--r--   0        0        0     1182 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/Menu.svelte
--rw-r--r--   0        0        0     1259 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/QuestionMark.svelte
--rw-r--r--   0        0        0     1707 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/Reset.svelte
--rw-r--r--   0        0        0     2164 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/Settings.svelte
--rw-r--r--   0        0        0     1861 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/VisibilityOff.svelte
--rw-r--r--   0        0        0     1476 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/VisibilityOn.svelte
--rw-r--r--   0        0        0      836 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/index.ts
--rw-r--r--   0        0        0      158 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/server/constants.ts
--rw-r--r--   0        0        0      953 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/server/utils/api.ts
--rw-r--r--   0        0        0       46 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/server/utils/index.ts
--rw-r--r--   0        0        0      109 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/server/utils/stubs.ts
--rw-r--r--   0        0        0      678 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/server/utils/stubs.ts.jinja
--rw-r--r--   0        0        0     2312 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/stores.ts
--rw-r--r--   0        0        0      324 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/types/common.ts
--rw-r--r--   0        0        0      224 2024-05-16 06:37:13.749848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/types/index.ts
--rw-r--r--   0        0        0    31445 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/types/keto.d.ts
--rw-r--r--   0        0        0   298809 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/types/kratos.d.ts
--rw-r--r--   0        0        0      511 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/types/user.d.ts
--rw-r--r--   0        0        0     2825 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/utils/api.ts
--rw-r--r--   0        0        0      483 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/utils/app.ts
--rw-r--r--   0        0        0     2348 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/utils/common.ts
--rw-r--r--   0        0        0       93 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/utils/index.ts
--rw-r--r--   0        0        0      225 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/utils/stubs.ts
--rw-r--r--   0        0        0     1283 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/utils/stubs.ts.jinja
--rw-r--r--   0        0        0      289 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/(account)/+layout.svelte
--rw-r--r--   0        0        0     4699 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/(account)/account/+page.server.ts
--rw-r--r--   0        0        0      335 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/(account)/account/+page.svelte
--rw-r--r--   0        0        0     7010 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/(account)/login/+page.server.ts
--rw-r--r--   0        0        0      590 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/(account)/login/+page.svelte
--rw-r--r--   0        0        0      438 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/(account)/logout/+server.ts
--rw-r--r--   0        0        0     5159 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.server.ts
--rw-r--r--   0        0        0      369 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.svelte
--rw-r--r--   0        0        0      463 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/(apps)/+layout.svelte
--rw-r--r--   0        0        0     1277 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/(apps)/+page.svelte
--rw-r--r--   0        0        0      448 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/(apps)/app/+layout.server.ts
--rw-r--r--   0        0        0      130 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/(apps)/app/+page.server.ts
--rw-r--r--   0        0        0     1008 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/+error.svelte
--rw-r--r--   0        0        0     2407 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/+layout.server.ts
--rw-r--r--   0        0        0      938 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/+layout.svelte
--rw-r--r--   0        0        0    25573 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/static/favicon.png
--rw-r--r--   0        0        0      276 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/svelte.config.js
--rw-r--r--   0        0        0     1835 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/tailwind.config.cjs
--rw-r--r--   0        0        0      601 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/tsconfig.json
--rw-r--r--   0        0        0      219 2024-05-16 06:37:13.753848 lungo_cli-0.4.1/src/lungo_cli/resources/web/vite.config.ts
--rw-r--r--   0        0        0     3385 1970-01-01 00:00:00.000000 lungo_cli-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-24 17:48:19.274924 lungo_cli-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2410 2024-05-24 17:48:19.274924 lungo_cli-0.4.2/README.md
+-rw-r--r--   0        0        0     1116 2024-05-24 17:48:19.274924 lungo_cli-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-24 17:48:19.274924 lungo_cli-0.4.2/src/lungo_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 17:48:19.274924 lungo_cli-0.4.2/src/lungo_cli/app/__init__.py
+-rw-r--r--   0        0        0     1264 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/app/main.py
+-rw-r--r--   0        0        0     1562 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/app/state.py
+-rw-r--r--   0        0        0        0 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/commands/__init__.py
+-rw-r--r--   0        0        0      743 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/commands/base.py
+-rw-r--r--   0        0        0      478 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/commands/check.py
+-rw-r--r--   0        0        0      922 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/commands/down.py
+-rw-r--r--   0        0        0     1246 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/commands/install.py
+-rw-r--r--   0        0        0     3387 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/commands/list.py
+-rw-r--r--   0        0        0     1243 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/commands/uninstall.py
+-rw-r--r--   0        0        0     2188 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/commands/up.py
+-rw-r--r--   0        0        0        0 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/core/__init__.py
+-rw-r--r--   0        0        0    12557 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/core/app.py
+-rw-r--r--   0        0        0     5973 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/core/console.py
+-rw-r--r--   0        0        0     1042 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/core/constants.py
+-rw-r--r--   0        0        0     7548 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/core/container.py
+-rw-r--r--   0        0        0     4559 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/core/context.py
+-rw-r--r--   0        0        0    10356 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/core/database.py
+-rw-r--r--   0        0        0     5978 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/core/file.py
+-rw-r--r--   0        0        0     2599 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/core/network.py
+-rw-r--r--   0        0        0    17104 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/core/plugin.py
+-rw-r--r--   0        0        0     2315 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/core/renderer.py
+-rw-r--r--   0        0        0     6583 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/core/storage.py
+-rw-r--r--   0        0        0        0 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1275 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/helpers/common.py
+-rw-r--r--   0        0        0     2494 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/helpers/crypto.py
+-rw-r--r--   0        0        0     1077 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/helpers/format.py
+-rw-r--r--   0        0        0        0 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/models/__init__.py
+-rw-r--r--   0        0        0     1108 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/models/base.py
+-rw-r--r--   0        0        0     2876 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/models/config.py
+-rw-r--r--   0        0        0      676 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/models/context.py
+-rw-r--r--   0        0        0     2964 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/models/plugin.py
+-rw-r--r--   0        0        0     1865 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/models/users.py
+-rw-r--r--   0        0        0        0 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/__init__.py
+-rw-r--r--   0        0        0      660 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/Dockerfile.jinja
+-rw-r--r--   0        0        0      280 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/README.md
+-rw-r--r--   0        0        0     2037 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0     1236 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/config/config_export.yaml.jinja
+-rw-r--r--   0        0        0      195 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/config/settings.yaml.jinja
+-rw-r--r--   0        0        0     1258 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/config/users_export.yaml.jinja
+-rw-r--r--   0        0        0     1300 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/nginx/site.conf.jinja
+-rw-r--r--   0        0        0      928 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/oathkeeper/access_rules.yaml.jinja
+-rw-r--r--   0        0        0      813 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/plugin.py
+-rw-r--r--   0        0        0      792 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderOutline.svelte
+-rw-r--r--   0        0        0      734 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderSolid.svelte
+-rw-r--r--   0        0        0      136 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/web/lib/icons/index.ts
+-rw-r--r--   0        0        0      100 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/web/routes/[...url]/+page.svelte
+-rw-r--r--   0        0        0     1100 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/Dockerfile.jinja
+-rw-r--r--   0        0        0      427 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/README.md
+-rw-r--r--   0        0        0     1544 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0     2774 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/config/config.py.jinja
+-rw-r--r--   0        0        0     1218 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/nginx/site.conf.jinja
+-rw-r--r--   0        0        0     1799 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/plugin.py
+-rw-r--r--   0        0        0       20 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/web/dependencies.txt
+-rw-r--r--   0        0        0     2025 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/web/lib/icons/Jupyter.svelte
+-rw-r--r--   0        0        0       58 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/web/lib/icons/index.ts
+-rw-r--r--   0        0        0      116 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/web/lib/server/constants.server.ts
+-rw-r--r--   0        0        0      207 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/web/lib/server/constants.server.ts.jinja
+-rw-r--r--   0        0        0     1336 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/web/routes/+layout.server.ts
+-rw-r--r--   0        0        0      100 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/web/routes/[...url]/+page.svelte
+-rw-r--r--   0        0        0      366 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/Dockerfile.jinja
+-rw-r--r--   0        0        0      275 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/README.md
+-rw-r--r--   0        0        0      573 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0     7494 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/config/conf.php.jinja
+-rw-r--r--   0        0        0      829 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/config/site.conf.jinja
+-rw-r--r--   0        0        0     1159 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/nginx/site.conf.jinja
+-rw-r--r--   0        0        0      933 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/oathkeeper/access_rules.yaml.jinja
+-rw-r--r--   0        0        0     1030 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/plugin.py
+-rw-r--r--   0        0        0      700 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteOutline.svelte
+-rw-r--r--   0        0        0      672 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteSolid.svelte
+-rw-r--r--   0        0        0      128 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/web/lib/icons/index.ts
+-rw-r--r--   0        0        0      100 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/web/routes/[...url]/+page.svelte
+-rw-r--r--   0        0        0      919 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/Dockerfile.jinja
+-rw-r--r--   0        0        0      418 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/README.md
+-rw-r--r--   0        0        0     1416 2024-05-24 17:48:19.278924 lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0      135 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/config/rserver.conf.jinja
+-rw-r--r--   0        0        0       30 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/config/rsession.conf
+-rw-r--r--   0        0        0     1432 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/nginx/site.conf.jinja
+-rw-r--r--   0        0        0     1435 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/plugin.py
+-rw-r--r--   0        0        0       20 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/web/dependencies.txt
+-rw-r--r--   0        0        0     1820 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioOutline.svelte
+-rw-r--r--   0        0        0     1563 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioSolid.svelte
+-rw-r--r--   0        0        0      140 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/web/lib/icons/index.ts
+-rw-r--r--   0        0        0      107 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/web/lib/server/constants.server.ts
+-rw-r--r--   0        0        0      195 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/web/lib/server/constants.server.ts.jinja
+-rw-r--r--   0        0        0     2216 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/web/routes/+layout.server.ts
+-rw-r--r--   0        0        0      100 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/web/routes/[...url]/+page.svelte
+-rw-r--r--   0        0        0      269 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rustdesk/README.md
+-rw-r--r--   0        0        0      975 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rustdesk/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0     1817 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rustdesk/plugin.py
+-rw-r--r--   0        0        0     1246 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rustdesk/web/lib/icons/Rustdesk.svelte
+-rw-r--r--   0        0        0     1257 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rustdesk/web/lib/icons/ScreenCast.svelte
+-rw-r--r--   0        0        0      124 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rustdesk/web/lib/icons/index.ts
+-rw-r--r--   0        0        0       74 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rustdesk/web/lib/server/constants.server.ts
+-rw-r--r--   0        0        0      127 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rustdesk/web/lib/server/constants.server.ts.jinja
+-rw-r--r--   0        0        0      248 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rustdesk/web/routes/+page.server.ts
+-rw-r--r--   0        0        0     1586 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/rustdesk/web/routes/+page.svelte
+-rw-r--r--   0        0        0      118 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/stirlingpdf/Dockerfile.jinja
+-rw-r--r--   0        0        0      280 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/stirlingpdf/README.md
+-rw-r--r--   0        0        0      651 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/stirlingpdf/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0      295 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/stirlingpdf/config/settings.yaml
+-rw-r--r--   0        0        0     1013 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/stirlingpdf/nginx/site.conf.jinja
+-rw-r--r--   0        0        0      888 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/stirlingpdf/plugin.py
+-rw-r--r--   0        0        0     1444 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/stirlingpdf/web/lib/icons/StirlingPdf.svelte
+-rw-r--r--   0        0        0       66 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/stirlingpdf/web/lib/icons/index.ts
+-rw-r--r--   0        0        0      100 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/stirlingpdf/web/routes/[...url]/+page.svelte
+-rw-r--r--   0        0        0      991 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/xray/README.md
+-rw-r--r--   0        0        0      599 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/xray/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0     1234 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/xray/config/config.json.jinja
+-rw-r--r--   0        0        0      423 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/xray/nginx/site.conf.jinja
+-rw-r--r--   0        0        0     1692 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/xray/plugin.py
+-rw-r--r--   0        0        0       33 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/xray/web/dependencies.txt
+-rw-r--r--   0        0        0     1594 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/xray/web/lib/components/CodeBlock.svelte
+-rw-r--r--   0        0        0       58 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/xray/web/lib/components/index.ts
+-rw-r--r--   0        0        0     2133 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/xray/web/lib/icons/NetworkLock.svelte
+-rw-r--r--   0        0        0     1897 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/xray/web/lib/icons/ProxyOutline.svelte
+-rw-r--r--   0        0        0     1808 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/xray/web/lib/icons/ProxySolid.svelte
+-rw-r--r--   0        0        0      198 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/xray/web/lib/icons/index.ts
+-rw-r--r--   0        0        0      239 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/xray/web/lib/server/constants.server.ts
+-rw-r--r--   0        0        0      508 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/xray/web/lib/server/constants.server.ts.jinja
+-rw-r--r--   0        0        0      836 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/xray/web/routes/+page.server.ts
+-rw-r--r--   0        0        0     6645 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/plugins/xray/web/routes/+page.svelte
+-rw-r--r--   0        0        0        0 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/__init__.py
+-rw-r--r--   0        0        0     5623 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/assets/config_references/config.yaml
+-rw-r--r--   0        0        0     1995 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/assets/config_references/users.yaml
+-rw-r--r--   0        0        0     6754 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/compose.yaml.jinja
+-rw-r--r--   0        0        0      363 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/config/keto/config.yaml.jinja
+-rw-r--r--   0        0        0     2116 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/config/kratos/config.yaml.jinja
+-rw-r--r--   0        0        0    14236 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.body.gotmpl.jinja
+-rw-r--r--   0        0        0      408 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.body.plaintext.gotmpl.jinja
+-rw-r--r--   0        0        0       51 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.subject.gotmpl.jinja
+-rw-r--r--   0        0        0    14238 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.gotmpl.jinja
+-rw-r--r--   0        0        0      410 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.plaintext.gotmpl.jinja
+-rw-r--r--   0        0        0       50 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.subject.gotmpl.jinja
+-rw-r--r--   0        0        0     2801 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/config/kratos/user.schema.json
+-rw-r--r--   0        0        0     1281 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx/conf.d/default.conf.jinja
+-rw-r--r--   0        0        0       92 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx/custom.d/jit.conf
+-rw-r--r--   0        0        0      207 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx/sites/apps.conf.jinja
+-rw-r--r--   0        0        0      834 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx/sites/oathkeeper.conf
+-rw-r--r--   0        0        0      712 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx/snippets/auth.conf
+-rw-r--r--   0        0        0      527 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx/snippets/proxy.conf
+-rw-r--r--   0        0        0      558 2024-05-24 17:48:19.282924 lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx/snippets/upstreams.conf.jinja
+-rw-r--r--   0        0        0     2257 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx_gateway/conf.d/default.conf.jinja
+-rw-r--r--   0        0        0       92 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx_gateway/custom.d/jit.conf
+-rw-r--r--   0        0        0       90 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx_gateway/snippets/certificate.conf
+-rw-r--r--   0        0        0     1547 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx_gateway/snippets/proxy.conf.jinja
+-rw-r--r--   0        0        0     1609 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx_gateway/snippets/rate_limiting.conf.jinja
+-rw-r--r--   0        0        0     1423 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/config/oathkeeper/access_rules.yaml.jinja
+-rw-r--r--   0        0        0     1634 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/config/oathkeeper/config.yaml.jinja
+-rw-r--r--   0        0        0      456 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/dockerfiles/keto_admin/compose.yaml.jinja
+-rw-r--r--   0        0        0      802 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/dockerfiles/kratos_admin/compose.yaml.jinja
+-rw-r--r--   0        0        0      832 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/dockerfiles/nginx.Dockerfile.jinja
+-rw-r--r--   0        0        0       82 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/excluded/kratos/secrets.yaml.jinja
+-rw-r--r--   0        0        0      426 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/.editorconfig
+-rw-r--r--   0        0        0       93 2024-05-24 17:48:19.598920 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/.git
+-rw-r--r--   0        0        0      519 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/.gitattributes
+-rw-r--r--   0        0        0      128 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CODEOWNERS
+-rw-r--r--   0        0        0      121 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     5476 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      323 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/.github/FUNDING.yml
+-rw-r--r--   0        0        0      105 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/.github/dependabot.yml
+-rw-r--r--   0        0        0      958 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/auto-merge.yml
+-rw-r--r--   0        0        0      322 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1284 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/server.yml
+-rw-r--r--   0        0        0       91 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/.gitignore
+-rw-r--r--   0        0        0    41306 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/CHANGELOG.md
+-rw-r--r--   0        0        0     1043 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/LICENSE.txt
+-rw-r--r--   0        0        0     4817 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/README.md
+-rw-r--r--   0        0        0      763 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/.default.conf
+-rw-r--r--   0        0        0      932 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/no-ssl.default.conf
+-rw-r--r--   0        0        0     1434 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/example.com.conf
+-rw-r--r--   0        0        0     1133 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/no-ssl.example.com.conf
+-rw-r--r--   0        0        0      314 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/basic.conf
+-rw-r--r--   0        0        0      739 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/requests.conf
+-rw-r--r--   0        0        0      761 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/resource_timing.conf
+-rw-r--r--   0        0        0      385 2024-05-24 17:48:20.134915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/errors/custom_errors.conf
+-rw-r--r--   0        0        0     1706 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/security_file_access.conf
+-rw-r--r--   0        0        0      701 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_filename-based_cache_busting.conf
+-rw-r--r--   0        0        0      685 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_svgz-compression.conf
+-rw-r--r--   0        0        0     1029 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/character_encodings.conf
+-rw-r--r--   0        0        0      650 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/media_types.conf
+-rw-r--r--   0        0        0     1198 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/content-security-policy.conf
+-rw-r--r--   0        0        0     2102 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/cross-origin-policy.conf
+-rw-r--r--   0        0        0     1121 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/permissions-policy.conf
+-rw-r--r--   0        0        0     1135 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/referrer-policy.conf
+-rw-r--r--   0        0        0      396 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/server_software_information.conf
+-rw-r--r--   0        0        0     2008 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/strict-transport-security.conf
+-rw-r--r--   0        0        0      871 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-content-type-options.conf
+-rw-r--r--   0        0        0     1800 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-frame-options.conf
+-rw-r--r--   0        0        0     1136 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/certificate_files.conf
+-rw-r--r--   0        0        0     1235 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ocsp_stapling.conf
+-rw-r--r--   0        0        0      797 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_balanced.conf
+-rw-r--r--   0        0        0     1818 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_strict.conf
+-rw-r--r--   0        0        0     1880 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ssl_engine.conf
+-rw-r--r--   0        0        0     2202 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-control.conf
+-rw-r--r--   0        0        0     1484 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-file-descriptors.conf
+-rw-r--r--   0        0        0     2220 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache_expiration.conf
+-rw-r--r--   0        0        0     2049 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/compression.conf
+-rw-r--r--   0        0        0     1435 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/content_transformation.conf
+-rw-r--r--   0        0        0      732 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_brotli.conf
+-rw-r--r--   0        0        0      572 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_gzip.conf
+-rw-r--r--   0        0        0     5775 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/mime.types
+-rw-r--r--   0        0        0     7293 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/nginx.conf
+-rw-r--r--   0        0        0      399 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/default.conf
+-rw-r--r--   0        0        0      678 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/secure.server.localhost.conf
+-rw-r--r--   0        0        0      782 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/server.localhost.conf
+-rw-r--r--   0        0        0      126 2024-05-24 17:48:20.138915 lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/www-server.localhost.conf
+-rw-r--r--   0        0        0      161 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/.dockerignore
+-rw-r--r--   0        0        0      160 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/.eslintignore
+-rw-r--r--   0        0        0      702 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/.eslintrc.cjs
+-rw-r--r--   0        0        0       19 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/.npmrc
+-rw-r--r--   0        0        0      160 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/.prettierignore
+-rw-r--r--   0        0        0      351 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/.prettierrc
+-rw-r--r--   0        0        0      763 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/Dockerfile.jinja
+-rw-r--r--   0        0        0    40573 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/assets/schemas/keto.openapi.json
+-rw-r--r--   0        0        0   300951 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/assets/schemas/kratos.openapi.json
+-rw-r--r--   0        0        0     1732 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/package.json
+-rw-r--r--   0        0        0   120519 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/pnpm-lock.yaml
+-rw-r--r--   0        0        0      264 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/postcss.config.cjs
+-rw-r--r--   0        0        0      304 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/app.d.ts
+-rw-r--r--   0        0        0      352 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/app.html
+-rw-r--r--   0        0        0     1736 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/app.pcss
+-rw-r--r--   0        0        0      248 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/hooks.server.ts
+-rw-r--r--   0        0        0     3137 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/actions.ts
+-rw-r--r--   0        0        0   146031 2024-05-24 17:48:19.286924 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/assets/cover.jpg
+-rw-r--r--   0        0        0     1713 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/AccountDropdown.svelte
+-rw-r--r--   0        0        0     5068 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/AppShell.svelte
+-rw-r--r--   0        0        0     7325 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/FormBuilder.svelte
+-rw-r--r--   0        0        0      556 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/HeroFrame.svelte
+-rw-r--r--   0        0        0      618 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/LoadingIndicator.svelte
+-rw-r--r--   0        0        0     1525 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/NavRail.svelte
+-rw-r--r--   0        0        0      887 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/PasswordInput.svelte
+-rw-r--r--   0        0        0     6343 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/PatchedIFrame.svelte
+-rw-r--r--   0        0        0      608 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/SwappableIcon.svelte
+-rw-r--r--   0        0        0     1691 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/ThemeSelector.svelte
+-rw-r--r--   0        0        0     1719 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/ThemeSelectorDropdown.svelte
+-rw-r--r--   0        0        0      566 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/index.ts
+-rw-r--r--   0        0        0      237 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/constants.ts
+-rw-r--r--   0        0        0     2166 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/Account.svelte
+-rw-r--r--   0        0        0      414 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/BaseIcon.svelte
+-rw-r--r--   0        0        0      432 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/Check.svelte
+-rw-r--r--   0        0        0     1031 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/Close.svelte
+-rw-r--r--   0        0        0     1337 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/DarkMode.svelte
+-rw-r--r--   0        0        0      427 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/Expand.svelte
+-rw-r--r--   0        0        0      522 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/Fullscreen.svelte
+-rw-r--r--   0        0        0     3326 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/LightMode.svelte
+-rw-r--r--   0        0        0      617 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/Logout.svelte
+-rw-r--r--   0        0        0     1182 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/Menu.svelte
+-rw-r--r--   0        0        0     1259 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/QuestionMark.svelte
+-rw-r--r--   0        0        0     1707 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/Reset.svelte
+-rw-r--r--   0        0        0     2164 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/Settings.svelte
+-rw-r--r--   0        0        0     1861 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/VisibilityOff.svelte
+-rw-r--r--   0        0        0     1476 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/VisibilityOn.svelte
+-rw-r--r--   0        0        0      836 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/index.ts
+-rw-r--r--   0        0        0      158 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/server/constants.ts
+-rw-r--r--   0        0        0      953 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/server/utils/api.ts
+-rw-r--r--   0        0        0       46 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/server/utils/index.ts
+-rw-r--r--   0        0        0      109 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/server/utils/stubs.ts
+-rw-r--r--   0        0        0      678 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/server/utils/stubs.ts.jinja
+-rw-r--r--   0        0        0     2312 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/stores.ts
+-rw-r--r--   0        0        0      324 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/types/common.ts
+-rw-r--r--   0        0        0      224 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/types/index.ts
+-rw-r--r--   0        0        0    31445 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/types/keto.d.ts
+-rw-r--r--   0        0        0   298809 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/types/kratos.d.ts
+-rw-r--r--   0        0        0      511 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/types/user.d.ts
+-rw-r--r--   0        0        0     2825 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/utils/api.ts
+-rw-r--r--   0        0        0      483 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/utils/app.ts
+-rw-r--r--   0        0        0     2348 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/utils/common.ts
+-rw-r--r--   0        0        0       93 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/utils/index.ts
+-rw-r--r--   0        0        0      225 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/utils/stubs.ts
+-rw-r--r--   0        0        0     1283 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/utils/stubs.ts.jinja
+-rw-r--r--   0        0        0      289 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/(account)/+layout.svelte
+-rw-r--r--   0        0        0     4683 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/(account)/account/+page.server.ts
+-rw-r--r--   0        0        0      335 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/(account)/account/+page.svelte
+-rw-r--r--   0        0        0     6994 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/(account)/login/+page.server.ts
+-rw-r--r--   0        0        0      590 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/(account)/login/+page.svelte
+-rw-r--r--   0        0        0      438 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/(account)/logout/+server.ts
+-rw-r--r--   0        0        0     5143 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.server.ts
+-rw-r--r--   0        0        0      369 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.svelte
+-rw-r--r--   0        0        0      463 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/(apps)/+layout.svelte
+-rw-r--r--   0        0        0     1277 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/(apps)/+page.svelte
+-rw-r--r--   0        0        0      448 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/(apps)/app/+layout.server.ts
+-rw-r--r--   0        0        0      130 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/(apps)/app/+page.server.ts
+-rw-r--r--   0        0        0     1008 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/+error.svelte
+-rw-r--r--   0        0        0     2375 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/+layout.server.ts
+-rw-r--r--   0        0        0      938 2024-05-24 17:48:19.290923 lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/+layout.svelte
+-rw-r--r--   0        0        0    25573 2024-05-24 17:48:19.294923 lungo_cli-0.4.2/src/lungo_cli/resources/web/static/favicon.png
+-rw-r--r--   0        0        0      276 2024-05-24 17:48:19.294923 lungo_cli-0.4.2/src/lungo_cli/resources/web/svelte.config.js
+-rw-r--r--   0        0        0     1835 2024-05-24 17:48:19.294923 lungo_cli-0.4.2/src/lungo_cli/resources/web/tailwind.config.cjs
+-rw-r--r--   0        0        0      601 2024-05-24 17:48:19.294923 lungo_cli-0.4.2/src/lungo_cli/resources/web/tsconfig.json
+-rw-r--r--   0        0        0      219 2024-05-24 17:48:19.294923 lungo_cli-0.4.2/src/lungo_cli/resources/web/vite.config.ts
+-rw-r--r--   0        0        0     3385 1970-01-01 00:00:00.000000 lungo_cli-0.4.2/PKG-INFO
```

### Comparing `lungo_cli-0.4.1/LICENSE` & `lungo_cli-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/README.md` & `lungo_cli-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/pyproject.toml` & `lungo_cli-0.4.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 120
 
 [tool.poetry]
 name = "lungo-cli"
-version = "0.4.1"
+version = "0.4.2"
 description = "A user-friendly home lab setup designed for small-to-mid-scale on-premises hosting."
 authors = ["raymond-u <36328498+raymond-u@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/raymond-u/lungo"
 documentation = "https://raymond-u.github.io/lungo/"
 keywords = ["homelab", "self-host"]
 packages = [{ include = "lungo_cli", from = "src" }]
@@ -17,27 +17,27 @@
 aenum = "^3.1.15"
 cryptography = "^42.0.7"
 jinja2 = "^3.1.4"
 packaging = "^24.0"
 platformdirs = "^4.2.2"
 pydantic = { extras = ["email"], version = "^2.7.1" }
 pydantic-yaml = "^1.3.0"
-requests = "^2.31.0"
+requests = "^2.32.2"
 typer = "^0.12.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.4.2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mike = "^2.1.1"
 mkdocs-glightbox = "^0.4.0"
-mkdocs-material = "^9.5.23"
+mkdocs-material = "^9.5.24"
 mkdocs-typer = "^0.0.3"
 
 [tool.poetry.scripts]
 lungo = "lungo_cli.app.main:app_wrapper"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `lungo_cli-0.4.1/src/lungo_cli/app/main.py` & `lungo_cli-0.4.2/src/lungo_cli/app/main.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/app/state.py` & `lungo_cli-0.4.2/src/lungo_cli/app/state.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/commands/base.py` & `lungo_cli-0.4.2/src/lungo_cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/commands/down.py` & `lungo_cli-0.4.2/src/lungo_cli/commands/down.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/commands/install.py` & `lungo_cli-0.4.2/src/lungo_cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/commands/list.py` & `lungo_cli-0.4.2/src/lungo_cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/commands/uninstall.py` & `lungo_cli-0.4.2/src/lungo_cli/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/commands/up.py` & `lungo_cli-0.4.2/src/lungo_cli/commands/up.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/core/app.py` & `lungo_cli-0.4.2/src/lungo_cli/core/app.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/core/console.py` & `lungo_cli-0.4.2/src/lungo_cli/core/console.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/core/constants.py` & `lungo_cli-0.4.2/src/lungo_cli/core/constants.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/core/container.py` & `lungo_cli-0.4.2/src/lungo_cli/core/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import subprocess
 from os import PathLike
 
 from typer import Exit
 
-from .console import Console
+from .console import Console, LogLevels
 from .constants import APP_NAME_CAPITALIZED, DOCKER_COMPOSE_URL, DOCKER_URL, PODMAN_COMPOSE_URL, PODMAN_URL
 from .context import ContextManager
 from .file import FileUtils
 from .storage import Storage
 from ..helpers.common import program_exists
 from ..helpers.format import format_command, format_link, format_program
 from ..models.base import EApp, EContainer, ECoreService
@@ -37,23 +37,26 @@
     def set_preferred_tool(self, tool: EContainer | None) -> None:
         self.preferred_tool = tool
 
     def run_shell_command(self, *command: str, cwd: str | PathLike[str] | None = None) -> None:
         command = list(filter(None, command))
 
         try:
-            if self.context_manager.dev:
+            if self.console.log_level < LogLevels.INFO:
                 with subprocess.Popen(
                     command,
                     stdout=subprocess.PIPE,
                     stderr=subprocess.STDOUT,
                     cwd=cwd or self.storage.bundled_dir,
                 ) as process:
                     for line in process.stdout:
-                        self.console.print(line.decode("utf8"))
+                        self.console.print(line.decode(), end="")
+
+                if process.returncode != 0:
+                    raise subprocess.CalledProcessError(process.returncode, command)
             else:
                 subprocess.run(
                     command,
                     stdout=subprocess.DEVNULL,
                     stderr=subprocess.DEVNULL,
                     cwd=cwd or self.storage.bundled_dir,
                     check=True,
```

### Comparing `lungo_cli-0.4.1/src/lungo_cli/core/context.py` & `lungo_cli-0.4.2/src/lungo_cli/core/context.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/core/database.py` & `lungo_cli-0.4.2/src/lungo_cli/core/database.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/core/file.py` & `lungo_cli-0.4.2/src/lungo_cli/core/file.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/core/network.py` & `lungo_cli-0.4.2/src/lungo_cli/core/network.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/core/plugin.py` & `lungo_cli-0.4.2/src/lungo_cli/core/plugin.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/core/renderer.py` & `lungo_cli-0.4.2/src/lungo_cli/core/renderer.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/core/storage.py` & `lungo_cli-0.4.2/src/lungo_cli/core/storage.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/helpers/common.py` & `lungo_cli-0.4.2/src/lungo_cli/helpers/common.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/helpers/crypto.py` & `lungo_cli-0.4.2/src/lungo_cli/helpers/crypto.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/helpers/format.py` & `lungo_cli-0.4.2/src/lungo_cli/helpers/format.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/models/base.py` & `lungo_cli-0.4.2/src/lungo_cli/models/base.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/models/config.py` & `lungo_cli-0.4.2/src/lungo_cli/models/config.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/models/context.py` & `lungo_cli-0.4.2/src/lungo_cli/models/context.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/models/plugin.py` & `lungo_cli-0.4.2/src/lungo_cli/models/plugin.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/models/users.py` & `lungo_cli-0.4.2/src/lungo_cli/models/users.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/Dockerfile.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/compose/compose.yaml.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/compose/compose.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/config/config_export.yaml.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/config/config_export.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/config/users_export.yaml.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/config/users_export.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/nginx/site.conf.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/nginx/site.conf.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/oathkeeper/access_rules.yaml.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/oathkeeper/access_rules.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/plugin.py` & `lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 from lungo_cli.core.plugin import BasePlugin, BaseSettings, PluginManifest
 
 
 class Plugin(BasePlugin[BaseSettings]):
     manifest = PluginManifest(
         name="filebrowser",
-        version="0.2.0",
+        version="0.2.1",
         descriptive_name="File Browser",
         description="File Browser as a Lungo plugin.",
         compatible_with="~=0.4.0",
         have_backend=True,
         backend_port=80,
         require_account=True,
         web_icon="icons/FolderOutline.svelte",
         web_alt_icon="icons/FolderSolid.svelte",
     )
 
     @override
     def get_custom_rendering_context(self) -> dict[str, Any]:
         return {
             "filebrowser_default_password_hash": "$2a$10$aulj1r/ROe0VnA1iE2/ojOItBBFeHK0KLMv5mnl3ECXfiNLKfcKHi",
-            "filebrowser_version": "v2.27.0",
+            "filebrowser_version": "v2.30.0",
         }
```

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderOutline.svelte` & `lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderOutline.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderSolid.svelte` & `lungo_cli-0.4.2/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderSolid.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/Dockerfile.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/compose/compose.yaml.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/compose/compose.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/config/config.py.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/config/config.py.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/nginx/site.conf.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/nginx/site.conf.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/plugin.py` & `lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class Settings(BaseSettings):
     password: str | None = None
 
 
 class Plugin(BasePlugin[Settings]):
     manifest = PluginManifest(
         name="jupyterhub",
-        version="0.2.0",
+        version="0.2.1",
         descriptive_name="JupyterHub",
         description="JupyterHub as a Lungo plugin.",
         compatible_with="~=0.4.0",
         have_backend=True,
         backend_port=80,
         require_account=True,
         web_icon="icons/Jupyter.svelte",
@@ -36,15 +36,15 @@
         return Settings
 
     @override
     def get_custom_rendering_context(self) -> dict[str, Any]:
         return {
             "jupyterhub_password": self.settings.password or self.file_utils.read_text(self.password_file),
             "jupyterhub_version": "4.1.5",
-            "jupyterlab_version": "4.2.0",
+            "jupyterlab_version": "4.2.1",
         }
 
     @override
     def on_plugin_initialization(self) -> None:
         if not self.cookie_secret_file.is_file():
             self.console.print_info("Generating JupyterHub cookie secret...")
             self.file_utils.write_text(self.cookie_secret_file, generate_random_hex(), True)
```

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/web/lib/icons/Jupyter.svelte` & `lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/web/lib/icons/Jupyter.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/jupyterhub/web/routes/+layout.server.ts` & `lungo_cli-0.4.2/src/lungo_cli/plugins/jupyterhub/web/routes/+layout.server.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/compose/compose.yaml.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/compose/compose.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/config/conf.php.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/config/conf.php.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/config/site.conf.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/config/site.conf.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/nginx/site.conf.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/nginx/site.conf.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/oathkeeper/access_rules.yaml.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/oathkeeper/access_rules.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/plugin.py` & `lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/plugin.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteOutline.svelte` & `lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteOutline.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteSolid.svelte` & `lungo_cli-0.4.2/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteSolid.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/Dockerfile.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/compose/compose.yaml.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/compose/compose.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/nginx/site.conf.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/nginx/site.conf.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/plugin.py` & `lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/plugin.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioOutline.svelte` & `lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioOutline.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioSolid.svelte` & `lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioSolid.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/rstudio/web/routes/+layout.server.ts` & `lungo_cli-0.4.2/src/lungo_cli/plugins/rstudio/web/routes/+layout.server.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/rustdesk/compose/compose.yaml.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/rustdesk/compose/compose.yaml.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -28,8 +28,12 @@
 
     environment:
       - ENCRYPTED_ONLY=1
       - KEY_PRIV={{ plugin.custom.rustdesk_private_key }}
       - KEY_PUB={{ plugin.custom.rustdesk_public_key }}
       - RELAY={{ local_ip }}:21117
 
+      - LIMIT_SPEED=838860800
+      - SINGLE_BANDWIDTH=838860800
+      - TOTAL_BANDWIDTH=838860800
+
     restart: 'unless-stopped'
```

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/rustdesk/plugin.py` & `lungo_cli-0.4.2/src/lungo_cli/plugins/rustdesk/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from lungo_cli.core.plugin import BasePlugin, BaseSettings, PluginManifest
 from lungo_cli.helpers.crypto import generate_raw_ed25519_keypair
 
 
 class Plugin(BasePlugin[BaseSettings]):
     manifest = PluginManifest(
         name="rustdesk",
-        version="0.1.0",
+        version="0.1.1",
         descriptive_name="RustDesk",
         description="RustDesk as a Lungo plugin.",
         compatible_with="~=0.4.0",
         have_backend=True,
         backend_host_ports=[21115, 21116, 21117],
         require_account=False,
         web_icon="icons/Rustdesk.svelte",
@@ -28,15 +28,15 @@
         return self.storage.generated_dir / self.manifest.name / "id_ed25519.pub"
 
     @override
     def get_custom_rendering_context(self) -> dict[str, Any]:
         return {
             "rustdesk_private_key": self.file_utils.read_text(self.private_key_file),
             "rustdesk_public_key": self.file_utils.read_text(self.public_key_file),
-            "rustdesk_server_version": "1.1.10-3",
+            "rustdesk_server_version": "1.1.11-1",
         }
 
     @override
     def on_plugin_initialization(self) -> None:
         if not self.private_key_file.is_file() or not self.public_key_file.is_file():
             self.console.print_info("Generating RustDesk keypair...")
```

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/rustdesk/web/lib/icons/Rustdesk.svelte` & `lungo_cli-0.4.2/src/lungo_cli/plugins/rustdesk/web/lib/icons/Rustdesk.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/rustdesk/web/lib/icons/ScreenCast.svelte` & `lungo_cli-0.4.2/src/lungo_cli/plugins/rustdesk/web/lib/icons/ScreenCast.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/rustdesk/web/routes/+page.svelte` & `lungo_cli-0.4.2/src/lungo_cli/plugins/rustdesk/web/routes/+page.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/stirlingpdf/compose/compose.yaml.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/stirlingpdf/compose/compose.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/stirlingpdf/nginx/site.conf.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/stirlingpdf/nginx/site.conf.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/stirlingpdf/plugin.py` & `lungo_cli-0.4.2/src/lungo_cli/plugins/stirlingpdf/plugin.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/stirlingpdf/web/lib/icons/StirlingPdf.svelte` & `lungo_cli-0.4.2/src/lungo_cli/plugins/stirlingpdf/web/lib/icons/StirlingPdf.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/xray/README.md` & `lungo_cli-0.4.2/src/lungo_cli/plugins/xray/README.md`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/xray/compose/compose.yaml.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/xray/compose/compose.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/xray/config/config.json.jinja` & `lungo_cli-0.4.2/src/lungo_cli/plugins/xray/config/config.json.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/xray/plugin.py` & `lungo_cli-0.4.2/src/lungo_cli/plugins/xray/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     domain_suffix_whitelist: list[str] = []
     ip_range_whitelist: list[IPv4Network] = []
 
 
 class Plugin(BasePlugin[Settings]):
     manifest = PluginManifest(
         name="xray",
-        version="0.2.0",
+        version="0.2.1",
         descriptive_name="Xray",
         description="Xray as a Lungo plugin.",
         compatible_with="~=0.4.0",
         have_backend=True,
         backend_port=80,
         require_account=True,
         web_icon="icons/ProxyOutline.svelte",
@@ -41,15 +41,15 @@
         salt = UUID(self.file_utils.read_text(self.salt_file))
 
         return {
             "xray_accounts": [
                 (account.email, uuid5(salt, account.username)) for account in self.context_manager.users.accounts
             ],
             "xray_salt": salt,
-            "xray_version": "1.8.11",
+            "xray_version": "1.8.13",
         }
 
     @override
     def on_plugin_initialization(self) -> None:
         if not self.salt_file.is_file():
             self.console.print_info("Generating Xray salt...")
             self.file_utils.write_text(self.salt_file, str(uuid1()), True)
```

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/xray/web/lib/components/CodeBlock.svelte` & `lungo_cli-0.4.2/src/lungo_cli/plugins/xray/web/lib/components/CodeBlock.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/xray/web/lib/icons/NetworkLock.svelte` & `lungo_cli-0.4.2/src/lungo_cli/plugins/xray/web/lib/icons/NetworkLock.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/xray/web/lib/icons/ProxyOutline.svelte` & `lungo_cli-0.4.2/src/lungo_cli/plugins/xray/web/lib/icons/ProxyOutline.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/xray/web/lib/icons/ProxySolid.svelte` & `lungo_cli-0.4.2/src/lungo_cli/plugins/xray/web/lib/icons/ProxySolid.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/xray/web/routes/+page.server.ts` & `lungo_cli-0.4.2/src/lungo_cli/plugins/xray/web/routes/+page.server.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/plugins/xray/web/routes/+page.svelte` & `lungo_cli-0.4.2/src/lungo_cli/plugins/xray/web/routes/+page.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/assets/config_references/config.yaml` & `lungo_cli-0.4.2/src/lungo_cli/resources/assets/config_references/config.yaml`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/assets/config_references/users.yaml` & `lungo_cli-0.4.2/src/lungo_cli/resources/assets/config_references/users.yaml`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/compose.yaml.jinja` & `lungo_cli-0.4.2/src/lungo_cli/resources/compose.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/config/kratos/config.yaml.jinja` & `lungo_cli-0.4.2/src/lungo_cli/resources/config/kratos/config.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.body.gotmpl.jinja` & `lungo_cli-0.4.2/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.body.gotmpl.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.gotmpl.jinja` & `lungo_cli-0.4.2/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.gotmpl.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/config/kratos/user.schema.json` & `lungo_cli-0.4.2/src/lungo_cli/resources/config/kratos/user.schema.json`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx/conf.d/default.conf.jinja` & `lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx/conf.d/default.conf.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx/sites/oathkeeper.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx/sites/oathkeeper.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx/snippets/auth.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx/snippets/auth.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx/snippets/proxy.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx/snippets/proxy.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx/snippets/upstreams.conf.jinja` & `lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx/snippets/upstreams.conf.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx_gateway/conf.d/default.conf.jinja` & `lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx_gateway/conf.d/default.conf.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx_gateway/snippets/proxy.conf.jinja` & `lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx_gateway/snippets/proxy.conf.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/config/nginx_gateway/snippets/rate_limiting.conf.jinja` & `lungo_cli-0.4.2/src/lungo_cli/resources/config/nginx_gateway/snippets/rate_limiting.conf.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/config/oathkeeper/access_rules.yaml.jinja` & `lungo_cli-0.4.2/src/lungo_cli/resources/config/oathkeeper/access_rules.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/config/oathkeeper/config.yaml.jinja` & `lungo_cli-0.4.2/src/lungo_cli/resources/config/oathkeeper/config.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/dockerfiles/kratos_admin/compose.yaml.jinja` & `lungo_cli-0.4.2/src/lungo_cli/resources/dockerfiles/kratos_admin/compose.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/dockerfiles/nginx.Dockerfile.jinja` & `lungo_cli-0.4.2/src/lungo_cli/resources/dockerfiles/nginx.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/.gitattributes` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/.gitattributes`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CONTRIBUTING.md` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/auto-merge.yml` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/auto-merge.yml`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/server.yml` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/server.yml`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/CHANGELOG.md` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/LICENSE.txt` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/README.md` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/README.md`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/.default.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/.default.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/no-ssl.default.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/no-ssl.default.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/example.com.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/example.com.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/no-ssl.example.com.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/no-ssl.example.com.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/requests.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/requests.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/resource_timing.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/resource_timing.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/security_file_access.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/security_file_access.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_filename-based_cache_busting.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_filename-based_cache_busting.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_svgz-compression.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_svgz-compression.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/character_encodings.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/character_encodings.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/media_types.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/media_types.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/content-security-policy.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/content-security-policy.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/cross-origin-policy.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/cross-origin-policy.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/permissions-policy.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/permissions-policy.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/referrer-policy.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/referrer-policy.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/strict-transport-security.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/strict-transport-security.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-content-type-options.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-content-type-options.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-frame-options.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-frame-options.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/certificate_files.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/certificate_files.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ocsp_stapling.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ocsp_stapling.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_balanced.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_balanced.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_strict.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_strict.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ssl_engine.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ssl_engine.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-control.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-control.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-file-descriptors.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-file-descriptors.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache_expiration.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache_expiration.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/compression.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/compression.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/content_transformation.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/content_transformation.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_brotli.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_brotli.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_gzip.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_gzip.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/mime.types` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/mime.types`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/nginx.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/secure.server.localhost.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/secure.server.localhost.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/server.localhost.conf` & `lungo_cli-0.4.2/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/server.localhost.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/.eslintrc.cjs` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/.eslintrc.cjs`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/Dockerfile.jinja` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/assets/schemas/keto.openapi.json` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/assets/schemas/keto.openapi.json`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/assets/schemas/kratos.openapi.json` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/assets/schemas/kratos.openapi.json`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/package.json` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9818376068376069%*

 * *Differences: {"'dependencies'": "{'openapi-fetch': '^0.9.7'}",*

 * * "'devDependencies'": "{'@sveltejs/kit': '^2.5.10', '@typescript-eslint/eslint-plugin': '^7.10.0', "*

 * *                      "'@typescript-eslint/parser': '^7.10.0', 'openapi-typescript': '^6.7.6'}"}*

```diff
@@ -1,28 +1,28 @@
 {
     "dependencies": {
-        "openapi-fetch": "^0.9.5",
+        "openapi-fetch": "^0.9.7",
         "set-cookie-parser": "^2.6.0"
     },
     "devDependencies": {
         "@sveltejs/adapter-node": "^5.0.1",
         "@sveltejs/enhanced-img": "^0.2.0",
-        "@sveltejs/kit": "^2.5.8",
+        "@sveltejs/kit": "^2.5.10",
         "@sveltejs/vite-plugin-svelte": "^3.1.0",
         "@tailwindcss/typography": "^0.5.13",
         "@types/set-cookie-parser": "^2.4.7",
-        "@typescript-eslint/eslint-plugin": "^7.9.0",
-        "@typescript-eslint/parser": "^7.9.0",
+        "@typescript-eslint/eslint-plugin": "^7.10.0",
+        "@typescript-eslint/parser": "^7.10.0",
         "autoprefixer": "^10.4.19",
         "daisyui": "^4.11.1",
         "eslint": "^8.57.0",
         "eslint-config-prettier": "^9.1.0",
         "eslint-plugin-svelte": "^2.39.0",
         "json-schema-to-typescript": "^14.0.4",
-        "openapi-typescript": "^6.7.5",
+        "openapi-typescript": "^6.7.6",
         "postcss": "^8.4.38",
         "postcss-load-config": "^4.0.2",
         "prettier": "^3.2.5",
         "prettier-plugin-svelte": "^3.2.3",
         "prettier-plugin-tailwindcss": "^0.5.14",
         "svelte": "^4.2.17",
         "svelte-check": "^3.7.1",
```

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/pnpm-lock.yaml` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/pnpm-lock.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -2,45 +2,45 @@
 
 settings:
   autoInstallPeers: true
   excludeLinksFromLockfile: false
 
 dependencies:
   openapi-fetch:
-    specifier: ^0.9.5
-    version: 0.9.5
+    specifier: ^0.9.7
+    version: 0.9.7
   set-cookie-parser:
     specifier: ^2.6.0
     version: 2.6.0
 
 devDependencies:
   '@sveltejs/adapter-node':
     specifier: ^5.0.1
-    version: 5.0.1(@sveltejs/kit@2.5.8)
+    version: 5.0.1(@sveltejs/kit@2.5.10)
   '@sveltejs/enhanced-img':
     specifier: ^0.2.0
     version: 0.2.0(svelte@4.2.17)
   '@sveltejs/kit':
-    specifier: ^2.5.8
-    version: 2.5.8(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.17)(vite@5.2.11)
+    specifier: ^2.5.10
+    version: 2.5.10(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.17)(vite@5.2.11)
   '@sveltejs/vite-plugin-svelte':
     specifier: ^3.1.0
     version: 3.1.0(svelte@4.2.17)(vite@5.2.11)
   '@tailwindcss/typography':
     specifier: ^0.5.13
     version: 0.5.13(tailwindcss@3.4.3)
   '@types/set-cookie-parser':
     specifier: ^2.4.7
     version: 2.4.7
   '@typescript-eslint/eslint-plugin':
-    specifier: ^7.9.0
-    version: 7.9.0(@typescript-eslint/parser@7.9.0)(eslint@8.57.0)(typescript@5.4.5)
+    specifier: ^7.10.0
+    version: 7.10.0(@typescript-eslint/parser@7.10.0)(eslint@8.57.0)(typescript@5.4.5)
   '@typescript-eslint/parser':
-    specifier: ^7.9.0
-    version: 7.9.0(eslint@8.57.0)(typescript@5.4.5)
+    specifier: ^7.10.0
+    version: 7.10.0(eslint@8.57.0)(typescript@5.4.5)
   autoprefixer:
     specifier: ^10.4.19
     version: 10.4.19(postcss@8.4.38)
   daisyui:
     specifier: ^4.11.1
     version: 4.11.1(postcss@8.4.38)
   eslint:
@@ -52,16 +52,16 @@
   eslint-plugin-svelte:
     specifier: ^2.39.0
     version: 2.39.0(eslint@8.57.0)(svelte@4.2.17)
   json-schema-to-typescript:
     specifier: ^14.0.4
     version: 14.0.4
   openapi-typescript:
-    specifier: ^6.7.5
-    version: 6.7.5
+    specifier: ^6.7.6
+    version: 6.7.6
   postcss:
     specifier: ^8.4.38
     version: 8.4.38
   postcss-load-config:
     specifier: ^4.0.2
     version: 4.0.2(postcss@8.4.38)
   prettier:
@@ -117,16 +117,16 @@
     engines: {node: '>= 16'}
     dependencies:
       '@jsdevtools/ono': 7.1.3
       '@types/json-schema': 7.0.15
       js-yaml: 4.1.0
     dev: true
 
-  /@emnapi/runtime@1.1.1:
-    resolution: {integrity: sha512-3bfqkzuR1KLx57nZfjr2NLnFOobvyS0aTszaEGCGqmYMVDRaGvgIZbjGSV/MHSSmLgQ/b9JFHQ5xm5WRZYd+XQ==}
+  /@emnapi/runtime@1.2.0:
+    resolution: {integrity: sha512-bV21/9LQmcQeCPEg3BDFtvwL6cwiTMksYNWQQ4KOxCZikEGalWtenoZ0wCiukJINlGCIi2KXx01g4FoH/LxpzQ==}
     requiresBuild: true
     dependencies:
       tslib: 2.6.2
     dev: true
     optional: true
 
   /@esbuild/aix-ppc64@0.20.2:
@@ -369,16 +369,16 @@
     dev: true
 
   /@eslint/js@8.57.0:
     resolution: {integrity: sha512-Ys+3g2TaW7gADOJzPt83SJtCDhMjndcDMFVQ/Tj9iA1BfJzFKD9mAUXT3OenpuPHbI6P/myECxRJrofUsDx/5g==}
     engines: {node: ^12.22.0 || ^14.17.0 || >=16.0.0}
     dev: true
 
-  /@fastify/busboy@2.1.0:
-    resolution: {integrity: sha512-+KpH+QxZU7O4675t3mnkQKcZZg56u+K/Ct2K+N2AZYNVK8kyeo/bI18tI8aPm3tvNNRyTWfj6s5tnGNlcbQRsA==}
+  /@fastify/busboy@2.1.1:
+    resolution: {integrity: sha512-vBZP4NlzfOlerQTnba4aqZoMhE/a9HY7HRqoOPaETQcSQuWEIyZMHGfVu6w9wGtGK5fED5qRs2DteVCjOH60sA==}
     engines: {node: '>=14'}
     dev: true
 
   /@humanwhocodes/config-array@0.11.14:
     resolution: {integrity: sha512-3T8LkOmg45BV5FICb15QQMsyUSWrQ8AygVfC7ZG32zOalnqrilm018ZVCw0eapXux8FtA33q8PSRSstjee3jSg==}
     engines: {node: '>=10.10.0'}
     dependencies:
@@ -560,15 +560,15 @@
 
   /@img/sharp-wasm32@0.33.3:
     resolution: {integrity: sha512-68zivsdJ0koE96stdUfM+gmyaK/NcoSZK5dV5CAjES0FUXS9lchYt8LAB5rTbM7nlWtxaU/2GON0HVN6/ZYJAQ==}
     engines: {node: ^18.17.0 || ^20.3.0 || >=21.0.0, npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
     cpu: [wasm32]
     requiresBuild: true
     dependencies:
-      '@emnapi/runtime': 1.1.1
+      '@emnapi/runtime': 1.2.0
     dev: true
     optional: true
 
   /@img/sharp-win32-ia32@0.33.3:
     resolution: {integrity: sha512-CyimAduT2whQD8ER4Ux7exKrtfoaUiVr7HG0zZvO0XTFn2idUWljjxv58GxNTkFb8/J9Ub9AqITGkJD6ZginxQ==}
     engines: {node: ^18.17.0 || ^20.3.0 || >=21.0.0, npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
     cpu: [ia32]
@@ -948,53 +948,53 @@
     resolution: {integrity: sha512-aGg7iToJjdklmxlUlJh/PaPNa4PmqHfyRMLunbL3eaMO0gp656+q1zOKkpJ/CVe9CryJv6tAN1HDoR8cNGzkag==}
     cpu: [x64]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@sveltejs/adapter-node@5.0.1(@sveltejs/kit@2.5.8):
+  /@sveltejs/adapter-node@5.0.1(@sveltejs/kit@2.5.10):
     resolution: {integrity: sha512-eYdmxdUWMW+dad1JfMsWBPY2vjXz9eE+52A2AQnXPScPJlIxIVk5mmbaEEzrZivLfO2wEcLTZ5vdC03W69x+iA==}
     peerDependencies:
       '@sveltejs/kit': ^2.4.0
     dependencies:
       '@rollup/plugin-commonjs': 25.0.7(rollup@4.12.0)
       '@rollup/plugin-json': 6.1.0(rollup@4.12.0)
       '@rollup/plugin-node-resolve': 15.2.3(rollup@4.12.0)
-      '@sveltejs/kit': 2.5.8(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.17)(vite@5.2.11)
+      '@sveltejs/kit': 2.5.10(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.17)(vite@5.2.11)
       rollup: 4.12.0
     dev: true
 
   /@sveltejs/enhanced-img@0.2.0(svelte@4.2.17):
     resolution: {integrity: sha512-W6wG0RxQYoL13LmUl8IBHeQatMXSd2ybrjg/WQuE5EoIJq+wUkf1hUDaMp9PHe4ubpnzWK/c0QaE5Ls+zjHimA==}
     dependencies:
       magic-string: 0.30.8
       svelte-parse-markup: 0.1.2(svelte@4.2.17)
       vite-imagetools: 7.0.1
     transitivePeerDependencies:
       - rollup
       - svelte
     dev: true
 
-  /@sveltejs/kit@2.5.8(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.17)(vite@5.2.11):
-    resolution: {integrity: sha512-ZQXYaVHd1p0kDGwOi4l82i5kAiUQtrhMthDKtJi0zVzmNupKJ0ZlBVAoceuarCuIntPNctyQchW29h5DkFxd1Q==}
+  /@sveltejs/kit@2.5.10(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.17)(vite@5.2.11):
+    resolution: {integrity: sha512-OqoyTmFG2cYmCFAdBfW+Qxbg8m23H4dv6KqwEt7ofr/ROcfcIl3Z/VT56L22H9f0uNZyr+9Bs1eh2gedOCK9kA==}
     engines: {node: '>=18.13'}
     hasBin: true
     requiresBuild: true
     peerDependencies:
       '@sveltejs/vite-plugin-svelte': ^3.0.0
       svelte: ^4.0.0 || ^5.0.0-next.0
       vite: ^5.0.3
     dependencies:
       '@sveltejs/vite-plugin-svelte': 3.1.0(svelte@4.2.17)(vite@5.2.11)
       '@types/cookie': 0.6.0
       cookie: 0.6.0
       devalue: 5.0.0
       esm-env: 1.0.0
-      import-meta-resolve: 4.0.0
+      import-meta-resolve: 4.1.0
       kleur: 4.1.5
       magic-string: 0.30.5
       mrmime: 2.0.0
       sade: 1.8.1
       set-cookie-parser: 2.6.0
       sirv: 2.0.4
       svelte: 4.2.17
@@ -1082,138 +1082,138 @@
 
   /@types/set-cookie-parser@2.4.7:
     resolution: {integrity: sha512-+ge/loa0oTozxip6zmhRIk8Z/boU51wl9Q6QdLZcokIGMzY5lFXYy/x7Htj2HTC6/KZP1hUbZ1ekx8DYXICvWg==}
     dependencies:
       '@types/node': 20.9.0
     dev: true
 
-  /@typescript-eslint/eslint-plugin@7.9.0(@typescript-eslint/parser@7.9.0)(eslint@8.57.0)(typescript@5.4.5):
-    resolution: {integrity: sha512-6e+X0X3sFe/G/54aC3jt0txuMTURqLyekmEHViqyA2VnxhLMpvA6nqmcjIy+Cr9tLDHPssA74BP5Mx9HQIxBEA==}
+  /@typescript-eslint/eslint-plugin@7.10.0(@typescript-eslint/parser@7.10.0)(eslint@8.57.0)(typescript@5.4.5):
+    resolution: {integrity: sha512-PzCr+a/KAef5ZawX7nbyNwBDtM1HdLIT53aSA2DDlxmxMngZ43O8SIePOeX8H5S+FHXeI6t97mTt/dDdzY4Fyw==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       '@typescript-eslint/parser': ^7.0.0
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
       '@eslint-community/regexpp': 4.10.0
-      '@typescript-eslint/parser': 7.9.0(eslint@8.57.0)(typescript@5.4.5)
-      '@typescript-eslint/scope-manager': 7.9.0
-      '@typescript-eslint/type-utils': 7.9.0(eslint@8.57.0)(typescript@5.4.5)
-      '@typescript-eslint/utils': 7.9.0(eslint@8.57.0)(typescript@5.4.5)
-      '@typescript-eslint/visitor-keys': 7.9.0
+      '@typescript-eslint/parser': 7.10.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/scope-manager': 7.10.0
+      '@typescript-eslint/type-utils': 7.10.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/utils': 7.10.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/visitor-keys': 7.10.0
       eslint: 8.57.0
       graphemer: 1.4.0
       ignore: 5.3.1
       natural-compare: 1.4.0
       ts-api-utils: 1.3.0(typescript@5.4.5)
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/parser@7.9.0(eslint@8.57.0)(typescript@5.4.5):
-    resolution: {integrity: sha512-qHMJfkL5qvgQB2aLvhUSXxbK7OLnDkwPzFalg458pxQgfxKDfT1ZDbHQM/I6mDIf/svlMkj21kzKuQ2ixJlatQ==}
+  /@typescript-eslint/parser@7.10.0(eslint@8.57.0)(typescript@5.4.5):
+    resolution: {integrity: sha512-2EjZMA0LUW5V5tGQiaa2Gys+nKdfrn2xiTIBLR4fxmPmVSvgPcKNW+AE/ln9k0A4zDUti0J/GZXMDupQoI+e1w==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
-      '@typescript-eslint/scope-manager': 7.9.0
-      '@typescript-eslint/types': 7.9.0
-      '@typescript-eslint/typescript-estree': 7.9.0(typescript@5.4.5)
-      '@typescript-eslint/visitor-keys': 7.9.0
+      '@typescript-eslint/scope-manager': 7.10.0
+      '@typescript-eslint/types': 7.10.0
+      '@typescript-eslint/typescript-estree': 7.10.0(typescript@5.4.5)
+      '@typescript-eslint/visitor-keys': 7.10.0
       debug: 4.3.4
       eslint: 8.57.0
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/scope-manager@7.9.0:
-    resolution: {integrity: sha512-ZwPK4DeCDxr3GJltRz5iZejPFAAr4Wk3+2WIBaj1L5PYK5RgxExu/Y68FFVclN0y6GGwH8q+KgKRCvaTmFBbgQ==}
+  /@typescript-eslint/scope-manager@7.10.0:
+    resolution: {integrity: sha512-7L01/K8W/VGl7noe2mgH0K7BE29Sq6KAbVmxurj8GGaPDZXPr8EEQ2seOeAS+mEV9DnzxBQB6ax6qQQ5C6P4xg==}
     engines: {node: ^18.18.0 || >=20.0.0}
     dependencies:
-      '@typescript-eslint/types': 7.9.0
-      '@typescript-eslint/visitor-keys': 7.9.0
+      '@typescript-eslint/types': 7.10.0
+      '@typescript-eslint/visitor-keys': 7.10.0
     dev: true
 
-  /@typescript-eslint/type-utils@7.9.0(eslint@8.57.0)(typescript@5.4.5):
-    resolution: {integrity: sha512-6Qy8dfut0PFrFRAZsGzuLoM4hre4gjzWJB6sUvdunCYZsYemTkzZNwF1rnGea326PHPT3zn5Lmg32M/xfJfByA==}
+  /@typescript-eslint/type-utils@7.10.0(eslint@8.57.0)(typescript@5.4.5):
+    resolution: {integrity: sha512-D7tS4WDkJWrVkuzgm90qYw9RdgBcrWmbbRkrLA4d7Pg3w0ttVGDsvYGV19SH8gPR5L7OtcN5J1hTtyenO9xE9g==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
-      '@typescript-eslint/typescript-estree': 7.9.0(typescript@5.4.5)
-      '@typescript-eslint/utils': 7.9.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/typescript-estree': 7.10.0(typescript@5.4.5)
+      '@typescript-eslint/utils': 7.10.0(eslint@8.57.0)(typescript@5.4.5)
       debug: 4.3.4
       eslint: 8.57.0
       ts-api-utils: 1.3.0(typescript@5.4.5)
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/types@7.9.0:
-    resolution: {integrity: sha512-oZQD9HEWQanl9UfsbGVcZ2cGaR0YT5476xfWE0oE5kQa2sNK2frxOlkeacLOTh9po4AlUT5rtkGyYM5kew0z5w==}
+  /@typescript-eslint/types@7.10.0:
+    resolution: {integrity: sha512-7fNj+Ya35aNyhuqrA1E/VayQX9Elwr8NKZ4WueClR3KwJ7Xx9jcCdOrLW04h51de/+gNbyFMs+IDxh5xIwfbNg==}
     engines: {node: ^18.18.0 || >=20.0.0}
     dev: true
 
-  /@typescript-eslint/typescript-estree@7.9.0(typescript@5.4.5):
-    resolution: {integrity: sha512-zBCMCkrb2YjpKV3LA0ZJubtKCDxLttxfdGmwZvTqqWevUPN0FZvSI26FalGFFUZU/9YQK/A4xcQF9o/VVaCKAg==}
+  /@typescript-eslint/typescript-estree@7.10.0(typescript@5.4.5):
+    resolution: {integrity: sha512-LXFnQJjL9XIcxeVfqmNj60YhatpRLt6UhdlFwAkjNc6jSUlK8zQOl1oktAP8PlWFzPQC1jny/8Bai3/HPuvN5g==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
-      '@typescript-eslint/types': 7.9.0
-      '@typescript-eslint/visitor-keys': 7.9.0
+      '@typescript-eslint/types': 7.10.0
+      '@typescript-eslint/visitor-keys': 7.10.0
       debug: 4.3.4
       globby: 11.1.0
       is-glob: 4.0.3
       minimatch: 9.0.4
       semver: 7.6.2
       ts-api-utils: 1.3.0(typescript@5.4.5)
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/utils@7.9.0(eslint@8.57.0)(typescript@5.4.5):
-    resolution: {integrity: sha512-5KVRQCzZajmT4Ep+NEgjXCvjuypVvYHUW7RHlXzNPuak2oWpVoD1jf5xCP0dPAuNIchjC7uQyvbdaSTFaLqSdA==}
+  /@typescript-eslint/utils@7.10.0(eslint@8.57.0)(typescript@5.4.5):
+    resolution: {integrity: sha512-olzif1Fuo8R8m/qKkzJqT7qwy16CzPRWBvERS0uvyc+DHd8AKbO4Jb7kpAvVzMmZm8TrHnI7hvjN4I05zow+tg==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       eslint: ^8.56.0
     dependencies:
       '@eslint-community/eslint-utils': 4.4.0(eslint@8.57.0)
-      '@typescript-eslint/scope-manager': 7.9.0
-      '@typescript-eslint/types': 7.9.0
-      '@typescript-eslint/typescript-estree': 7.9.0(typescript@5.4.5)
+      '@typescript-eslint/scope-manager': 7.10.0
+      '@typescript-eslint/types': 7.10.0
+      '@typescript-eslint/typescript-estree': 7.10.0(typescript@5.4.5)
       eslint: 8.57.0
     transitivePeerDependencies:
       - supports-color
       - typescript
     dev: true
 
-  /@typescript-eslint/visitor-keys@7.9.0:
-    resolution: {integrity: sha512-iESPx2TNLDNGQLyjKhUvIKprlP49XNEK+MvIf9nIO7ZZaZdbnfWKHnXAgufpxqfA0YryH8XToi4+CjBgVnFTSQ==}
+  /@typescript-eslint/visitor-keys@7.10.0:
+    resolution: {integrity: sha512-9ntIVgsi6gg6FIq9xjEO4VQJvwOqA3jaBFQJ/6TK5AvEup2+cECI6Fh7QiBxmfMHXU0V0J4RyPeOU1VDNzl9cg==}
     engines: {node: ^18.18.0 || >=20.0.0}
     dependencies:
-      '@typescript-eslint/types': 7.9.0
+      '@typescript-eslint/types': 7.10.0
       eslint-visitor-keys: 3.4.3
     dev: true
 
   /@ungap/structured-clone@1.2.0:
     resolution: {integrity: sha512-zuVdFrMJiuCDQUMCzQaD6KL28MjnqqN8XnAqiEq9PNm/hCPTSGfrXCOfwj1ow4LFb/tNymJPwsNbVePc1xFqrQ==}
     dev: true
 
@@ -2106,16 +2106,16 @@
     resolution: {integrity: sha512-veYYhQa+D1QBKznvhUHxb8faxlrwUnxseDAbAp457E0wLNio2bOSKnjYDhMj+YiAq61xrMGhQk9iXVk5FzgQMw==}
     engines: {node: '>=6'}
     dependencies:
       parent-module: 1.0.1
       resolve-from: 4.0.0
     dev: true
 
-  /import-meta-resolve@4.0.0:
-    resolution: {integrity: sha512-okYUR7ZQPH+efeuMJGlq4f8ubUgO50kByRPyt/Cy1Io4PSRsPjxME+YlVaCOx+NIToW7hCsZNFJyTPFFKepRSA==}
+  /import-meta-resolve@4.1.0:
+    resolution: {integrity: sha512-I6fiaX09Xivtk+THaMfAwnA3MVA5Big1WHF1Dfx9hFuvNIWpXnorlkzhcQf6ehrqQiiZECRt1poOAkPmer3ruw==}
     dev: true
 
   /imurmurhash@0.1.4:
     resolution: {integrity: sha512-JmXMZ6wuvDmLiHEml9ykzqO6lwFbof0GG4IkcGaENdCRDDmMVnny7s5HsIgHCbaq0w2MyPhDqkhTUgS2LU2PHA==}
     engines: {node: '>=0.8.19'}
     dev: true
 
@@ -2514,33 +2514,33 @@
 
   /once@1.4.0:
     resolution: {integrity: sha512-lNaJgI+2Q5URQBkccEKHTQOPaXdUxnZZElQTZY0MFUAuaEqe1E+Nyvgdz/aIyNi6Z9MzO5dv1H8n58/GELp3+w==}
     dependencies:
       wrappy: 1.0.2
     dev: true
 
-  /openapi-fetch@0.9.5:
-    resolution: {integrity: sha512-ToRnypJB2G5bEUZqJ4mGty/qDVgAZ4BW0znlXQAECxAp4EM8dYtgQ1mrw2Ij6W7knN4VawHvFq8uTqzXyMGNPA==}
+  /openapi-fetch@0.9.7:
+    resolution: {integrity: sha512-NMp/GEmWSGO0b2d731IdGXcMP2PF85Rk1q+oy2Mx/DYMdP3pgTZTRamKxgZpkHhM4iOVsyD1iP5HKL9Fr6CH2Q==}
     dependencies:
       openapi-typescript-helpers: 0.0.8
     dev: false
 
   /openapi-typescript-helpers@0.0.8:
     resolution: {integrity: sha512-1eNjQtbfNi5Z/kFhagDIaIRj6qqDzhjNJKz8cmMW0CVdGwT6e1GLbAfgI0d28VTJa1A8jz82jm/4dG8qNoNS8g==}
     dev: false
 
-  /openapi-typescript@6.7.5:
-    resolution: {integrity: sha512-ZD6dgSZi0u1QCP55g8/2yS5hNJfIpgqsSGHLxxdOjvY7eIrXzj271FJEQw33VwsZ6RCtO/NOuhxa7GBWmEudyA==}
+  /openapi-typescript@6.7.6:
+    resolution: {integrity: sha512-c/hfooPx+RBIOPM09GSxABOZhYPblDoyaGhqBkD/59vtpN21jEuWKDlM0KYTvqJVlSYjKs0tBcIdeXKChlSPtw==}
     hasBin: true
     dependencies:
       ansi-colors: 4.1.3
       fast-glob: 3.3.2
       js-yaml: 4.1.0
       supports-color: 9.4.0
-      undici: 5.28.3
+      undici: 5.28.4
       yargs-parser: 21.1.1
     dev: true
 
   /optionator@0.9.3:
     resolution: {integrity: sha512-JjCoypp+jKn1ttEFExxhetCKeJt9zhAgAve5FXHixTvFDW/5aEktX9bufBKLRRMdU7bNtpLfcGu94B3cdEJgjg==}
     engines: {node: '>= 0.8.0'}
     dependencies:
@@ -3377,19 +3377,19 @@
     hasBin: true
     dev: true
 
   /undici-types@5.26.5:
     resolution: {integrity: sha512-JlCMO+ehdEIKqlFxk6IfVoAUVmgz7cU7zD/h9XZ0qzeosSHmUJVOzSQvvYSYWXkFXC+IfLKSIffhv0sVZup6pA==}
     dev: true
 
-  /undici@5.28.3:
-    resolution: {integrity: sha512-3ItfzbrhDlINjaP0duwnNsKpDQk3acHI3gVJ1z4fmwMK31k5G9OVIAMLSIaP6w4FaGkaAkN6zaQO9LUvZ1t7VA==}
+  /undici@5.28.4:
+    resolution: {integrity: sha512-72RFADWFqKmUb2hmmvNODKL3p9hcB6Gt2DOQMis1SEBaV6a4MH8soBvzg+95CYhCKPFedut2JY9bMfrDl9D23g==}
     engines: {node: '>=14.0'}
     dependencies:
-      '@fastify/busboy': 2.1.0
+      '@fastify/busboy': 2.1.1
     dev: true
 
   /update-browserslist-db@1.0.13(browserslist@4.23.0):
     resolution: {integrity: sha512-xebP81SNcPuNpPP3uzeW1NYXxI3rxyJzF3pD6sH4jE7o/IX+WtSpwnVU+qIsDPyk0d3hmFQ7mjqc6AtV604hbg==}
     hasBin: true
     peerDependencies:
       browserslist: '>= 4.21.0'
```

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/app.pcss` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/app.pcss`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/actions.ts` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/actions.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/assets/cover.jpg` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/assets/cover.jpg`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/AccountDropdown.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/AccountDropdown.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/AppShell.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/AppShell.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/FormBuilder.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/FormBuilder.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/HeroFrame.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/HeroFrame.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/LoadingIndicator.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/LoadingIndicator.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/NavRail.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/NavRail.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/PasswordInput.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/PasswordInput.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/PatchedIFrame.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/PatchedIFrame.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/SwappableIcon.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/SwappableIcon.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/ThemeSelector.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/ThemeSelector.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/ThemeSelectorDropdown.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/ThemeSelectorDropdown.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/components/index.ts` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/components/index.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/Account.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/Account.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/Close.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/Close.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/DarkMode.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/DarkMode.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/Fullscreen.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/Fullscreen.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/LightMode.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/LightMode.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/Logout.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/Logout.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/Menu.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/Menu.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/QuestionMark.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/QuestionMark.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/Reset.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/Reset.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/Settings.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/Settings.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/VisibilityOff.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/VisibilityOff.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/VisibilityOn.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/VisibilityOn.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/icons/index.ts` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/icons/index.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/server/utils/api.ts` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/server/utils/api.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/server/utils/stubs.ts.jinja` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/server/utils/stubs.ts.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/stores.ts` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/stores.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/types/keto.d.ts` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/types/keto.d.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/types/kratos.d.ts` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/types/kratos.d.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/utils/api.ts` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/utils/api.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/utils/common.ts` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/utils/common.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/lib/utils/stubs.ts.jinja` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/lib/utils/stubs.ts.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/(account)/account/+page.server.ts` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/(account)/account/+page.server.ts`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 })
         }
     },
 }
 
 export async function load({ cookies, fetch, request }) {
     const client = createKratosClient(getCookieHeader(request), cookies, fetch)
-    const response = await client.GET("/self-service/settings/browser", { params: {} })
+    const response = await client.GET("/self-service/settings/browser")
 
     switch (response.response.status) {
         case 200:
             return {
                 flow: getFlowId(response.data!.ui.action),
                 messages: response.data!.ui.messages,
                 nodes: response.data!.ui.nodes,
```

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/(account)/login/+page.server.ts` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/(account)/login/+page.server.ts`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                 })
         }
     },
 }
 
 export async function load({ cookies, fetch, request }) {
     const client = createKratosClient(getCookieHeader(request), cookies, fetch)
-    const response = await client.GET("/self-service/login/browser", { params: {} })
+    const response = await client.GET("/self-service/login/browser")
 
     switch (response.response.status) {
         case 200:
             return {
                 flow: getFlowId(response.data!.ui.action),
                 messages: response.data!.ui.messages,
                 nodes: response.data!.ui.nodes,
```

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/(account)/login/+page.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/(account)/login/+page.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.server.ts` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.server.ts`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                 })
         }
     },
 }
 
 export async function load({ cookies, fetch, request }) {
     const client = createKratosClient(getCookieHeader(request), cookies, fetch)
-    const response = await client.GET("/self-service/recovery/browser", { params: {} })
+    const response = await client.GET("/self-service/recovery/browser")
 
     switch (response.response.status) {
         case 200:
             return {
                 flow: getFlowId(response.data!.ui.action),
                 messages: response.data!.ui.messages,
                 nodes: response.data!.ui.nodes,
```

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/(apps)/+page.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/(apps)/+page.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/+error.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/+error.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/+layout.server.ts` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/+layout.server.ts`

 * *Files 8% similar despite different names*

```diff
@@ -28,29 +28,29 @@
     return apps
 }
 
 export async function load({ cookies, fetch, request, url }) {
     const title = url.pathname.split("/").pop() || "home"
 
     const client = createKratosClient(getCookieHeader(request), cookies, fetch)
-    const response = await client.GET("/sessions/whoami", { params: {} })
+    const response = await client.GET("/sessions/whoami")
 
     switch (response.response.status) {
         case 200:
             break
         default:
             return {
                 apps: await getAllowedApps(fetch),
                 logoutToken: undefined,
                 title,
                 userInfo: undefined,
             }
     }
 
-    const response2 = await client.GET("/self-service/logout/browser", { params: {} })
+    const response2 = await client.GET("/self-service/logout/browser")
 
     switch (response2.response.status) {
         case 200:
             return {
                 apps: await getAllowedApps(fetch, (response.data!.identity as User).traits!.username),
                 logoutToken: response2.data!.logout_token,
                 title,
```

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/src/routes/+layout.svelte` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/src/routes/+layout.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/static/favicon.png` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/static/favicon.png`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/tailwind.config.cjs` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/tailwind.config.cjs`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/src/lungo_cli/resources/web/tsconfig.json` & `lungo_cli-0.4.2/src/lungo_cli/resources/web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.4.1/PKG-INFO` & `lungo_cli-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lungo-cli
-Version: 0.4.1
+Version: 0.4.2
 Summary: A user-friendly home lab setup designed for small-to-mid-scale on-premises hosting.
 Home-page: https://github.com/raymond-u/lungo
 Keywords: homelab,self-host
 Author: raymond-u
 Author-email: 36328498+raymond-u@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Requires-Dist: aenum (>=3.1.15,<4.0.0)
 Requires-Dist: cryptography (>=42.0.7,<43.0.0)
 Requires-Dist: jinja2 (>=3.1.4,<4.0.0)
 Requires-Dist: packaging (>=24.0,<25.0)
 Requires-Dist: platformdirs (>=4.2.2,<5.0.0)
 Requires-Dist: pydantic-yaml (>=1.3.0,<2.0.0)
 Requires-Dist: pydantic[email] (>=2.7.1,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2.32.2,<3.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Project-URL: Documentation, https://raymond-u.github.io/lungo/
 Project-URL: Repository, https://github.com/raymond-u/lungo
 Description-Content-Type: text/markdown
 
 <br>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: lungo-cli Version: 0.4.1 Summary: A user-friendly
+Metadata-Version: 2.1 Name: lungo-cli Version: 0.4.2 Summary: A user-friendly
 home lab setup designed for small-to-mid-scale on-premises hosting. Home-page:
 https://github.com/raymond-u/lungo Keywords: homelab,self-host Author: raymond-
 u Author-email: 36328498+raymond-u@users.noreply.github.com Requires-Python:
 >=3.12,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: aenum (>=3.1.15,<4.0.0)
 Requires-Dist: cryptography (>=42.0.7,<43.0.0) Requires-Dist: jinja2
 (>=3.1.4,<4.0.0) Requires-Dist: packaging (>=24.0,<25.0) Requires-Dist:
 platformdirs (>=4.2.2,<5.0.0) Requires-Dist: pydantic-yaml (>=1.3.0,<2.0.0)
 Requires-Dist: pydantic[email] (>=2.7.1,<3.0.0) Requires-Dist: requests
-(>=2.31.0,<3.0.0) Requires-Dist: typer (>=0.12.3,<0.13.0) Project-URL:
+(>=2.32.2,<3.0.0) Requires-Dist: typer (>=0.12.3,<0.13.0) Project-URL:
 Documentation, https://raymond-u.github.io/lungo/ Project-URL: Repository,
 https://github.com/raymond-u/lungo Description-Content-Type: text/markdown
                                 ************ _[[_LL_uu_nn_gg_oo_]]
                                      LLuunnggoo
                                      ************
   A user-friendly home lab setup designed for small-to-mid-scale on-premises
                                    hosting.
```

