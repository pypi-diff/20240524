# Comparing `tmp/langserve-0.2.0rc1.tar.gz` & `tmp/langserve-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langserve-0.2.0rc1.tar", max compression
+gzip compressed data, was "langserve-0.2.1.tar", max compression
```

## Comparing `langserve-0.2.0rc1.tar` & `langserve-0.2.1.tar`

### file list

```diff
@@ -1,145 +1,145 @@
--rw-r--r--   0        0        0     3757 2024-05-15 20:31:12.045390 langserve-0.2.0rc1/LICENSE
--rw-r--r--   0        0        0    38879 2024-05-15 20:31:12.049390 langserve-0.2.0rc1/README.md
--rw-r--r--   0        0        0      505 2024-05-15 20:31:12.053390 langserve-0.2.0rc1/langserve/__init__.py
--rw-r--r--   0        0        0    64386 2024-05-15 20:31:12.053390 langserve-0.2.0rc1/langserve/api_handler.py
--rw-r--r--   0        0        0    14240 2024-05-15 20:31:12.053390 langserve-0.2.0rc1/langserve/callbacks.py
--rw-r--r--   0        0        0      436 2024-05-15 20:31:12.053390 langserve-0.2.0rc1/langserve/chat_playground/.eslintrc.cjs
--rw-r--r--   0        0        0      266 2024-05-15 20:31:12.053390 langserve-0.2.0rc1/langserve/chat_playground/.gitignore
--rw-r--r--   0        0        0     1263 2024-05-15 20:31:12.053390 langserve-0.2.0rc1/langserve/chat_playground/README.md
--rw-r--r--   0        0        0    23810 2024-05-15 20:31:12.053390 langserve-0.2.0rc1/langserve/chat_playground/dist/assets/index-434ff580.css
--rw-r--r--   0        0        0   494586 2024-05-15 20:31:12.053390 langserve-0.2.0rc1/langserve/chat_playground/dist/assets/index-86d4d9c0.js
--rw-r--r--   0        0        0    40410 2024-05-15 20:31:12.053390 langserve-0.2.0rc1/langserve/chat_playground/dist/favicon.ico
--rw-r--r--   0        0        0     1141 2024-05-15 20:31:12.053390 langserve-0.2.0rc1/langserve/chat_playground/dist/index.html
--rw-r--r--   0        0        0      981 2024-05-15 20:31:12.053390 langserve-0.2.0rc1/langserve/chat_playground/index.html
--rw-r--r--   0        0        0     1526 2024-05-15 20:31:12.053390 langserve-0.2.0rc1/langserve/chat_playground/package.json
--rw-r--r--   0        0        0       81 2024-05-15 20:31:12.053390 langserve-0.2.0rc1/langserve/chat_playground/postcss.config.js
--rw-r--r--   0        0        0    40410 2024-05-15 20:31:12.053390 langserve-0.2.0rc1/langserve/chat_playground/public/favicon.ico
--rw-r--r--   0        0        0     2554 2024-05-15 20:31:12.053390 langserve-0.2.0rc1/langserve/chat_playground/src/App.css
--rw-r--r--   0        0        0     2989 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/App.tsx
--rw-r--r--   0        0        0      310 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/ArrowUp.svg
--rw-r--r--   0        0        0     2626 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/ChatIcon.svg
--rw-r--r--   0        0        0      789 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/CheckCircleIcon.svg
--rw-r--r--   0        0        0      328 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/CheckCircleIcon2.svg
--rw-r--r--   0        0        0      505 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/ChevronRight.svg
--rw-r--r--   0        0        0     1153 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/CircleSpinIcon.svg
--rw-r--r--   0        0        0      823 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/CodeIcon.svg
--rw-r--r--   0        0        0     1328 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/CopyIcon.svg
--rw-r--r--   0        0        0     1744 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/EmptyState.svg
--rw-r--r--   0        0        0    11000 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/LangServeLogo.svg
--rw-r--r--   0        0        0     2350 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/PadlockIcon.svg
--rw-r--r--   0        0        0      670 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/PlusIcon.svg
--rw-r--r--   0        0        0      400 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/RefreshCW.svg
--rw-r--r--   0        0        0     1260 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/SendIcon.svg
--rw-r--r--   0        0        0     1831 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/ShareIcon.svg
--rw-r--r--   0        0        0      374 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/ThumbsDownIcon.svg
--rw-r--r--   0        0        0      354 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/ThumbsUpIcon.svg
--rw-r--r--   0        0        0     1509 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/TrashIcon.svg
--rw-r--r--   0        0        0      346 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/assets/XCircle.svg
--rw-r--r--   0        0        0     1578 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/components/AutosizeTextarea.tsx
--rw-r--r--   0        0        0     4288 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/components/ChatMessage.tsx
--rw-r--r--   0        0        0     7735 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/components/ChatWindow.tsx
--rw-r--r--   0        0        0     5116 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/components/ShareDialog.tsx
--rw-r--r--   0        0        0     3463 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/components/feedback/CorrectnessFeedback.tsx
--rw-r--r--   0        0        0      308 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/main.tsx
--rw-r--r--   0        0        0      368 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/types.tsx
--rw-r--r--   0        0        0     3924 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/useSchemas.tsx
--rw-r--r--   0        0        0     2345 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/useStreamCallback.tsx
--rw-r--r--   0        0        0     3406 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/useStreamLog.tsx
--rw-r--r--   0        0        0      183 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/utils/cn.ts
--rw-r--r--   0        0        0     5344 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/utils/defaults.ts
--rw-r--r--   0        0        0      140 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/utils/json-refs.d.ts
--rw-r--r--   0        0        0   367401 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/utils/json-refs.js
--rw-r--r--   0        0        0      227 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/utils/messages.ts
--rw-r--r--   0        0        0      726 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/utils/path.ts
--rw-r--r--   0        0        0      548 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/utils/schema.ts
--rw-r--r--   0        0        0      330 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/utils/simplifySchema.ts
--rw-r--r--   0        0        0      147 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/utils/str.ts
--rw-r--r--   0        0        0      958 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/utils/url.ts
--rw-r--r--   0        0        0       87 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/src/vite-env.d.ts
--rw-r--r--   0        0        0      950 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/tailwind.config.js
--rw-r--r--   0        0        0      605 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/tsconfig.json
--rw-r--r--   0        0        0      213 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/tsconfig.node.json
--rw-r--r--   0        0        0      571 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/vite.config.ts
--rw-r--r--   0        0        0   134098 2024-05-15 20:31:12.057390 langserve-0.2.0rc1/langserve/chat_playground/yarn.lock
--rw-r--r--   0        0        0    31643 2024-05-15 20:31:12.061390 langserve-0.2.0rc1/langserve/client.py
--rw-r--r--   0        0        0    14983 2024-05-15 20:31:12.061390 langserve-0.2.0rc1/langserve/lzstring.py
--rw-r--r--   0        0        0      436 2024-05-15 20:31:12.061390 langserve-0.2.0rc1/langserve/playground/.eslintrc.cjs
--rw-r--r--   0        0        0      266 2024-05-15 20:31:12.061390 langserve-0.2.0rc1/langserve/playground/.gitignore
--rw-r--r--   0        0        0     1263 2024-05-15 20:31:12.061390 langserve-0.2.0rc1/langserve/playground/README.md
--rw-r--r--   0        0        0    16476 2024-05-15 20:31:12.061390 langserve-0.2.0rc1/langserve/playground/dist/assets/index-52e8ab2f.css
--rw-r--r--   0        0        0  1332675 2024-05-15 20:31:12.065390 langserve-0.2.0rc1/langserve/playground/dist/assets/index-dbc96538.js
--rw-r--r--   0        0        0    40410 2024-05-15 20:31:12.065390 langserve-0.2.0rc1/langserve/playground/dist/favicon.ico
--rw-r--r--   0        0        0      916 2024-05-15 20:31:12.065390 langserve-0.2.0rc1/langserve/playground/dist/index.html
--rw-r--r--   0        0        0      756 2024-05-15 20:31:12.065390 langserve-0.2.0rc1/langserve/playground/index.html
--rw-r--r--   0        0        0     1616 2024-05-15 20:31:12.065390 langserve-0.2.0rc1/langserve/playground/package.json
--rw-r--r--   0        0        0       81 2024-05-15 20:31:12.065390 langserve-0.2.0rc1/langserve/playground/postcss.config.js
--rw-r--r--   0        0        0    40410 2024-05-15 20:31:12.065390 langserve-0.2.0rc1/langserve/playground/public/favicon.ico
--rw-r--r--   0        0        0     2081 2024-05-15 20:31:12.065390 langserve-0.2.0rc1/langserve/playground/src/App.css
--rw-r--r--   0        0        0     7176 2024-05-15 20:31:12.065390 langserve-0.2.0rc1/langserve/playground/src/App.tsx
--rw-r--r--   0        0        0     2626 2024-05-15 20:31:12.065390 langserve-0.2.0rc1/langserve/playground/src/assets/ChatIcon.svg
--rw-r--r--   0        0        0      792 2024-05-15 20:31:12.065390 langserve-0.2.0rc1/langserve/playground/src/assets/CheckCircleIcon.svg
--rw-r--r--   0        0        0      505 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/assets/ChevronRight.svg
--rw-r--r--   0        0        0     1153 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/assets/CircleSpinIcon.svg
--rw-r--r--   0        0        0      823 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/assets/CodeIcon.svg
--rw-r--r--   0        0        0     1328 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/assets/CopyIcon.svg
--rw-r--r--   0        0        0     2350 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/assets/PadlockIcon.svg
--rw-r--r--   0        0        0      670 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/assets/PlusIcon.svg
--rw-r--r--   0        0        0     1260 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/assets/SendIcon.svg
--rw-r--r--   0        0        0     1831 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/assets/ShareIcon.svg
--rw-r--r--   0        0        0     1089 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/assets/ThumbsDownIcon.svg
--rw-r--r--   0        0        0      549 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/assets/ThumbsUpIcon.svg
--rw-r--r--   0        0        0     1509 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/assets/TrashIcon.svg
--rw-r--r--   0        0        0     1424 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/AutosizeTextarea.tsx
--rw-r--r--   0        0        0     5541 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/ChatMessageInput.tsx
--rw-r--r--   0        0        0     5595 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/ChatMessageTuplesControlRenderer.tsx
--rw-r--r--   0        0        0     5168 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/ChatMessagesControlRenderer.tsx
--rw-r--r--   0        0        0     1076 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/CustomAnyOfRenderer.tsx
--rw-r--r--   0        0        0     2519 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/DeleteDialog.tsx
--rw-r--r--   0        0        0    13357 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/MaterialTableControl.tsx
--rw-r--r--   0        0        0     1562 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/NoBorderTableCell.tsx
--rw-r--r--   0        0        0     3182 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/TableToolbar.tsx
--rw-r--r--   0        0        0     1819 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/ValidationIcon.tsx
--rw-r--r--   0        0        0     3680 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/CustomArrayControlRenderer.tsx
--rw-r--r--   0        0        0     2617 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/CustomTextAreaCell.tsx
--rw-r--r--   0        0        0     1256 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/FileBase64Tester.tsx
--rw-r--r--   0        0        0     2468 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/IntermediateSteps.tsx
--rw-r--r--   0        0        0     2941 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/JsonTextAreaCell.tsx
--rw-r--r--   0        0        0     5189 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/ShareDialog.tsx
--rw-r--r--   0        0        0     3320 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/StreamOutput.tsx
--rw-r--r--   0        0        0     2347 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/SubmitButton.tsx
--rw-r--r--   0        0        0     2910 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/components/feedback/CorrectnessFeedback.tsx
--rw-r--r--   0        0        0      308 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/main.tsx
--rw-r--r--   0        0        0     3372 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/renderers.tsx
--rw-r--r--   0        0        0     1580 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/sections/SectionConfigure.tsx
--rw-r--r--   0        0        0     2125 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/sections/SectionInputs.tsx
--rw-r--r--   0        0        0      358 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/types.tsx
--rw-r--r--   0        0        0     2633 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/useSchemas.tsx
--rw-r--r--   0        0        0     2345 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/useStreamCallback.tsx
--rw-r--r--   0        0        0     3401 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/useStreamLog.tsx
--rw-r--r--   0        0        0      183 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/utils/cn.ts
--rw-r--r--   0        0        0     5344 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/utils/defaults.ts
--rw-r--r--   0        0        0      140 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/utils/json-refs.d.ts
--rw-r--r--   0        0        0   367401 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/utils/json-refs.js
--rw-r--r--   0        0        0      227 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/utils/messages.ts
--rw-r--r--   0        0        0      726 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/utils/path.ts
--rw-r--r--   0        0        0      548 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/utils/schema.ts
--rw-r--r--   0        0        0      330 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/utils/simplifySchema.ts
--rw-r--r--   0        0        0      147 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/utils/str.ts
--rw-r--r--   0        0        0      958 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/utils/url.ts
--rw-r--r--   0        0        0       87 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/src/vite-env.d.ts
--rw-r--r--   0        0        0      781 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/tailwind.config.js
--rw-r--r--   0        0        0      605 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/tsconfig.json
--rw-r--r--   0        0        0      213 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/tsconfig.node.json
--rw-r--r--   0        0        0      539 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/vite.config.ts
--rw-r--r--   0        0        0   135134 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/playground/yarn.lock
--rw-r--r--   0        0        0     3543 2024-05-15 20:31:12.061390 langserve-0.2.0rc1/langserve/playground.py
--rw-r--r--   0        0        0        0 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/py.typed
--rw-r--r--   0        0        0     1187 2024-05-15 20:31:12.069390 langserve-0.2.0rc1/langserve/pydantic_v1.py
--rw-r--r--   0        0        0     5349 2024-05-15 20:31:12.073390 langserve-0.2.0rc1/langserve/schema.py
--rw-r--r--   0        0        0     7004 2024-05-15 20:31:12.073390 langserve-0.2.0rc1/langserve/serialization.py
--rw-r--r--   0        0        0    46956 2024-05-15 20:31:12.073390 langserve-0.2.0rc1/langserve/server.py
--rw-r--r--   0        0        0     4089 2024-05-15 20:31:12.073390 langserve-0.2.0rc1/langserve/server_sent_events.py
--rw-r--r--   0        0        0    17233 2024-05-15 20:31:12.073390 langserve-0.2.0rc1/langserve/validation.py
--rw-r--r--   0        0        0      307 2024-05-15 20:31:12.073390 langserve-0.2.0rc1/langserve/version.py
--rw-r--r--   0        0        0     2570 2024-05-15 20:31:12.073390 langserve-0.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0    39832 1970-01-01 00:00:00.000000 langserve-0.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3757 2024-05-24 17:12:35.305724 langserve-0.2.1/LICENSE
+-rw-r--r--   0        0        0    38967 2024-05-24 17:12:35.305724 langserve-0.2.1/README.md
+-rw-r--r--   0        0        0      505 2024-05-24 17:12:35.309724 langserve-0.2.1/langserve/__init__.py
+-rw-r--r--   0        0        0    64398 2024-05-24 17:12:35.309724 langserve-0.2.1/langserve/api_handler.py
+-rw-r--r--   0        0        0    14240 2024-05-24 17:12:35.309724 langserve-0.2.1/langserve/callbacks.py
+-rw-r--r--   0        0        0      436 2024-05-24 17:12:35.309724 langserve-0.2.1/langserve/chat_playground/.eslintrc.cjs
+-rw-r--r--   0        0        0      266 2024-05-24 17:12:35.309724 langserve-0.2.1/langserve/chat_playground/.gitignore
+-rw-r--r--   0        0        0     1263 2024-05-24 17:12:35.309724 langserve-0.2.1/langserve/chat_playground/README.md
+-rw-r--r--   0        0        0    23810 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/dist/assets/index-434ff580.css
+-rw-r--r--   0        0        0   494586 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/dist/assets/index-86d4d9c0.js
+-rw-r--r--   0        0        0    40410 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/dist/favicon.ico
+-rw-r--r--   0        0        0     1141 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/dist/index.html
+-rw-r--r--   0        0        0      981 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/index.html
+-rw-r--r--   0        0        0     1526 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/package.json
+-rw-r--r--   0        0        0       81 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/postcss.config.js
+-rw-r--r--   0        0        0    40410 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/public/favicon.ico
+-rw-r--r--   0        0        0     2554 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/src/App.css
+-rw-r--r--   0        0        0     2989 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/src/App.tsx
+-rw-r--r--   0        0        0      310 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/src/assets/ArrowUp.svg
+-rw-r--r--   0        0        0     2626 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/src/assets/ChatIcon.svg
+-rw-r--r--   0        0        0      789 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/src/assets/CheckCircleIcon.svg
+-rw-r--r--   0        0        0      328 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/src/assets/CheckCircleIcon2.svg
+-rw-r--r--   0        0        0      505 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/src/assets/ChevronRight.svg
+-rw-r--r--   0        0        0     1153 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/src/assets/CircleSpinIcon.svg
+-rw-r--r--   0        0        0      823 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/src/assets/CodeIcon.svg
+-rw-r--r--   0        0        0     1328 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/src/assets/CopyIcon.svg
+-rw-r--r--   0        0        0     1744 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/src/assets/EmptyState.svg
+-rw-r--r--   0        0        0    11000 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/src/assets/LangServeLogo.svg
+-rw-r--r--   0        0        0     2350 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/src/assets/PadlockIcon.svg
+-rw-r--r--   0        0        0      670 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/src/assets/PlusIcon.svg
+-rw-r--r--   0        0        0      400 2024-05-24 17:12:35.313724 langserve-0.2.1/langserve/chat_playground/src/assets/RefreshCW.svg
+-rw-r--r--   0        0        0     1260 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/assets/SendIcon.svg
+-rw-r--r--   0        0        0     1831 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/assets/ShareIcon.svg
+-rw-r--r--   0        0        0      374 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/assets/ThumbsDownIcon.svg
+-rw-r--r--   0        0        0      354 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/assets/ThumbsUpIcon.svg
+-rw-r--r--   0        0        0     1509 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/assets/TrashIcon.svg
+-rw-r--r--   0        0        0      346 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/assets/XCircle.svg
+-rw-r--r--   0        0        0     1578 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/components/AutosizeTextarea.tsx
+-rw-r--r--   0        0        0     4288 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/components/ChatMessage.tsx
+-rw-r--r--   0        0        0     7735 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/components/ChatWindow.tsx
+-rw-r--r--   0        0        0     5116 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/components/ShareDialog.tsx
+-rw-r--r--   0        0        0     3463 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/components/feedback/CorrectnessFeedback.tsx
+-rw-r--r--   0        0        0      308 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/main.tsx
+-rw-r--r--   0        0        0      368 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/types.tsx
+-rw-r--r--   0        0        0     3924 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/useSchemas.tsx
+-rw-r--r--   0        0        0     2345 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/useStreamCallback.tsx
+-rw-r--r--   0        0        0     3406 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/useStreamLog.tsx
+-rw-r--r--   0        0        0      183 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/utils/cn.ts
+-rw-r--r--   0        0        0     5344 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/utils/defaults.ts
+-rw-r--r--   0        0        0      140 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/utils/json-refs.d.ts
+-rw-r--r--   0        0        0   367401 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/utils/json-refs.js
+-rw-r--r--   0        0        0      227 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/utils/messages.ts
+-rw-r--r--   0        0        0      726 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/utils/path.ts
+-rw-r--r--   0        0        0      548 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/utils/schema.ts
+-rw-r--r--   0        0        0      330 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/utils/simplifySchema.ts
+-rw-r--r--   0        0        0      147 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/utils/str.ts
+-rw-r--r--   0        0        0      958 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/utils/url.ts
+-rw-r--r--   0        0        0       87 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/src/vite-env.d.ts
+-rw-r--r--   0        0        0      950 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/tailwind.config.js
+-rw-r--r--   0        0        0      605 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/tsconfig.json
+-rw-r--r--   0        0        0      213 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/tsconfig.node.json
+-rw-r--r--   0        0        0      571 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/vite.config.ts
+-rw-r--r--   0        0        0   134098 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/chat_playground/yarn.lock
+-rw-r--r--   0        0        0    31643 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/client.py
+-rw-r--r--   0        0        0    14983 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/lzstring.py
+-rw-r--r--   0        0        0      436 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/playground/.eslintrc.cjs
+-rw-r--r--   0        0        0      266 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/playground/.gitignore
+-rw-r--r--   0        0        0     1263 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/playground/README.md
+-rw-r--r--   0        0        0    16476 2024-05-24 17:12:35.321724 langserve-0.2.1/langserve/playground/dist/assets/index-52e8ab2f.css
+-rw-r--r--   0        0        0  1332675 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/dist/assets/index-dbc96538.js
+-rw-r--r--   0        0        0    40410 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/dist/favicon.ico
+-rw-r--r--   0        0        0      916 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/dist/index.html
+-rw-r--r--   0        0        0      756 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/index.html
+-rw-r--r--   0        0        0     1616 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/package.json
+-rw-r--r--   0        0        0       81 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/postcss.config.js
+-rw-r--r--   0        0        0    40410 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/public/favicon.ico
+-rw-r--r--   0        0        0     2081 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/src/App.css
+-rw-r--r--   0        0        0     7176 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/src/App.tsx
+-rw-r--r--   0        0        0     2626 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/src/assets/ChatIcon.svg
+-rw-r--r--   0        0        0      792 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/src/assets/CheckCircleIcon.svg
+-rw-r--r--   0        0        0      505 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/src/assets/ChevronRight.svg
+-rw-r--r--   0        0        0     1153 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/src/assets/CircleSpinIcon.svg
+-rw-r--r--   0        0        0      823 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/src/assets/CodeIcon.svg
+-rw-r--r--   0        0        0     1328 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/src/assets/CopyIcon.svg
+-rw-r--r--   0        0        0     2350 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/src/assets/PadlockIcon.svg
+-rw-r--r--   0        0        0      670 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/src/assets/PlusIcon.svg
+-rw-r--r--   0        0        0     1260 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/src/assets/SendIcon.svg
+-rw-r--r--   0        0        0     1831 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/src/assets/ShareIcon.svg
+-rw-r--r--   0        0        0     1089 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/src/assets/ThumbsDownIcon.svg
+-rw-r--r--   0        0        0      549 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/src/assets/ThumbsUpIcon.svg
+-rw-r--r--   0        0        0     1509 2024-05-24 17:12:35.325724 langserve-0.2.1/langserve/playground/src/assets/TrashIcon.svg
+-rw-r--r--   0        0        0     1424 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/AutosizeTextarea.tsx
+-rw-r--r--   0        0        0     5541 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/ChatMessageInput.tsx
+-rw-r--r--   0        0        0     5595 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/ChatMessageTuplesControlRenderer.tsx
+-rw-r--r--   0        0        0     5168 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/ChatMessagesControlRenderer.tsx
+-rw-r--r--   0        0        0     1076 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/CustomAnyOfRenderer.tsx
+-rw-r--r--   0        0        0     2519 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/CustomArrayControlRenderer/DeleteDialog.tsx
+-rw-r--r--   0        0        0    13357 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/CustomArrayControlRenderer/MaterialTableControl.tsx
+-rw-r--r--   0        0        0     1562 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/CustomArrayControlRenderer/NoBorderTableCell.tsx
+-rw-r--r--   0        0        0     3182 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/CustomArrayControlRenderer/TableToolbar.tsx
+-rw-r--r--   0        0        0     1819 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/CustomArrayControlRenderer/ValidationIcon.tsx
+-rw-r--r--   0        0        0     3680 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/CustomArrayControlRenderer.tsx
+-rw-r--r--   0        0        0     2617 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/CustomTextAreaCell.tsx
+-rw-r--r--   0        0        0     1256 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/FileBase64Tester.tsx
+-rw-r--r--   0        0        0     2468 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/IntermediateSteps.tsx
+-rw-r--r--   0        0        0     2941 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/JsonTextAreaCell.tsx
+-rw-r--r--   0        0        0     5189 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/ShareDialog.tsx
+-rw-r--r--   0        0        0     3320 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/StreamOutput.tsx
+-rw-r--r--   0        0        0     2347 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/SubmitButton.tsx
+-rw-r--r--   0        0        0     2910 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/components/feedback/CorrectnessFeedback.tsx
+-rw-r--r--   0        0        0      308 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/main.tsx
+-rw-r--r--   0        0        0     3372 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/renderers.tsx
+-rw-r--r--   0        0        0     1580 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/sections/SectionConfigure.tsx
+-rw-r--r--   0        0        0     2125 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/sections/SectionInputs.tsx
+-rw-r--r--   0        0        0      358 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/types.tsx
+-rw-r--r--   0        0        0     2633 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/useSchemas.tsx
+-rw-r--r--   0        0        0     2345 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/useStreamCallback.tsx
+-rw-r--r--   0        0        0     3401 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/useStreamLog.tsx
+-rw-r--r--   0        0        0      183 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/utils/cn.ts
+-rw-r--r--   0        0        0     5344 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/utils/defaults.ts
+-rw-r--r--   0        0        0      140 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/utils/json-refs.d.ts
+-rw-r--r--   0        0        0   367401 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/utils/json-refs.js
+-rw-r--r--   0        0        0      227 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/utils/messages.ts
+-rw-r--r--   0        0        0      726 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/utils/path.ts
+-rw-r--r--   0        0        0      548 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/utils/schema.ts
+-rw-r--r--   0        0        0      330 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/utils/simplifySchema.ts
+-rw-r--r--   0        0        0      147 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/utils/str.ts
+-rw-r--r--   0        0        0      958 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/utils/url.ts
+-rw-r--r--   0        0        0       87 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/src/vite-env.d.ts
+-rw-r--r--   0        0        0      781 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/tailwind.config.js
+-rw-r--r--   0        0        0      605 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/tsconfig.json
+-rw-r--r--   0        0        0      213 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/tsconfig.node.json
+-rw-r--r--   0        0        0      539 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/vite.config.ts
+-rw-r--r--   0        0        0   135134 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/playground/yarn.lock
+-rw-r--r--   0        0        0     3543 2024-05-24 17:12:35.317724 langserve-0.2.1/langserve/playground.py
+-rw-r--r--   0        0        0        0 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/py.typed
+-rw-r--r--   0        0        0     1187 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/pydantic_v1.py
+-rw-r--r--   0        0        0     5349 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/schema.py
+-rw-r--r--   0        0        0     7004 2024-05-24 17:12:35.329724 langserve-0.2.1/langserve/serialization.py
+-rw-r--r--   0        0        0    46956 2024-05-24 17:12:35.333724 langserve-0.2.1/langserve/server.py
+-rw-r--r--   0        0        0     4089 2024-05-24 17:12:35.333724 langserve-0.2.1/langserve/server_sent_events.py
+-rw-r--r--   0        0        0    17233 2024-05-24 17:12:35.333724 langserve-0.2.1/langserve/validation.py
+-rw-r--r--   0        0        0      307 2024-05-24 17:12:35.333724 langserve-0.2.1/langserve/version.py
+-rw-r--r--   0        0        0     2567 2024-05-24 17:12:35.333724 langserve-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    39917 1970-01-01 00:00:00.000000 langserve-0.2.1/PKG-INFO
```

### Comparing `langserve-0.2.0rc1/LICENSE` & `langserve-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/README.md` & `langserve-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -163,25 +163,25 @@
     title="LangChain Server",
     version="1.0",
     description="A simple api server using Langchain's Runnable interfaces",
 )
 
 add_routes(
     app,
-    ChatOpenAI(),
+    ChatOpenAI(model="gpt-3.5-turbo-0125"),
     path="/openai",
 )
 
 add_routes(
     app,
-    ChatAnthropic(),
+    ChatAnthropic(model="claude-3-haiku-20240307"),
     path="/anthropic",
 )
 
