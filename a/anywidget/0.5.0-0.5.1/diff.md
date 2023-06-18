# Comparing `tmp/anywidget-0.5.0.tar.gz` & `tmp/anywidget-0.5.1.tar.gz`

## Comparing `anywidget-0.5.0.tar` & `anywidget-0.5.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 anywidget-0.5.0/CITATION.cff
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget.json
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 anywidget-0.5.0/package.json
--rw-r--r--   0        0        0   259753 2020-02-02 00:00:00.000000 anywidget-0.5.0/pnpm-lock.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.5.0/pnpm-workspace.yaml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.5.0/.changeset/config.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/__init__.py
--rw-r--r--   0        0        0    25087 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/_descriptor.py
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/_file_contents.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/_protocols.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/_util.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/_version.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/experimental.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/py.typed
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/widget.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/labextension/package.json
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/labextension/static/138.2f08930b7b6074de7077.js
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/labextension/static/326.fa2e8950755c9713ac12.js
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/labextension/static/remoteEntry.3346a2ae3844083123da.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/nbextension/extension.js
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/nbextension/index.js
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/astro.config.js
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/package.json
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/tailwind.config.cjs
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/tsconfig.json
--rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/anywidget-overview.png
--rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/banner-dark.png
--rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/banner-light.png
--rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/banner-minimal.png
--rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/client-js-diagram.png
--rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/default-og-image.png
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/favicon.svg
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/make-scrollable-code-focusable.js
--rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/widget-overview.png
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/scripts/ipynb.mjs
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/scripts/render.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/scripts/utils.mjs
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/consts.ts
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/env.d.ts
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/languages.ts
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/util.ts
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/CodeHero.astro
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/ConfettiButton.astro
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/CounterButton.astro
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/HeadCommon.astro
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/HeadSEO.astro
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Hero.astro
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Footer/AvatarList.astro
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Footer/Footer.astro
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/AnyWidgetLogo.astro
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/AstroLogo.astro
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/Header.astro
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/HeaderButton.css
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/LanguageSelect.css
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/LanguageSelect.tsx
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/Search.css
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/Search.tsx
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/SidebarToggle.css
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/SidebarToggle.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/SkipToContent.astro
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/ThemeToggleButton.css
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/ThemeToggleButton.tsx
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/LeftSidebar/LeftSidebar.astro
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/PageContent/PageContent.astro
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/RightSidebar/MoreMenu.astro
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/RightSidebar/RightSidebar.astro
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/RightSidebar/TableOfContents.tsx
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/examples/Counter.astro
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/layouts/MainLayout.astro
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/layouts/SplashLayout.astro
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/pages/index.astro
--rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/pages/blog/anywidget-02.md
--rw-r--r--   0        0        0    22438 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/pages/blog/introducing-anywidget.mdx
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/pages/en/bundling.md
--rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/pages/en/experimental.md
--rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/pages/en/getting-started.mdx
--rw-r--r--   0        0        0    10534 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/pages/en/notebooks/counter.ipynb
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/styles/index.css
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/styles/theme.css
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.5.0/examples/Counter.ipynb
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 anywidget-0.5.0/examples/minimal_example.ipynb
--rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 anywidget-0.5.0/packages/anywidget/CHANGELOG.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.5.0/packages/anywidget/build.mjs
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.5.0/packages/anywidget/package.json
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.5.0/packages/anywidget/src/index.js
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.5.0/packages/anywidget/src/plugin.js
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 anywidget-0.5.0/packages/anywidget/src/widget.js
--rw-r--r--   0        0        0    10214 2020-02-02 00:00:00.000000 anywidget-0.5.0/tests/test_descriptor.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 anywidget-0.5.0/tests/test_experimental.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.5.0/tests/test_file_contents.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.5.0/tests/test_protocols.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.5.0/tests/test_utils.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.5.0/tests/test_widget.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.5.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.5.0/LICENSE
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 anywidget-0.5.0/README.md
--rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 anywidget-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 anywidget-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 anywidget-0.5.1/CITATION.cff
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget.json
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 anywidget-0.5.1/package.json
+-rw-r--r--   0        0        0   259753 2020-02-02 00:00:00.000000 anywidget-0.5.1/pnpm-lock.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.5.1/pnpm-workspace.yaml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.5.1/.changeset/config.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/__init__.py
+-rw-r--r--   0        0        0    25087 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/_descriptor.py
+-rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/_file_contents.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/_protocols.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/_util.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/_version.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/experimental.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/py.typed
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/widget.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/labextension/package.json
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/labextension/static/138.8acbfebf26b04f3c9d53.js
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/labextension/static/326.f2f979ab7119ae78c2be.js
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/labextension/static/remoteEntry.73f706fd5f93400afdaf.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/nbextension/extension.js
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 anywidget-0.5.1/anywidget/nbextension/index.js
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/astro.config.js
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/package.json
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/tailwind.config.cjs
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/tsconfig.json
+-rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/anywidget-overview.png
+-rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/banner-dark.png
+-rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/banner-light.png
+-rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/banner-minimal.png
+-rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/client-js-diagram.png
+-rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/default-og-image.png
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/favicon.svg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/make-scrollable-code-focusable.js
+-rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/public/widget-overview.png
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/scripts/ipynb.mjs
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/scripts/render.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/scripts/utils.mjs
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/consts.ts
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/env.d.ts
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/languages.ts
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/util.ts
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/CodeHero.astro
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/ConfettiButton.astro
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/CounterButton.astro
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/HeadCommon.astro
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/HeadSEO.astro
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Hero.astro
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Footer/AvatarList.astro
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Footer/Footer.astro
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/AnyWidgetLogo.astro
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/AstroLogo.astro
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/Header.astro
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/HeaderButton.css
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/LanguageSelect.css
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/LanguageSelect.tsx
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/Search.css
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/Search.tsx
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/SidebarToggle.css
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/SidebarToggle.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/SkipToContent.astro
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/ThemeToggleButton.css
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/Header/ThemeToggleButton.tsx
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/LeftSidebar/LeftSidebar.astro
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/PageContent/PageContent.astro
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/RightSidebar/MoreMenu.astro
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/RightSidebar/RightSidebar.astro
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/RightSidebar/TableOfContents.tsx
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/components/examples/Counter.astro
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/layouts/MainLayout.astro
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/layouts/SplashLayout.astro
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/pages/index.astro
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/pages/blog/anywidget-02.md
+-rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/pages/blog/introducing-anywidget.mdx
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/pages/en/bundling.md
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/pages/en/experimental.md
+-rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/pages/en/getting-started.mdx
+-rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md
+-rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/pages/en/notebooks/counter.ipynb
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/styles/index.css
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.5.1/docs/src/styles/theme.css
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 anywidget-0.5.1/examples/Counter.ipynb
+-rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 anywidget-0.5.1/examples/minimal_example.ipynb
+-rw-r--r--   0        0        0     7145 2020-02-02 00:00:00.000000 anywidget-0.5.1/packages/anywidget/CHANGELOG.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.5.1/packages/anywidget/build.mjs
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.5.1/packages/anywidget/package.json
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.5.1/packages/anywidget/src/index.js
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.5.1/packages/anywidget/src/plugin.js
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 anywidget-0.5.1/packages/anywidget/src/widget.js
+-rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 anywidget-0.5.1/tests/test_descriptor.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 anywidget-0.5.1/tests/test_experimental.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.5.1/tests/test_file_contents.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.5.1/tests/test_protocols.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.5.1/tests/test_utils.py
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 anywidget-0.5.1/tests/test_widget.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.5.1/LICENSE
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 anywidget-0.5.1/README.md
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 anywidget-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 anywidget-0.5.1/PKG-INFO
```

### Comparing `anywidget-0.5.0/.pre-commit-config.yaml` & `anywidget-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/CITATION.cff` & `anywidget-0.5.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/package.json` & `anywidget-0.5.1/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/pnpm-lock.yaml` & `anywidget-0.5.1/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/anywidget/_descriptor.py` & `anywidget-0.5.1/anywidget/_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/anywidget/_file_contents.py` & `anywidget-0.5.1/anywidget/_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/anywidget/_protocols.py` & `anywidget-0.5.1/anywidget/_protocols.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/anywidget/_util.py` & `anywidget-0.5.1/anywidget/_util.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/anywidget/experimental.py` & `anywidget-0.5.1/anywidget/experimental.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/anywidget/widget.py` & `anywidget-0.5.1/anywidget/widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/anywidget/labextension/package.json` & `anywidget-0.5.1/anywidget/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95703125%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.73f706fd5f93400afdaf.js'}}",*

 * * "'version'": "'0.5.1'"}*

