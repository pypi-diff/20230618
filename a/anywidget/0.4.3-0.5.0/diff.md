# Comparing `tmp/anywidget-0.4.3.tar.gz` & `tmp/anywidget-0.5.0.tar.gz`

## Comparing `anywidget-0.4.3.tar` & `anywidget-0.5.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 anywidget-0.4.3/CITATION.cff
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget.json
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 anywidget-0.4.3/package.json
--rw-r--r--   0        0        0   259862 2020-02-02 00:00:00.000000 anywidget-0.4.3/pnpm-lock.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.4.3/pnpm-workspace.yaml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.4.3/.changeset/config.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/__init__.py
--rw-r--r--   0        0        0    25087 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/_descriptor.py
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/_file_contents.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/_protocols.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/_util.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/_version.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/experimental.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/py.typed
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/widget.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/labextension/package.json
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/labextension/static/138.0afe77da678bd56cb574.js
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/labextension/static/326.34a64ac7689c2caccba1.js
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/labextension/static/remoteEntry.9d280f9a4b339dfca42d.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/nbextension/extension.js
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/nbextension/index.js
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/astro.config.js
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/package.json
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/tailwind.config.cjs
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/tsconfig.json
--rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/anywidget-overview.png
--rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/banner-dark.png
--rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/banner-light.png
--rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/banner-minimal.png
--rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/client-js-diagram.png
--rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/default-og-image.png
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/favicon.svg
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/make-scrollable-code-focusable.js
--rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/widget-overview.png
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/scripts/ipynb.mjs
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/scripts/render.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/scripts/utils.mjs
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/consts.ts
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/env.d.ts
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/languages.ts
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/util.ts
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/CodeHero.astro
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/ConfettiButton.astro
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/CounterButton.astro
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/HeadCommon.astro
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/HeadSEO.astro
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Hero.astro
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Footer/AvatarList.astro
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Footer/Footer.astro
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/AnyWidgetLogo.astro
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/AstroLogo.astro
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/Header.astro
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/HeaderButton.css
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/LanguageSelect.css
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/LanguageSelect.tsx
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/Search.css
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/Search.tsx
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/SidebarToggle.css
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/SidebarToggle.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/SkipToContent.astro
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/ThemeToggleButton.css
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/ThemeToggleButton.tsx
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/LeftSidebar/LeftSidebar.astro
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/PageContent/PageContent.astro
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/RightSidebar/MoreMenu.astro
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/RightSidebar/RightSidebar.astro
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/RightSidebar/TableOfContents.tsx
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/examples/Counter.astro
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/layouts/MainLayout.astro
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/layouts/SplashLayout.astro
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/pages/index.astro
--rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/pages/blog/anywidget-02.md
--rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/pages/blog/introducing-anywidget.mdx
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/pages/en/bundling.md
--rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/pages/en/experimental.md
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/pages/en/getting-started.mdx
--rw-r--r--   0        0        0    10622 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/pages/en/jupyter-widgets-the-good-parts.md
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/pages/en/notebooks/counter.ipynb
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/styles/index.css
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/styles/theme.css
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.4.3/examples/Counter.ipynb
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 anywidget-0.4.3/examples/minimal_example.ipynb
--rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 anywidget-0.4.3/packages/anywidget/CHANGELOG.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.4.3/packages/anywidget/build.mjs
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.4.3/packages/anywidget/package.json
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.4.3/packages/anywidget/src/index.js
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.4.3/packages/anywidget/src/plugin.js
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 anywidget-0.4.3/packages/anywidget/src/widget.js
--rw-r--r--   0        0        0    10214 2020-02-02 00:00:00.000000 anywidget-0.4.3/tests/test_descriptor.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 anywidget-0.4.3/tests/test_experimental.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.4.3/tests/test_file_contents.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.4.3/tests/test_protocols.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.4.3/tests/test_utils.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.4.3/tests/test_widget.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.4.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.4.3/LICENSE
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 anywidget-0.4.3/README.md
--rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 anywidget-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 anywidget-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 anywidget-0.5.0/CITATION.cff
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget.json
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 anywidget-0.5.0/package.json
+-rw-r--r--   0        0        0   259753 2020-02-02 00:00:00.000000 anywidget-0.5.0/pnpm-lock.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.5.0/pnpm-workspace.yaml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.5.0/.changeset/config.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/__init__.py
+-rw-r--r--   0        0        0    25087 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/_descriptor.py
+-rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/_file_contents.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/_protocols.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/_util.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/_version.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/experimental.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/py.typed
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/widget.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/labextension/package.json
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/labextension/static/138.2f08930b7b6074de7077.js
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/labextension/static/326.fa2e8950755c9713ac12.js
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/labextension/static/remoteEntry.3346a2ae3844083123da.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/nbextension/extension.js
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 anywidget-0.5.0/anywidget/nbextension/index.js
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/astro.config.js
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/package.json
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/tailwind.config.cjs
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/tsconfig.json
+-rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/anywidget-overview.png
+-rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/banner-dark.png
+-rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/banner-light.png
+-rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/banner-minimal.png
+-rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/client-js-diagram.png
+-rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/default-og-image.png
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/favicon.svg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/make-scrollable-code-focusable.js
+-rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/public/widget-overview.png
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/scripts/ipynb.mjs
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/scripts/render.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/scripts/utils.mjs
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/consts.ts
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/env.d.ts
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/languages.ts
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/util.ts
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/CodeHero.astro
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/ConfettiButton.astro
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/CounterButton.astro
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/HeadCommon.astro
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/HeadSEO.astro
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Hero.astro
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Footer/AvatarList.astro
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Footer/Footer.astro
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/AnyWidgetLogo.astro
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/AstroLogo.astro
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/Header.astro
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/HeaderButton.css
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/LanguageSelect.css
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/LanguageSelect.tsx
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/Search.css
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/Search.tsx
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/SidebarToggle.css
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/SidebarToggle.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/SkipToContent.astro
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/ThemeToggleButton.css
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/Header/ThemeToggleButton.tsx
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/LeftSidebar/LeftSidebar.astro
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/PageContent/PageContent.astro
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/RightSidebar/MoreMenu.astro
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/RightSidebar/RightSidebar.astro
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/RightSidebar/TableOfContents.tsx
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/components/examples/Counter.astro
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/layouts/MainLayout.astro
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/layouts/SplashLayout.astro
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/pages/index.astro
+-rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/pages/blog/anywidget-02.md
+-rw-r--r--   0        0        0    22438 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/pages/blog/introducing-anywidget.mdx
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/pages/en/bundling.md
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/pages/en/experimental.md
+-rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/pages/en/getting-started.mdx
+-rw-r--r--   0        0        0    10534 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/pages/en/notebooks/counter.ipynb
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/styles/index.css
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.5.0/docs/src/styles/theme.css
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.5.0/examples/Counter.ipynb
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 anywidget-0.5.0/examples/minimal_example.ipynb
+-rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 anywidget-0.5.0/packages/anywidget/CHANGELOG.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.5.0/packages/anywidget/build.mjs
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.5.0/packages/anywidget/package.json
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.5.0/packages/anywidget/src/index.js
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.5.0/packages/anywidget/src/plugin.js
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 anywidget-0.5.0/packages/anywidget/src/widget.js
+-rw-r--r--   0        0        0    10214 2020-02-02 00:00:00.000000 anywidget-0.5.0/tests/test_descriptor.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 anywidget-0.5.0/tests/test_experimental.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.5.0/tests/test_file_contents.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.5.0/tests/test_protocols.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.5.0/tests/test_utils.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.5.0/tests/test_widget.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 anywidget-0.5.0/README.md
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 anywidget-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 anywidget-0.5.0/PKG-INFO
```

### Comparing `anywidget-0.4.3/.pre-commit-config.yaml` & `anywidget-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/CITATION.cff` & `anywidget-0.5.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/package.json` & `anywidget-0.5.0/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/pnpm-lock.yaml` & `anywidget-0.5.0/pnpm-lock.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -106,19 +106,15 @@
         specifier: ^2 || ^3 || ^4 || ^5 || ^6
         version: 6.0.2(crypto@1.0.1)
     devDependencies:
       '@jupyterlab/builder':
         specifier: ^3.6.2
         version: 3.6.2(crypto@1.0.1)(esbuild@0.17.12)
 