-model = ChatAnthropic()
+model = ChatAnthropic(model="claude-3-haiku-20240307")
 prompt = ChatPromptTemplate.from_template("tell me a joke about {topic}")
 add_routes(
     app,
     prompt | model,
     path="/joke",
 )
```

### Comparing `langserve-0.2.0rc1/langserve/api_handler.py` & `langserve-0.2.1/langserve/api_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -848,15 +848,15 @@
                 # serializable format before returned in the response.
                 callback_events=callback_events,
                 metadata=InvokeResponseMetadata(
                     run_id=run_id,
                     feedback_tokens=[
                         FeedbackToken(
                             key=feedback_key,
-                            url=feedback_token.url,
+                            token_url=feedback_token.url,
                             expires_at=feedback_token.expires_at.isoformat(),
                         )
                     ]
                     if feedback_token
                     else [],
                 ),
             ),
@@ -995,15 +995,15 @@
         if feedback_tokens:
             metadatas = [
                 InvokeResponseMetadata(
                     run_id=run_id,
                     feedback_tokens=[
                         FeedbackToken(
                             key=feedback_key,
-                            url=feedback_token.url,
+                            token_url=feedback_token.url,
                             expires_at=feedback_token.expires_at.isoformat(),
                         )
                     ],
                 )
                 for run_id, feedback_token in zip(run_ids, feedback_tokens)
             ]
         else:
```

### Comparing `langserve-0.2.0rc1/langserve/callbacks.py` & `langserve-0.2.1/langserve/callbacks.py`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/README.md` & `langserve-0.2.1/langserve/chat_playground/README.md`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/dist/assets/index-434ff580.css` & `langserve-0.2.1/langserve/chat_playground/dist/assets/index-434ff580.css`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/dist/assets/index-86d4d9c0.js` & `langserve-0.2.1/langserve/chat_playground/dist/assets/index-86d4d9c0.js`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/dist/favicon.ico` & `langserve-0.2.1/langserve/chat_playground/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/dist/index.html` & `langserve-0.2.1/langserve/chat_playground/dist/index.html`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/index.html` & `langserve-0.2.1/langserve/chat_playground/index.html`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/package.json` & `langserve-0.2.1/langserve/chat_playground/package.json`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/public/favicon.ico` & `langserve-0.2.1/langserve/chat_playground/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/App.css` & `langserve-0.2.1/langserve/chat_playground/src/App.css`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/App.tsx` & `langserve-0.2.1/langserve/chat_playground/src/App.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/assets/ChatIcon.svg` & `langserve-0.2.1/langserve/chat_playground/src/assets/ChatIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/assets/CheckCircleIcon.svg` & `langserve-0.2.1/langserve/chat_playground/src/assets/CheckCircleIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/assets/CircleSpinIcon.svg` & `langserve-0.2.1/langserve/chat_playground/src/assets/CircleSpinIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/assets/CodeIcon.svg` & `langserve-0.2.1/langserve/chat_playground/src/assets/CodeIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/assets/CopyIcon.svg` & `langserve-0.2.1/langserve/chat_playground/src/assets/CopyIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/assets/EmptyState.svg` & `langserve-0.2.1/langserve/chat_playground/src/assets/EmptyState.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/assets/LangServeLogo.svg` & `langserve-0.2.1/langserve/chat_playground/src/assets/LangServeLogo.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/assets/PadlockIcon.svg` & `langserve-0.2.1/langserve/chat_playground/src/assets/PadlockIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/assets/PlusIcon.svg` & `langserve-0.2.1/langserve/chat_playground/src/assets/PlusIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/assets/SendIcon.svg` & `langserve-0.2.1/langserve/chat_playground/src/assets/SendIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/assets/ShareIcon.svg` & `langserve-0.2.1/langserve/chat_playground/src/assets/ShareIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/assets/TrashIcon.svg` & `langserve-0.2.1/langserve/chat_playground/src/assets/TrashIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/components/AutosizeTextarea.tsx` & `langserve-0.2.1/langserve/chat_playground/src/components/AutosizeTextarea.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/components/ChatMessage.tsx` & `langserve-0.2.1/langserve/chat_playground/src/components/ChatMessage.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/components/ChatWindow.tsx` & `langserve-0.2.1/langserve/chat_playground/src/components/ChatWindow.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/components/ShareDialog.tsx` & `langserve-0.2.1/langserve/chat_playground/src/components/ShareDialog.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/components/feedback/CorrectnessFeedback.tsx` & `langserve-0.2.1/langserve/chat_playground/src/components/feedback/CorrectnessFeedback.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/useSchemas.tsx` & `langserve-0.2.1/langserve/chat_playground/src/useSchemas.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/useStreamCallback.tsx` & `langserve-0.2.1/langserve/chat_playground/src/useStreamCallback.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/useStreamLog.tsx` & `langserve-0.2.1/langserve/chat_playground/src/useStreamLog.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/utils/defaults.ts` & `langserve-0.2.1/langserve/chat_playground/src/utils/defaults.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/utils/json-refs.js` & `langserve-0.2.1/langserve/chat_playground/src/utils/json-refs.js`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/utils/path.ts` & `langserve-0.2.1/langserve/chat_playground/src/utils/path.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/utils/schema.ts` & `langserve-0.2.1/langserve/chat_playground/src/utils/schema.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/src/utils/url.ts` & `langserve-0.2.1/langserve/chat_playground/src/utils/url.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/tailwind.config.js` & `langserve-0.2.1/langserve/chat_playground/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/tsconfig.json` & `langserve-0.2.1/langserve/chat_playground/tsconfig.json`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/vite.config.ts` & `langserve-0.2.1/langserve/chat_playground/vite.config.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/chat_playground/yarn.lock` & `langserve-0.2.1/langserve/chat_playground/yarn.lock`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/client.py` & `langserve-0.2.1/langserve/client.py`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/lzstring.py` & `langserve-0.2.1/langserve/lzstring.py`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/README.md` & `langserve-0.2.1/langserve/playground/README.md`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/dist/assets/index-52e8ab2f.css` & `langserve-0.2.1/langserve/playground/dist/assets/index-52e8ab2f.css`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/dist/assets/index-dbc96538.js` & `langserve-0.2.1/langserve/playground/dist/assets/index-dbc96538.js`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/dist/favicon.ico` & `langserve-0.2.1/langserve/playground/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/dist/index.html` & `langserve-0.2.1/langserve/playground/dist/index.html`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/index.html` & `langserve-0.2.1/langserve/playground/index.html`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/package.json` & `langserve-0.2.1/langserve/playground/package.json`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/public/favicon.ico` & `langserve-0.2.1/langserve/playground/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/App.css` & `langserve-0.2.1/langserve/playground/src/App.css`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/App.tsx` & `langserve-0.2.1/langserve/playground/src/App.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/assets/ChatIcon.svg` & `langserve-0.2.1/langserve/playground/src/assets/ChatIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/assets/CheckCircleIcon.svg` & `langserve-0.2.1/langserve/playground/src/assets/CheckCircleIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/assets/CircleSpinIcon.svg` & `langserve-0.2.1/langserve/playground/src/assets/CircleSpinIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/assets/CodeIcon.svg` & `langserve-0.2.1/langserve/playground/src/assets/CodeIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/assets/CopyIcon.svg` & `langserve-0.2.1/langserve/playground/src/assets/CopyIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/assets/PadlockIcon.svg` & `langserve-0.2.1/langserve/playground/src/assets/PadlockIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/assets/PlusIcon.svg` & `langserve-0.2.1/langserve/playground/src/assets/PlusIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/assets/SendIcon.svg` & `langserve-0.2.1/langserve/playground/src/assets/SendIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/assets/ShareIcon.svg` & `langserve-0.2.1/langserve/playground/src/assets/ShareIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/assets/ThumbsDownIcon.svg` & `langserve-0.2.1/langserve/playground/src/assets/ThumbsDownIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/assets/ThumbsUpIcon.svg` & `langserve-0.2.1/langserve/playground/src/assets/ThumbsUpIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/assets/TrashIcon.svg` & `langserve-0.2.1/langserve/playground/src/assets/TrashIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/AutosizeTextarea.tsx` & `langserve-0.2.1/langserve/playground/src/components/AutosizeTextarea.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/ChatMessageInput.tsx` & `langserve-0.2.1/langserve/playground/src/components/ChatMessageInput.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/ChatMessageTuplesControlRenderer.tsx` & `langserve-0.2.1/langserve/playground/src/components/ChatMessageTuplesControlRenderer.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/ChatMessagesControlRenderer.tsx` & `langserve-0.2.1/langserve/playground/src/components/ChatMessagesControlRenderer.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/CustomAnyOfRenderer.tsx` & `langserve-0.2.1/langserve/playground/src/components/CustomAnyOfRenderer.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/DeleteDialog.tsx` & `langserve-0.2.1/langserve/playground/src/components/CustomArrayControlRenderer/DeleteDialog.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/MaterialTableControl.tsx` & `langserve-0.2.1/langserve/playground/src/components/CustomArrayControlRenderer/MaterialTableControl.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/NoBorderTableCell.tsx` & `langserve-0.2.1/langserve/playground/src/components/CustomArrayControlRenderer/NoBorderTableCell.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/TableToolbar.tsx` & `langserve-0.2.1/langserve/playground/src/components/CustomArrayControlRenderer/TableToolbar.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/ValidationIcon.tsx` & `langserve-0.2.1/langserve/playground/src/components/CustomArrayControlRenderer/ValidationIcon.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/CustomArrayControlRenderer.tsx` & `langserve-0.2.1/langserve/playground/src/components/CustomArrayControlRenderer.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/CustomTextAreaCell.tsx` & `langserve-0.2.1/langserve/playground/src/components/CustomTextAreaCell.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/FileBase64Tester.tsx` & `langserve-0.2.1/langserve/playground/src/components/FileBase64Tester.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/IntermediateSteps.tsx` & `langserve-0.2.1/langserve/playground/src/components/IntermediateSteps.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/JsonTextAreaCell.tsx` & `langserve-0.2.1/langserve/playground/src/components/JsonTextAreaCell.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/ShareDialog.tsx` & `langserve-0.2.1/langserve/playground/src/components/ShareDialog.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/StreamOutput.tsx` & `langserve-0.2.1/langserve/playground/src/components/StreamOutput.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/SubmitButton.tsx` & `langserve-0.2.1/langserve/playground/src/components/SubmitButton.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/components/feedback/CorrectnessFeedback.tsx` & `langserve-0.2.1/langserve/playground/src/components/feedback/CorrectnessFeedback.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/renderers.tsx` & `langserve-0.2.1/langserve/playground/src/renderers.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/sections/SectionConfigure.tsx` & `langserve-0.2.1/langserve/playground/src/sections/SectionConfigure.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/sections/SectionInputs.tsx` & `langserve-0.2.1/langserve/playground/src/sections/SectionInputs.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/useSchemas.tsx` & `langserve-0.2.1/langserve/playground/src/useSchemas.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/useStreamCallback.tsx` & `langserve-0.2.1/langserve/playground/src/useStreamCallback.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/useStreamLog.tsx` & `langserve-0.2.1/langserve/playground/src/useStreamLog.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/utils/defaults.ts` & `langserve-0.2.1/langserve/playground/src/utils/defaults.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/utils/json-refs.js` & `langserve-0.2.1/langserve/playground/src/utils/json-refs.js`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/utils/path.ts` & `langserve-0.2.1/langserve/playground/src/utils/path.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/utils/schema.ts` & `langserve-0.2.1/langserve/playground/src/utils/schema.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/src/utils/url.ts` & `langserve-0.2.1/langserve/playground/src/utils/url.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/tailwind.config.js` & `langserve-0.2.1/langserve/playground/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/tsconfig.json` & `langserve-0.2.1/langserve/playground/tsconfig.json`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/vite.config.ts` & `langserve-0.2.1/langserve/playground/vite.config.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground/yarn.lock` & `langserve-0.2.1/langserve/playground/yarn.lock`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/playground.py` & `langserve-0.2.1/langserve/playground.py`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/pydantic_v1.py` & `langserve-0.2.1/langserve/pydantic_v1.py`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/schema.py` & `langserve-0.2.1/langserve/schema.py`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/serialization.py` & `langserve-0.2.1/langserve/serialization.py`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/server.py` & `langserve-0.2.1/langserve/server.py`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/server_sent_events.py` & `langserve-0.2.1/langserve/server_sent_events.py`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/langserve/validation.py` & `langserve-0.2.1/langserve/validation.py`

 * *Files identical despite different names*