```diff
@@ -22,15 +22,15 @@
     },
     "files": [
         "dist"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.3346a2ae3844083123da.js"
+            "load": "static/remoteEntry.73f706fd5f93400afdaf.js"
         },
         "extension": "src/plugin",
         "outputDir": "../../anywidget/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -42,9 +42,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.5.0"
+    "version": "0.5.1"
 }
```

### Comparing `anywidget-0.5.0/anywidget/labextension/static/138.2f08930b7b6074de7077.js` & `anywidget-0.5.1/anywidget/labextension/static/138.8acbfebf26b04f3c9d53.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -116,11 +116,11 @@
                             return await this._anywidget_cached_cleanup(), super.remove()
                         }
                     }
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.5.0"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.5.1"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.5.0/anywidget/labextension/static/326.fa2e8950755c9713ac12.js` & `anywidget-0.5.1/anywidget/labextension/static/326.f2f979ab7119ae78c2be.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -134,11 +134,11 @@
                             return await this._anywidget_cached_cleanup(), super.remove()
                         }
                     }
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.5.0"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.5.1"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.5.0/anywidget/labextension/static/remoteEntry.3346a2ae3844083123da.js` & `anywidget-0.5.1/anywidget/labextension/static/remoteEntry.73f706fd5f93400afdaf.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, f, l, s, d, p, c, h, v = {
+    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, v = {
             408: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(138).then((() => () => t(138))),
                         "./extension": () => t.e(326).then((() => () => t(326)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -22,109 +22,109 @@
                     get: () => o,
                     init: () => a
                 })
             }
         },
         g = {};
 