-  packages/types:
-    dependencies:
-      '@jupyter-widgets/base':
-        specifier: ^6.0.1
-        version: 6.0.2(crypto@1.0.1)
+  packages/types: {}
 
   packages/vite:
     devDependencies:
       vite:
         specifier: ^4.1.4
         version: 4.1.4(@types/node@18.14.6)
```

### Comparing `anywidget-0.4.3/anywidget/_descriptor.py` & `anywidget-0.5.0/anywidget/_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/anywidget/_file_contents.py` & `anywidget-0.5.0/anywidget/_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/anywidget/_protocols.py` & `anywidget-0.5.0/anywidget/_protocols.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/anywidget/_util.py` & `anywidget-0.5.0/anywidget/_util.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/anywidget/experimental.py` & `anywidget-0.5.0/anywidget/experimental.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/anywidget/widget.py` & `anywidget-0.5.0/anywidget/widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/anywidget/labextension/package.json` & `anywidget-0.5.0/anywidget/labextension/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95703125%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.3346a2ae3844083123da.js'}}",*

 * * "'version'": "'0.5.0'"}*

```diff
@@ -22,15 +22,15 @@
     },
     "files": [
         "dist"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.9d280f9a4b339dfca42d.js"
+            "load": "static/remoteEntry.3346a2ae3844083123da.js"
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
-    "version": "0.4.3"
+    "version": "0.5.0"
 }
```