### Comparing `langserve-0.2.0rc1/pyproject.toml` & `langserve-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langserve"
-version = "0.2.0rc1"
+version = "0.2.1"
 description = ""
 readme = "README.md"
 authors = ["LangChain"]
 license = "LangServe"
 repository = "https://github.com/langchain-ai/langserve"
 exclude = ["langserve/playground,langserve/chat_playground"]
 include = ["langserve/playground/dist/**/*", "langserve/chat_playground/dist/**/*"]
```

### Comparing `langserve-0.2.0rc1/PKG-INFO` & `langserve-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langserve
-Version: 0.2.0rc1
+Version: 0.2.1
 Summary: 
 Home-page: https://github.com/langchain-ai/langserve
 License: LangServe
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -189,25 +189,25 @@
     title="LangChain Server",
     version="1.0",
     description="A simple api server using Langchain's Runnable interfaces",
 )
 
 add_routes(
     app,
-    ChatOpenAI(),
+    ChatOpenAI(model="gpt-3.5-turbo-0125"),
     path="/openai",
 )
 
 add_routes(
     app,
-    ChatAnthropic(),
+    ChatAnthropic(model="claude-3-haiku-20240307"),
     path="/anthropic",
 )
 
-model = ChatAnthropic()
+model = ChatAnthropic(model="claude-3-haiku-20240307")
 prompt = ChatPromptTemplate.from_template("tell me a joke about {topic}")
 add_routes(
     app,
     prompt | model,
     path="/joke",
 )
```