-    function b(e) {
+    function m(e) {
         var r = g[e];
         if (void 0 !== r) return r.exports;
         var t = g[e] = {
             exports: {}
         };
-        return v[e](t, t.exports, b), t.exports
+        return v[e](t, t.exports, m), t.exports
     }
-    b.m = v, b.c = g, b.n = e => {
+    m.m = v, m.c = g, m.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return b.d(r, {
+        return m.d(r, {
             a: r
         }), r
-    }, b.d = (e, r) => {
-        for (var t in r) b.o(r, t) && !b.o(e, t) && Object.defineProperty(e, t, {
+    }, m.d = (e, r) => {
+        for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, b.f = {}, b.e = e => Promise.all(Object.keys(b.f).reduce(((r, t) => (b.f[t](e, r), r)), [])), b.u = e => e + "." + {
-        138: "2f08930b7b6074de7077",
-        326: "fa2e8950755c9713ac12"
+    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
+        138: "8acbfebf26b04f3c9d53",
+        326: "f2f979ab7119ae78c2be"
     } [e] + ".js?v=" + {
-        138: "2f08930b7b6074de7077",
-        326: "fa2e8950755c9713ac12"
-    } [e], b.g = function() {
+        138: "8acbfebf26b04f3c9d53",
+        326: "f2f979ab7119ae78c2be"
+    } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), b.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", b.l = (t, n, o, a) => {
+    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", m.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var f = document.getElementsByTagName("script"), l = 0; l < f.length; l++) {
-                    var s = f[l];
+                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
+                    var s = l[f];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
                         i = s;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, b.nc && i.setAttribute("nonce", b.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, b.r = e => {
+    }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        b.S = {};
+        m.S = {};
         var e = {},
             r = {};
-        b.I = (t, n) => {
+        m.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                b.o(b.S, t) || (b.S[t] = {});
-                var a = b.S[t],
+                m.o(m.S, t) || (m.S[t] = {});
+                var a = m.S[t],
                     i = "anywidget",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => b.e(138).then((() => () => b(138))),
+                        get: () => m.e(138).then((() => () => m(138))),
                         from: i,
                         eager: !1
                     })
-                })("anywidget", "0.5.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("anywidget", "0.5.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        b.g.importScripts && (e = b.g.location + "");
-        var r = b.g.document;
+        m.g.importScripts && (e = m.g.location + "");
+        var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             t.length && (e = t[t.length - 1].src)
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), b.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -147,128 +147,128 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
         for (a = 1; a < e.length; a++) {
             var u = e[a];
-            i.push(0 === u ? "not(" + f() + ")" : 1 === u ? "(" + f() + " || " + f() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
-        return f();
+        return l();
 
-        function f() {
+        function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var i = 0, u = 1, f = !0;; u++, i++) {
-                var l, s, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(l = r[i]))[0])) return !f || ("u" == d ? u > n && !o : "" == d != o);
+            for (var i = 0, u = 1, l = !0;; u++, i++) {
+                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
                 if ("u" == s) {
-                    if (!f || "u" != d) return !1
-                } else if (f)
+                    if (!l || "u" != d) return !1
+                } else if (l)
                     if (d == s)
                         if (u <= n) {
-                            if (l != e[u]) return !1
+                            if (f != e[u]) return !1
                         } else {
-                            if (o ? l > e[u] : l < e[u]) return !1;
-                            l != e[u] && (f = !1)
+                            if (o ? f > e[u] : f < e[u]) return !1;
+                            f != e[u] && (l = !1)
                         }
                 else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
-                    f = !1, u--
+                    l = !1, u--
                 } else {
                     if (u <= n || s < d != o) return !1;
-                    f = !1
-                } else "s" != d && "n" != d && (f = !1, u--)
+                    l = !1
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
-        var t = b.S[e];
-        if (!t || !b.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = m.S[e];
+        if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(f(e, t, o, n)), s(e[t][o])
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), s(e[t][o])
     }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
-        var a = b.I(r);
-        return a && a.then ? a.then(e.bind(e, r, b.S[r], t, n, o)) : e(r, b.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), l(r, 0, t, n)))), p = {}, c = {
+        var a = m.I(r);
+        return a && a.then ? a.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), p = {}, c = {
         395: () => d("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
         ])
     }, h = {
         326: [395]
-    }, b.f.consumes = (e, r) => {
-        b.o(h, e) && h[e].forEach((e => {
-            if (b.o(p, e)) return r.push(p[e]);
+    }, m.f.consumes = (e, r) => {
+        m.o(h, e) && h[e].forEach((e => {
+            if (m.o(p, e)) return r.push(p[e]);
             var t = r => {
-                    p[e] = 0, b.m[e] = t => {
-                        delete b.c[e], t.exports = r()
+                    p[e] = 0, m.m[e] = t => {
+                        delete m.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete p[e], b.m[e] = t => {
-                        throw delete b.c[e], r
+                    delete p[e], m.m[e] = t => {
+                        throw delete m.c[e], r
                     }
                 };
             try {
                 var o = c[e]();
                 o.then ? r.push(p[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             957: 0
         };
-        b.f.j = (r, t) => {
-            var n = b.o(e, r) ? e[r] : void 0;
+        m.f.j = (r, t) => {
+            var n = m.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var a = b.p + b.u(r),
+                    var a = m.p + m.u(r),
                         i = new Error;
-                    b.l(a, (t => {
-                        if (b.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    m.l(a, (t => {
+                        if (m.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
                                 a = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
-                    f = 0;
+                    l = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) b.o(i, n) && (b.m[n] = i[n]);
-                    u && u(b)
+                    for (n in i) m.o(i, n) && (m.m[n] = i[n]);
+                    u && u(m)
                 }
-                for (r && r(t); f < a.length; f++) o = a[f], b.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkanywidget = self.webpackChunkanywidget || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var m = b(408);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = m
+    var y = m(408);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = y
 })();
```

### Comparing `anywidget-0.5.0/anywidget/nbextension/index.js` & `anywidget-0.5.1/anywidget/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 // package.json
 var name = "anywidget";
-var version = "0.5.0";
+var version = "0.5.1";
 
 // src/widget.js
 function is_href(str) {
     return str.startsWith("http://") || str.startsWith("https://");
 }
 async function load_css_href(href, anywidget_id) {
     let prev = document.querySelector(`link[id='${anywidget_id}']`);
```

### Comparing `anywidget-0.5.0/docs/README.md` & `anywidget-0.5.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/astro.config.js` & `anywidget-0.5.1/docs/astro.config.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/package.json` & `anywidget-0.5.1/docs/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/public/anywidget-overview.png` & `anywidget-0.5.1/docs/public/anywidget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/public/banner-dark.png` & `anywidget-0.5.1/docs/public/banner-dark.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/public/banner-light.png` & `anywidget-0.5.1/docs/public/banner-light.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/public/banner-minimal.png` & `anywidget-0.5.1/docs/public/banner-minimal.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/public/client-js-diagram.png` & `anywidget-0.5.1/docs/public/client-js-diagram.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/public/default-og-image.png` & `anywidget-0.5.1/docs/public/default-og-image.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/public/favicon.svg` & `anywidget-0.5.1/docs/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/public/widget-overview.png` & `anywidget-0.5.1/docs/public/widget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/scripts/ipynb.mjs` & `anywidget-0.5.1/docs/scripts/ipynb.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/scripts/utils.mjs` & `anywidget-0.5.1/docs/scripts/utils.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/consts.ts` & `anywidget-0.5.1/docs/src/consts.ts`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/CodeHero.astro` & `anywidget-0.5.1/docs/src/components/CodeHero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/CounterButton.astro` & `anywidget-0.5.1/docs/src/components/CounterButton.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/HeadCommon.astro` & `anywidget-0.5.1/docs/src/components/HeadCommon.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/HeadSEO.astro` & `anywidget-0.5.1/docs/src/components/HeadSEO.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/Hero.astro` & `anywidget-0.5.1/docs/src/components/Hero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/Footer/AvatarList.astro` & `anywidget-0.5.1/docs/src/components/Footer/AvatarList.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/Header/AnyWidgetLogo.astro` & `anywidget-0.5.1/docs/src/components/Header/AnyWidgetLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/Header/AstroLogo.astro` & `anywidget-0.5.1/docs/src/components/Header/AstroLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/Header/Header.astro` & `anywidget-0.5.1/docs/src/components/Header/Header.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/Header/HeaderButton.css` & `anywidget-0.5.1/docs/src/components/Header/HeaderButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/Header/LanguageSelect.css` & `anywidget-0.5.1/docs/src/components/Header/LanguageSelect.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/Header/LanguageSelect.tsx` & `anywidget-0.5.1/docs/src/components/Header/LanguageSelect.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/Header/Search.css` & `anywidget-0.5.1/docs/src/components/Header/Search.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/Header/Search.tsx` & `anywidget-0.5.1/docs/src/components/Header/Search.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/Header/SidebarToggle.tsx` & `anywidget-0.5.1/docs/src/components/Header/SidebarToggle.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/Header/ThemeToggleButton.css` & `anywidget-0.5.1/docs/src/components/Header/ThemeToggleButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/Header/ThemeToggleButton.tsx` & `anywidget-0.5.1/docs/src/components/Header/ThemeToggleButton.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/LeftSidebar/LeftSidebar.astro` & `anywidget-0.5.1/docs/src/components/LeftSidebar/LeftSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/PageContent/PageContent.astro` & `anywidget-0.5.1/docs/src/components/PageContent/PageContent.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/RightSidebar/MoreMenu.astro` & `anywidget-0.5.1/docs/src/components/RightSidebar/MoreMenu.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/RightSidebar/RightSidebar.astro` & `anywidget-0.5.1/docs/src/components/RightSidebar/RightSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/RightSidebar/TableOfContents.tsx` & `anywidget-0.5.1/docs/src/components/RightSidebar/TableOfContents.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/components/examples/Counter.astro` & `anywidget-0.5.1/docs/src/components/examples/Counter.astro`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 let widgetCode = `
 import anywidget
 import traitlets
 
 
 class CounterWidget(anywidget.AnyWidget):
     _esm = """
-    export function render(view) {
-      let count = () => view.model.get("value");
+    export function render({ model, el }) {
+      let count = () => model.get("value");
       let btn = document.createElement("button");
       btn.innerHTML = \`count is \${count()}\`;
       btn.addEventListener("click", () => {
-        view.model.set("value", count() + 1);
-        view.model.save_changes();
+        model.set("value", count() + 1);
+        model.save_changes();
       });
-      view.model.on("change:value", () => {
+      model.on("change:value", () => {
         btn.innerHTML = \`count is \${count()}\`;
       });
-      view.el.appendChild(btn);
+      el.appendChild(btn);
     }
     """
     value = traitlets.Int(0).tag(sync=True)
 `;
 
 let notebookCode = `\
 from mywidget import CounterWidget
```

### Comparing `anywidget-0.5.0/docs/src/layouts/MainLayout.astro` & `anywidget-0.5.1/docs/src/layouts/MainLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/layouts/SplashLayout.astro` & `anywidget-0.5.1/docs/src/layouts/SplashLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/pages/blog/anywidget-02.md` & `anywidget-0.5.1/docs/src/pages/blog/anywidget-02.md`

 * *Files 5% similar despite different names*

```diff
@@ -121,28 +121,28 @@
 // @ts-check
 /**
  * @typedef Model
  * @prop {number} value - the current count value
  */
 
 /** @type {import("anywidget/types").Render<Model>} */
-export function render(view) {
-	let value = view.model.get("value");
+export function render({ model, el }) {
+	let value = model.get("value");
 	//^? number
 
-	view.model.get("nope");
+	model.get("nope");
 	// type error, `nope` is not defined on Model
 
-	view.model.set("value", "not a number");
+	model.set("value", "not a number");
 	//^? type error, must be a number
 }
 ```
 
 The `import("anywidget/widget").Render<Model>` utilty strictly types the `render` function such that
-`view.model.get` and `view.model.set` are typed based on the user-defined `Model`.
+`model.get` and `model.set` are typed based on the user-defined `Model`.
 
 This feature brings Jupyter Widgets one step closer to having **end-to-end type safety**, and
 the use of TypeScript within JSDoc comments means that widget front-end code can benefit
 from static analysis without additional compilation, much like Python's builtin type hints.
 
 ### Defining Custom Cleanup Logic
 
@@ -152,15 +152,15 @@
 when dealing with complex event listeners, subscriptions, or third-party libraries that require proper
 teardown.
 
 Although this feature might not be essential for all use cases, it provides a flexible and more declarative
 way to ensure proper cleanup when needed:
 
 ```javascript
-export function render(view) {
+export function render({ model, el }) {
 	// Create DOM elements and set up subscribers
 	return () => {
 		// Optionally cleanup
 	};
 }
 ```
 
@@ -172,16 +172,16 @@
 import * as React from "https://esm.sh/react@18";
 import * as ReactDOM from "https://esm.sh/react-dom@18/client";
 
 function App(props) {
 	return <h1>Hello, world</h1>;
 }
 
-export function render(view) {
-	let root = ReactDOM.createRoot(view.el);
+export function render({ model, el }) {
+	let root = ReactDOM.createRoot(el);
 	root.render(<App />);
 	return () => root.unmount();
 }
 ```
 
 > Note: The above front-end code requires transformation with tool like `esbuild`
 > to allow for the special JSX syntax (e.g., `<App />`).
```

### Comparing `anywidget-0.5.0/docs/src/pages/blog/introducing-anywidget.mdx` & `anywidget-0.5.1/docs/src/pages/blog/introducing-anywidget.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 import anywidget
 import traitlets
 
 
 class CounterWidget(anywidget.AnyWidget):
     # Widget front-end JavaScript code
     _esm = """
-    export function render(view) {
-      let getCount = () => view.model.get("count");
+    export function render({ model, el }) {
+      let getCount = () => model.get("count");
       let button = document.createElement("button");
       button.innerHTML = `count is ${getCount()}`;
       button.addEventListener("click", () => {
-        view.model.set("count", getCount() + 1);
-        view.model.save_changes();
+        model.set("count", getCount() + 1);
+        model.save_changes();
       });
-      view.model.on("change:count", () => {
+      model.on("change:count", () => {
         button.innerHTML = `count is ${getCount()}`;
       });
-      view.el.appendChild(button);
+      el.appendChild(button);
     }
     """
     # Stateful property that can be accessed by JavaScript & Python
     count = traitlets.Int(0).tag(sync=True)
 ```
 
 _... to create custom widgets that work in Jupyter notebooks, JupyterLab, Google
@@ -406,21 +406,21 @@
 ```python
 import anywidget
 import traitlets
 
 class ExampleWidget(anywidget.AnyWidget):
     # anywidget, required #
     _esm = """
-    export function render(view) {
-        view.el.classList.add("custom-widget");
+    export function render({ model, el }) {
+        el.classList.add("custom-widget");
         function value_changed() {
-            view.el.textContent = view.model.get("value");
+            el.textContent = model.get("value");
         }
         value_changed();
-        view.model.on("change:value", value_changed);
+        model.on("change:value", value_changed);
     }
     """
     # anywidget, optional #
     _css = """
     .custom-widget {
         background-color: lightseagreen;
         padding: 0px 2px;
@@ -480,27 +480,27 @@
 ```python
 import anywidget
 import traitlets
 
 
 class CounterWidget(anywidget.AnyWidget):
     _esm = """
-    export function render(view) {
-      let getCount = () => view.model.get("count");
+    export function render({ model, el }) {
+      let getCount = () => model.get("count");
       let button = document.createElement("button");
       button.classList.add("counter-button");
       button.innerHTML = `count is ${getCount()}`;
       button.addEventListener("click", () => {
-        view.model.set("count", getCount() + 1);
-        view.model.save_changes();
+        model.set("count", getCount() + 1);
+        model.save_changes();
       });
-      view.model.on("change:count", () => {
+      model.on("change:count", () => {
         button.innerHTML = `count is ${getCount()}`;
       });
-      view.el.appendChild(button);
+      el.appendChild(button);
     }
     """
     _css="""
     .counter-button { background-color: #ea580c; }
     .counter-button:hover { background-color: #9a3412; }
     """
     count = traitlets.Int(0).tag(sync=True)
@@ -522,22 +522,22 @@
 ```python
 import anywidget
 
 class ConfettiWidget(anywidget.AnyWidget):
     _esm = """
     import confetti from "https://esm.sh/canvas-confetti@1.6";
 
-    export function render(view) {
+    export function render({ model, el }) {
       let btn = document.createElement("button");
       btn.classList.add("confetti-button");
       btn.innerHTML = "click me!";
       btn.addEventListener("click", () => {
         confetti();
       });
-      view.el.appendChild(btn);
+      el.appendChild(btn);
     }
     """
     _css="""
     .confetti-button { background-color: #ea580c; }
     .confetti-button:hover { background-color: #9a3412; }
     """
```

### Comparing `anywidget-0.5.0/docs/src/pages/en/bundling.md` & `anywidget-0.5.1/docs/src/pages/en/bundling.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/pages/en/experimental.md` & `anywidget-0.5.1/docs/src/pages/en/experimental.md`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 any python object that implements a known data-class pattern and observer.
 
 Here's an example of how to use the `widget` decorator to create a widget from a
 `dataclasses.dataclass`, that uses psygnal's [evented-dataclass pattern](https://psygnal.readthedocs.io/en/latest/dataclasses/) for
 observers:
 
 ```python
-esm = "export function render(view) {}"
+esm = "export function render({ model, el }) {}"
 css = ".foo { color: red;}"
 
 @widget(esm=esm, css=css)
 @psygnal.evented
 @dataclasses.dataclass
 class Foo:
     bar: str = "baz"
```

### Comparing `anywidget-0.5.0/docs/src/pages/en/getting-started.mdx` & `anywidget-0.5.1/docs/src/pages/en/getting-started.mdx`

 * *Files 3% similar despite different names*

```diff
@@ -33,27 +33,27 @@
 
 ```python
 import anywidget
 import traitlets
 
 class CounterWidget(anywidget.AnyWidget):
     _esm = """
-    export function render(view) {
-      let getCount = () => view.model.get("count");
+    export function render({ model, el }) {
+      let getCount = () => model.get("count");
       let button = document.createElement("button");
       button.classList.add("counter-button");
       button.innerHTML = `count is ${getCount()}`;
       button.addEventListener("click", () => {
-        view.model.set("count", getCount() + 1);
-        view.model.save_changes();
+        model.set("count", getCount() + 1);
+        model.save_changes();
       });
-      view.model.on("change:count", () => {
+      model.on("change:count", () => {
         button.innerHTML = `count is ${getCount()}`;
       });
-      view.el.appendChild(button);
+      el.appendChild(button);
     }
     """
     _css="""
     .counter-button { background-color: #ea580c; }
     .counter-button:hover { background-color: #9a3412; }
     """
     count = traitlets.Int(0).tag(sync=True)
```

### Comparing `anywidget-0.5.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md` & `anywidget-0.5.1/docs/src/pages/en/jupyter-widgets-the-good-parts.md`

 * *Files 4% similar despite different names*

```diff
@@ -109,39 +109,39 @@
 It defines an Integer `my_value` trait, which is synchronized with the front
 end. The `render` function now has the ability to:
 
 - **get** `my_value`
 
 ```javascript
 // index.js
-export function render(view) {
-	let my_value = view.model.get("my_value");
+export function render({ model, el }) {
+	let my_value = model.get("my_value");
 }
 ```
 
 - **set** `my_value`
 
 ```javascript
 // index.js
-export function render(view) {
-	view.model.set("my_value", 42);
-	view.model.save_changes(); // required to send update to Python
+export function render({ model, el }) {
+	model.set("my_value", 42);
+	model.save_changes(); // required to send update to Python
 }
 ```
 
 - **listen for changes to** `my_value` (and register event handlers)
 
 ```javascript
 // index.js
-export function render(view) {
+export function render({ model, el }) {
 	function on_change() {
-		let new_my_value = view.model.get("my_value");
+		let new_my_value = model.get("my_value");
 		console.log(`The 'my_value' changed to: ${new_my_value}`);
 	}
-	view.model.on("change:my_value", on_change);
+	model.on("change:my_value", on_change);
 }
 ```
 
 > **Note**: In the snippet above, `on_change` is called an _**event handler**_
 > because it executes any time `my_value` is updated from either Python or the
 > front-end code (i.e., a _change_ event).
 
@@ -172,21 +172,21 @@
 It doesn't matter if our widget is updated from JavaScript or Python, the IPython
 framework ensures it stays in sync with all the different components.
 
 ### 2. Custom messages
 
 A second mechanism to send data to the front end is with custom messages. Within
 your `render` function, you can listen to `msg:custom` events on the
-`view.model`. For example,
+`model`. For example,
 
 ```python
 class CustomMessageWidget(anywidget.AnyWidget):
     _esm = """
-    export function render(view) {
-      view.model.on("msg:custom", msg => {
+    export function render({ model, el }) {
+      model.on("msg:custom", msg => {
          console.log(`new message: ${JSON.stringify(msg)}`);
        });
     }
     """
 
 widget = CustomMessageWidget()
 widget # display the widget
@@ -241,15 +241,15 @@
   discern what is and (perhaps more importantly) is **_not_** standard JavaScript.
   I recommend reading Lin Clark's ["_ES modules: A cartoon deep-dive_"](https://hacks.mozilla.org/2018/03/es-modules-a-cartoon-deep-dive/)
   to learn more.
 
 - **Prefer Traitlets over custom messages for state synchronization**. Widget state can be
   fully recreated from traits without Python running, whereas custom messages require both
   an active Python kernel and special ordering of function calls. Write logic that treats
-  your `view.model` as the source of truth (see
+  your `model` as the source of truth (see
   [Two-Way Data-Binding Example](https://anywidget.dev/blog/introducing-anywidget/#examples)).
 
 - **Use the browser console**. View errors or intermediate values in your front-end
   code with the browser's [developer tools](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_are_browser_developer_tools).
   Getting comfortable with the console will help demystify the front end and enable you
   to quickly debug your widgets.
```

### Comparing `anywidget-0.5.0/docs/src/pages/en/notebooks/counter.ipynb` & `anywidget-0.5.1/docs/src/pages/en/notebooks/counter.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9935411932255137%*

 * *Differences: {"'cells'": "{3: {'metadata': {'execution': OrderedDict([('iopub.execute_input', "*

 * *            "'2023-06-18T16:10:06.975633Z'), ('iopub.status.busy', '2023-06-18T16:10:06.975336Z'), "*

 * *            "('iopub.status.idle', '2023-06-18T16:10:07.074307Z'), ('shell.execute_reply', "*

 * *            "'2023-06-18T16:10:07.073439Z')])}, 'outputs': {0: {'data': "*

 * *            "{'application/vnd.jupyter.widget-view+json': {'model_id': "*

 * *            "'7b1259728d614a06bcee5b64f97ccdee'}}}}, 'source': {insert: [(6, '    export […]*

```diff
@@ -31,21 +31,27 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "c47b8145",
             "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2023-06-18T16:10:06.975633Z",
+                    "iopub.status.busy": "2023-06-18T16:10:06.975336Z",
+                    "iopub.status.idle": "2023-06-18T16:10:07.074307Z",
+                    "shell.execute_reply": "2023-06-18T16:10:07.073439Z"
+                },
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "5039567750744ede88b340994ef62c56",
+                            "model_id": "7b1259728d614a06bcee5b64f97ccdee",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "CounterWidget(value=60)"
                         ]
                     },
@@ -57,27 +63,27 @@
             "source": [
                 "import anywidget\n",
                 "import traitlets\n",
                 "\n",
                 "\n",
                 "class CounterWidget(anywidget.AnyWidget):\n",
                 "    _esm = \"\"\"\n",
-                "    export function render(view) {\n",
-                "      let count = () => view.model.get(\"value\");\n",
+                "    export function render({ model, el }) {\n",
+                "      let count = () => model.get(\"value\");\n",
                 "      let btn = document.createElement(\"button\");\n",
                 "      btn.classList.add(\"counter-button\");\n",
                 "      btn.innerHTML = `count is ${count()}`;\n",
                 "      btn.addEventListener(\"click\", () => {\n",
-                "        view.model.set(\"value\", count() + 1);\n",
-                "        view.model.save_changes();\n",
+                "        model.set(\"value\", count() + 1);\n",
+                "        model.save_changes();\n",
                 "      });\n",
-                "      view.model.on(\"change:value\", () => {\n",
+                "      model.on(\"change:value\", () => {\n",
                 "        btn.innerHTML = `count is ${count()}`;\n",
                 "      });\n",
-                "      view.el.appendChild(btn);\n",
+                "      el.appendChild(btn);\n",
                 "    }\n",
                 "    \"\"\"\n",
                 "    _css = \"\"\"\n",
                 "    .counter-button {\n",
                 "      background-image: linear-gradient(to right, #a1c4fd, #c2e9fb);\n",
                 "      border: 0;\n",
                 "      border-radius: 10px;\n",
@@ -102,20 +108,27 @@
                 "By treating the model as the source of truth, whether Python kernel or JavaScript update value, the count displayed is correct. Additionally, a single model serves as the source of truth for all _views_ of that model. Therefore when `w` is displayed in another cell, the view is synchronized with the the output cell above."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "1b0f1a15",
-            "metadata": {},
+            "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2023-06-18T16:10:07.081408Z",
+                    "iopub.status.busy": "2023-06-18T16:10:07.081086Z",
+                    "iopub.status.idle": "2023-06-18T16:10:07.085910Z",
+                    "shell.execute_reply": "2023-06-18T16:10:07.085275Z"
+                }
+            },
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "5039567750744ede88b340994ef62c56",
+                            "model_id": "7b1259728d614a06bcee5b64f97ccdee",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "CounterWidget(value=60)"
                         ]
                     },
@@ -136,20 +149,27 @@
                 "But the state of a new widget instance is independent,"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "6e489ed7-f08e-4d19-9e94-e6f213449b0d",
-            "metadata": {},
+            "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2023-06-18T16:10:07.089553Z",
+                    "iopub.status.busy": "2023-06-18T16:10:07.089164Z",
+                    "iopub.status.idle": "2023-06-18T16:10:07.096121Z",
+                    "shell.execute_reply": "2023-06-18T16:10:07.095311Z"
+                }
+            },
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "ddad887826c24b59b5b2cc61727ef347",
+                            "model_id": "ca1ffd693fb74e609f9290d1d50cd056",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "CounterWidget()"
                         ]
                     },
@@ -183,64 +203,166 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.0"
+            "version": "3.11.3"
         },
         "widgets": {
             "application/vnd.jupyter.widget-state+json": {
                 "state": {
-                    "0be76018ffb341bda3060a47b4e8d4c5": {
+                    "5d447bcad70b488abb50f978900948b8": {
                         "model_module": "@jupyter-widgets/base",
                         "model_module_version": "2.0.0",
                         "model_name": "LayoutModel",
-                        "state": {}
-                    },
-                    "2f6c05fcff3e495b913580d2af7a7c79": {
-                        "model_module": "@jupyter-widgets/base",
-                        "model_module_version": "2.0.0",
-                        "model_name": "LayoutModel",
-                        "state": {}
+                        "state": {
+                            "_model_module": "@jupyter-widgets/base",
+                            "_model_module_version": "2.0.0",
+                            "_model_name": "LayoutModel",
+                            "_view_count": null,
+                            "_view_module": "@jupyter-widgets/base",
+                            "_view_module_version": "2.0.0",
+                            "_view_name": "LayoutView",
+                            "align_content": null,
+                            "align_items": null,
+                            "align_self": null,
+                            "border_bottom": null,
+                            "border_left": null,
+                            "border_right": null,
+                            "border_top": null,
+                            "bottom": null,
+                            "display": null,
+                            "flex": null,
+                            "flex_flow": null,
+                            "grid_area": null,
+                            "grid_auto_columns": null,
+                            "grid_auto_flow": null,
+                            "grid_auto_rows": null,
+                            "grid_column": null,
+                            "grid_gap": null,
+                            "grid_row": null,
+                            "grid_template_areas": null,
+                            "grid_template_columns": null,
+                            "grid_template_rows": null,
+                            "height": null,
+                            "justify_content": null,
+                            "justify_items": null,
+                            "left": null,
+                            "margin": null,
+                            "max_height": null,
+                            "max_width": null,
+                            "min_height": null,
+                            "min_width": null,
+                            "object_fit": null,
+                            "object_position": null,
+                            "order": null,
+                            "overflow": null,
+                            "padding": null,
+                            "right": null,
+                            "top": null,
+                            "visibility": null,
+                            "width": null
+                        }
                     },
-                    "5039567750744ede88b340994ef62c56": {
+                    "7b1259728d614a06bcee5b64f97ccdee": {
                         "model_module": "anywidget",
-                        "model_module_version": "0.0.4",
+                        "model_module_version": "0.5.0",
                         "model_name": "AnyModel",
                         "state": {
                             "_anywidget_id": "__main__.CounterWidget",
                             "_css": "\n    .counter-button {\n      background-image: linear-gradient(to right, #a1c4fd, #c2e9fb);\n      border: 0;\n      border-radius: 10px;\n      padding: 10px 50px;\n      color: white;\n    }\n    ",
-                            "_esm": "\n    export function render(view) {\n      let count = () => view.model.get(\"value\");\n      let btn = document.createElement(\"button\");\n      btn.classList.add(\"counter-button\");\n      btn.innerHTML = `count is ${count()}`;\n      btn.addEventListener(\"click\", () => {\n        view.model.set(\"value\", count() + 1);\n        view.model.save_changes();\n      });\n      view.model.on(\"change:value\", () => {\n        btn.innerHTML = `count is ${count()}`;\n      });\n      view.el.appendChild(btn);\n    }\n    ",
+                            "_dom_classes": [],
+                            "_esm": "\n    export function render({ model, el }) {\n      let count = () => model.get(\"value\");\n      let btn = document.createElement(\"button\");\n      btn.classList.add(\"counter-button\");\n      btn.innerHTML = `count is ${count()}`;\n      btn.addEventListener(\"click\", () => {\n        model.set(\"value\", count() + 1);\n        model.save_changes();\n      });\n      model.on(\"change:value\", () => {\n        btn.innerHTML = `count is ${count()}`;\n      });\n      el.appendChild(btn);\n    }\n    ",
                             "_model_module": "anywidget",
-                            "_model_module_version": "0.0.4",
+                            "_model_module_version": "0.5.0",
                             "_model_name": "AnyModel",
+                            "_view_count": null,
                             "_view_module": "anywidget",
-                            "_view_module_version": "0.0.4",
+                            "_view_module_version": "0.5.0",
                             "_view_name": "AnyView",
-                            "layout": "IPY_MODEL_2f6c05fcff3e495b913580d2af7a7c79",
+                            "layout": "IPY_MODEL_814ccd14aa424d7f94d02c887c00eb0d",
+                            "tabbable": null,
+                            "tooltip": null,
                             "value": 60
                         }
                     },
-                    "ddad887826c24b59b5b2cc61727ef347": {
+                    "814ccd14aa424d7f94d02c887c00eb0d": {
+                        "model_module": "@jupyter-widgets/base",
+                        "model_module_version": "2.0.0",
+                        "model_name": "LayoutModel",
+                        "state": {
+                            "_model_module": "@jupyter-widgets/base",
+                            "_model_module_version": "2.0.0",
+                            "_model_name": "LayoutModel",
+                            "_view_count": null,
+                            "_view_module": "@jupyter-widgets/base",
+                            "_view_module_version": "2.0.0",
+                            "_view_name": "LayoutView",
+                            "align_content": null,
+                            "align_items": null,
+                            "align_self": null,
+                            "border_bottom": null,
+                            "border_left": null,
+                            "border_right": null,
+                            "border_top": null,
+                            "bottom": null,
+                            "display": null,
+                            "flex": null,
+                            "flex_flow": null,
+                            "grid_area": null,
+                            "grid_auto_columns": null,
+                            "grid_auto_flow": null,
+                            "grid_auto_rows": null,
+                            "grid_column": null,
+                            "grid_gap": null,
+                            "grid_row": null,
+                            "grid_template_areas": null,
+                            "grid_template_columns": null,
+                            "grid_template_rows": null,
+                            "height": null,
+                            "justify_content": null,
+                            "justify_items": null,
+                            "left": null,
+                            "margin": null,
+                            "max_height": null,
+                            "max_width": null,
+                            "min_height": null,
+                            "min_width": null,
+                            "object_fit": null,
+                            "object_position": null,
+                            "order": null,
+                            "overflow": null,
+                            "padding": null,
+                            "right": null,
+                            "top": null,
+                            "visibility": null,
+                            "width": null
+                        }
+                    },
+                    "ca1ffd693fb74e609f9290d1d50cd056": {
                         "model_module": "anywidget",
-                        "model_module_version": "0.0.4",
+                        "model_module_version": "0.5.0",
                         "model_name": "AnyModel",
                         "state": {
                             "_anywidget_id": "__main__.CounterWidget",
                             "_css": "\n    .counter-button {\n      background-image: linear-gradient(to right, #a1c4fd, #c2e9fb);\n      border: 0;\n      border-radius: 10px;\n      padding: 10px 50px;\n      color: white;\n    }\n    ",
-                            "_esm": "\n    export function render(view) {\n      let count = () => view.model.get(\"value\");\n      let btn = document.createElement(\"button\");\n      btn.classList.add(\"counter-button\");\n      btn.innerHTML = `count is ${count()}`;\n      btn.addEventListener(\"click\", () => {\n        view.model.set(\"value\", count() + 1);\n        view.model.save_changes();\n      });\n      view.model.on(\"change:value\", () => {\n        btn.innerHTML = `count is ${count()}`;\n      });\n      view.el.appendChild(btn);\n    }\n    ",
+                            "_dom_classes": [],
+                            "_esm": "\n    export function render({ model, el }) {\n      let count = () => model.get(\"value\");\n      let btn = document.createElement(\"button\");\n      btn.classList.add(\"counter-button\");\n      btn.innerHTML = `count is ${count()}`;\n      btn.addEventListener(\"click\", () => {\n        model.set(\"value\", count() + 1);\n        model.save_changes();\n      });\n      model.on(\"change:value\", () => {\n        btn.innerHTML = `count is ${count()}`;\n      });\n      el.appendChild(btn);\n    }\n    ",
                             "_model_module": "anywidget",
-                            "_model_module_version": "0.0.4",
+                            "_model_module_version": "0.5.0",
                             "_model_name": "AnyModel",
+                            "_view_count": null,
                             "_view_module": "anywidget",
-                            "_view_module_version": "0.0.4",
+                            "_view_module_version": "0.5.0",
                             "_view_name": "AnyView",
-                            "layout": "IPY_MODEL_0be76018ffb341bda3060a47b4e8d4c5",
+                            "layout": "IPY_MODEL_5d447bcad70b488abb50f978900948b8",
+                            "tabbable": null,
+                            "tooltip": null,
                             "value": 0
                         }
                     }
                 },
                 "version_major": 2,
                 "version_minor": 0
             }
```

### Comparing `anywidget-0.5.0/docs/src/styles/index.css` & `anywidget-0.5.1/docs/src/styles/index.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/docs/src/styles/theme.css` & `anywidget-0.5.1/docs/src/styles/theme.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/examples/Counter.ipynb` & `anywidget-0.5.1/examples/Counter.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821924603174603%*

 * *Differences: {"'cells'": "{1: {'execution_count': 1, 'metadata': {'execution': "*

 * *            "OrderedDict([('iopub.execute_input', '2023-06-18T16:10:51.469018Z'), "*

 * *            "('iopub.status.busy', '2023-06-18T16:10:51.468707Z'), ('iopub.status.idle', "*

 * *            "'2023-06-18T16:10:51.564156Z'), ('shell.execute_reply', "*

 * *            "'2023-06-18T16:10:51.563215Z')])}, 'outputs': [OrderedDict([('data', "*

 * *            "OrderedDict([('application/vnd.jupyter.widget-view+json', OrderedDict([('model_id', "*

 * *            "'4 […]*

```diff
@@ -6,40 +6,62 @@
             "metadata": {},
             "source": [
                 "[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/manzt/anywidget/blob/main/examples/Counter.ipynb)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 1,
             "id": "c47b8145",
             "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2023-06-18T16:10:51.469018Z",
+                    "iopub.status.busy": "2023-06-18T16:10:51.468707Z",
+                    "iopub.status.idle": "2023-06-18T16:10:51.564156Z",
+                    "shell.execute_reply": "2023-06-18T16:10:51.563215Z"
+                },
                 "tags": []
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "application/vnd.jupyter.widget-view+json": {
+                            "model_id": "45a61ffd762a4520b9214dbd22641b15",
+                            "version_major": 2,
+                            "version_minor": 0
+                        },
+                        "text/plain": [
+                            "Counter()"
+                        ]
+                    },
+                    "execution_count": 1,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "import anywidget\n",
                 "import traitlets\n",
                 "\n",
                 "\n",
                 "class Counter(anywidget.AnyWidget):\n",
                 "    _esm = \"\"\"\n",
-                "    export function render(view) {\n",
-                "      let count = () => view.model.get(\"value\");\n",
+                "    export function render({ model, el }) {\n",
+                "      let count = () => model.get(\"value\");\n",
                 "      let btn = document.createElement(\"button\");\n",
                 "      btn.classList.add(\"counter-button\");\n",
                 "      btn.innerHTML = `count is ${count()}`;\n",
                 "      btn.addEventListener(\"click\", () => {\n",
-                "        view.model.set(\"value\", count() + 1);\n",
-                "        view.model.save_changes();\n",
+                "        model.set(\"value\", count() + 1);\n",
+                "        model.save_changes();\n",
                 "      });\n",
-                "      view.model.on(\"change:value\", () => {\n",
+                "      model.on(\"change:value\", () => {\n",
                 "        btn.innerHTML = `count is ${count()}`;\n",
                 "      });\n",
-                "      view.el.appendChild(btn);\n",
+                "      el.appendChild(btn);\n",
                 "    }\n",
                 "    \"\"\"\n",
                 "    _css = \"\"\"\n",
                 "    .counter-button {\n",
                 "      background-color: rgba(148, 163, 184, 0.1);\n",
                 "      border-radius: 10px;\n",
                 "      padding: 0.5em 1em;\n",
@@ -66,65 +88,92 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.0"
+            "version": "3.11.3"
         },
         "widgets": {
             "application/vnd.jupyter.widget-state+json": {
                 "state": {
-                    "0be76018ffb341bda3060a47b4e8d4c5": {
-                        "model_module": "@jupyter-widgets/base",
-                        "model_module_version": "2.0.0",
-                        "model_name": "LayoutModel",
-                        "state": {}
-                    },
-                    "2f6c05fcff3e495b913580d2af7a7c79": {
-                        "model_module": "@jupyter-widgets/base",
-                        "model_module_version": "2.0.0",
-                        "model_name": "LayoutModel",
-                        "state": {}
-                    },
-                    "5039567750744ede88b340994ef62c56": {
+                    "45a61ffd762a4520b9214dbd22641b15": {
                         "model_module": "anywidget",
-                        "model_module_version": "0.0.4",
+                        "model_module_version": "0.5.0",
                         "model_name": "AnyModel",
                         "state": {
-                            "_anywidget_id": "__main__.CounterWidget",
-                            "_css": "\n    .counter-button {\n      background-image: linear-gradient(to right, #a1c4fd, #c2e9fb);\n      border: 0;\n      border-radius: 10px;\n      padding: 10px 50px;\n      color: white;\n    }\n    ",
-                            "_esm": "\n    export function render(view) {\n      let count = () => view.model.get(\"value\");\n      let btn = document.createElement(\"button\");\n      btn.classList.add(\"counter-button\");\n      btn.innerHTML = `count is ${count()}`;\n      btn.addEventListener(\"click\", () => {\n        view.model.set(\"value\", count() + 1);\n        view.model.save_changes();\n      });\n      view.model.on(\"change:value\", () => {\n        btn.innerHTML = `count is ${count()}`;\n      });\n      view.el.appendChild(btn);\n    }\n    ",
+                            "_anywidget_id": "__main__.Counter",
+                            "_css": "\n    .counter-button {\n      background-color: rgba(148, 163, 184, 0.1);\n      border-radius: 10px;\n      padding: 0.5em 1em;\n      font-size: 2em;\n    }\n    ",
+                            "_dom_classes": [],
+                            "_esm": "\n    export function render({ model, el }) {\n      let count = () => model.get(\"value\");\n      let btn = document.createElement(\"button\");\n      btn.classList.add(\"counter-button\");\n      btn.innerHTML = `count is ${count()}`;\n      btn.addEventListener(\"click\", () => {\n        model.set(\"value\", count() + 1);\n        model.save_changes();\n      });\n      model.on(\"change:value\", () => {\n        btn.innerHTML = `count is ${count()}`;\n      });\n      el.appendChild(btn);\n    }\n    ",
                             "_model_module": "anywidget",
-                            "_model_module_version": "0.0.4",
+                            "_model_module_version": "0.5.0",
                             "_model_name": "AnyModel",
+                            "_view_count": null,
                             "_view_module": "anywidget",
-                            "_view_module_version": "0.0.4",
+                            "_view_module_version": "0.5.0",
                             "_view_name": "AnyView",
-                            "layout": "IPY_MODEL_2f6c05fcff3e495b913580d2af7a7c79",
-                            "value": 60
+                            "layout": "IPY_MODEL_c36fdefcbce6447c9bfae4d7b2849057",
+                            "tabbable": null,
+                            "tooltip": null,
+                            "value": 0
                         }
                     },
-                    "ddad887826c24b59b5b2cc61727ef347": {
-                        "model_module": "anywidget",
-                        "model_module_version": "0.0.4",
-                        "model_name": "AnyModel",
+                    "c36fdefcbce6447c9bfae4d7b2849057": {
+                        "model_module": "@jupyter-widgets/base",
+                        "model_module_version": "2.0.0",
+                        "model_name": "LayoutModel",
                         "state": {
-                            "_anywidget_id": "__main__.CounterWidget",
-                            "_css": "\n    .counter-button {\n      background-image: linear-gradient(to right, #a1c4fd, #c2e9fb);\n      border: 0;\n      border-radius: 10px;\n      padding: 10px 50px;\n      color: white;\n    }\n    ",
-                            "_esm": "\n    export function render(view) {\n      let count = () => view.model.get(\"value\");\n      let btn = document.createElement(\"button\");\n      btn.classList.add(\"counter-button\");\n      btn.innerHTML = `count is ${count()}`;\n      btn.addEventListener(\"click\", () => {\n        view.model.set(\"value\", count() + 1);\n        view.model.save_changes();\n      });\n      view.model.on(\"change:value\", () => {\n        btn.innerHTML = `count is ${count()}`;\n      });\n      view.el.appendChild(btn);\n    }\n    ",
-                            "_model_module": "anywidget",
-                            "_model_module_version": "0.0.4",
-                            "_model_name": "AnyModel",
-                            "_view_module": "anywidget",
-                            "_view_module_version": "0.0.4",
-                            "_view_name": "AnyView",
-                            "layout": "IPY_MODEL_0be76018ffb341bda3060a47b4e8d4c5",
-                            "value": 0
+                            "_model_module": "@jupyter-widgets/base",
+                            "_model_module_version": "2.0.0",
+                            "_model_name": "LayoutModel",
+                            "_view_count": null,
+                            "_view_module": "@jupyter-widgets/base",
+                            "_view_module_version": "2.0.0",
+                            "_view_name": "LayoutView",
+                            "align_content": null,
+                            "align_items": null,
+                            "align_self": null,
+                            "border_bottom": null,
+                            "border_left": null,
+                            "border_right": null,
+                            "border_top": null,
+                            "bottom": null,
+                            "display": null,
+                            "flex": null,
+                            "flex_flow": null,
+                            "grid_area": null,
+                            "grid_auto_columns": null,
+                            "grid_auto_flow": null,
+                            "grid_auto_rows": null,
+                            "grid_column": null,
+                            "grid_gap": null,
+                            "grid_row": null,
+                            "grid_template_areas": null,
+                            "grid_template_columns": null,
+                            "grid_template_rows": null,
+                            "height": null,
+                            "justify_content": null,
+                            "justify_items": null,
+                            "left": null,
+                            "margin": null,
+                            "max_height": null,
+                            "max_width": null,
+                            "min_height": null,
+                            "min_width": null,
+                            "object_fit": null,
+                            "object_position": null,
+                            "order": null,
+                            "overflow": null,
+                            "padding": null,
+                            "right": null,
+                            "top": null,
+                            "visibility": null,
+                            "width": null
                         }
                     }
                 },
                 "version_major": 2,
                 "version_minor": 0
             }
         }
```

### Comparing `anywidget-0.5.0/packages/anywidget/CHANGELOG.md` & `anywidget-0.5.1/packages/anywidget/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # anywidget
 
+## 0.5.1
+
+### Patch Changes
+
+- Updated dependencies [[`79098be`](https://github.com/manzt/anywidget/commit/79098be4bc5a1ce1023318b179b8e73ab3e59be3)]:
+  - @anywidget/vite@0.1.0
+
 ## 0.5.0
 
 ### Minor Changes
 
 - feat: restrict backbone model access in render context ([#140](https://github.com/manzt/anywidget/pull/140))
 
 - feat!: Limit view fields exposed to render function ([#138](https://github.com/manzt/anywidget/pull/138))
```

### Comparing `anywidget-0.5.0/packages/anywidget/build.mjs` & `anywidget-0.5.1/packages/anywidget/build.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/packages/anywidget/package.json` & `anywidget-0.5.1/packages/anywidget/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.5.1'"}*

```diff
@@ -38,9 +38,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.5.0"
+    "version": "0.5.1"
 }
```

### Comparing `anywidget-0.5.0/packages/anywidget/src/widget.js` & `anywidget-0.5.1/packages/anywidget/src/widget.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/tests/test_descriptor.py` & `anywidget-0.5.1/tests/test_descriptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,15 @@
     """Test that the file contents are inferred from the file path."""
 
     site_packages = tmp_path / "site-packages"
     site_packages.mkdir()
 
     esm = site_packages / "foo.js"
     esm.write_text(
-        "export function render(view) { view.el.innerText = 'Hello, world'; }"
+        "export function render({ model, el }) { el.innerText = 'Hello, world'; }"
     )
 
     class Foo:
         _repr_mimebundle_ = MimeBundleDescriptor(_esm=esm, autodetect_observer=False)
         value: int = 1
 
         def _get_anywidget_state(self):
```

### Comparing `anywidget-0.5.0/tests/test_experimental.py` & `anywidget-0.5.1/tests/test_experimental.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import psygnal
 from anywidget._descriptor import ReprMimeBundle
 from anywidget.experimental import MimeBundleDescriptor, widget
 
 
 def test_decorator():
-    esm = "export function render(view) {}"
+    esm = "export function render({ model , el }) {}"
     css = ".foo { color: red;}"
 
     @widget(esm=esm, css=css)
     @psygnal.evented
     @dataclasses.dataclass
     class Foo:
         bar: str = "baz"
```

### Comparing `anywidget-0.5.0/tests/test_file_contents.py` & `anywidget-0.5.1/tests/test_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/tests/test_utils.py` & `anywidget-0.5.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/tests/test_widget.py` & `anywidget-0.5.1/tests/test_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         pkg = json.load(f)
 
     assert anywidget.__version__ == pkg["version"]
 
 
 def test_basic():
     ESM = """
-    export function render(view) {
-        view.el.innerText = "Hello, world";
+    export function render({ model, el }) {
+        el.innerText = "Hello, world";
     }
     """
 
     class Widget(anywidget.AnyWidget):
         _esm = t.Unicode(ESM).tag(sync=True)
 
     w = Widget()
@@ -46,16 +46,16 @@
 
     assert w.has_trait("_esm")
     assert w._esm == _DEFAULT_ESM
 
 
 def test_creates_fully_qualified_identifier():
     ESM = """
-    export function render(view) {
-        view.el.innerText = "Hello, world";
+    export function render({ model, el }) {
+        el.innerText = "Hello, world";
     }
     """
 
     class Widget(anywidget.AnyWidget):
         _module = t.Unicode(ESM).tag(sync=True)
 
     w = Widget()
@@ -66,16 +66,16 @@
 
 def test_infer_traitlets():
     CSS = """
     .foo { background-color: black; }
     """
 
     ESM = """
-    export function render(view) {
-        view.el.innerText = "Hello, world";
+    export function render({ model, el }) {
+        el.innerText = "Hello, world";
     }
     """
 
     class Widget(anywidget.AnyWidget):
         _esm = ESM
         _css = CSS
 
@@ -90,16 +90,16 @@
 
 def test_infer_traitlets_partial():
     CSS = """
     .foo { background-color: black; }
     """
 
     ESM = """
-    export function render(view) {
-        view.el.innerText = "Hello, world";
+    export function render({ model, el }) {
+        el.innerText = "Hello, world";
     }
     """
 
     class Widget(anywidget.AnyWidget):
         _esm = t.Unicode(ESM).tag(foo="bar")
         _css = CSS
 
@@ -131,15 +131,15 @@
     assert bundle[0] and _WIDGET_MIME_TYPE in bundle[0]
     assert _WIDGET_MIME_TYPE in bundle[1]
 
 
 def test_infer_file_contents(tmp_path: pathlib.Path):
     esm = tmp_path / "foo.js"
     esm.write_text(
-        "export function render(view) { view.el.innerText = 'Hello, world'; }"
+        "export function render({ model, el }) { el.innerText = 'Hello, world'; }"
     )
 
     site_packages = tmp_path / "site-packages"
     site_packages.mkdir()
     css = site_packages / "styles.css"
     css.write_text(".foo { background-color: black; }")
 
@@ -203,15 +203,15 @@
     assert w._esm == str(tmp_path / "foo.js")
     assert w._css == css
 
 
 def test_explicit_file_contents(tmp_path: pathlib.Path):
     path = tmp_path / "foo.js"
     path.write_text(
-        "export function render(view) { view.el.innerText = 'Hello, world'; }"
+        "export function render({ model, el }) { el.innerText = 'Hello, world'; }"
     )
     esm = FileContents(path, start_thread=False)
 
     class Widget(anywidget.AnyWidget):
         _esm = esm
 
     assert Widget._esm == esm
```

### Comparing `anywidget-0.5.0/LICENSE` & `anywidget-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/README.md` & `anywidget-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,26 +44,26 @@
 ```python
 import anywidget
 import traitlets
 
 class CounterWidget(anywidget.AnyWidget):
     # Widget front-end JavaScript code
     _esm = """
-    export function render(view) {
-      let getCount = () => view.model.get("count");
+    export function render({ model, el }) {
+      let getCount = () => model.get("count");
       let button = document.createElement("button");
       button.innerHTML = `count is ${getCount()}`;
       button.addEventListener("click", () => {
-        view.model.set("count", getCount() + 1);
-        view.model.save_changes();
+        model.set("count", getCount() + 1);
+        model.save_changes();
       });
-      view.model.on("change:count", () => {
+      model.on("change:count", () => {
         button.innerHTML = `count is ${getCount()}`;
       });
-      view.el.appendChild(button);
+      el.appendChild(button);
     }
     """
     # Stateful property that can be accessed by JavaScript & Python
     count = traitlets.Int(0).tag(sync=True)
 ```
 
 Front-end code can also live in separate files (recommend):
```

### Comparing `anywidget-0.5.0/pyproject.toml` & `anywidget-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.0/PKG-INFO` & `anywidget-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anywidget
-Version: 0.5.0
+Version: 0.5.1
 Summary: custom jupyter widgets made easy
 Project-URL: homepage, https://github.com/manzt/anywidget
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata; python_version < '3.8'
@@ -69,26 +69,26 @@
 ```python
 import anywidget
 import traitlets
 
 class CounterWidget(anywidget.AnyWidget):
     # Widget front-end JavaScript code
     _esm = """
-    export function render(view) {
-      let getCount = () => view.model.get("count");
+    export function render({ model, el }) {
+      let getCount = () => model.get("count");
       let button = document.createElement("button");
       button.innerHTML = `count is ${getCount()}`;
       button.addEventListener("click", () => {
-        view.model.set("count", getCount() + 1);
-        view.model.save_changes();
+        model.set("count", getCount() + 1);
+        model.save_changes();
       });
-      view.model.on("change:count", () => {
+      model.on("change:count", () => {
         button.innerHTML = `count is ${getCount()}`;
       });
-      view.el.appendChild(button);
+      el.appendChild(button);
     }
     """
     # Stateful property that can be accessed by JavaScript & Python
     count = traitlets.Int(0).tag(sync=True)
 ```
 
 Front-end code can also live in separate files (recommend):
```