### Comparing `anywidget-0.4.3/anywidget/labextension/static/138.0afe77da678bd56cb574.js` & `anywidget-0.5.0/anywidget/labextension/static/326.fa2e8950755c9713ac12.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,102 +1,144 @@
 "use strict";
 (self.webpackChunkanywidget = self.webpackChunkanywidget || []).push([
-    [138], {
-        138: (e, t, i) => {
-            i.r(t), i(203), define(["@jupyter-widgets/base"], create)
+    [326], {
+        326: (e, t, n) => {
+            n.r(t), n.d(t, {
+                default: () => s
+            });
+            var i = n(395),
+                a = n(203),
+                d = n(147);
+            const s = {
+                id: `${d.u2}:plugin`,
+                requires: [i.IJupyterWidgetRegistry],
+                activate: (e, t) => {
+                    let n = (0, a.Z)(i);
+                    t.registerWidget({
+                        name: d.u2,
+                        version: d.i8,
+                        exports: n
+                    })
+                },
+                autoStart: !0
+            }
         },
-        203: (e, t, i) => {
-            i.d(t, {
+        203: (e, t, n) => {
+            n.d(t, {
                 Z: () => c
             });
-            var n = i(147);
+            var i = n(147);
 
             function a(e) {
                 return e.startsWith("http://") || e.startsWith("https://")
             }
-            async function s(e, t) {
+            async function d(e, t) {
                 if (e) return a(e) ? async function(e, t) {
-                    let i = document.querySelector(`link[id='${t}']`);
-                    if (i) {
-                        let t = i.cloneNode();
-                        return t.href = e, t.addEventListener("load", (() => i?.remove())), void i.after(t)
+                    let n = document.querySelector(`link[id='${t}']`);
+                    if (n) {
+                        let t = n.cloneNode();
+                        return t.href = e, t.addEventListener("load", (() => n?.remove())), void n.after(t)
                     }
                     return new Promise((t => {
-                        let i = Object.assign(document.createElement("link"), {
+                        let n = Object.assign(document.createElement("link"), {
                             rel: "stylesheet",
                             href: e,
                             onload: t
                         });
-                        document.head.appendChild(i)
+                        document.head.appendChild(n)
                     }))
                 }(e, t): function(e, t) {
-                    let i = document.querySelector(`style[id='${t}']`);
-                    if (i) return void(i.textContent = e);
-                    let n = Object.assign(document.createElement("style"), {
+                    let n = document.querySelector(`style[id='${t}']`);
+                    if (n) return void(n.textContent = e);
+                    let i = Object.assign(document.createElement("style"), {
                         id: t,
                         type: "text/css"
                     });
-                    n.appendChild(document.createTextNode(e)), document.head.appendChild(n)
+                    i.appendChild(document.createTextNode(e)), document.head.appendChild(i)
                 }(e, t)
             }
-            async function d(e) {
+            async function s(e) {
                 if (a(e)) return import(e);
-                let t, i = URL.createObjectURL(new Blob([e], {
+                let t, n = URL.createObjectURL(new Blob([e], {
                     type: "text/javascript"
                 }));
                 try {
-                    t = await import(i)
+                    t = await import(n)
                 } catch (e) {
                     throw console.log(e), e
                 }
-                return URL.revokeObjectURL(i), t
+                return URL.revokeObjectURL(n), t
+            }
+
+            function o(e) {
+                return {
+                    model: {
+                        get: e.model.get.bind(e.model),
+                        set: e.model.set.bind(e.model),
+                        save_changes: e.model.save_changes.bind(e.model),
+                        on(t, n) {
+                            e.model.on(t, n, e)
+                        },
+                        off(t, n) {
+                            e.model.off(t, n, e)
+                        }
+                    },
+                    el: e.el
+                }
             }
 
-            function c(e) {
-                class t extends e.DOMWidgetModel {
+            function c({
+                DOMWidgetModel: e,
+                DOMWidgetView: t
+            }) {
+                class n extends e {
                     static model_name = "AnyModel";
-                    static model_module = n.u2;
-                    static model_module_version = n.i8;
+                    static model_module = i.u2;
+                    static model_module_version = i.i8;
                     static view_name = "AnyView";
-                    static view_module = n.u2;
-                    static view_module_version = n.i8;
+                    static view_module = i.u2;
+                    static view_module_version = i.i8;
                     initialize(...e) {
                         super.initialize(...e), this.on("change:_css", (() => {
                             let e = this.get("_anywidget_id");
-                            e && (console.debug(`[anywidget] css hot updated: ${e}`), s(this.get("_css"), e))
+                            e && (console.debug(`[anywidget] css hot updated: ${e}`), d(this.get("_css"), e))
                         })), this.on("change:_esm", (async () => {
                             let e = this.get("_anywidget_id");
                             if (!e) return;
                             console.debug(`[anywidget] esm hot updated: ${e}`);
                             let t = Object.values(this.views ?? {});
                             for await (let e of t) {
-                                let t = await d(this.get("_esm"));
-                                await e._anywidget_cached_cleanup(), e.$el.empty(), e.stopListening(this);
-                                let i = await t.render(e);
-                                e._anywidget_cached_cleanup = i ?? (() => {})
+                                let t = await s(this.get("_esm"));
+                                try {
+                                    await e._anywidget_cached_cleanup()
+                                } catch (t) {
+                                    console.warn("[anywidget] error cleaning up previous module.", t), e._anywidget_cached_cleanup = () => {}
+                                }
+                                this.off(null, null, e), e.$el.empty();
+                                let n = await t.render(o(e));
+                                e._anywidget_cached_cleanup = n ?? (() => {})
                             }
                         }))
                     }
                 }
-                class i extends e.DOMWidgetView {
-                    async render() {
-                        await s(this.model.get("_css"), this.model.get("_anywidget_id"));
-                        let e = await d(this.model.get("_esm")),
-                            t = await e.render(this);
-                        this._anywidget_cached_cleanup = t ?? (() => {})
-                    }
-                    _anywidget_cached_cleanup() {}
-                    async remove() {
-                        return await this._anywidget_cached_cleanup(), super.remove()
-                    }
-                }
                 return {
-                    AnyModel: t,
-                    AnyView: i
+                    AnyModel: n,
+                    AnyView: class extends t {
+                        async render() {
+                            await d(this.model.get("_css"), this.model.get("_anywidget_id"));
+                            let e = await s(this.model.get("_esm")),
+                                t = await e.render(o(this));
+                            this._anywidget_cached_cleanup = t ?? (() => {})
+                        }
+                        _anywidget_cached_cleanup() {}
+                        async remove() {
+                            return await this._anywidget_cached_cleanup(), super.remove()
+                        }
+                    }
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.4.3"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.5.0"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.4.3/anywidget/labextension/static/326.34a64ac7689c2caccba1.js` & `anywidget-0.5.0/anywidget/labextension/static/138.2f08930b7b6074de7077.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,120 +1,126 @@
 "use strict";
 (self.webpackChunkanywidget = self.webpackChunkanywidget || []).push([
-    [326], {
-        326: (e, t, i) => {
-            i.r(t), i.d(t, {
-                default: () => d
-            });
-            var n = i(395),
-                a = i(203),
-                s = i(147);
-            const d = {
-                id: `${s.u2}:plugin`,
-                requires: [n.IJupyterWidgetRegistry],
-                activate: (e, t) => {
-                    let i = (0, a.Z)(n);
-                    t.registerWidget({
-                        name: s.u2,
-                        version: s.i8,
-                        exports: i
-                    })
-                },
-                autoStart: !0
-            }
+    [138], {
+        138: (e, t, n) => {
+            n.r(t), n(203), define(["@jupyter-widgets/base"], create)
         },
-        203: (e, t, i) => {
-            i.d(t, {
+        203: (e, t, n) => {
+            n.d(t, {
                 Z: () => c
             });
-            var n = i(147);
+            var i = n(147);
 
             function a(e) {
                 return e.startsWith("http://") || e.startsWith("https://")
             }
-            async function s(e, t) {
+            async function d(e, t) {
                 if (e) return a(e) ? async function(e, t) {
-                    let i = document.querySelector(`link[id='${t}']`);
-                    if (i) {
-                        let t = i.cloneNode();
-                        return t.href = e, t.addEventListener("load", (() => i?.remove())), void i.after(t)
+                    let n = document.querySelector(`link[id='${t}']`);
+                    if (n) {
+                        let t = n.cloneNode();
+                        return t.href = e, t.addEventListener("load", (() => n?.remove())), void n.after(t)
                     }
                     return new Promise((t => {
-                        let i = Object.assign(document.createElement("link"), {
+                        let n = Object.assign(document.createElement("link"), {
                             rel: "stylesheet",
                             href: e,
                             onload: t
                         });
-                        document.head.appendChild(i)
+                        document.head.appendChild(n)
                     }))
                 }(e, t): function(e, t) {
-                    let i = document.querySelector(`style[id='${t}']`);
-                    if (i) return void(i.textContent = e);
-                    let n = Object.assign(document.createElement("style"), {
+                    let n = document.querySelector(`style[id='${t}']`);
+                    if (n) return void(n.textContent = e);
+                    let i = Object.assign(document.createElement("style"), {
                         id: t,
                         type: "text/css"
                     });
-                    n.appendChild(document.createTextNode(e)), document.head.appendChild(n)
+                    i.appendChild(document.createTextNode(e)), document.head.appendChild(i)
                 }(e, t)
             }
-            async function d(e) {
+            async function s(e) {
                 if (a(e)) return import(e);
-                let t, i = URL.createObjectURL(new Blob([e], {
+                let t, n = URL.createObjectURL(new Blob([e], {
                     type: "text/javascript"
                 }));
                 try {
-                    t = await import(i)
+                    t = await import(n)
                 } catch (e) {
                     throw console.log(e), e
                 }
-                return URL.revokeObjectURL(i), t
+                return URL.revokeObjectURL(n), t
+            }
+
+            function o(e) {
+                return {
+                    model: {
+                        get: e.model.get.bind(e.model),
+                        set: e.model.set.bind(e.model),
+                        save_changes: e.model.save_changes.bind(e.model),
+                        on(t, n) {
+                            e.model.on(t, n, e)
+                        },
+                        off(t, n) {
+                            e.model.off(t, n, e)
+                        }
+                    },
+                    el: e.el
+                }
             }
 
-            function c(e) {
-                class t extends e.DOMWidgetModel {
+            function c({
+                DOMWidgetModel: e,
+                DOMWidgetView: t
+            }) {
+                class n extends e {
                     static model_name = "AnyModel";
-                    static model_module = n.u2;
-                    static model_module_version = n.i8;
+                    static model_module = i.u2;
+                    static model_module_version = i.i8;
                     static view_name = "AnyView";
-                    static view_module = n.u2;
-                    static view_module_version = n.i8;
+                    static view_module = i.u2;
+                    static view_module_version = i.i8;
                     initialize(...e) {
                         super.initialize(...e), this.on("change:_css", (() => {
                             let e = this.get("_anywidget_id");
-                            e && (console.debug(`[anywidget] css hot updated: ${e}`), s(this.get("_css"), e))
+                            e && (console.debug(`[anywidget] css hot updated: ${e}`), d(this.get("_css"), e))
                         })), this.on("change:_esm", (async () => {
                             let e = this.get("_anywidget_id");
                             if (!e) return;
                             console.debug(`[anywidget] esm hot updated: ${e}`);
                             let t = Object.values(this.views ?? {});
                             for await (let e of t) {
-                                let t = await d(this.get("_esm"));
-                                await e._anywidget_cached_cleanup(), e.$el.empty(), e.stopListening(this);
-                                let i = await t.render(e);
-                                e._anywidget_cached_cleanup = i ?? (() => {})
+                                let t = await s(this.get("_esm"));
+                                try {
+                                    await e._anywidget_cached_cleanup()
+                                } catch (t) {
+                                    console.warn("[anywidget] error cleaning up previous module.", t), e._anywidget_cached_cleanup = () => {}
+                                }
+                                this.off(null, null, e), e.$el.empty();
+                                let n = await t.render(o(e));
+                                e._anywidget_cached_cleanup = n ?? (() => {})
                             }
                         }))
                     }
                 }
-                class i extends e.DOMWidgetView {
-                    async render() {
-                        await s(this.model.get("_css"), this.model.get("_anywidget_id"));
-                        let e = await d(this.model.get("_esm")),
-                            t = await e.render(this);
-                        this._anywidget_cached_cleanup = t ?? (() => {})
-                    }
-                    _anywidget_cached_cleanup() {}
-                    async remove() {
-                        return await this._anywidget_cached_cleanup(), super.remove()
-                    }
-                }
                 return {
-                    AnyModel: t,
-                    AnyView: i
+                    AnyModel: n,
+                    AnyView: class extends t {
+                        async render() {
+                            await d(this.model.get("_css"), this.model.get("_anywidget_id"));
+                            let e = await s(this.model.get("_esm")),
+                                t = await e.render(o(this));
+                            this._anywidget_cached_cleanup = t ?? (() => {})
+                        }
+                        _anywidget_cached_cleanup() {}
+                        async remove() {
+                            return await this._anywidget_cached_cleanup(), super.remove()
+                        }
+                    }
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.4.3"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.5.0"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.4.3/anywidget/labextension/static/remoteEntry.9d280f9a4b339dfca42d.js` & `anywidget-0.5.0/anywidget/labextension/static/remoteEntry.3346a2ae3844083123da.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, d, s, f, c, p, h, v = {
+    var e, r, t, n, o, a, i, u, f, l, s, d, p, c, h, v = {
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
 
-    function m(e) {
+    function b(e) {
         var r = g[e];
         if (void 0 !== r) return r.exports;
         var t = g[e] = {
             exports: {}
         };
-        return v[e](t, t.exports, m), t.exports
+        return v[e](t, t.exports, b), t.exports
     }
-    m.m = v, m.c = g, m.n = e => {
+    b.m = v, b.c = g, b.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return m.d(r, {
+        return b.d(r, {
             a: r
         }), r
-    }, m.d = (e, r) => {
-        for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
+    }, b.d = (e, r) => {
+        for (var t in r) b.o(r, t) && !b.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        138: "0afe77da678bd56cb574",
-        326: "34a64ac7689c2caccba1"
+    }, b.f = {}, b.e = e => Promise.all(Object.keys(b.f).reduce(((r, t) => (b.f[t](e, r), r)), [])), b.u = e => e + "." + {
+        138: "2f08930b7b6074de7077",
+        326: "fa2e8950755c9713ac12"
     } [e] + ".js?v=" + {
-        138: "0afe77da678bd56cb574",
-        326: "34a64ac7689c2caccba1"
-    } [e], m.g = function() {
+        138: "2f08930b7b6074de7077",
+        326: "fa2e8950755c9713ac12"
+    } [e], b.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", m.l = (t, n, o, a) => {
+    }(), b.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", b.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
-                    var s = l[d];
+                for (var f = document.getElementsByTagName("script"), l = 0; l < f.length; l++) {
+                    var s = f[l];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
                         i = s;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var f = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, b.nc && i.setAttribute("nonce", b.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            var d = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, m.r = e => {
+    }, b.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        m.S = {};
+        b.S = {};
         var e = {},
             r = {};
-        m.I = (t, n) => {
+        b.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                m.o(m.S, t) || (m.S[t] = {});
-                var a = m.S[t],
+                b.o(b.S, t) || (b.S[t] = {});
+                var a = b.S[t],
                     i = "anywidget",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => m.e(138).then((() => () => m(138))),
+                        get: () => b.e(138).then((() => () => b(138))),
                         from: i,
                         eager: !1
                     })
-                })("anywidget", "0.4.3"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("anywidget", "0.5.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        m.g.importScripts && (e = m.g.location + "");
-        var r = m.g.document;
+        b.g.importScripts && (e = b.g.location + "");
+        var r = b.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             t.length && (e = t[t.length - 1].src)
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), b.p = e
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
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
+            i.push(0 === u ? "not(" + f() + ")" : 1 === u ? "(" + f() + " || " + f() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
-        return l();
+        return f();
 
-        function l() {
+        function f() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var d, s, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
+            for (var i = 0, u = 1, f = !0;; u++, i++) {
+                var l, s, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(l = r[i]))[0])) return !f || ("u" == d ? u > n && !o : "" == d != o);
                 if ("u" == s) {
-                    if (!l || "u" != f) return !1
-                } else if (l)
-                    if (f == s)
+                    if (!f || "u" != d) return !1
+                } else if (f)
+                    if (d == s)
                         if (u <= n) {
-                            if (d != e[u]) return !1
+                            if (l != e[u]) return !1
                         } else {
-                            if (o ? d > e[u] : d < e[u]) return !1;
-                            d != e[u] && (l = !1)
+                            if (o ? l > e[u] : l < e[u]) return !1;
+                            l != e[u] && (f = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
-                    l = !1, u--
+                    f = !1, u--
                 } else {
-                    if (u <= n || s < f != o) return !1;
-                    l = !1
-                } else "s" != f && "n" != f && (l = !1, u--)
+                    if (u <= n || s < d != o) return !1;
+                    f = !1
+                } else "s" != d && "n" != d && (f = !1, u--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
-        return !!p()
+        return !!c()
     }, i = (e, r) => {
-        var t = m.S[e];
-        if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = b.S[e];
+        if (!t || !b.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", d = (e, r, t, n) => {
+    }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), s(e[t][o])
-    }, s = e => (e.loaded = 1, e.get()), f = (e => function(r, t, n, o) {
-        var a = m.I(r);
-        return a && a.then ? a.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), c = {}, p = {
-        395: () => f("default", "@jupyter-widgets/base", [, [1, 6],
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(f(e, t, o, n)), s(e[t][o])
+    }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
+        var a = b.I(r);
+        return a && a.then ? a.then(e.bind(e, r, b.S[r], t, n, o)) : e(r, b.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), l(r, 0, t, n)))), p = {}, c = {
+        395: () => d("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
         ])
     }, h = {
         326: [395]
-    }, m.f.consumes = (e, r) => {
-        m.o(h, e) && h[e].forEach((e => {
-            if (m.o(c, e)) return r.push(c[e]);
+    }, b.f.consumes = (e, r) => {
+        b.o(h, e) && h[e].forEach((e => {
+            if (b.o(p, e)) return r.push(p[e]);
             var t = r => {
-                    c[e] = 0, m.m[e] = t => {
-                        delete m.c[e], t.exports = r()
+                    p[e] = 0, b.m[e] = t => {
+                        delete b.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete c[e], m.m[e] = t => {
-                        throw delete m.c[e], r
+                    delete p[e], b.m[e] = t => {
+                        throw delete b.c[e], r
                     }
                 };
             try {
-                var o = p[e]();
-                o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
+                var o = c[e]();
+                o.then ? r.push(p[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             957: 0
         };
-        m.f.j = (r, t) => {
-            var n = m.o(e, r) ? e[r] : void 0;
+        b.f.j = (r, t) => {
+            var n = b.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var a = m.p + m.u(r),
+                    var a = b.p + b.u(r),
                         i = new Error;
-                    m.l(a, (t => {
-                        if (m.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    b.l(a, (t => {
+                        if (b.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
                                 a = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
-                    l = 0;
+                    f = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) m.o(i, n) && (m.m[n] = i[n]);
-                    u && u(m)
+                    for (n in i) b.o(i, n) && (b.m[n] = i[n]);
+                    u && u(b)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); f < a.length; f++) o = a[f], b.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkanywidget = self.webpackChunkanywidget || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var y = m(408);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = y
+    var m = b(408);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).anywidget = m
 })();
```

### Comparing `anywidget-0.4.3/anywidget/nbextension/index.js` & `anywidget-0.5.0/anywidget/nbextension/index.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 // package.json
 var name = "anywidget";
-var version = "0.4.3";
+var version = "0.5.0";
 
 // src/widget.js
 function is_href(str) {
     return str.startsWith("http://") || str.startsWith("https://");
 }
 async function load_css_href(href, anywidget_id) {
     let prev = document.querySelector(`link[id='${anywidget_id}']`);
@@ -70,23 +70,53 @@
         console.log(e);
         throw e;
     }
     URL.revokeObjectURL(url);
     return widget;
 }
 
-function widget_default(base) {
-    class AnyModel extends base.DOMWidgetModel {
+function extract_context(view) {
+    let model = {
+        /** @param {string} name */
+        get: view.model.get.bind(view.model),
+        set: view.model.set.bind(view.model),
+        save_changes: view.model.save_changes.bind(view.model),
+        /**
+         * @param {string} name
+         * @param {any} callback
+         */
+        on(name2, callback) {
+            view.model.on(name2, callback, view);
+        },
+        /**
+         * @param {string} name
+         * @param {any} callback
+         */
+        off(name2, callback) {
+            view.model.off(name2, callback, view);
+        }
+    };
+    return {
+        model,
+        el: view.el
+    };
+}
+
+function widget_default({
+    DOMWidgetModel,
+    DOMWidgetView
+}) {
+    class AnyModel extends DOMWidgetModel {
         static model_name = "AnyModel";
         static model_module = name;
         static model_module_version = version;
         static view_name = "AnyView";
         static view_module = name;
         static view_module_version = version;
-        /** @param {Parameters<InstanceType<base["DOMWidgetModel"]>["initialize"]>} args */
+        /** @param {Parameters<InstanceType<DOMWidgetModel>["initialize"]>} args */
         initialize(...args) {
             super.initialize(...args);
             this.on("change:_css", () => {
                 let id = this.get("_anywidget_id");
                 if (!id)
                     return;
                 console.debug(`[anywidget] css hot updated: ${id}`);
@@ -94,33 +124,42 @@
             });
             this.on("change:_esm", async () => {
                 let id = this.get("_anywidget_id");
                 if (!id)
                     return;
                 console.debug(`[anywidget] esm hot updated: ${id}`);
                 let views = (
-                    /** @type {Promise<AnyView>[]} */
+                    /** @type {unknown} */
                     Object.values(this.views ?? {})
                 );
-                for await (let view of views) {
+                for await (
+                    let view of
+                        /** @type {Promise<AnyView>[]} */
+                        views
+                ) {
                     let widget = await load_esm(this.get("_esm"));
-                    await view._anywidget_cached_cleanup();
+                    try {
+                        await view._anywidget_cached_cleanup();
+                    } catch (e) {
+                        console.warn("[anywidget] error cleaning up previous module.", e);
+                        view._anywidget_cached_cleanup = () => {};
+                    }
+                    this.off(null, null, view);
                     view.$el.empty();
-                    view.stopListening(this);
-                    let cleanup = await widget.render(view);
+                    let cleanup = await widget.render(extract_context(view));
                     view._anywidget_cached_cleanup = cleanup ?? (() => {});
                 }
             });
         }
     }
-    class AnyView extends base.DOMWidgetView {
+    class AnyView extends DOMWidgetView {
         async render() {
             await load_css(this.model.get("_css"), this.model.get("_anywidget_id"));
             let widget = await load_esm(this.model.get("_esm"));
-            let cleanup = await widget.render(this);
+            let cleanup = await widget.render(extract_context(this));
             this._anywidget_cached_cleanup = cleanup ?? (() => {});
         }
         /** @type {() => Promise<void> | void} */
         _anywidget_cached_cleanup() {}
         async remove() {
             await this._anywidget_cached_cleanup();
             return super.remove();
```

### Comparing `anywidget-0.4.3/docs/README.md` & `anywidget-0.5.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/astro.config.js` & `anywidget-0.5.0/docs/astro.config.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/package.json` & `anywidget-0.5.0/docs/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/public/anywidget-overview.png` & `anywidget-0.5.0/docs/public/anywidget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/public/banner-dark.png` & `anywidget-0.5.0/docs/public/banner-dark.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/public/banner-light.png` & `anywidget-0.5.0/docs/public/banner-light.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/public/banner-minimal.png` & `anywidget-0.5.0/docs/public/banner-minimal.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/public/client-js-diagram.png` & `anywidget-0.5.0/docs/public/client-js-diagram.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/public/default-og-image.png` & `anywidget-0.5.0/docs/public/default-og-image.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/public/favicon.svg` & `anywidget-0.5.0/docs/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/public/widget-overview.png` & `anywidget-0.5.0/docs/public/widget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/scripts/ipynb.mjs` & `anywidget-0.5.0/docs/scripts/ipynb.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/scripts/utils.mjs` & `anywidget-0.5.0/docs/scripts/utils.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/consts.ts` & `anywidget-0.5.0/docs/src/consts.ts`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/CodeHero.astro` & `anywidget-0.5.0/docs/src/components/CodeHero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/CounterButton.astro` & `anywidget-0.5.0/docs/src/components/CounterButton.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/HeadCommon.astro` & `anywidget-0.5.0/docs/src/components/HeadCommon.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/HeadSEO.astro` & `anywidget-0.5.0/docs/src/components/HeadSEO.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/Hero.astro` & `anywidget-0.5.0/docs/src/components/Hero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/Footer/AvatarList.astro` & `anywidget-0.5.0/docs/src/components/Footer/AvatarList.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/Header/AnyWidgetLogo.astro` & `anywidget-0.5.0/docs/src/components/Header/AnyWidgetLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/Header/AstroLogo.astro` & `anywidget-0.5.0/docs/src/components/Header/AstroLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/Header/Header.astro` & `anywidget-0.5.0/docs/src/components/Header/Header.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/Header/HeaderButton.css` & `anywidget-0.5.0/docs/src/components/Header/HeaderButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/Header/LanguageSelect.css` & `anywidget-0.5.0/docs/src/components/Header/LanguageSelect.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/Header/LanguageSelect.tsx` & `anywidget-0.5.0/docs/src/components/Header/LanguageSelect.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/Header/Search.css` & `anywidget-0.5.0/docs/src/components/Header/Search.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/Header/Search.tsx` & `anywidget-0.5.0/docs/src/components/Header/Search.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/Header/SidebarToggle.tsx` & `anywidget-0.5.0/docs/src/components/Header/SidebarToggle.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/Header/ThemeToggleButton.css` & `anywidget-0.5.0/docs/src/components/Header/ThemeToggleButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/Header/ThemeToggleButton.tsx` & `anywidget-0.5.0/docs/src/components/Header/ThemeToggleButton.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/LeftSidebar/LeftSidebar.astro` & `anywidget-0.5.0/docs/src/components/LeftSidebar/LeftSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/PageContent/PageContent.astro` & `anywidget-0.5.0/docs/src/components/PageContent/PageContent.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/RightSidebar/MoreMenu.astro` & `anywidget-0.5.0/docs/src/components/RightSidebar/MoreMenu.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/RightSidebar/RightSidebar.astro` & `anywidget-0.5.0/docs/src/components/RightSidebar/RightSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/RightSidebar/TableOfContents.tsx` & `anywidget-0.5.0/docs/src/components/RightSidebar/TableOfContents.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/components/examples/Counter.astro` & `anywidget-0.5.0/docs/src/components/examples/Counter.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/layouts/MainLayout.astro` & `anywidget-0.5.0/docs/src/layouts/MainLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/layouts/SplashLayout.astro` & `anywidget-0.5.0/docs/src/layouts/SplashLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/pages/blog/anywidget-02.md` & `anywidget-0.5.0/docs/src/pages/blog/anywidget-02.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/pages/blog/introducing-anywidget.mdx` & `anywidget-0.5.0/docs/src/pages/blog/introducing-anywidget.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -439,16 +439,16 @@
 ... and each subclass specifies:
 
 - `_esm` the <u>**required**</u> ECMAScript module for the widget. It must
   export a `render` function to define custom rendering logic and initialize dynamic
   updates for the widget.
 
 ```javascript
-/** @param {import("@jupyter-widgets/base").DOMWidgetView} */
-export function render(view) {
+/** @param {{ model: DOMWidgetModel, el: HTMLElement }} context */
+export function render({ model, el }) {
 	// Render model contents and setup dynamic updates
 }
 ```
 
 - `_css` an <u>**optional**</u> CSS stylesheet to load for the widget.
 
 All custom stateful properties (e.g., `ExampleWidget.value`) are defined via [`traitlets`](https://ipywidgets.readthedocs.io/en/8.0.2/examples/Widget%20Custom.html#sync=True-traitlets)
@@ -552,16 +552,16 @@
 [PyPI](https://pypi.org/project/anywidget/). To install, just run:
 
 ```bash
 pip install anywidget
 ```
 
 **anywidget** is new and still under active development. **It should _not_
-yet be used in production since the API can change and some critical features are missing**
-(e.g., APIs to extend the `DOMWidgetModel` with custom serializers and `DOMWidgetView` with lifecycle hooks). With that said, it is already [in use](https://github.com/vitessce/vitessce-python) and ready for testing.
+yet be used in production since the API can change and some critical features are missing**.
+With that said, it is already [in use](https://github.com/vitessce/vitessce-python) and ready for testing.
 
 I hope using **anywidget** is simple and enjoyable. I have personally found
 it valuable in my work as a visualization researcher to quickly iterate on new
 ideas to interactively explore biomedical datasets.
 
 If **anywidget** is interesting or exciting to you, please reach out and get involved
 on [GitHub](https://github.com/manzt/anywidget)! Happy coding.
```

### Comparing `anywidget-0.4.3/docs/src/pages/en/bundling.md` & `anywidget-0.5.0/docs/src/pages/en/bundling.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/pages/en/experimental.md` & `anywidget-0.5.0/docs/src/pages/en/experimental.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/pages/en/getting-started.mdx` & `anywidget-0.5.0/docs/src/pages/en/getting-started.mdx`

 * *Files 5% similar despite different names*

```diff
@@ -74,42 +74,42 @@
 - `_css` specifies an <u>**optional**</u> CSS stylesheet to load for the widget. It can be a full URL or plain text. Styles are loaded
   in the global scope if using this feature, so take care in avoid global overrides.
 
 - `_esm` specifies a <u>**required**</u> [ECMAScript module](https://nodejs.org/api/esm.html) for the widget.
   It must _must_ export a `render` custom rendering logic and initializes dynamic updates for the custom widget.
 
 ```javascript
-/** @param view {import("@jupyter-widgets/base").DOMWidgetView} */
-export function render(view) {
+/** @param {{ model: DOMWidgetModel, el: HTMLElement }} context */
+export function render({ model, el }) {
 	// Render model contents and setup dynamic updates
 	// See Jupyter widgets docs for more information: https://ipywidgets.readthedocs.io/en/8.0.2/examples/Widget%20Custom.html#Rendering-model-contents
 }
 ```
 
 ECMAScript modules are the offical standard format to package JavaScript code for reuse and are supported
 natively across [all major browsers](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules#javascript.statements.export).
 Therefore, dependencies can be imported directly via a fully qualified URL.
 
 ```javascript
 import * as d3 from "https://esm.sh/d3@7";
 
-/** @param view {import("@jupyter-widgets/base").DOMWidgetView} */
-export function render(view) {
-	let selection = d3.select(view.el);
+/** @param {{ model: DOMWidgetModel, el: HTMLElement }} context */
+export function render({ model, el }) {
+	let selection = d3.select(el);
 	/* ... */
 }
 ```
 
 The `render` function can also (optionally) return a callback that is executed any time the view is
 removed from the DOM. This feature is useful when dealing with complex event listeners, subscriptions,
 or third-party libraries that require proper teardwon.
 
 ```javascript
-/** @param view {import("@jupyter-widgets/base").DOMWidgetView} */
-export function render(view) {
+/** @param {{ model: DOMWidgetModel, el: HTMLElement }} context */
+export function render({ model, el }) {
 	// Create DOM elements and set up subscribers
 	return () => {
 		// Optionally cleanup
 	};
 }
 ```
```

### Comparing `anywidget-0.4.3/docs/src/pages/en/jupyter-widgets-the-good-parts.md` & `anywidget-0.5.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,17 @@
 This section frames the Juptyer Widgets documentation in the context of **anywidget**.
 Remember that **anywidget** is just abstraction over traditional Jupyter Widgets
 that removes boilerplate and packaging details.
 
 ### Comparison with traditional Jupyter Widgets
 
 **anywidget** simplies creating your widget's front-end code. Its only requirement
-is that your widget front-end code is a valid [JavaScript module](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules) and exports a function
-called `render`. This `render` function just an alias for the traditional
-[`DOMWidgetView.render`](https://ipywidgets.readthedocs.io/en/8.0.2/examples/Widget%20Custom.html#Render-method) method,
-except that your Widget's view is passed as the first argument.
+is that your widget front-end code is a valid [JavaScript module](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules) 
+and exports a function called `render`. This `render` function is similar to the traditional
+[`DOMWidgetView.render`](https://ipywidgets.readthedocs.io/en/8.0.2/examples/Widget%20Custom.html#Render-method).
 
 Concretely, custom widgets are traditionally defined like:
 
 ```javascript
 import { DOMWidgetModel, DOMWidgetView } from "@jupyter-widgets/base";
 
 // All boilerplate, anywidget takes care of this ...
@@ -45,51 +44,50 @@
 }
 
 export { CustomModel, CustomView };
 ```
 
 ... which must be transformed, bundled, and installed in multiple notebook environments.
 
-In **anywidget**, the above code simplies to just:
+In **anywidget**, the above code simplies to:
 
 ```javascript
-/** @param view {DOMWidgetView} view */
-export function render(view) {
-	let el = view.el;
-	let model = view.model;
+/** @param {{ model: DOMWidgetModel, el: HTMLElement }} context */
+export function render(context) {
+	let el = context.el;
+	let model = context.model;
 	/* ... */
 }
 ```
 
-... which explicity defines the widget view (i.e., `CustomView`) via the `render`
+... which explicity defines the widget view via the `render`
 function, and (implicitly) **anywidget** defines the associated widget
 model (i.e., `CustomModel`). **anywidget** front-end code is often so
 minimal that it can easily be inlined as a Python string:
 
 ```python
 class CustomWidget(anywidget.AnyWidget):
     _esm = """
-    /** @param {DOMWidgetView} view */
-    export function render(view) {
-      let el = view.el;
-      let model = view.model;
+    export function render(context) {
+      let el = context.el;
+      let model = context.model;
       /* ... */
     }
     """
 ```
 
 ### The `render` function
 
 Just like `DOMWidgetView.render`, your widget's `render` function
 is executed exactly **one per output cell** that displays the widget instance.
 Therefore, `render` primarily serves two purposes:
 
-1. Initializing content to display (i.e., create and append element(s) to `view.el`)
+1. Initializing content to display (i.e., create and append element(s) to `context.el`)
 2. Registering event handlers to update or display model state any time it changes
-   (i.e., passing callbacks to `view.model.on`)
+   (i.e., passing callbacks to `context.model.on`)
 
 ## Connecting JavaScript with Python
 
 The Jupyter Widgets framework is build on top of the IPython Comm framework (short for communication).
 It's worth reading the [_Low Level Widget Explanation_](https://ipywidgets.readthedocs.io/en/8.0.2/examples/Widget%20Low%20Level.html#Low-Level-Widget-Explanation)
 to understand the core of Jupyter Widget's Model, View, Controller (MVC) architecture, but in
 short the Comm framework exposes two mechanisms to send/receive data to/from the frond end:
```

### Comparing `anywidget-0.4.3/docs/src/pages/en/notebooks/counter.ipynb` & `anywidget-0.5.0/docs/src/pages/en/notebooks/counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/styles/index.css` & `anywidget-0.5.0/docs/src/styles/index.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/docs/src/styles/theme.css` & `anywidget-0.5.0/docs/src/styles/theme.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/examples/Counter.ipynb` & `anywidget-0.5.0/examples/Counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/examples/minimal_example.ipynb` & `anywidget-0.5.0/examples/minimal_example.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/packages/anywidget/CHANGELOG.md` & `anywidget-0.5.0/packages/anywidget/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # anywidget
 
+## 0.5.0
+
+### Minor Changes
+
+- feat: restrict backbone model access in render context ([#140](https://github.com/manzt/anywidget/pull/140))
+
+- feat!: Limit view fields exposed to render function ([#138](https://github.com/manzt/anywidget/pull/138))
+
+  BREAKING: The render function's argument has been refactored from a full `AnyView` to a simple object. This object only exposes the `model` and `el` fields to the user-provided `render` function. This change aims to simplify the API and reduce potential misuse. Please ensure your render function only depends on these fields.
+
+### Patch Changes
+
+- Updated dependencies [[`fc2a626`](https://github.com/manzt/anywidget/commit/fc2a626804dd867cb11d1a9bdecbc713f19cc3be), [`521c0ed`](https://github.com/manzt/anywidget/commit/521c0ede62fbba45eba6bb873fda1c5a16461f2e)]:
+  - @anywidget/types@0.1.0
+
 ## 0.4.3
 
 ### Patch Changes
 
 - fix: Specify UTF-8 encoding in `FileContents.__str__` ([#135](https://github.com/manzt/anywidget/pull/135))
 
   Fixes an `UnicodeDecodeError` observed on Windows when special characters are present in `_esm` or `_css` elements of a widget.
```

### Comparing `anywidget-0.4.3/packages/anywidget/build.mjs` & `anywidget-0.5.0/packages/anywidget/build.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/packages/anywidget/package.json` & `anywidget-0.5.0/packages/anywidget/package.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.5.0'"}*

```diff
@@ -38,9 +38,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.4.3"
+    "version": "0.5.0"
 }
```

### Comparing `anywidget-0.4.3/packages/anywidget/src/widget.js` & `anywidget-0.5.0/packages/anywidget/src/widget.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,16 @@
 // @ts-check
 import {
     name,
     version
 } from "../package.json";
 
-/** @typedef {import("@jupyter-widgets/base").WidgetView} WidgetView */
-
 /**
  *  @typedef AnyWidgetModule
- *  @prop render {(view: WidgetView) => Promise<undefined | (() => Promise<void>)>}
+ *  @prop render {import("@anywidget/types").Render}
  */
 
 /**
  * @param {string} str
  * @returns {str is "https://${string}" | "http://${string}"}
  */
 function is_href(str) {
@@ -101,26 +99,65 @@
         console.log(e);
         throw e;
     }
     URL.revokeObjectURL(url);
     return widget;
 }
 
+/**
+ * @param {import("@jupyter-widgets/base").DOMWidgetView} view
+ * @returns {import("@anywidget/types").RenderContext}
+ *
+ * Prunes the view down to the minimum context necessary for rendering.
+ * Calls to `model.get` and `model.set` automatically add the view as
+ * context to the model, so we can gracefully unsubscribe from events
+ * added by the user-defined render.
+ */
+function extract_context(view) {
+    let model = {
+        /** @param {string} name */
+        get: view.model.get.bind(view.model),
+        set: view.model.set.bind(view.model),
+        save_changes: view.model.save_changes.bind(view.model),
+        /**
+         * @param {string} name
+         * @param {any} callback
+         */
+        on(name, callback) {
+            view.model.on(name, callback, view);
+        },
+        /**
+         * @param {string} name
+         * @param {any} callback
+         */
+        off(name, callback) {
+            view.model.off(name, callback, view);
+        },
+    };
+    return {
+        model,
+        el: view.el
+    };
+}
+
 /** @param {typeof import("@jupyter-widgets/base")} base */
-export default function(base) {
-    class AnyModel extends base.DOMWidgetModel {
+export default function({
+    DOMWidgetModel,
+    DOMWidgetView
+}) {
+    class AnyModel extends DOMWidgetModel {
         static model_name = "AnyModel";
         static model_module = name;
         static model_module_version = version;
 
         static view_name = "AnyView";
         static view_module = name;
         static view_module_version = version;
 
-        /** @param {Parameters<InstanceType<base["DOMWidgetModel"]>["initialize"]>} args */
+        /** @param {Parameters<InstanceType<DOMWidgetModel>["initialize"]>} args */
         initialize(...args) {
             super.initialize(...args);
 
             // Handles CSS updates from anywidget during development.
             this.on("change:_css", () => {
                 let id = this.get("_anywidget_id");
                 // _esm/_css/_anywidget_id traits are set dynamically within `anywidget.AnyWidget.__init__`,
@@ -134,53 +171,50 @@
 
             // Handles ESM updates from anywidget during development.
             this.on("change:_esm", async () => {
                 let id = this.get("_anywidget_id");
                 if (!id) return;
                 console.debug(`[anywidget] esm hot updated: ${id}`);
 
-                let views = ( /** @type {Promise<AnyView>[]} */ (Object.values(this.views ?? {})));
-
-                for await (let view of views) {
+                let views = ( /** @type {unknown} */ (Object.values(this.views ?? {})));
 
+                for await (let view of ( /** @type {Promise<AnyView>[]} */ (views))) {
                     // load updated esm
                     let widget = await load_esm(this.get("_esm"));
 
                     // call any cleanup logic defined by the previous module.
-                    await view._anywidget_cached_cleanup();
+                    try {
+                        await view._anywidget_cached_cleanup();
+                    } catch (e) {
+                        console.warn("[anywidget] error cleaning up previous module.", e);
+                        view._anywidget_cached_cleanup = () => {};
+                    }
+
+                    // Remove all event listeners added by the user-defined render.
+                    this.off(null, null, view);
 
                     // `view.$el` is a cached jQuery object for the view's element.
                     // This removes all child nodes but avoids deleting the root so
                     // we can rerender.
                     view.$el.empty();
 
-                    // Unsubscribe from any handlers registered to `view.listenTo`
-                    // Sadly we can't just `model.off` because it removes everything,
-                    // including handlers not setup by the child view.
-                    //
-                    // We could override `model.on` with a particular `context` if none is
-                    // provided, letting us unsubscribe from only events from views
-                    // e.g., `model.off(null, null, anywidgetSymbol)`, but that might
-                    // be more trouble than it's worth and this is just a feature for
-                    // development.
-                    view.stopListening(this);
-
                     // render the view with the updated render
-                    let cleanup = await widget.render(view);
+                    let cleanup = await widget.render(extract_context(view));
+
                     view._anywidget_cached_cleanup = cleanup ?? (() => {});
                 }
             });
         }
     }
 
-    class AnyView extends base.DOMWidgetView {
+    class AnyView extends DOMWidgetView {
         async render() {
             await load_css(this.model.get("_css"), this.model.get("_anywidget_id"));
             let widget = await load_esm(this.model.get("_esm"));
-            let cleanup = await widget.render(this);
+            let cleanup = await widget.render(extract_context(this));
             this._anywidget_cached_cleanup = cleanup ?? (() => {});
         }
 
         /** @type {() => Promise<void> | void} */
         _anywidget_cached_cleanup() {}
 
         async remove() {
```

### Comparing `anywidget-0.4.3/tests/test_descriptor.py` & `anywidget-0.5.0/tests/test_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/tests/test_experimental.py` & `anywidget-0.5.0/tests/test_experimental.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/tests/test_file_contents.py` & `anywidget-0.5.0/tests/test_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/tests/test_utils.py` & `anywidget-0.5.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/tests/test_widget.py` & `anywidget-0.5.0/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/LICENSE` & `anywidget-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/README.md` & `anywidget-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/pyproject.toml` & `anywidget-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.3/PKG-INFO` & `anywidget-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anywidget
-Version: 0.4.3
+Version: 0.5.0
 Summary: custom jupyter widgets made easy
 Project-URL: homepage, https://github.com/manzt/anywidget
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata; python_version < '3.8'
```

