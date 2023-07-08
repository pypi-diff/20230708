# Comparing `tmp/jupyterlab_nodeeditor-1.0.3.tar.gz` & `tmp/jupyterlab_nodeeditor-1.0.4.tar.gz`

## Comparing `jupyterlab_nodeeditor-1.0.3.tar` & `jupyterlab_nodeeditor-1.0.4.tar`

### file list

```diff
@@ -1,435 +1,453 @@
--rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/.copier-answers.yml
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/.gitmodules
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/.prettierignore
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/.yarnrc.yml
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/CHANGELOG.md
--rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/RELEASE.md
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/dev.sh
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/init.sh
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/install.json
--rwxr-xr-x   0        0        0     6214 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/package.json
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/setup.py
--rwxr-xr-x   0        0        0      583 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/tsconfig.json
--rwxr-xr-x   0        0        0   215226 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/yarn.lock
--rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/.copier-answers.yml
--rwxr-xr-x   0        0        0     1587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/.gitignore
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/.prettierignore
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/.yarnrc.yml
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/CHANGELOG.md
--rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/LICENSE
--rwxr-xr-x   0        0        0     2571 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/README.md
--rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/RELEASE.md
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/install.json
--rwxr-xr-x   0        0        0     5198 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/package.json
--rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/pyproject.toml
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/setup.py
--rwxr-xr-x   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/tsconfig.json
--rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/jupyterlab_nodeeditor/__init__.py
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/schema/plugin.json
--rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/src/index.ts
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/style/base.css
--rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/style/index.css
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/_temp_extension/style/index.js
--rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/.babelrc
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/.editorconfig
--rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/.eslintrc
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/.git
--rwxr-xr-x   0        0        0      376 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/.gitignore
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/.npmignore
--rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/.nvmrc
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/.travis.yml
--rwxr-xr-x   0        0        0     3369 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/CODE_OF_CONDUCT.md
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/LICENSE
--rwxr-xr-x   0        0        0     2069 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/README.md
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/cypress.json
--rwxr-xr-x   0        0        0   533606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/logo.ai
--rwxr-xr-x   0        0        0    15873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/logo.png
--rwxr-xr-x   0        0        0     3123 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/logo.svg
--rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/package.json
--rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/rollup.config.js
--rwxr-xr-x   0        0        0   675825 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/yarn.lock
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/cypress/fixtures/example.json
--rwxr-xr-x   0        0        0     4389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/cypress/integration/NodeEditorSpec.js
--rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/cypress/plugins/index.js
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/cypress/support/commands.js
--rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/cypress/support/index.js
--rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/.gitignore
--rwxr-xr-x   0        0        0      721 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/README.md
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/babel.config.js
--rwxr-xr-x   0        0        0     3301 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docusaurus.config.js
--rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/package.json
--rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/sidebars.js
--rwxr-xr-x   0        0        0   428509 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/yarn.lock
--rwxr-xr-x   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/blog/2019-05-28-hola.md
--rwxr-xr-x   0        0        0      428 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/blog/2019-05-29-hello-world.md
--rwxr-xr-x   0        0        0      452 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/blog/2019-05-30-welcome.md
--rwxr-xr-x   0        0        0     4098 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/components/AnatomyExample.js
--rwxr-xr-x   0        0        0     1446 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/components/Colors.js
--rwxr-xr-x   0        0        0     5622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/components/ControlExamples.js
--rwxr-xr-x   0        0        0     5735 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/components/DynamicNodesExamples.js
--rwxr-xr-x   0        0        0     2495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/components/DynamicThemingExample.js
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/components/FlexRow.js
--rwxr-xr-x   0        0        0    16960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/components/GettingStartedExample.js
--rwxr-xr-x   0        0        0     6137 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/NodeEditor.mdx
--rwxr-xr-x   0        0        0     5303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/RootEngine.mdx
--rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/anatomy.mdx
--rwxr-xr-x   0        0        0     8565 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/basic-config.mdx
--rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/colors.mdx
--rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/comments.mdx
--rwxr-xr-x   0        0        0     8897 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/controls.mdx
--rwxr-xr-x   0        0        0      525 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/defining-nodes.mdx
--rwxr-xr-x   0        0        0     4129 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/doc1.md
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/doc2.md
--rwxr-xr-x   0        0        0     2173 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/doc3.md
--rwxr-xr-x   0        0        0     5038 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/dynamic-nodes.mdx
--rwxr-xr-x   0        0        0     7241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/faq.mdx
--rwxr-xr-x   0        0        0    10532 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/flume-config.mdx
--rwxr-xr-x   0        0        0     4261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/logic-nodes.mdx
--rwxr-xr-x   0        0        0      521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/mdx.md
--rwxr-xr-x   0        0        0     2232 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/node-editor.mdx
--rwxr-xr-x   0        0        0     2909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/overview.mdx
--rwxr-xr-x   0        0        0      898 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/quick-start.mdx
--rwxr-xr-x   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/root-engine.mdx
--rwxr-xr-x   0        0        0     2978 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/root-node.mdx
--rwxr-xr-x   0        0        0     2981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/running-logic.mdx
--rwxr-xr-x   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/saving-nodes.mdx
--rwxr-xr-x   0        0        0     1929 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/theming.mdx
--rwxr-xr-x   0        0        0     2296 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/type-safety.mdx
--rwxr-xr-x   0        0        0     4178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/using-with-react.mdx
--rwxr-xr-x   0        0        0     1818 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/docs/using-without-react.mdx
--rwxr-xr-x   0        0        0     8877 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/src/exampleFlumeConfig.js
--rwxr-xr-x   0        0        0    49415 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/src/components/TypeSafe.js
--rwxr-xr-x   0        0        0     1304 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/src/css/custom.css
--rwxr-xr-x   0        0        0    15622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/src/pages/index.js
--rwxr-xr-x   0        0        0    11943 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/src/pages/styles.module.css
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/.nojekyll
--rwxr-xr-x   0        0        0     4297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/60fps.svg
--rwxr-xr-x   0        0        0     5914 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/android-chrome-192x192.png
--rwxr-xr-x   0        0        0    17474 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/android-chrome-512x512.png
--rwxr-xr-x   0        0        0     5337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/apple-touch-icon.png
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/arrow-right-blue.svg
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/arrow-right-green.svg
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/arrow-right-red.svg
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/arrow-right-red_1.svg
--rwxr-xr-x   0        0        0      436 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/arrow-right.svg
--rwxr-xr-x   0        0        0     3193 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/controls.svg
--rwxr-xr-x   0        0        0   539930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/example_editors.png
--rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/favicon-16x16.png
--rwxr-xr-x   0        0        0      765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/favicon-32x32.png
--rwxr-xr-x   0        0        0    15406 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/favicon.ico
--rwxr-xr-x   0        0        0   127864 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/fb-img.png
--rwxr-xr-x   0        0        0   737734 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/flume-short-web.mp4
--rwxr-xr-x   0        0        0     5893 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/friends-graph.svg
--rwxr-xr-x   0        0        0    48634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/hero-nodes.svg
--rwxr-xr-x   0        0        0     1860 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/logo-dark.svg
--rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/logo.svg
--rwxr-xr-x   0        0        0     5626 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/netlify.svg
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/page-curve-blue.svg
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/page-curve-dark.svg
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/page-curve.svg
--rwxr-xr-x   0        0        0     1588 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/performance-tile.svg
--rwxr-xr-x   0        0        0      377 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/play-icon.svg
--rwxr-xr-x   0        0        0     2880 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/react-tile.svg
--rwxr-xr-x   0        0        0     1823 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/size-tile.svg
--rwxr-xr-x   0        0        0     2330 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/theme-tile.svg
--rwxr-xr-x   0        0        0     1643 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/theme.svg
--rwxr-xr-x   0        0        0    41674 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/type-safe-node.svg
--rwxr-xr-x   0        0        0    21728 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/type-safe-nodes.svg
--rwxr-xr-x   0        0        0    31457 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/undraw_docusaurus_mountain.svg
--rwxr-xr-x   0        0        0    35968 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/undraw_docusaurus_react.svg
--rwxr-xr-x   0        0        0    11784 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/undraw_docusaurus_tree.svg
--rwxr-xr-x   0        0        0   146113 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/valid_port_types.png
--rwxr-xr-x   0        0        0      499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/wordmark_white.svg
--rwxr-xr-x   0        0        0       28 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/.eslintrc
--rwxr-xr-x   0        0        0   105919 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/README.md
--rwxr-xr-x   0        0        0     1168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/package.json
--rwxr-xr-x   0        0        0   913821 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/yarn.lock
--rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/public/index.html
--rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/public/manifest.json
--rwxr-xr-x   0        0        0    18960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/App.js
--rwxr-xr-x   0        0        0      318 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/index.css
--rwxr-xr-x   0        0        0     1503 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/index.js
--rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/TestRoutes/TestEditor.js
--rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/TestRoutes/nodes.js
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/components/Checkbox.js
--rwxr-xr-x   0        0        0     1895 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/components/FloatingNavigation.js
--rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/components/Header.js
--rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/components/LogicEditor.js
--rwxr-xr-x   0        0        0      380 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/components/Modal.js
--rwxr-xr-x   0        0        0     2000 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/components/OptionsEditor.js
--rwxr-xr-x   0        0        0      736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/icons/BoxIcon.js
--rwxr-xr-x   0        0        0     1223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/icons/FormIcon.js
--rwxr-xr-x   0        0        0     3783 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/icons/GearIcon.js
--rwxr-xr-x   0        0        0     6066 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/Attributes.js
--rwxr-xr-x   0        0        0     2886 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/Body.js
--rwxr-xr-x   0        0        0     2020 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/Field.js
--rwxr-xr-x   0        0        0    10739 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/Form.css
--rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/Form.js
--rwxr-xr-x   0        0        0     1834 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/InputTypes.js
--rwxr-xr-x   0        0        0     6297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/NodeTypes.js
--rwxr-xr-x   0        0        0     2937 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/PreviewField.js
--rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/Sidebar.js
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/defaultNodes.js
--rwxr-xr-x   0        0        0      815 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/designerReducer.js
--rwxr-xr-x   0        0        0     1261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/fieldTypes.js
--rwxr-xr-x   0        0        0     1560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/fieldsReducer.js
--rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/formHandler.js
--rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/previewFieldsReducer.js
--rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/resolveLogic.js
--rwxr-xr-x   0        0        0     8710 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/wizardLogic/logicTypes.js
--rwxr-xr-x   0        0        0     1910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Forms/Forms.css
--rwxr-xr-x   0        0        0     1854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Forms/Forms.js
--rwxr-xr-x   0        0        0      754 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Records/Records.css
--rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Records/Records.js
--rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/.eslintrc
--rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/Cache.js
--rwxr-xr-x   0        0        0     4158 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/RootEngine.js
--rwxr-xr-x   0        0        0     1377 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/commentsReducer.js
--rwxr-xr-x   0        0        0     6241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/connectionCalculator.js
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/constants.js
--rwxr-xr-x   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/context.js
--rwxr-xr-x   0        0        0     9569 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/index.js
--rwxr-xr-x   0        0        0    13868 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/nodesReducer.js
--rwxr-xr-x   0        0        0      460 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/stageReducer.js
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/styles.css
--rwxr-xr-x   0        0        0     1191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/toastsReducer.js
--rwxr-xr-x   0        0        0     8905 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/typeBuilders.js
--rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/utilities.js
--rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Checkbox/Checkbox.css
--rwxr-xr-x   0        0        0      651 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Checkbox/Checkbox.js
--rwxr-xr-x   0        0        0     1134 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/ColorPicker/ColorPicker.css
--rwxr-xr-x   0        0        0     1934 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/ColorPicker/ColorPicker.js
--rwxr-xr-x   0        0        0     2159 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Comment/Comment.css
--rwxr-xr-x   0        0        0     5506 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Comment/Comment.js
--rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Connection/Connection.css
--rwxr-xr-x   0        0        0      847 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Connection/Connection.js
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Connections/Connections.css
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Connections/Connections.js
--rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/ContextMenu/ContextMenu.css
--rwxr-xr-x   0        0        0     7010 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/ContextMenu/ContextMenu.js
--rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Control/Control.css
--rwxr-xr-x   0        0        0     2731 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Control/Control.js
--rwxr-xr-x   0        0        0     3751 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Draggable/Draggable.js
--rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/IoPorts/IoPorts.css
--rwxr-xr-x   0        0        0    12769 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/IoPorts/IoPorts.js
--rwxr-xr-x   0        0        0      468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Node/Node.css
--rwxr-xr-x   0        0        0     7392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Node/Node.js
--rwxr-xr-x   0        0        0     2001 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Select/Select.css
--rwxr-xr-x   0        0        0     3645 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Select/Select.js
--rwxr-xr-x   0        0        0     1284 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Stage/Stage.css
--rwxr-xr-x   0        0        0     8901 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Stage/Stage.js
--rwxr-xr-x   0        0        0      435 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/TextInput/TextInput.css
--rwxr-xr-x   0        0        0     3063 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/TextInput/TextInput.js
--rwxr-xr-x   0        0        0     2223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Toaster/Toaster.css
--rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/components/Toaster/Toaster.js
--rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/hooks/usePrevious.js
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/img/grid.png
--rwxr-xr-x   0        0        0     8912 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/tests/dynamic.test.js
--rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/tests/nodes.js
--rwxr-xr-x   0        0        0     1409 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/tests/ssr.test.js
--rwxr-xr-x   0        0        0     1397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/flume/src/tests/test.js
--rwxr-xr-x   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/__init__.py
--rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/_version.py
--rwxr-xr-x   0        0        0     5542 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/package.json
--rwxr-xr-x   0        0        0     6214 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig
--rwxr-xr-x   0        0        0     9164 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json
--rwxr-xr-x   0        0        0     3987 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js.LICENSE.txt
--rwxr-xr-x   0        0        0     6292 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3672 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js.LICENSE.txt
--rwxr-xr-x   0        0        0    18679 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3638 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2267 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js.LICENSE.txt
--rwxr-xr-x   0        0        0      930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7685 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js.LICENSE.txt
--rwxr-xr-x   0        0        0     5560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js.LICENSE.txt
--rwxr-xr-x   0        0        0    11356 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1849 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4595 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3213 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js.LICENSE.txt
--rwxr-xr-x   0        0        0    10308 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js.LICENSE.txt
--rwxr-xr-x   0        0        0     5078 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1183 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js.LICENSE.txt
--rwxr-xr-x   0        0        0     5424 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4994 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js
--rwxr-xr-x   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3888 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js.LICENSE.txt
--rwxr-xr-x   0        0        0     9725 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4055 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3672 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     9126 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js.LICENSE.txt
--rwxr-xr-x   0        0        0  3246909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js
--rwxr-xr-x   0        0        0      576 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2846 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4006 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1927 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1892 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4030 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js.LICENSE.txt
--rwxr-xr-x   0        0        0    17021 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2459 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2519 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7231 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1911 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js.LICENSE.txt
--rwxr-xr-x   0        0        0     6491 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js.LICENSE.txt
--rwxr-xr-x   0        0        0    32283 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js.LICENSE.txt
--rwxr-xr-x   0        0        0    32835 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js.LICENSE.txt
--rwxr-xr-x   0        0        0     6820 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1951 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js.LICENSE.txt
--rwxr-xr-x   0        0        0    16144 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3065 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3470 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js.LICENSE.txt
--rwxr-xr-x   0        0        0    11882 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2342 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js.LICENSE.txt
--rwxr-xr-x   0        0        0    38168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js.LICENSE.txt
--rwxr-xr-x   0        0        0     5447 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2567 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3657 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3351 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3653 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js.LICENSE.txt
--rwxr-xr-x   0        0        0    10379 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8109 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js.LICENSE.txt
--rwxr-xr-x   0        0        0    73464 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf
--rwxr-xr-x   0        0        0     3654 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8.b10d47f837675650f39c.js
--rwxr-xr-x   0        0        0     8337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7938 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js.LICENSE.txt
--rwxr-xr-x   0        0        0    22618 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8401.d14444e38cb7aa24efdd.js
--rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js.LICENSE.txt
--rwxr-xr-x   0        0        0    14242 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2658 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3155 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4242 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js.LICENSE.txt
--rwxr-xr-x   0        0        0   196525 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8863.13ee8eba41cde457103f.js
--rwxr-xr-x   0        0        0     2899 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1501 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4332 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4994 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3017 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/9687.0805ace94c0cdeaabf35.js
--rwxr-xr-x   0        0        0     4099 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/9747.77aa0e73ef6f7f90faff.js
--rwxr-xr-x   0        0        0     5873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js.LICENSE.txt
--rwxr-xr-x   0        0        0    13543 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js.LICENSE.txt
--rwxr-xr-x   0        0        0    12832 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/remoteEntry.02d460eb6f0da6b03b5c.js
--rwxr-xr-x   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/style.js
--rwxr-xr-x   0        0        0     8629 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/third-party-licenses.json
--rwxr-xr-x   0        0        0     9164 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/schema/plugin.json
--rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/src/ReRunIcon.tsx
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/src/arrownIcon.tsx
--rwxr-xr-x   0        0        0     1455 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/src/clearIcon.tsx
--rwxr-xr-x   0        0        0      954 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/src/deleteIcon.tsx
--rwxr-xr-x   0        0        0     1505 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/src/exportIcon.tsx
--rwxr-xr-x   0        0        0     1310 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/src/factory.ts
--rwxr-xr-x   0        0        0    37305 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/src/flumeConfig.tsx
--rwxr-xr-x   0        0        0     7454 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/src/imageViewer.tsx
--rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/src/index.ts
--rwxr-xr-x   0        0        0     2268 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/src/lockIcon.tsx
--rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/src/model.ts
--rwxr-xr-x   0        0        0      807 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/src/newIcon.tsx
--rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/src/runIcon.tsx
--rwxr-xr-x   0        0        0     1778 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/src/utils.tsx
--rwxr-xr-x   0        0        0   142272 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/src/widget.tsx
--rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/src/yesIcon.tsx
--rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/style/base.css
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/style/index.css
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/style/index.js
--rwxr-xr-x   0        0        0     1596 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/.gitignore
--rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/LICENSE
--rwxr-xr-x   0        0        0     2557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/README.md
--rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/.copier-answers.yml
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/.gitmodules
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/.prettierignore
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/.yarnrc.yml
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/CHANGELOG.md
+-rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/RELEASE.md
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/dev.sh
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/init.sh
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/install.json
+-rwxr-xr-x   0        0        0     6248 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/package.json
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/setup.py
+-rwxr-xr-x   0        0        0      583 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/tsconfig.json
+-rwxr-xr-x   0        0        0   215696 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/yarn.lock
+-rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/.vscode/settings.json
+-rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/.copier-answers.yml
+-rwxr-xr-x   0        0        0     1587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/.gitignore
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/.prettierignore
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/.yarnrc.yml
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/LICENSE
+-rwxr-xr-x   0        0        0     2571 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/README.md
+-rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/RELEASE.md
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/install.json
+-rwxr-xr-x   0        0        0     5198 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/package.json
+-rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/pyproject.toml
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/setup.py
+-rwxr-xr-x   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/tsconfig.json
+-rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/jupyterlab_nodeeditor/__init__.py
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/schema/plugin.json
+-rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/src/index.ts
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/style/base.css
+-rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/style/index.css
+-rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/_temp_extension/style/index.js
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/.babelrc
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/.editorconfig
+-rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/.eslintrc
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/.git
+-rwxr-xr-x   0        0        0      376 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/.gitignore
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/.npmignore
+-rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/.nvmrc
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/.travis.yml
+-rwxr-xr-x   0        0        0     3369 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/LICENSE
+-rwxr-xr-x   0        0        0     2069 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/README.md
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/cypress.json
+-rwxr-xr-x   0        0        0   533606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/logo.ai
+-rwxr-xr-x   0        0        0    15873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/logo.png
+-rwxr-xr-x   0        0        0     3123 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/logo.svg
+-rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/package.json
+-rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/rollup.config.js
+-rwxr-xr-x   0        0        0   675825 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/yarn.lock
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/cypress/fixtures/example.json
+-rwxr-xr-x   0        0        0     4389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/cypress/integration/NodeEditorSpec.js
+-rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/cypress/plugins/index.js
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/cypress/support/commands.js
+-rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/cypress/support/index.js
+-rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/.gitignore
+-rwxr-xr-x   0        0        0      721 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/README.md
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/babel.config.js
+-rwxr-xr-x   0        0        0     3301 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docusaurus.config.js
+-rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/package.json
+-rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/sidebars.js
+-rwxr-xr-x   0        0        0   428509 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/yarn.lock
+-rwxr-xr-x   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/blog/2019-05-28-hola.md
+-rwxr-xr-x   0        0        0      428 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/blog/2019-05-29-hello-world.md
+-rwxr-xr-x   0        0        0      452 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/blog/2019-05-30-welcome.md
+-rwxr-xr-x   0        0        0     4098 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/components/AnatomyExample.js
+-rwxr-xr-x   0        0        0     1446 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/components/Colors.js
+-rwxr-xr-x   0        0        0     5622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/components/ControlExamples.js
+-rwxr-xr-x   0        0        0     5735 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/components/DynamicNodesExamples.js
+-rwxr-xr-x   0        0        0     2495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/components/DynamicThemingExample.js
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/components/FlexRow.js
+-rwxr-xr-x   0        0        0    16960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/components/GettingStartedExample.js
+-rwxr-xr-x   0        0        0     6137 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/NodeEditor.mdx
+-rwxr-xr-x   0        0        0     5303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/RootEngine.mdx
+-rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/anatomy.mdx
+-rwxr-xr-x   0        0        0     8565 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/basic-config.mdx
+-rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/colors.mdx
+-rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/comments.mdx
+-rwxr-xr-x   0        0        0     8897 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/controls.mdx
+-rwxr-xr-x   0        0        0      525 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/defining-nodes.mdx
+-rwxr-xr-x   0        0        0     4129 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/doc1.md
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/doc2.md
+-rwxr-xr-x   0        0        0     2173 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/doc3.md
+-rwxr-xr-x   0        0        0     5038 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/dynamic-nodes.mdx
+-rwxr-xr-x   0        0        0     7241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/faq.mdx
+-rwxr-xr-x   0        0        0    10532 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/flume-config.mdx
+-rwxr-xr-x   0        0        0     4261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/logic-nodes.mdx
+-rwxr-xr-x   0        0        0      521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/mdx.md
+-rwxr-xr-x   0        0        0     2232 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/node-editor.mdx
+-rwxr-xr-x   0        0        0     2909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/overview.mdx
+-rwxr-xr-x   0        0        0      898 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/quick-start.mdx
+-rwxr-xr-x   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/root-engine.mdx
+-rwxr-xr-x   0        0        0     2978 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/root-node.mdx
+-rwxr-xr-x   0        0        0     2981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/running-logic.mdx
+-rwxr-xr-x   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/saving-nodes.mdx
+-rwxr-xr-x   0        0        0     1929 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/theming.mdx
+-rwxr-xr-x   0        0        0     2296 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/type-safety.mdx
+-rwxr-xr-x   0        0        0     4178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/using-with-react.mdx
+-rwxr-xr-x   0        0        0     1818 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/docs/using-without-react.mdx
+-rwxr-xr-x   0        0        0     8877 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/src/exampleFlumeConfig.js
+-rwxr-xr-x   0        0        0    49415 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/src/components/TypeSafe.js
+-rwxr-xr-x   0        0        0     1304 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/src/css/custom.css
+-rwxr-xr-x   0        0        0    15622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/src/pages/index.js
+-rwxr-xr-x   0        0        0    11943 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/src/pages/styles.module.css
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/.nojekyll
+-rwxr-xr-x   0        0        0     4297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/60fps.svg
+-rwxr-xr-x   0        0        0     5914 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/android-chrome-192x192.png
+-rwxr-xr-x   0        0        0    17474 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/android-chrome-512x512.png
+-rwxr-xr-x   0        0        0     5337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/apple-touch-icon.png
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/arrow-right-blue.svg
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/arrow-right-green.svg
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/arrow-right-red.svg
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/arrow-right-red_1.svg
+-rwxr-xr-x   0        0        0      436 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/arrow-right.svg
+-rwxr-xr-x   0        0        0     3193 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/controls.svg
+-rwxr-xr-x   0        0        0   539930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/example_editors.png
+-rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/favicon-16x16.png
+-rwxr-xr-x   0        0        0      765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/favicon-32x32.png
+-rwxr-xr-x   0        0        0    15406 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/favicon.ico
+-rwxr-xr-x   0        0        0   127864 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/fb-img.png
+-rwxr-xr-x   0        0        0   737734 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/flume-short-web.mp4
+-rwxr-xr-x   0        0        0     5893 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/friends-graph.svg
+-rwxr-xr-x   0        0        0    48634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/hero-nodes.svg
+-rwxr-xr-x   0        0        0     1860 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/logo-dark.svg
+-rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/logo.svg
+-rwxr-xr-x   0        0        0     5626 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/netlify.svg
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/page-curve-blue.svg
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/page-curve-dark.svg
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/page-curve.svg
+-rwxr-xr-x   0        0        0     1588 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/performance-tile.svg
+-rwxr-xr-x   0        0        0      377 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/play-icon.svg
+-rwxr-xr-x   0        0        0     2880 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/react-tile.svg
+-rwxr-xr-x   0        0        0     1823 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/size-tile.svg
+-rwxr-xr-x   0        0        0     2330 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/theme-tile.svg
+-rwxr-xr-x   0        0        0     1643 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/theme.svg
+-rwxr-xr-x   0        0        0    41674 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/type-safe-node.svg
+-rwxr-xr-x   0        0        0    21728 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/type-safe-nodes.svg
+-rwxr-xr-x   0        0        0    31457 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/undraw_docusaurus_mountain.svg
+-rwxr-xr-x   0        0        0    35968 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/undraw_docusaurus_react.svg
+-rwxr-xr-x   0        0        0    11784 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/undraw_docusaurus_tree.svg
+-rwxr-xr-x   0        0        0   146113 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/valid_port_types.png
+-rwxr-xr-x   0        0        0      499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/wordmark_white.svg
+-rwxr-xr-x   0        0        0       28 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/.eslintrc
+-rwxr-xr-x   0        0        0   105919 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/README.md
+-rwxr-xr-x   0        0        0     1168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/package.json
+-rwxr-xr-x   0        0        0   913821 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/yarn.lock
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/public/index.html
+-rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/public/manifest.json
+-rwxr-xr-x   0        0        0    18960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/App.js
+-rwxr-xr-x   0        0        0      318 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/index.css
+-rwxr-xr-x   0        0        0     1503 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/index.js
+-rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/TestRoutes/TestEditor.js
+-rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/TestRoutes/nodes.js
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/components/Checkbox.js
+-rwxr-xr-x   0        0        0     1895 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/components/FloatingNavigation.js
+-rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/components/Header.js
+-rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/components/LogicEditor.js
+-rwxr-xr-x   0        0        0      380 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/components/Modal.js
+-rwxr-xr-x   0        0        0     2000 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/components/OptionsEditor.js
+-rwxr-xr-x   0        0        0      736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/icons/BoxIcon.js
+-rwxr-xr-x   0        0        0     1223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/icons/FormIcon.js
+-rwxr-xr-x   0        0        0     3783 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/icons/GearIcon.js
+-rwxr-xr-x   0        0        0     6066 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/Attributes.js
+-rwxr-xr-x   0        0        0     2886 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/Body.js
+-rwxr-xr-x   0        0        0     2020 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/Field.js
+-rwxr-xr-x   0        0        0    10739 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/Form.css
+-rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/Form.js
+-rwxr-xr-x   0        0        0     1834 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/InputTypes.js
+-rwxr-xr-x   0        0        0     6297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/NodeTypes.js
+-rwxr-xr-x   0        0        0     2937 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/PreviewField.js
+-rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/Sidebar.js
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/defaultNodes.js
+-rwxr-xr-x   0        0        0      815 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/designerReducer.js
+-rwxr-xr-x   0        0        0     1261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/fieldTypes.js
+-rwxr-xr-x   0        0        0     1560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/fieldsReducer.js
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/formHandler.js
+-rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/previewFieldsReducer.js
+-rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/resolveLogic.js
+-rwxr-xr-x   0        0        0     8710 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/wizardLogic/logicTypes.js
+-rwxr-xr-x   0        0        0     1910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Forms/Forms.css
+-rwxr-xr-x   0        0        0     1854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Forms/Forms.js
+-rwxr-xr-x   0        0        0      754 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Records/Records.css
+-rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Records/Records.js
+-rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/.eslintrc
+-rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/Cache.js
+-rwxr-xr-x   0        0        0     4158 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/RootEngine.js
+-rwxr-xr-x   0        0        0     2060 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/commentsReducer.js
+-rwxr-xr-x   0        0        0     6241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/connectionCalculator.js
+-rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/constants.js
+-rwxr-xr-x   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/context.js
+-rwxr-xr-x   0        0        0     9649 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/index.js
+-rwxr-xr-x   0        0        0    14282 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/nodesReducer.js
+-rwxr-xr-x   0        0        0      460 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/stageReducer.js
+-rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/styles.css
+-rwxr-xr-x   0        0        0     1191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/toastsReducer.js
+-rwxr-xr-x   0        0        0     8905 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/typeBuilders.js
+-rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/utilities.js
+-rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Checkbox/Checkbox.css
+-rwxr-xr-x   0        0        0      651 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Checkbox/Checkbox.js
+-rwxr-xr-x   0        0        0     1134 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/ColorPicker/ColorPicker.css
+-rwxr-xr-x   0        0        0     1934 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/ColorPicker/ColorPicker.js
+-rwxr-xr-x   0        0        0     2159 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Comment/Comment.css
+-rwxr-xr-x   0        0        0     7028 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Comment/Comment.js
+-rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Connection/Connection.css
+-rwxr-xr-x   0        0        0      847 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Connection/Connection.js
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Connections/Connections.css
+-rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Connections/Connections.js
+-rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/ContextMenu/ContextMenu.css
+-rwxr-xr-x   0        0        0     7071 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/ContextMenu/ContextMenu.js
+-rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Control/Control.css
+-rwxr-xr-x   0        0        0     2731 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Control/Control.js
+-rwxr-xr-x   0        0        0     3751 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Draggable/Draggable.js
+-rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/IoPorts/IoPorts.css
+-rwxr-xr-x   0        0        0    12769 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/IoPorts/IoPorts.js
+-rwxr-xr-x   0        0        0      468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Node/Node.css
+-rwxr-xr-x   0        0        0     7392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Node/Node.js
+-rwxr-xr-x   0        0        0     2001 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Select/Select.css
+-rwxr-xr-x   0        0        0     3675 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Select/Select.js
+-rwxr-xr-x   0        0        0     1284 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Stage/Stage.css
+-rwxr-xr-x   0        0        0     9421 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Stage/Stage.js
+-rwxr-xr-x   0        0        0      435 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/TextInput/TextInput.css
+-rwxr-xr-x   0        0        0     3405 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/TextInput/TextInput.js
+-rwxr-xr-x   0        0        0     2223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Toaster/Toaster.css
+-rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/components/Toaster/Toaster.js
+-rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/hooks/usePrevious.js
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/img/grid.png
+-rwxr-xr-x   0        0        0     8912 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/tests/dynamic.test.js
+-rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/tests/nodes.js
+-rwxr-xr-x   0        0        0     1409 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/tests/ssr.test.js
+-rwxr-xr-x   0        0        0     1397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/flume/src/tests/test.js
+-rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/__init__.py
+-rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/_version.py
+-rwxr-xr-x   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/select.py
+-rwxr-xr-x   0        0        0     2578 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/utils.py
+-rwxr-xr-x   0        0        0    20983 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/build_log.json
+-rwxr-xr-x   0        0        0     5572 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/package.json
+-rwxr-xr-x   0        0        0     6248 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig
+-rwxr-xr-x   0        0        0    11646 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json
+-rwxr-xr-x   0        0        0    73464 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf
+-rwxr-xr-x   0        0        0    17913 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/data_image_png_base64_iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5_AAAAAXNSR0IArs4c6QAAAARnQU1-5f4412.8573e56b3e457c1d826b.js
+-rwxr-xr-x   0        0        0   540985 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/lib_index_js.fceee7b240a6c38ea32d.js
+-rwxr-xr-x   0        0        0   854051 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/lib_index_js.fceee7b240a6c38ea32d.js.map
+-rwxr-xr-x   0        0        0     6996 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_apex_apex_js.9982e0769f40abee234a.js
+-rwxr-xr-x   0        0        0     9200 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_apex_apex_js.9982e0769f40abee234a.js.map
+-rwxr-xr-x   0        0        0     2664 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_azcli_azcli_js.182cee8a9aa456f6febd.js
+-rwxr-xr-x   0        0        0     2645 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_azcli_azcli_js.182cee8a9aa456f6febd.js.map
+-rwxr-xr-x   0        0        0     3696 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_bat_bat_js.55db1a421d24f3d884a7.js
+-rwxr-xr-x   0        0        0     4079 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_bat_bat_js.55db1a421d24f3d884a7.js.map
+-rwxr-xr-x   0        0        0     4786 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_bicep_bicep_js.1d144118bc30d3f19464.js
+-rwxr-xr-x   0        0        0     5791 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_bicep_bicep_js.1d144118bc30d3f19464.js.map
+-rwxr-xr-x   0        0        0     4505 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_cameligo_cameligo_js.1674e1b671d71f42a4c2.js
+-rwxr-xr-x   0        0        0     5512 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_cameligo_cameligo_js.1674e1b671d71f42a4c2.js.map
+-rwxr-xr-x   0        0        0     6584 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_coffee_coffee_js.5203585c44a43b4dd973.js
+-rwxr-xr-x   0        0        0     8209 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_coffee_coffee_js.5203585c44a43b4dd973.js.map
+-rwxr-xr-x   0        0        0     9106 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_cpp_cpp_js.0fa4bdcecb4b3a69eb94.js
+-rwxr-xr-x   0        0        0    11989 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_cpp_cpp_js.0fa4bdcecb4b3a69eb94.js.map
+-rwxr-xr-x   0        0        0     7946 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_csharp_csharp_js.d17276a727e138d62758.js
+-rwxr-xr-x   0        0        0    10449 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_csharp_csharp_js.d17276a727e138d62758.js.map
+-rwxr-xr-x   0        0        0     2937 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_csp_csp_js.7d0541c505bba64c05d9.js
+-rwxr-xr-x   0        0        0     2761 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_csp_csp_js.7d0541c505bba64c05d9.js.map
+-rwxr-xr-x   0        0        0     7137 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_css_css_js.ee8ef84415cbaf78afb7.js
+-rwxr-xr-x   0        0        0     9112 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_css_css_js.ee8ef84415cbaf78afb7.js.map
+-rwxr-xr-x   0        0        0     6218 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_cypher_cypher_js.a0c83171cb974949a02c.js
+-rwxr-xr-x   0        0        0     7949 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_cypher_cypher_js.a0c83171cb974949a02c.js.map
+-rwxr-xr-x   0        0        0     7205 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_dart_dart_js.4420e06db9a150d9b45c.js
+-rwxr-xr-x   0        0        0     9164 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_dart_dart_js.4420e06db9a150d9b45c.js.map
+-rwxr-xr-x   0        0        0     4248 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_dockerfile_dockerfile_js.2f95d8158ea4f41996f4.js
+-rwxr-xr-x   0        0        0     4888 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_dockerfile_dockerfile_js.2f95d8158ea4f41996f4.js.map
+-rwxr-xr-x   0        0        0     9034 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_ecl_ecl_js.0f56bcbc2002bbee3a30.js
+-rwxr-xr-x   0        0        0    12353 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_ecl_ecl_js.0f56bcbc2002bbee3a30.js.map
+-rwxr-xr-x   0        0        0     3901 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_flow9_flow9_js.ee19c04e3556e2f3320e.js
+-rwxr-xr-x   0        0        0     4596 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_flow9_flow9_js.ee19c04e3556e2f3320e.js.map
+-rwxr-xr-x   0        0        0     5484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_fsharp_fsharp_js.7a7fd32fad2f13d0265b.js
+-rwxr-xr-x   0        0        0     6809 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_fsharp_fsharp_js.7a7fd32fad2f13d0265b.js.map
+-rwxr-xr-x   0        0        0     5105 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_go_go_js.5be77765d5a4b7ffa983.js
+-rwxr-xr-x   0        0        0     6431 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_go_go_js.5be77765d5a4b7ffa983.js.map
+-rwxr-xr-x   0        0        0     4459 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_graphql_graphql_js.4a586f64f410b2ee3f6a.js
+-rwxr-xr-x   0        0        0     5215 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_graphql_graphql_js.4a586f64f410b2ee3f6a.js.map
+-rwxr-xr-x   0        0        0     6040 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_hcl_hcl_js.230c7d363321015f2c60.js
+-rwxr-xr-x   0        0        0     7144 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_hcl_hcl_js.230c7d363321015f2c60.js.map
+-rwxr-xr-x   0        0        0     9137 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_html_html_js.6d7d95bee6027181f0af.js
+-rwxr-xr-x   0        0        0    11085 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_html_html_js.6d7d95bee6027181f0af.js.map
+-rwxr-xr-x   0        0        0     2728 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_ini_ini_js.b4cd6fd84ced941317a1.js
+-rwxr-xr-x   0        0        0     2854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_ini_ini_js.b4cd6fd84ced941317a1.js.map
+-rwxr-xr-x   0        0        0     5758 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_java_java_js.b5a0555fb9f413aebaf1.js
+-rwxr-xr-x   0        0        0     7187 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_java_java_js.b5a0555fb9f413aebaf1.js.map
+-rwxr-xr-x   0        0        0     6132 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_kotlin_kotlin_js.84d331c6922c4b011779.js
+-rwxr-xr-x   0        0        0     7750 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_kotlin_kotlin_js.84d331c6922c4b011779.js.map
+-rwxr-xr-x   0        0        0     6347 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_less_less_js.0cefe82e77a5f720a3a8.js
+-rwxr-xr-x   0        0        0     7847 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_less_less_js.0cefe82e77a5f720a3a8.js.map
+-rwxr-xr-x   0        0        0     4730 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_lexon_lexon_js.5856d26bc8d67dadde9e.js
+-rwxr-xr-x   0        0        0     5606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_lexon_lexon_js.5856d26bc8d67dadde9e.js.map
+-rwxr-xr-x   0        0        0     7442 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_liquid_liquid_js.ccc8e1bb782d3bdb55c0.js
+-rwxr-xr-x   0        0        0     9108 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_liquid_liquid_js.ccc8e1bb782d3bdb55c0.js.map
+-rwxr-xr-x   0        0        0     4386 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_lua_lua_js.7bb5d5716d12f5c2174e.js
+-rwxr-xr-x   0        0        0     5307 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_lua_lua_js.7bb5d5716d12f5c2174e.js.map
+-rwxr-xr-x   0        0        0     5283 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_m3_m3_js.afda01e1b4bcc050d4f2.js
+-rwxr-xr-x   0        0        0     6629 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_m3_m3_js.afda01e1b4bcc050d4f2.js.map
+-rwxr-xr-x   0        0        0     6771 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_markdown_markdown_js.1fb78cdc3130ad3eaba3.js
+-rwxr-xr-x   0        0        0     8213 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_markdown_markdown_js.1fb78cdc3130ad3eaba3.js.map
+-rwxr-xr-x   0        0        0     5181 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_mips_mips_js.1bf6111c8b5601cd2b20.js
+-rwxr-xr-x   0        0        0     6277 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_mips_mips_js.1bf6111c8b5601cd2b20.js.map
+-rwxr-xr-x   0        0        0     8230 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_msdax_msdax_js.64aeebc1b0c103ab96af.js
+-rwxr-xr-x   0        0        0    10919 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_msdax_msdax_js.64aeebc1b0c103ab96af.js.map
+-rwxr-xr-x   0        0        0     4838 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_objective-c_objective-c_js.8c0d01235bc1d630adfa.js
+-rwxr-xr-x   0        0        0     5873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_objective-c_objective-c_js.8c0d01235bc1d630adfa.js.map
+-rwxr-xr-x   0        0        0     5648 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_pascal_pascal_js.df74d1d4ca179e1b1afd.js
+-rwxr-xr-x   0        0        0     7341 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_pascal_pascal_js.df74d1d4ca179e1b1afd.js.map
+-rwxr-xr-x   0        0        0     4257 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_pascaligo_pascaligo_js.ff3af5a55838b031f360.js
+-rwxr-xr-x   0        0        0     5106 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_pascaligo_pascaligo_js.ff3af5a55838b031f360.js.map
+-rwxr-xr-x   0        0        0     3938 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_pla_pla_js.1932e28a5d8475c1ee52.js
+-rwxr-xr-x   0        0        0     4566 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_pla_pla_js.1932e28a5d8475c1ee52.js.map
+-rwxr-xr-x   0        0        0     6473 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_powershell_powershell_js.e3c2ee7998ea24edb731.js
+-rwxr-xr-x   0        0        0     8014 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_powershell_powershell_js.e3c2ee7998ea24edb731.js.map
+-rwxr-xr-x   0        0        0     9200 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_pug_pug_js.9926ff3fec177afe4c34.js
+-rwxr-xr-x   0        0        0    12274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_pug_pug_js.9926ff3fec177afe4c34.js.map
+-rwxr-xr-x   0        0        0     7044 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_python_python_js.f9cd61ae70cb69be71d9.js
+-rwxr-xr-x   0        0        0     8652 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_python_python_js.f9cd61ae70cb69be71d9.js.map
+-rwxr-xr-x   0        0        0     5760 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_qsharp_qsharp_js.3159e1b26ee42f37dc9e.js
+-rwxr-xr-x   0        0        0     7569 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_qsharp_qsharp_js.3159e1b26ee42f37dc9e.js.map
+-rwxr-xr-x   0        0        0     5896 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_r_r_js.08cb4e804cb3e9a28ace.js
+-rwxr-xr-x   0        0        0     7493 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_r_r_js.08cb4e804cb3e9a28ace.js.map
+-rwxr-xr-x   0        0        0     6486 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_redis_redis_js.8ae88e112ec72cfcf9f7.js
+-rwxr-xr-x   0        0        0     8468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_redis_redis_js.8ae88e112ec72cfcf9f7.js.map
+-rwxr-xr-x   0        0        0     6415 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_restructuredtext_restructuredtext_js.562d4848347010a99e0e.js
+-rwxr-xr-x   0        0        0     7509 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_restructuredtext_restructuredtext_js.562d4848347010a99e0e.js.map
+-rwxr-xr-x   0        0        0     7373 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_rust_rust_js.7c87889f44878696136b.js
+-rwxr-xr-x   0        0        0     9872 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_rust_rust_js.7c87889f44878696136b.js.map
+-rwxr-xr-x   0        0        0     3779 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_sb_sb_js.ae2f354ae4f12d7bd72b.js
+-rwxr-xr-x   0        0        0     4229 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_sb_sb_js.ae2f354ae4f12d7bd72b.js.map
+-rwxr-xr-x   0        0        0     3729 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_scheme_scheme_js.e36dc0d354f0f5b3fbf0.js
+-rwxr-xr-x   0        0        0     4205 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_scheme_scheme_js.e36dc0d354f0f5b3fbf0.js.map
+-rwxr-xr-x   0        0        0     9582 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_scss_scss_js.35f4327ac70035ac003a.js
+-rwxr-xr-x   0        0        0    12633 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_scss_scss_js.35f4327ac70035ac003a.js.map
+-rwxr-xr-x   0        0        0     5689 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_shell_shell_js.d8464c269c4488a6b1fe.js
+-rwxr-xr-x   0        0        0     7135 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_shell_shell_js.d8464c269c4488a6b1fe.js.map
+-rwxr-xr-x   0        0        0     5158 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_sophia_sophia_js.e3f378c1653b0a1e984f.js
+-rwxr-xr-x   0        0        0     6252 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_sophia_sophia_js.e3f378c1653b0a1e984f.js.map
+-rwxr-xr-x   0        0        0     4895 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_sparql_sparql_js.d0d19d5b847835e9b1e3.js
+-rwxr-xr-x   0        0        0     6025 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_sparql_sparql_js.d0d19d5b847835e9b1e3.js.map
+-rwxr-xr-x   0        0        0     8323 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_swift_swift_js.47b7cefa925e9c066b7c.js
+-rwxr-xr-x   0        0        0    10656 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_swift_swift_js.47b7cefa925e9c066b7c.js.map
+-rwxr-xr-x   0        0        0     6239 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_tcl_tcl_js.d48ef01cf0e13cf29944.js
+-rwxr-xr-x   0        0        0     8056 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_tcl_tcl_js.d48ef01cf0e13cf29944.js.map
+-rwxr-xr-x   0        0        0     9704 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_twig_twig_js.d82831f1acc1c666fb3d.js
+-rwxr-xr-x   0        0        0    12280 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_twig_twig_js.d82831f1acc1c666fb3d.js.map
+-rwxr-xr-x   0        0        0     9551 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_typescript_typescript_js.0ae9761d4b0d1e6cfa16.js
+-rwxr-xr-x   0        0        0    11825 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_typescript_typescript_js.0ae9761d4b0d1e6cfa16.js.map
+-rwxr-xr-x   0        0        0     9174 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_vb_vb_js.a4905a4081d413b6d210.js
+-rwxr-xr-x   0        0        0    12065 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_vb_vb_js.a4905a4081d413b6d210.js.map
+-rwxr-xr-x   0        0        0     9782 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_wgsl_wgsl_js.645eabcb3aff15176c38.js
+-rwxr-xr-x   0        0        0    12972 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_wgsl_wgsl_js.645eabcb3aff15176c38.js.map
+-rwxr-xr-x   0        0        0     4982 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_xml_xml_js.aacaca7fd9d934e1d513.js
+-rwxr-xr-x   0        0        0     5400 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_xml_xml_js.aacaca7fd9d934e1d513.js.map
+-rwxr-xr-x   0        0        0     7285 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_yaml_yaml_js.f54c221e346beb62289c.js
+-rwxr-xr-x   0        0        0     8643 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_yaml_yaml_js.f54c221e346beb62289c.js.map
+-rwxr-xr-x   0        0        0    23727 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_process_browser_js-data_image_png_base64_iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAAC-c7fe92.426b74ce6f751a6627be.js
+-rwxr-xr-x   0        0        0     6843 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/node_modules_process_browser_js-data_image_png_base64_iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAAC-c7fe92.426b74ce6f751a6627be.js.map
+-rwxr-xr-x   0        0        0    41803 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/remoteEntry.51eae0d238432037ae0e.js
+-rwxr-xr-x   0        0        0    41012 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/remoteEntry.51eae0d238432037ae0e.js.map
+-rwxr-xr-x   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/style.js
+-rwxr-xr-x   0        0        0    19500 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/style_index_js.81c2517e7d07af255c14.js
+-rwxr-xr-x   0        0        0    15018 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/style_index_js.81c2517e7d07af255c14.js.map
+-rwxr-xr-x   0        0        0    43753 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-flume_node_modules_prop-types_index_js-node_modules_process_browser_js.42651e68d03e160d6f50.js
+-rwxr-xr-x   0        0        0    49836 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-flume_node_modules_prop-types_index_js-node_modules_process_browser_js.42651e68d03e160d6f50.js.map
+-rwxr-xr-x   0        0        0    22154 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_abap_abap_js.b9acd748da7ff3350995.js
+-rwxr-xr-x   0        0        0    32103 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_abap_abap_js.b9acd748da7ff3350995.js.map
+-rwxr-xr-x   0        0        0    14810 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_clojure_clojure_js.a5f8283882d0bdb93925.js
+-rwxr-xr-x   0        0        0    20622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_clojure_clojure_js.a5f8283882d0bdb93925.js.map
+-rwxr-xr-x   0        0        0    15527 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_elixir_elixir_js.2979134714531778d948.js
+-rwxr-xr-x   0        0        0    19907 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_elixir_elixir_js.2979134714531778d948.js.map
+-rwxr-xr-x   0        0        0    26576 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_freemarker2_freemarker2_js.7d62e95fa6c125a74bf5.js
+-rwxr-xr-x   0        0        0    33791 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_freemarker2_freemarker2_js.7d62e95fa6c125a74bf5.js.map
+-rwxr-xr-x   0        0        0    11996 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_handlebars_handlebars_js.f2c604f0bc3f6423e8c7.js
+-rwxr-xr-x   0        0        0    14936 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_handlebars_handlebars_js.f2c604f0bc3f6423e8c7.js.map
+-rwxr-xr-x   0        0        0    12598 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_javascript_javascript_js.c3c5914a19d6e077645e.js
+-rwxr-xr-x   0        0        0    14289 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_javascript_javascript_js.c3c5914a19d6e077645e.js.map
+-rwxr-xr-x   0        0        0    11534 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_julia_julia_js.660cedb0abb2fe3e27a7.js
+-rwxr-xr-x   0        0        0    15462 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_julia_julia_js.660cedb0abb2fe3e27a7.js.map
+-rwxr-xr-x   0        0        0    17119 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_mysql_mysql_js.4dcbef8818f057aeaab3.js
+-rwxr-xr-x   0        0        0    23804 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_mysql_mysql_js.4dcbef8818f057aeaab3.js.map
+-rwxr-xr-x   0        0        0    13235 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_perl_perl_js.92abc34c6cf667e58d20.js
+-rwxr-xr-x   0        0        0    18301 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_perl_perl_js.92abc34c6cf667e58d20.js.map
+-rwxr-xr-x   0        0        0    19185 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_pgsql_pgsql_js.0964523139d4821964b6.js
+-rwxr-xr-x   0        0        0    25614 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_pgsql_pgsql_js.0964523139d4821964b6.js.map
+-rwxr-xr-x   0        0        0    12885 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_php_php_js.89c54b836095365cbd76.js
+-rwxr-xr-x   0        0        0    16472 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_php_php_js.89c54b836095365cbd76.js.map
+-rwxr-xr-x   0        0        0    12904 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_postiats_postiats_js.39e416b365187b825ab1.js
+-rwxr-xr-x   0        0        0    17558 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_postiats_postiats_js.39e416b365187b825ab1.js.map
+-rwxr-xr-x   0        0        0    22953 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_powerquery_powerquery_js.794f25521bfb793e2592.js
+-rwxr-xr-x   0        0        0    29584 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_powerquery_powerquery_js.794f25521bfb793e2592.js.map
+-rwxr-xr-x   0        0        0    13967 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_protobuf_protobuf_js.109b1979e218a3fccb2a.js
+-rwxr-xr-x   0        0        0    18320 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_protobuf_protobuf_js.109b1979e218a3fccb2a.js.map
+-rwxr-xr-x   0        0        0    14667 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_razor_razor_js.963081f3fb1d7074c622.js
+-rwxr-xr-x   0        0        0    18604 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_razor_razor_js.963081f3fb1d7074c622.js.map
+-rwxr-xr-x   0        0        0    17358 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_redshift_redshift_js.2bec585aca61add92a63.js
+-rwxr-xr-x   0        0        0    23435 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_redshift_redshift_js.2bec585aca61add92a63.js.map
+-rwxr-xr-x   0        0        0    13475 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_ruby_ruby_js.f1d2de0d3708113d1047.js
+-rwxr-xr-x   0        0        0    17609 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_ruby_ruby_js.f1d2de0d3708113d1047.js.map
+-rwxr-xr-x   0        0        0    11370 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_scala_scala_js.17d63d898fcd57883055.js
+-rwxr-xr-x   0        0        0    14258 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_scala_scala_js.17d63d898fcd57883055.js.map
+-rwxr-xr-x   0        0        0    26840 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_solidity_solidity_js.60c54c6dab98bc84fed9.js
+-rwxr-xr-x   0        0        0    37198 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_solidity_solidity_js.60c54c6dab98bc84fed9.js.map
+-rwxr-xr-x   0        0        0    15932 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_sql_sql_js.e41c82d9fa334693ad98.js
+-rwxr-xr-x   0        0        0    22315 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_sql_sql_js.e41c82d9fa334693ad98.js.map
+-rwxr-xr-x   0        0        0    11243 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_st_st_js.da9aa70576309f2d7607.js
+-rwxr-xr-x   0        0        0    15184 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_st_st_js.da9aa70576309f2d7607.js.map
+-rwxr-xr-x   0        0        0    12392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_systemverilog_systemverilog_js.d4906f14a72eeea290d0.js
+-rwxr-xr-x   0        0        0    16673 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_systemverilog_systemverilog_js.d4906f14a72eeea290d0.js.map
+-rwxr-xr-x   0        0        0 10725780 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_editor_editor_main_js.2f82887a25519ad5606c.js
+-rwxr-xr-x   0        0        0  9781956 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_editor_editor_main_js.2f82887a25519ad5606c.js.map
+-rwxr-xr-x   0        0        0    71400 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_language_css_cssMode_js.0e78e528ecf4b44f65e3.js
+-rwxr-xr-x   0        0        0    83402 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_language_css_cssMode_js.0e78e528ecf4b44f65e3.js.map
+-rwxr-xr-x   0        0        0    72566 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_language_html_htmlMode_js.4d082c3f023de51f874a.js
+-rwxr-xr-x   0        0        0    84609 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_language_html_htmlMode_js.4d082c3f023de51f874a.js.map
+-rwxr-xr-x   0        0        0    86490 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_language_json_jsonMode_js.3877344c5bc28d2c62f1.js
+-rwxr-xr-x   0        0        0   102226 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_language_json_jsonMode_js.3877344c5bc28d2c62f1.js.map
+-rwxr-xr-x   0        0        0    44884 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_language_typescript_tsMode_js.532242b4e273f33ae96d.js
+-rwxr-xr-x   0        0        0    50468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_language_typescript_tsMode_js.532242b4e273f33ae96d.js.map
+-rwxr-xr-x   0        0        0    58952 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_react-portal_es_index_js.e0238c949efe3800e101.js
+-rwxr-xr-x   0        0        0    59619 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_react-portal_es_index_js.e0238c949efe3800e101.js.map
+-rwxr-xr-x   0        0        0    33766 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_uuid_dist_esm-browser_index_js.50ddbbbe16d9fbb8e598.js
+-rwxr-xr-x   0        0        0    25722 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_uuid_dist_esm-browser_index_js.50ddbbbe16d9fbb8e598.js.map
+-rwxr-xr-x   0        0        0    11646 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/schema/plugin.json
+-rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/src/ReRunIcon.tsx
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/src/arrownIcon.tsx
+-rwxr-xr-x   0        0        0     1455 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/src/clearIcon.tsx
+-rwxr-xr-x   0        0        0      954 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/src/deleteIcon.tsx
+-rwxr-xr-x   0        0        0     1505 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/src/exportIcon.tsx
+-rwxr-xr-x   0        0        0     1310 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/src/factory.ts
+-rwxr-xr-x   0        0        0    37793 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/src/flumeConfig.tsx
+-rwxr-xr-x   0        0        0     7454 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/src/imageViewer.tsx
+-rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/src/index.ts
+-rwxr-xr-x   0        0        0     2268 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/src/lockIcon.tsx
+-rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/src/model.ts
+-rwxr-xr-x   0        0        0      807 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/src/newIcon.tsx
+-rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/src/runIcon.tsx
+-rwxr-xr-x   0        0        0     2349 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/src/utils.tsx
+-rwxr-xr-x   0        0        0   169230 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/src/widget.tsx
+-rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/src/yesIcon.tsx
+-rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/style/base.css
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/style/index.css
+-rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/style/index.js
+-rwxr-xr-x   0        0        0   254494 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/test_ext/1.jpeg
+-rwxr-xr-x   0        0        0   153675 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/test_ext/2.jpeg
+-rwxr-xr-x   0        0        0     2162 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/test_ext/main.ipynb
+-rwxr-xr-x   0        0        0   545469 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/test_ext/testlib.ipynb
+-rwxr-xr-x   0        0        0     1586 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/.gitignore
+-rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/LICENSE
+-rwxr-xr-x   0        0        0     2557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/README.md
+-rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.4/PKG-INFO
```

### Comparing `jupyterlab_nodeeditor-1.0.3/RELEASE.md` & `jupyterlab_nodeeditor-1.0.4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/package.json` & `jupyterlab_nodeeditor-1.0.4/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768518518518517%*

 * *Differences: {"'dependencies'": "{'react-portal': '^4.2.2'}", "'version'": "'1.0.4'"}*

```diff
@@ -10,14 +10,15 @@
         "@jupyterlab/application": "^4.0.2",
         "@jupyterlab/apputils": "^4.1.2",
         "@jupyterlab/completer": "^4.0.2",
         "@jupyterlab/notebook": "^4.0.2",
         "@jupyterlab/shared-models": "^3.6.3",
         "@lumino/widgets": "^2.0.1",
         "monaco-editor": "^0.39.0",
+        "react-portal": "^4.2.2",
         "uuid": "^9.0.0"
     },
     "description": "\u4e00\u4e2a\u8282\u70b9\u7f16\u8f91\u5668",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
@@ -174,9 +175,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.3"
+    "version": "1.0.4"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.3/tsconfig.json` & `jupyterlab_nodeeditor-1.0.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/yarn.lock` & `jupyterlab_nodeeditor-1.0.4/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3796,14 +3796,15 @@
     css-loader: ^6.7.1
     eslint: ^8.36.0
     eslint-config-prettier: ^8.7.0
     eslint-plugin-prettier: ^4.2.1
     monaco-editor: ^0.39.0
     npm-run-all: ^4.1.5
     prettier: ^2.8.7
+    react-portal: ^4.2.2
     rimraf: ^4.4.1
     source-map-loader: ^1.0.2
     style-loader: ^3.3.1
     stylelint: ^14.9.1
     stylelint-config-prettier: ^9.0.4
     stylelint-config-recommended: ^8.0.0
     stylelint-config-standard: ^26.0.0
@@ -4649,15 +4650,15 @@
 "process@npm:^0.11.10":
   version: 0.11.10
   resolution: "process@npm:0.11.10"
   checksum: bfcce49814f7d172a6e6a14d5fa3ac92cc3d0c3b9feb1279774708a719e19acd673995226351a082a9ae99978254e320ccda4240ddc474ba31a76c79491ca7c3
   languageName: node
   linkType: hard
 
-"prop-types@npm:^15.8.1":
+"prop-types@npm:^15.5.8, prop-types@npm:^15.8.1":
   version: 15.8.1
   resolution: "prop-types@npm:15.8.1"
   dependencies:
     loose-envify: ^1.4.0
     object-assign: ^4.1.1
     react-is: ^16.13.1
   checksum: c056d3f1c057cb7ff8344c645450e14f088a915d078dcda795041765047fa080d38e5d626560ccaac94a4e16e3aa15f3557c1a9a8d1174530955e992c675e459
@@ -4723,14 +4724,26 @@
 "react-is@npm:^18.2.0":
   version: 18.2.0
   resolution: "react-is@npm:18.2.0"
   checksum: e72d0ba81b5922759e4aff17e0252bd29988f9642ed817f56b25a3e217e13eea8a7f2322af99a06edb779da12d5d636e9fda473d620df9a3da0df2a74141d53e
   languageName: node
   linkType: hard
 
+"react-portal@npm:^4.2.2":
+  version: 4.2.2
+  resolution: "react-portal@npm:4.2.2"
+  dependencies:
+    prop-types: ^15.5.8
+  peerDependencies:
+    react: ^16.0.0-0 || ^17.0.0-0 || ^18.0.0-0
+    react-dom: ^16.0.0-0 || ^17.0.0-0 || ^18.0.0-0
+  checksum: dc7cd0c6907d1859c0eca4571108934ac791eb9eaf020529a26d4732b7bb556a53bf7e87e868f9918bd60c58f512cc36a49aef5671c964d0a49494168fb2abe0
+  languageName: node
+  linkType: hard
+
 "react@npm:^18.2.0":
   version: 18.2.0
   resolution: "react@npm:18.2.0"
   dependencies:
     loose-envify: ^1.1.0
   checksum: 88e38092da8839b830cda6feef2e8505dec8ace60579e46aa5490fc3dc9bba0bd50336507dc166f43e3afc1c42939c09fe33b25fae889d6f402721dcd78fca1b
   languageName: node
```

### Comparing `jupyterlab_nodeeditor-1.0.3/_temp_extension/.gitignore` & `jupyterlab_nodeeditor-1.0.4/_temp_extension/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/_temp_extension/LICENSE` & `jupyterlab_nodeeditor-1.0.4/_temp_extension/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/_temp_extension/README.md` & `jupyterlab_nodeeditor-1.0.4/_temp_extension/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/_temp_extension/RELEASE.md` & `jupyterlab_nodeeditor-1.0.4/_temp_extension/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/_temp_extension/package.json` & `jupyterlab_nodeeditor-1.0.4/_temp_extension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/_temp_extension/pyproject.toml` & `jupyterlab_nodeeditor-1.0.4/_temp_extension/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/_temp_extension/tsconfig.json` & `jupyterlab_nodeeditor-1.0.4/_temp_extension/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/_temp_extension/jupyterlab_nodeeditor/__init__.py` & `jupyterlab_nodeeditor-1.0.4/_temp_extension/jupyterlab_nodeeditor/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/_temp_extension/src/index.ts` & `jupyterlab_nodeeditor-1.0.4/_temp_extension/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/CODE_OF_CONDUCT.md` & `jupyterlab_nodeeditor-1.0.4/flume/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/LICENSE` & `jupyterlab_nodeeditor-1.0.4/flume/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/README.md` & `jupyterlab_nodeeditor-1.0.4/flume/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/logo.ai` & `jupyterlab_nodeeditor-1.0.4/flume/logo.ai`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/logo.png` & `jupyterlab_nodeeditor-1.0.4/flume/logo.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/logo.svg` & `jupyterlab_nodeeditor-1.0.4/flume/logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/package.json` & `jupyterlab_nodeeditor-1.0.4/flume/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/rollup.config.js` & `jupyterlab_nodeeditor-1.0.4/flume/rollup.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/yarn.lock` & `jupyterlab_nodeeditor-1.0.4/flume/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/cypress/integration/NodeEditorSpec.js` & `jupyterlab_nodeeditor-1.0.4/flume/cypress/integration/NodeEditorSpec.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/cypress/plugins/index.js` & `jupyterlab_nodeeditor-1.0.4/flume/cypress/plugins/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/cypress/support/commands.js` & `jupyterlab_nodeeditor-1.0.4/flume/cypress/support/commands.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/cypress/support/index.js` & `jupyterlab_nodeeditor-1.0.4/flume/cypress/support/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/README.md` & `jupyterlab_nodeeditor-1.0.4/flume/docs/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docusaurus.config.js` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/package.json` & `jupyterlab_nodeeditor-1.0.4/flume/docs/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/yarn.lock` & `jupyterlab_nodeeditor-1.0.4/flume/docs/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/components/AnatomyExample.js` & `jupyterlab_nodeeditor-1.0.4/flume/docs/components/AnatomyExample.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/components/Colors.js` & `jupyterlab_nodeeditor-1.0.4/flume/docs/components/Colors.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/components/ControlExamples.js` & `jupyterlab_nodeeditor-1.0.4/flume/docs/components/ControlExamples.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/components/DynamicNodesExamples.js` & `jupyterlab_nodeeditor-1.0.4/flume/docs/components/DynamicNodesExamples.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/components/DynamicThemingExample.js` & `jupyterlab_nodeeditor-1.0.4/flume/docs/components/DynamicThemingExample.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/components/GettingStartedExample.js` & `jupyterlab_nodeeditor-1.0.4/flume/docs/components/GettingStartedExample.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/NodeEditor.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/NodeEditor.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/RootEngine.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/RootEngine.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/anatomy.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/anatomy.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/basic-config.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/basic-config.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/colors.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/colors.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/comments.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/comments.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/controls.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/controls.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/defining-nodes.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/defining-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/doc1.md` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/doc1.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/doc3.md` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/doc3.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/dynamic-nodes.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/dynamic-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/faq.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/faq.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/flume-config.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/flume-config.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/logic-nodes.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/logic-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/mdx.md` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/mdx.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/node-editor.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/node-editor.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/overview.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/overview.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/quick-start.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/quick-start.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/root-engine.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/root-engine.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/root-node.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/root-node.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/running-logic.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/running-logic.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/saving-nodes.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/saving-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/theming.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/theming.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/type-safety.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/type-safety.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/using-with-react.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/using-with-react.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/docs/using-without-react.mdx` & `jupyterlab_nodeeditor-1.0.4/flume/docs/docs/using-without-react.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/src/exampleFlumeConfig.js` & `jupyterlab_nodeeditor-1.0.4/flume/docs/src/exampleFlumeConfig.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/src/components/TypeSafe.js` & `jupyterlab_nodeeditor-1.0.4/flume/docs/src/components/TypeSafe.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/src/css/custom.css` & `jupyterlab_nodeeditor-1.0.4/flume/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/src/pages/index.js` & `jupyterlab_nodeeditor-1.0.4/flume/docs/src/pages/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/src/pages/styles.module.css` & `jupyterlab_nodeeditor-1.0.4/flume/docs/src/pages/styles.module.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/60fps.svg` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/60fps.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/android-chrome-192x192.png` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/android-chrome-512x512.png` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/apple-touch-icon.png` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/controls.svg` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/controls.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/example_editors.png` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/example_editors.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/favicon-32x32.png` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/favicon.ico` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/fb-img.png` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/fb-img.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/flume-short-web.mp4` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/flume-short-web.mp4`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/friends-graph.svg` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/friends-graph.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/hero-nodes.svg` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/hero-nodes.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/logo-dark.svg` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/logo.svg` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/netlify.svg` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/netlify.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/performance-tile.svg` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/performance-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/react-tile.svg` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/react-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/size-tile.svg` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/size-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/theme-tile.svg` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/theme-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/theme.svg` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/theme.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/type-safe-node.svg` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/type-safe-node.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/type-safe-nodes.svg` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/type-safe-nodes.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/undraw_docusaurus_mountain.svg` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/undraw_docusaurus_mountain.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/undraw_docusaurus_react.svg` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/undraw_docusaurus_react.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/undraw_docusaurus_tree.svg` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/undraw_docusaurus_tree.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/docs/static/img/valid_port_types.png` & `jupyterlab_nodeeditor-1.0.4/flume/docs/static/img/valid_port_types.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/README.md` & `jupyterlab_nodeeditor-1.0.4/flume/example/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/package.json` & `jupyterlab_nodeeditor-1.0.4/flume/example/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/yarn.lock` & `jupyterlab_nodeeditor-1.0.4/flume/example/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/public/index.html` & `jupyterlab_nodeeditor-1.0.4/flume/example/public/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/App.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/App.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/index.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/TestRoutes/TestEditor.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/TestRoutes/TestEditor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/TestRoutes/nodes.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/TestRoutes/nodes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/components/Checkbox.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/components/Checkbox.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/components/FloatingNavigation.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/components/FloatingNavigation.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/components/LogicEditor.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/components/LogicEditor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/components/OptionsEditor.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/components/OptionsEditor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/icons/BoxIcon.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/icons/BoxIcon.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/icons/FormIcon.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/icons/FormIcon.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/icons/GearIcon.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/icons/GearIcon.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/Attributes.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/Attributes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/Body.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/Body.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/Field.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/Field.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/Form.css` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/Form.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/Form.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/Form.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/InputTypes.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/InputTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/NodeTypes.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/NodeTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/PreviewField.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/PreviewField.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/Sidebar.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/Sidebar.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/designerReducer.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/designerReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/fieldTypes.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/fieldTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/fieldsReducer.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/fieldsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/previewFieldsReducer.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/previewFieldsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/resolveLogic.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/resolveLogic.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Form/wizardLogic/logicTypes.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Form/wizardLogic/logicTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Forms/Forms.css` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Forms/Forms.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Forms/Forms.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Forms/Forms.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Records/Records.css` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Records/Records.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/example/src/pages/Records/Records.js` & `jupyterlab_nodeeditor-1.0.4/flume/example/src/pages/Records/Records.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/RootEngine.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/RootEngine.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/connectionCalculator.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/connectionCalculator.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/context.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/context.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/index.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -26,15 +26,17 @@
 import {
     createConnections
 } from "./connectionCalculator";
 import nodesReducer, {
     connectNodesReducer,
     getInitialNodes
 } from "./nodesReducer";
-import commentsReducer from "./commentsReducer";
+import {
+    connectCommentsReducer
+} from "./commentsReducer";
 import toastsReducer from "./toastsReducer";
 import stageReducer from "./stageReducer";
 import usePrevious from "./hooks/usePrevious";
 import clamp from "lodash/clamp";
 import Cache from "./Cache";
 import {
     STAGE_ID,
@@ -95,21 +97,17 @@
                 owner
             },
             setSideEffectToasts
         ), {},
         () => getInitialNodes(initialNodes, defaultNodes, nodeTypes, portTypes, context)
     );
 
-    if (owner) {
-        owner.dispatchNodes = dispatchNodes
-        owner.getInitialNodes = getInitialNodes
-    }
 
     const [comments, dispatchComments] = React.useReducer(
-        commentsReducer,
+        connectCommentsReducer(owner),
         initialComments || {}
     );
     React.useEffect(() => {
         dispatchNodes({
             type: "HYDRATE_DEFAULT_NODES"
         });
     }, []);
@@ -175,22 +173,26 @@
         if (sideEffectToasts) {
             dispatchToasts(sideEffectToasts)
             setSideEffectToasts(null)
         }
     }, [sideEffectToasts])
 
     if (owner && owner.outOptions) {
+        owner.dispatchNodes = dispatchNodes
+        owner.getInitialNodes = getInitialNodes
+        owner.dispatchComments = dispatchComments
         owner.outOptions({
             // 导出刷新cache, 当重新初始化所有的nodes的时候需要刷新cache
             refreshCache: () => {
                 cache.current = new Cache()
             },
             recalculateStageRect,
             nanoid,
             editorId,
+            triggerRecalculation,
         })
     }
 
     return ( <
         PortTypesContext.Provider value = {
             portTypes
         } >
```

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/nodesReducer.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/nodesReducer.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -238,14 +238,26 @@
         ).reduce((obj2, control) => {
             obj2[control.name] = control.defaultValue;
             return obj2;
         }, {});
         return obj;
     }, {});
 };
+
+const clearNodes = (nodes) => {
+    let keys = []
+    for (const key in nodes) {
+        keys.push(key)
+    }
+    for (const key of keys) {
+        nodes = removeNode(nodes, key)
+    }
+    return nodes
+}
+
 const nodesReducer = (
     nodes,
     action = {}, {
         nodeTypes,
         portTypes,
         cache,
         circularBehavior,
@@ -304,18 +316,24 @@
 
     const rebuildNodeConnections = (nodes, node) => {
         for (const portName in node.connections.inputs) {
             let from = node.connections.inputs[portName][0]
             if (!from) continue
             let targetNode = nodes[from.nodeId]
             if (!targetNode) continue
-            targetNode.connections.outputs[from.portName] = [{
-                nodeId: node.id,
-                portName: portName
-            }]
+            targetNode.connections.outputs[from.portName] = targetNode.connections.outputs[from.portName] || []
+            let ret = targetNode.connections.outputs[from.portName].findIndex((value, index) => {
+                value.nodeId == node.id && value.portName == portName
+            })
+            if (ret == -1) {
+                targetNode.connections.outputs[from.portName].push({
+                    nodeId: node.id,
+                    portName
+                })
+            }
         }
 
         for (const portName in node.connections.outputs) {
             let to = node.connections.outputs[portName][0]
             if (!to) continue
             let targetNode = nodes[to.nodeId]
             if (!targetNode) continue
@@ -447,18 +465,21 @@
         }
         case "ADD_NODES": {
             const {
                 nodes: add_nodes
             } = action;
             let _nodes = nodes
             for (const node of add_nodes) {
-                _nodes = rebuildNodeConnections({
+                _nodes = {
                     ..._nodes,
                     [node.id]: node
-                }, node)
+                }
+            }
+            for (const node of add_nodes) {
+                _nodes = rebuildNodeConnections(_nodes, _nodes[node.id])
             }
             return _nodes
         }
 
         case "REMOVE_NODE": {
             const {
                 nodeId
@@ -543,26 +564,19 @@
                     x,
                     y
                 }
             };
         }
         // 用于清空所有的节点
         case "CLEAR": {
-            let keys = []
-            let nodes = action.nodes
-            for (const key in nodes) {
-                keys.push(key)
-            }
-            for (const key of keys) {
-                nodes = removeNode(nodes, key)
-            }
-            return {}
+            return clearNodes(nodes)
         }
 
         case "RE_INIT": {
+            clearNodes(nodes)
             return action.nodes
         }
 
         case "SET_NODE_WIDTH": {
             const {
                 nodeId,
                 width
```

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/toastsReducer.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/toastsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/typeBuilders.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/typeBuilders.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/utilities.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/utilities.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/Checkbox/Checkbox.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/Checkbox/Checkbox.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/ColorPicker/ColorPicker.css` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/ColorPicker/ColorPicker.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/ColorPicker/ColorPicker.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/ColorPicker/ColorPicker.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/Comment/Comment.css` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/Comment/Comment.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/Connection/Connection.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/Connection/Connection.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/ContextMenu/ContextMenu.css` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/ContextMenu/ContextMenu.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/ContextMenu/ContextMenu.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/ContextMenu/ContextMenu.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -99,15 +99,15 @@
         React.useEffect(() => {
             if (!filter) {
                 setFilterOptions(options)
                 return
             }
             let opts = filterOptions(filter, options)
             setFilterOptions(opts)
-            if (owner) {
+            if (owner && owner.onContextMenuFilter) {
                 owner.onContextMenuFilter(filter, opts, setFilterOptions, filterOptions, from)
             }
 
             if (onFilter) {
                 onFilter(filter, opts, setFilterOptions, filterOptions, from)
             }
         }, [filter, options])
@@ -171,14 +171,15 @@
         }, [selectedIndex]);
 
         if (owner && owner.outOptions) {
             owner.outOptions({
                 setFilter,
                 setFilterOptions,
                 filterOptions,
+                menuInputRef: filterInput
             })
 
             React.useEffect(() => {
                 owner.onMenuStateChange(true, hideFilter, from)
                 return () => {
                     owner.onMenuStateChange(false, hideFilter, from)
                 }
```

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/Control/Control.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/Control/Control.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/Draggable/Draggable.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/Draggable/Draggable.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/IoPorts/IoPorts.css` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/IoPorts/IoPorts.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/IoPorts/IoPorts.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/IoPorts/IoPorts.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/Node/Node.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/Node/Node.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/Select/Select.css` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/Select/Select.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/Select/Select.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/Select/Select.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -89,28 +89,28 @@
                                 } <
                                 /OptionChip>
                             );
                         })
                     } <
                     /div>
                 ) : null
-            ) : data ? ( <
+            ) : (data || data == 0) ? ( <
                 SelectedOption wrapperRef = {
                     wrapper
                 }
                 option = {
                     selectedOption
                 }
                 onClick = {
                     openDrawer
                 }
                 />
             ) : null
         } {
-            (allowMultiple || !data) &&
+            (allowMultiple || (!data && data != 0)) &&
             <
             div className = {
                 selectStyles.wrapper
             }
             ref = {
                 wrapper
             }
```

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/Stage/Stage.css` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/Stage/Stage.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/Stage/Stage.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/Stage/Stage.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -171,23 +171,32 @@
         setMenuOpen(false);
     };
 
     const byScale = value => (1 / scale) * value;
 
     const addNode = ({
         node,
-        internalType
+        internalType,
+        position = null
     }) => {
         const wrapperRect = wrapper.current.getBoundingClientRect();
-        const x =
-            byScale(menuCoordinates.x - wrapperRect.x - wrapperRect.width / 2) +
-            byScale(translate.x);
-        const y =
-            byScale(menuCoordinates.y - wrapperRect.y - wrapperRect.height / 2) +
-            byScale(translate.y);
+        let x = 0
+        let y = 0
+        if (position) {
+            x = position.x
+            y = position.y
+        } else {
+            x =
+                byScale(menuCoordinates.x - wrapperRect.x - wrapperRect.width / 2) +
+                byScale(translate.x);
+            y =
+                byScale(menuCoordinates.y - wrapperRect.y - wrapperRect.height / 2) +
+                byScale(translate.y);
+        }
+
         if (internalType === "comment") {
             dispatchComments({
                 type: "ADD_COMMENT",
                 x,
                 y
             });
         } else {
@@ -196,14 +205,25 @@
                 x,
                 y,
                 nodeType: node.type
             });
         }
     };
 
+    const backScale = value => value * scale
+    const nodeXY2ClientXY = (x, y) => {
+        const wrapperRect = wrapper.current.getBoundingClientRect();
+        const retX = backScale(x - byScale(translate.x)) + wrapperRect.x + wrapperRect.width / 2
+        const retY = backScale(y - byScale(translate.y)) + wrapperRect.y + wrapperRect.height / 2
+        return {
+            x: retX,
+            y: retY
+        }
+    }
+
     const handleDocumentKeyUp = e => {
         if (e.which === 32) {
             setSpaceIsPressed(false);
             document.removeEventListener("keyup", handleDocumentKeyUp);
         }
     };
 
@@ -255,14 +275,15 @@
     // 导出函数
     if (owner && owner.outOptions) {
         owner.outOptions({
             addNode,
             setMenuOpen,
             setMenuCoordinates,
             handleContextMenu,
+            nodeXY2ClientXY,
             draggableRef: wrapper,
             translateWrapper,
             scaleWrapper,
             dispatchStageState,
             stagetScale: scale,
             stagetTranslate: translate,
         })
```

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/TextInput/TextInput.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/TextInput/TextInput.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -15,14 +15,16 @@
     nodeId,
     portName,
     name,
 }) => {
     const numberInput = React.useRef()
     const recalculateStageRect = React.useContext(RecalculateStageRectContext)
     const owner = React.useContext(OwnerContext)
+    const isInputting = React.useRef(false)
+
 
     const handleDragEnd = () => {
         document.removeEventListener("mousemove", handleMouseMove);
         document.removeEventListener("mouseup", handleDragEnd);
     };
 
     const handleMouseMove = e => {
@@ -31,19 +33,29 @@
     };
 
     const handlePossibleResize = e => {
         e.stopPropagation();
         recalculateStageRect();
         document.addEventListener("mousemove", handleMouseMove);
         document.addEventListener("mouseup", handleDragEnd);
-        if (owner) {
+        if (owner && owner.setInputing) {
             owner.setInputing(true)
+            isInputting.current = true
         }
     };
 
+    React.useEffect(() => {
+        return () => {
+            if (isInputting.current && owner && owner.setInputing) {
+                owner.setInputing(false)
+                isInputting.current = false
+            }
+        }
+    }, [])
+
     return ( <
         div className = {
             styles.wrapper
         }
         data - flume - component = "text-input" > {
             type === "number" ? ( <
                 input data - flume - component = "text-input-number"
@@ -74,15 +86,15 @@
                 }
                 onBlur = {
                     e => {
                         if (!e.target.value) {
                             onChange(0);
                             numberInput.current.value = 0;
                         }
-                        if (owner) {
+                        if (owner && owner.setInputing) {
                             owner.setInputing(false)
                         }
                     }
                 }
                 step = {
                     step || "1"
                 }
@@ -148,15 +160,15 @@
                     portName
                 }
                 data - name = {
                     name
                 }
                 onBlur = {
                     e => {
-                        if (owner) {
+                        if (owner && owner.setInputing) {
                             owner.setInputing(false)
                         }
                     }
                 }
                 />
             )
         } <
```

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/Toaster/Toaster.css` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/Toaster/Toaster.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/components/Toaster/Toaster.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/components/Toaster/Toaster.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/tests/dynamic.test.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/tests/dynamic.test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/tests/nodes.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/tests/nodes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/tests/ssr.test.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/tests/ssr.test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/flume/src/tests/test.js` & `jupyterlab_nodeeditor-1.0.4/flume/src/tests/test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/package.json` & `jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.976417824074074%*

 * *Differences: {"'dependencies'": "{'react-portal': '^4.2.2'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.51eae0d238432037ae0e.js'}}",*

 * * "'version'": "'1.0.4'"}*

```diff
@@ -10,14 +10,15 @@
         "@jupyterlab/application": "^4.0.2",
         "@jupyterlab/apputils": "^4.1.2",
         "@jupyterlab/completer": "^4.0.2",
         "@jupyterlab/notebook": "^4.0.2",
         "@jupyterlab/shared-models": "^3.6.3",
         "@lumino/widgets": "^2.0.1",
         "monaco-editor": "^0.39.0",
+        "react-portal": "^4.2.2",
         "uuid": "^9.0.0"
     },
     "description": "\u4e00\u4e2a\u8282\u70b9\u7f16\u8f91\u5668",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
@@ -106,15 +107,15 @@
         "schema/**/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/github_username/jupyterlab_nodeeditor",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.02d460eb6f0da6b03b5c.js",
+            "load": "static/remoteEntry.51eae0d238432037ae0e.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_nodeeditor/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -179,9 +180,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.3"
+    "version": "1.0.4"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig` & `jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768518518518517%*

 * *Differences: {"'dependencies'": "{'react-portal': '^4.2.2'}", "'version'": "'1.0.4'"}*

```diff
@@ -10,14 +10,15 @@
         "@jupyterlab/application": "^4.0.2",
         "@jupyterlab/apputils": "^4.1.2",
         "@jupyterlab/completer": "^4.0.2",
         "@jupyterlab/notebook": "^4.0.2",
         "@jupyterlab/shared-models": "^3.6.3",
         "@lumino/widgets": "^2.0.1",
         "monaco-editor": "^0.39.0",
+        "react-portal": "^4.2.2",
         "uuid": "^9.0.0"
     },
     "description": "\u4e00\u4e2a\u8282\u70b9\u7f16\u8f91\u5668",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
@@ -174,9 +175,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.3"
+    "version": "1.0.4"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json` & `jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9728145424836602%*

 * *Differences: {"'jupyter.lab.menus'": "{'main': {0: {'items': {insert: [(2, OrderedDict([('command', "*

 * *                        "'nd-delete')])), (4, OrderedDict([('command', 'nd-copy')])), (29, "*

 * *                        "OrderedDict([('command', 'nd-cell-up')])), (30, OrderedDict([('command', "*

 * *                        "'nd-cell-down')])), (32, OrderedDict([('command', "*

 * *                        "'nd-open-comment-color-picker')])), (33, OrderedDict([('command', "*

 * *                        "'nd-combine-selected-nodes')])), (3 […]*

```diff
@@ -9,17 +9,23 @@
                     {
                         "command": "nd-load"
                     },
                     {
                         "command": "nd-create"
                     },
                     {
+                        "command": "nd-delete"
+                    },
+                    {
                         "command": "nd-rename"
                     },
                     {
+                        "command": "nd-copy"
+                    },
+                    {
                         "command": "nd-run-all-cells"
                     },
                     {
                         "command": "nd-clear-run-cache"
                     },
                     {
                         "command": "nd-undo"
@@ -84,62 +90,84 @@
                     {
                         "command": "nd-edit-pre-cell"
                     },
                     {
                         "command": "nd-edit-next-cell"
                     },
                     {
+                        "command": "nd-cell-up"
+                    },
+                    {
+                        "command": "nd-cell-down"
+                    },
+                    {
                         "command": "nd-set-as-default"
+                    },
+                    {
+                        "command": "nd-open-comment-color-picker"
+                    },
+                    {
+                        "command": "nd-combine-selected-nodes"
+                    },
+                    {
+                        "command": "nd-separate-selected-node"
                     }
                 ],
                 "label": "\u8282\u70b9\u7f16\u8f91\u5668",
                 "rank": 100
             }
         ]
     },
     "jupyter.lab.shortcuts": [
         {
             "command": "nd-load",
             "keys": [
-                "Accel R"
+                "L"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-create",
             "keys": [
-                "Alt N"
+                "N"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-delete",
             "keys": [
-                "Alt D"
+                "X"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-rename",
             "keys": [
-                "Alt R"
+                "R"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
+        },
+        {
+            "command": "nd-copy",
+            "keys": [
+                "Shift F"
+            ],
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-run-all-cells",
             "keys": [
-                "Accel Alt R"
+                "Shift R"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
         },
         {
             "command": "nd-clear-run-cache",
             "keys": [
-                "Alt C"
+                "Shift C"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
         },
         {
             "command": "nd-undo",
             "keys": [
                 "Accel Z"
@@ -152,38 +180,38 @@
                 "Accel Y"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-reset-viewport",
             "keys": [
-                "Alt G"
+                "G"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-toggle-output-area",
             "keys": [
-                "Accel O"
+                "Accel E"
             ],
             "selector": "[data-show-image-viewer=false]"
         },
         {
             "command": "nd-clear-output-area",
             "keys": [
                 "Accel L"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false]"
         },
         {
             "command": "nd-open-code-editor",
             "keys": [
-                "Accel E"
+                "E"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-kernel-interrupt",
             "keys": [
                 "Accel I"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
@@ -194,24 +222,24 @@
                 "Accel K"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
         },
         {
             "command": "nd-select-all",
             "keys": [
-                "Accel Alt A"
+                "Accel A"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-delete-selected-nodes",
             "keys": [
-                "Delete"
+                "D"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-copy-selected-nodes",
             "keys": [
                 "Accel C"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
@@ -222,17 +250,17 @@
                 "Accel V"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-focus-to-selected-nodes",
             "keys": [
-                "Alt F"
+                "F"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-close-image-viewer",
             "keys": [
                 "Escape"
             ],
             "selector": "[data-show-image-viewer=true][data-show-code-editor=false]"
@@ -281,12 +309,54 @@
         },
         {
             "command": "nd-edit-next-cell",
             "keys": [
                 "Alt ArrowDown"
             ],
             "selector": "[data-show-image-viewer=false][data-use-diff-editor=false]"
+        },
+        {
+            "command": "nd-cell-up",
+            "keys": [
+                "Shift ArrowUp"
+            ],
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
+        },
+        {
+            "command": "nd-cell-down",
+            "keys": [
+                "Shift ArrowDown"
+            ],
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
+        },
+        {
+            "command": "nd-set-as-default",
+            "keys": [
+                "Alt Shift D"
+            ],
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
+        },
+        {
+            "command": "nd-open-comment-color-picker",
+            "keys": [
+                "C"
+            ],
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
+        },
+        {
+            "command": "nd-combine-selected-nodes",
+            "keys": [
+                "B"
+            ],
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
+        },
+        {
+            "command": "nd-separate-selected-node",
+            "keys": [
+                "Shift B"
+            ],
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         }
     ],
     "title": "\u8282\u70b9\u7f16\u8f91\u5668",
     "type": "object"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.3/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf` & `jupyterlab_nodeeditor-1.0.4/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/schema/plugin.json` & `jupyterlab_nodeeditor-1.0.4/schema/plugin.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9728145424836602%*

 * *Differences: {"'jupyter.lab.menus'": "{'main': {0: {'items': {insert: [(2, OrderedDict([('command', "*

 * *                        "'nd-delete')])), (4, OrderedDict([('command', 'nd-copy')])), (29, "*

 * *                        "OrderedDict([('command', 'nd-cell-up')])), (30, OrderedDict([('command', "*

 * *                        "'nd-cell-down')])), (32, OrderedDict([('command', "*

 * *                        "'nd-open-comment-color-picker')])), (33, OrderedDict([('command', "*

 * *                        "'nd-combine-selected-nodes')])), (3 […]*

```diff
@@ -9,17 +9,23 @@
                     {
                         "command": "nd-load"
                     },
                     {
                         "command": "nd-create"
                     },
                     {
+                        "command": "nd-delete"
+                    },
+                    {
                         "command": "nd-rename"
                     },
                     {
+                        "command": "nd-copy"
+                    },
+                    {
                         "command": "nd-run-all-cells"
                     },
                     {
                         "command": "nd-clear-run-cache"
                     },
                     {
                         "command": "nd-undo"
@@ -84,62 +90,84 @@
                     {
                         "command": "nd-edit-pre-cell"
                     },
                     {
                         "command": "nd-edit-next-cell"
                     },
                     {
+                        "command": "nd-cell-up"
+                    },
+                    {
+                        "command": "nd-cell-down"
+                    },
+                    {
                         "command": "nd-set-as-default"
+                    },
+                    {
+                        "command": "nd-open-comment-color-picker"
+                    },
+                    {
+                        "command": "nd-combine-selected-nodes"
+                    },
+                    {
+                        "command": "nd-separate-selected-node"
                     }
                 ],
                 "label": "\u8282\u70b9\u7f16\u8f91\u5668",
                 "rank": 100
             }
         ]
     },
     "jupyter.lab.shortcuts": [
         {
             "command": "nd-load",
             "keys": [
-                "Accel R"
+                "L"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-create",
             "keys": [
-                "Alt N"
+                "N"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-delete",
             "keys": [
-                "Alt D"
+                "X"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-rename",
             "keys": [
-                "Alt R"
+                "R"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
+        },
+        {
+            "command": "nd-copy",
+            "keys": [
+                "Shift F"
+            ],
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-run-all-cells",
             "keys": [
-                "Accel Alt R"
+                "Shift R"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
         },
         {
             "command": "nd-clear-run-cache",
             "keys": [
-                "Alt C"
+                "Shift C"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
         },
         {
             "command": "nd-undo",
             "keys": [
                 "Accel Z"
@@ -152,38 +180,38 @@
                 "Accel Y"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-reset-viewport",
             "keys": [
-                "Alt G"
+                "G"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-toggle-output-area",
             "keys": [
-                "Accel O"
+                "Accel E"
             ],
             "selector": "[data-show-image-viewer=false]"
         },
         {
             "command": "nd-clear-output-area",
             "keys": [
                 "Accel L"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false]"
         },
         {
             "command": "nd-open-code-editor",
             "keys": [
-                "Accel E"
+                "E"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-kernel-interrupt",
             "keys": [
                 "Accel I"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
@@ -194,24 +222,24 @@
                 "Accel K"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
         },
         {
             "command": "nd-select-all",
             "keys": [
-                "Accel Alt A"
+                "Accel A"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-delete-selected-nodes",
             "keys": [
-                "Delete"
+                "D"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-copy-selected-nodes",
             "keys": [
                 "Accel C"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
@@ -222,17 +250,17 @@
                 "Accel V"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-focus-to-selected-nodes",
             "keys": [
-                "Alt F"
+                "F"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-close-image-viewer",
             "keys": [
                 "Escape"
             ],
             "selector": "[data-show-image-viewer=true][data-show-code-editor=false]"
@@ -281,12 +309,54 @@
         },
         {
             "command": "nd-edit-next-cell",
             "keys": [
                 "Alt ArrowDown"
             ],
             "selector": "[data-show-image-viewer=false][data-use-diff-editor=false]"
+        },
+        {
+            "command": "nd-cell-up",
+            "keys": [
+                "Shift ArrowUp"
+            ],
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
+        },
+        {
+            "command": "nd-cell-down",
+            "keys": [
+                "Shift ArrowDown"
+            ],
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
+        },
+        {
+            "command": "nd-set-as-default",
+            "keys": [
+                "Alt Shift D"
+            ],
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
+        },
+        {
+            "command": "nd-open-comment-color-picker",
+            "keys": [
+                "C"
+            ],
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
+        },
+        {
+            "command": "nd-combine-selected-nodes",
+            "keys": [
+                "B"
+            ],
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
+        },
+        {
+            "command": "nd-separate-selected-node",
+            "keys": [
+                "Shift B"
+            ],
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         }
     ],
     "title": "\u8282\u70b9\u7f16\u8f91\u5668",
     "type": "object"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.3/src/ReRunIcon.tsx` & `jupyterlab_nodeeditor-1.0.4/src/ReRunIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/src/arrownIcon.tsx` & `jupyterlab_nodeeditor-1.0.4/src/arrownIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/src/clearIcon.tsx` & `jupyterlab_nodeeditor-1.0.4/src/clearIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/src/deleteIcon.tsx` & `jupyterlab_nodeeditor-1.0.4/src/deleteIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/src/exportIcon.tsx` & `jupyterlab_nodeeditor-1.0.4/src/exportIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/src/factory.ts` & `jupyterlab_nodeeditor-1.0.4/src/factory.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/src/flumeConfig.tsx` & `jupyterlab_nodeeditor-1.0.4/src/flumeConfig.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,40 @@
     },
     control: (ports, label, name, defaultValue) => {
         return ports.control({
             label: "控制",
             name: "control",
         })
     },
+    ["jupyterlab_nodeeditor.select.select"]: (ports, label, name, defaultValue) => {
+        return ports.select({
+            label,
+            name,
+            controls: [
+                Controls.select({
+                    name,
+                    label,
+                    options: defaultValue
+                })
+            ]
+        })
+    },
+    ["jupyterlab_nodeeditor.select.mselect"]: (ports, label, name, defaultValue) => {
+        return ports.mselect({
+            label,
+            name,
+            controls: [
+                Controls.multiselect({
+                    name,
+                    label,
+                    options: defaultValue
+                })
+            ]
+        })
+    }
 }
 
 let renderCache = {}
 
 export function common_out(ports) {
     return [
         get_port_func("control")(ports),
@@ -187,17 +213,17 @@
     return maxV
 }
 
 export function tuple_value_name(index) {
     return `v${index}`
 }
 
-export function set_port_control_value(nodeId, port_name, value: any) {
+export function set_port_control_value(targetElement, nodeId, port_name, value: any) {
     let selector = `[data-node-id='${nodeId}'][data-port-name='${port_name}']`
-    let element = document.querySelector(selector)
+    let element = targetElement.querySelector(selector)
     if (!element || !element.parentElement) return false
     let port_type = element.getAttribute("data-port-type")
     switch (port_type) {
         case "string":
         case "any": {
             let textAreaElements = element.parentElement.getElementsByTagName("textarea")
             if (textAreaElements.length <= 0) return false
@@ -383,15 +409,15 @@
                             executionContext.setShowImg(true)
                         }
 
                         const onLoad = (e) => {
                             try {
                                 executionContext.updateNodeConnections(portProps.nodeId)
                             } catch (error) {
-                                
+
                             }
                         }
                         return (
                             <div>
                                 <button onClick={showImg}>浏览</button>
                                 <button onClick={e => {
                                     let new_index = (data.index - 1 + data.urls.length) % data.urls.length
@@ -814,34 +840,28 @@
             initialWidth: 250,
             inputs: ports => [
                 get_port_func("control")(ports),
                 get_port_func("string")(ports, "url列表", "urls"),
                 ports.image({ hidePort: true })
 
             ],
-            outputs: ports => [
-                get_port_func("control")(ports),
-                get_port_func("string")(ports, "url列表", "urls"),
-            ]
+            outputs: common_out
         })
         .addNodeType({
             type: "video",
             label: "视频(show video)",
             description: "视频(show video)",
             initialWidth: 250,
             inputs: ports => [
                 get_port_func("control")(ports),
                 get_port_func("string")(ports, "url列表", "urls"),
                 ports.video({ hidePort: true })
 
             ],
-            outputs: ports => [
-                get_port_func("control")(ports),
-                get_port_func("string")(ports, "url列表", "urls"),
-            ]
+            outputs: common_out
         })
         .addNodeType({
             type: "any",
             label: "任意类型(any)",
             description: "任意类型(any)",
             initialWidth: buildNodeWidth("any", headerFontsize, nodeMinWidth, nodeMaxWidth),
             inputs: ports => [
@@ -869,15 +889,15 @@
 
                     let cache = tupleCache[nodeId]
                     if (!cache || cache.length != inputData.tuple_editor.tuple_editor.length) {
                         setTimeout(() => {
                             let index = 0
                             for (const port_type of inputData.tuple_editor.tuple_editor) {
                                 let name = tuple_value_name(index++)
-                                set_port_control_value(nodeId, name,
+                                set_port_control_value(executionContext.node, nodeId, name,
                                     inputData[name] ? inputData[name][name] : null)
                             }
                         })
                     }
 
                     tupleCache[nodeId] = JSON.parse(JSON.stringify(inputData.tuple_editor.tuple_editor))
                 }
@@ -918,15 +938,15 @@
                         }
                     }
 
                     if (!cache || resetData) {
                         setTimeout(() => {
                             for (const name in inputData.dict_editor.dict_editor) {
                                 tmp_name = make_dict_name(name, port_type)
-                                set_port_control_value(nodeId, tmp_name,
+                                set_port_control_value(executionContext.node, nodeId, tmp_name,
                                     inputData[tmp_name] ? inputData[tmp_name][tmp_name] : null)
                             }
                         })
                     }
                     dictCache[nodeId] = JSON.parse(JSON.stringify(inputData.dict_editor.dict_editor))
                 }
                 return ret
```

### Comparing `jupyterlab_nodeeditor-1.0.3/src/imageViewer.tsx` & `jupyterlab_nodeeditor-1.0.4/src/imageViewer.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/src/index.ts` & `jupyterlab_nodeeditor-1.0.4/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/src/lockIcon.tsx` & `jupyterlab_nodeeditor-1.0.4/src/lockIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/src/newIcon.tsx` & `jupyterlab_nodeeditor-1.0.4/src/newIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/src/runIcon.tsx` & `jupyterlab_nodeeditor-1.0.4/src/runIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/src/widget.tsx` & `jupyterlab_nodeeditor-1.0.4/src/widget.tsx`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,95 @@
 import { DocumentWidget, DocumentRegistry } from "@jupyterlab/docregistry"
 import {
     Dialog,
     showDialog,
     SessionContextDialogs,
     ReactWidget,
     ICommandPalette,
+    showErrorMessage,
 } from "@jupyterlab/apputils";
 import {
     JupyterFrontEnd,
 } from "@jupyterlab/application"
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { ITranslator, nullTranslator } from '@jupyterlab/translation';
 import { KernelError } from "@jupyterlab/notebook";
 import { KernelMessage } from '@jupyterlab/services';
 import { IOutput } from '@jupyterlab/nbformat';
 import { NodeBookModel } from "./model";
 import { OutputArea, OutputAreaModel } from "@jupyterlab/outputarea"
-import { CodeCellModel, CellModel } from "@jupyterlab/cells"
+import { CodeCellModel } from "@jupyterlab/cells"
 import {
     RenderMimeRegistry,
     standardRendererFactories
 } from '@jupyterlab/rendermime';
 import {
     NodeMap,
     FlumeConfig,
     generateMenuOption,
     Ower,
     NodeEditor,
     GetSvgContainerRef,
     SvgContainerStyle,
-    ContextMenu
+    ContextMenu,
 } from "../flume";
 import React, { useState } from "react"
+import { Portal } from "react-portal"
 import createConfig, {
     setImageUrls,
     refreshImageUrls,
     get_port_func,
     tuple_value_name,
     get_tuple_max_index,
     parse_dict_name,
     headerFontsize,
     nodeMinWidth,
     nodeMaxWidth,
     common_out,
 } from "./flumeConfig"
 import { v4 as uuidv4 } from "uuid"
-import { buildNodeWidth, cloneDeep, nextFrame, findAll } from './utils'
+import {
+    buildNodeWidth,
+    cloneDeep,
+    nextFrame,
+    findAll,
+    rectsIntersect
+} from './utils'
 import RunIcon from "./runIcon";
 import DeleteIcon from "./deleteIcon";
 import ImageViewer from "./imageViewer";
 import ReRunIcon from "./ReRunIcon";
 import LockIcon from "./lockIcon";
 import ArrownIcon from "./arrownIcon";
 import ClearIcon from "./clearIcon";
 import ExportIcon from "./exportIcon";
 import YesIcon from "./yesIcon";
 import * as monaco from 'monaco-editor';
 
+
 const nodeInitBoxShadow = "0px 4px 8px rgba(0,0,0,0)"
 const nodeSelectedBoxShadow = "0px 0px 10px 10px rgb(0 216 255)"
 const nodeRunningBoxShadow = "rgb(52 255 223) 0px 0px 7px 10px"
 const nodeErrorBoxShadow = "rgb(255 38 227) 0px 0px 10px 10px"
 const kernelStateMap = {
     "idle": "空闲",
     "busy": "繁忙"
 }
+const nodeIdLength = 10
+const commentIdLength = 11
+
 export class NodeEditorWidget extends ReactWidget {
     private _context: DocumentRegistry.IContext<NodeBookModel>; // 上下文
     private _app: JupyterFrontEnd
     private _palette: ICommandPalette
     private _settings: ISettingRegistry
     private _isReady: boolean = false   // 是否一切都准备就绪了
     private _stopCreateNodeType = false // 是否停止向python请求complete
     private _internal_options: any[] = [] // 内部选项，用于右键菜单的选项
-    private _isSaveNodes = true // 是否保存nodes,用于有时候需要阻止修改nodes
+    private _needSaveNodes = false // 是否保存nodes,用于有时候需要阻止修改nodes
     private _curNodesId = ""    // 当前的nodes的ID
     private _loadingNodes = false   // 是否正在加载节点数据
     private _nodeTypes = {} // 缓存的节点类型，用于在保存节点的时候保存到文件中，加载节点时，直接用
     private _redoList: any[] = [] // 保存的操作和它的反向操作，用于撤销和重做
     private _redoListIndex = 0 // 操作的索引，用于指示当前撤销到了哪一步
     private _redoListMaxLength = 200 // 用于限制_redoList要保存多少步的操作
     private _redoing: any = null // 是否正在执行撤销或重做操作
@@ -111,45 +123,50 @@
     private _outputAreaContainerRef
     private _outputAreaAutoScroll = true
     private _runningNodeId: any = null
     private _runningError = false
     private _exportingCodeNodeId = null
     private _exportRet: any[] = []
     private _exportIndent = ""
-    private _showMsgToNotebook = true
     private _setshowCodeEditor
     private _codeEditorValueCache = ""
     private _saveCode: any = null
     private _setUseDiffEditor
     private _curEditingCellIndex = -1
     private _stopFilterCell = false
     private _codeEditor: monaco.editor.IStandaloneCodeEditor | null = null
     private _codeDiffEditor: monaco.editor.IStandaloneDiffEditor | null = null
     private _cellIndexInputRef
     private _renameCache = ""
     private _interruptingKernel = false
     private _curNodesIsDefault = false
+    private _codeEditorNeedSave = true
+    private _commandsMap = {}
+    private _sizeCache = { width: 0, height: 0 }
+    private _kernelStateLabelNodeEditorRef
+    private _kernelStateLabelCodeEditorRef
+    private _nodeIsDefaultLabelRef
+    private _needLoadData: any = null
 
 
     scaleSpeed = 0.01 // 缩放的速度，_scaleDistance * scaleSpeed 就是新的缩放值
     selectedNodes = new Set<string>() // 选择的节点
     keyEventFilter = new Set<string>()// 按键过滤器，用于过滤键盘操作
     editorOptions = {} // 有flume导出的函数变量等。。
     setShowImg: any // 用于设置是否打开图片查看器 setShowImg(true/false)
     setShowImgUrls: any // 用于设置图片查看器的urls数据
     setShowImgStartIndex: any // 用于设置图片查看器当前的图片地址索引，img的src=[urls[index]]
     curNodeName = "" // 当前节点数据的名称
     setCurNodeName: any // 用于设置curNodeName
     editorNodes: NodeMap = {}  // 编辑器内当前的节点数据
-    setEditorNodes: any // 用于同步节点数据到编辑器
     editorConfig: FlumeConfig // flume的配置文件state,
-    setEditorConfig: any // 用于将flume配置修改传递到编辑器
     dispatchNodes: any // 从flume里面导出来的函数，用于在外面修改nodes
     getInitialNodes: any // 从flume里面导出来的函数，用于解析存储的nodes
-
+    editorComments: any
+    dispatchComments: any
     constructor(
         context: DocumentRegistry.IContext<NodeBookModel>,
         app: JupyterFrontEnd,
         palette: ICommandPalette,
         settings: ISettingRegistry,
     ) {
         super();
@@ -174,14 +191,48 @@
         const model = new OutputAreaModel();
         this._outputArea = new OutputArea({
             model,
             rendermime,
         });
         model.changed.connect(() => { this._onOutputModelChanged() })
 
+        // 注册事件
+        this.node.addEventListener("focusin", e => {
+            this._onFocusIn()
+        })
+        this.node.addEventListener("focusout", e => {
+            this._onFocusOut()
+        })
+        this.node.addEventListener("keydown", async e => {
+            await this.onKeyDown(e)
+        })
+        this.node.addEventListener("keyup", async e => {
+            await this.onkeyUp(e)
+        })
+        this.node.addEventListener("mouseenter", e => {
+            this._mouseMove = e
+        })
+        this.node.addEventListener("mousemove", async e => {
+            await this.onMouseMove(e)
+        })
+        this.node.addEventListener("command", async e => {
+            await this._onCommand(e as CustomEvent)
+        })
+        this.node.addEventListener("resize", e => {
+            this._onResize()
+        })
+
+        // 注册size监测
+        this._sizeCache = {
+            width: this.node.clientWidth,
+            height: this.node.clientHeight
+        }
+        setInterval(() => {
+            this.onInterval()
+        }, 100)
 
         // 注册python的语法
         monaco.languages.register({ id: "python" })
         monaco.languages.setMonarchTokensProvider("python", {
             defaultToken: '',
             tokenPostfix: '.python',
             keywords: [
@@ -415,24 +466,14 @@
             // 图片浏览器的数据
             const [showImgUrls, setShowImgUrls] = useState(false)
             this.setShowImgUrls = setShowImgUrls
             // 当前图片的索引
             const [showImgStartIndex, setShowImgStartIndex] = useState(0)
             this.setShowImgStartIndex = setShowImgStartIndex
 
-            // 节点编辑器的节点类型配置
-            const [conf, setConf] = useState(this.editorConfig)
-            this.editorConfig = conf
-            this.setEditorConfig = setConf
-
-            // 当前的节点
-            const [nodes, setNodes] = useState(this.editorNodes)
-            this.editorNodes = nodes
-            this.setEditorNodes = setNodes
-
             // 节点的名称
             const [nodesName, setNodesName] = useState("未命名")
             this.curNodeName = nodesName
             this.setCurNodeName = setNodesName
 
             // 用来保存最外层控件
             const containerRef = React.useRef(null)
@@ -441,15 +482,23 @@
             // 输出引用
             const outputAreaContainerRef = React.useRef(null)
             this._outputAreaContainerRef = outputAreaContainerRef
 
             // 输出控制
             const [showOutput, setShowOutput] = useState(false)
             this._showOutputArea = showOutput
-            this._setShowOutputArea = setShowOutput
+            this._setShowOutputArea = (value) => {
+                if (!value) {
+                    try {
+                        ReactWidget.detach(this._outputArea)
+                    } catch (error) {
+                    }
+                }
+                setShowOutput(value)
+            }
 
             // 编辑器容器
             const editorContainerRef = React.useRef(null)
             this._editorContainerRef = editorContainerRef
 
             // 编辑器控制
             const [showCodeEditor, setshowCodeEditor] = useState(false)
@@ -459,21 +508,18 @@
             this._setUseDiffEditor = setUseDiffEditor
             const [codeEditorMenuOpen, setCodeEditorMenuOpen] = React.useState(false);
             const [menuCoordinates, setMenuCoordinates] = React.useState({ x: 0, y: 0 });
             const [codeEditorMenuOptions, setCodeEditorMenuOptions] = useState([] as any)
             const cellIndexInputRef = React.useRef(null)
             this._cellIndexInputRef = cellIndexInputRef
 
-            // 注册键盘事件
-            const handleKeyDown = async e => { await this.onKeyDown(e) }
-            const handleKeyUp = async e => { await this.onkeyUp(e) }
-            const mouseMove = async e => { await this.onMouseMove(e) }
-            const handleMouseEnter = e => {
-                this._mouseMove = e
-            }
+            // 状态显示
+            this._kernelStateLabelNodeEditorRef = React.useRef(null)
+            this._kernelStateLabelCodeEditorRef = React.useRef(null)
+            this._nodeIsDefaultLabelRef = React.useRef(null)
 
             React.useEffect(() => {
                 if (!showImg) {
                     // 获取真个Draggable组件
                     const draggableRef = this.editorOptions["draggableRef"]
                     if (draggableRef.current) {
                         // 获取焦点，否则不能进行空格位移操作
@@ -485,41 +531,26 @@
                     this._setshowCodeEditor(false)
                     this._setShowOutputArea(false)
                 }
             }, [showImg])
 
             const preScrollTop = React.useRef(0)
             React.useEffect(() => {
-                const element = outputAreaContainerRef.current as unknown as HTMLElement
-                let left = "0px"
-                let width = "100%"
                 if (showOutput) {
+                    const element = outputAreaContainerRef.current as unknown as HTMLElement
                     ReactWidget.attach(
                         this._outputArea,
                         element,
                         null
                     )
-                    this._outputArea.show()
-                    element.scrollTop = element.scrollHeight - element.clientHeight;
-                    const rect = element.getBoundingClientRect()
-                    left = `${rect.width}px`
-                    const container = containerRef.current as unknown as HTMLDivElement
-                    const containerRect = container.getBoundingClientRect()
-                    width = `${(containerRect.width - rect.width) / containerRect.width * 100}%`
-
                     // 保存一些必要数据
+                    element.scrollTop = element.scrollHeight - element.clientHeight;
                     preScrollTop.current = element.scrollTop
                 }
-
-                // 设置编辑器的位置和宽度
-                let editor = editorContainerRef.current as unknown as HTMLElement
-                editor.style.left = left
-                editor.style.width = width
-
-
+                this._onResize()
             }, [showOutput])
 
             const onOutputAreaScroll = (e: React.UIEvent<HTMLDivElement, UIEvent>) => {
                 let element = e.target as HTMLDivElement
 
                 // 计算滚动方向
                 let scrollUp = element.scrollTop - preScrollTop.current < 0
@@ -565,47 +596,39 @@
                             this._codeDiffEditor.focus()
                         } else {
                             this._codeEditor = monaco.editor.create(
                                 codeEditorRef.current as unknown as HTMLElement, {
                                 theme: "vs-dark",
                                 language: "python",
                             })
-
                             this._codeEditor.focus()
-
                             this._codeEditor.onDidChangeModelContent(e => {
                                 this._onCodeEditorChange(this._codeEditor?.getValue(), e)
                             })
 
                             this._codeEditor.onContextMenu(e => {
                                 handleCodeEditorContextMenu(e)
                             })
                         }
                     }
-
                 }
             }, [showCodeEditor])
 
             const handleCodeEditorContextMenu = (e: monaco.editor.IEditorMouseEvent) => {
                 e.event.preventDefault()
                 setMenuCoordinates({ x: e.event.posx, y: e.event.posy });
                 setCodeEditorMenuOpen(true)
-                setTimeout(() => {
-                    let inputElement = document.querySelector('[data-flume-component="ctx-menu-input"]') as HTMLInputElement
-                    inputElement.focus()
-                })
                 return false;
             }
 
 
             const closeContextMenu = () => {
                 setCodeEditorMenuOpen(false);
             };
 
-
             React.useEffect(() => {
                 if (codeEditorMenuOpen) {
                     const length = this._context.model.cells.length
                     const options: any[] = []
                     for (let index = 0; index < length; index++) {
                         options.push({
                             label: `Cell_${index}`,
@@ -624,22 +647,18 @@
             }, [codeEditorMenuOpen])
 
             const iconLength = 24
             const codeEditorIconLength = 50
             return <Ower.Provider value={this}>
                 <div ref={containerRef}
                     className="nd-container"
-                    onKeyDown={handleKeyDown}
-                    onKeyUp={handleKeyUp}
-                    onMouseMove={mouseMove}
-                    onMouseEnter={handleMouseEnter}
                     data-show-image-viewer={showImg}
                     data-show-code-editor={showCodeEditor}
                     data-use-diff-editor={useDiffEditor}
-                    data-inputing="falses"
+                    data-inputing="false"
                 >
                     {/* 输出浏览器 */}
                     {showOutput && <div
                         style={{
                             position: "absolute",
                             left: "0px",
                             top: "0px",
@@ -662,16 +681,15 @@
                                 element.scrollTop = 0;
                             }} width={iconLength} height={iconLength} rotate="90deg" leaveColor="black" />
                             <ArrownIcon onClick={() => {
                                 const element = outputAreaContainerRef.current as unknown as HTMLElement
                                 element.scrollTop = element.scrollHeight - element.clientHeight;
                             }} width={iconLength} height={iconLength} rotate="-90deg" leaveColor="black" />
                             <DeleteIcon onClick={() => {
-                                try { ReactWidget.detach(this._outputArea) } catch { }
-                                setShowOutput(false)
+                                this._setShowOutputArea(false)
                             }} width={iconLength} height={iconLength} leaveColor="black" />
                         </div>
                         <div ref={outputAreaContainerRef}
                             style={{
                                 width: "100%",
                                 height: `calc(100% - ${iconLength}px)`,
                                 overflowY: "scroll",
@@ -686,37 +704,40 @@
                             position: "absolute",
                             left: "0px",
                             top: "0px",
                             width: "100%",
                             height: "100%",
                         }}>
                         {/* 编辑器 */}
-                        <NodeEditor nodeTypes={conf.nodeTypes}
-                            portTypes={conf.portTypes}
-                            circularBehavior="allow"
+                        <NodeEditor nodeTypes={this.editorConfig.nodeTypes}
+                            portTypes={this.editorConfig.portTypes}
+                            circularBehavior="warn"
                             onChange={nodes => this.onNodesChange(nodes)}
                             context={this}
                             renderNodeHeader={(header, currentNodeType, options, id) => {
                                 return this.renderNodeHeader(header, currentNodeType, options, id)
                             }}
+                            onCommentsChange={comments => {
+                                this.onCommentsChange(comments)
+                            }}
                         ></NodeEditor>
                         {/* 上层工具栏 */}
                         <div style={{ position: "absolute", right: "0px", top: "0px" }} >
                             <span style={{
                                 alignItems: "center",
                                 color: "#fff",
                             }}>
                                 <label>名称:({nodesName})</label>
                                 <br />
-                                <label data-name="node-editor-kernel-state-label" style={{
+                                <label ref={this._kernelStateLabelNodeEditorRef} style={{
                                     height: "100%",
                                     backgroundColor: "rgba(0, 0, 0, 0)"
                                 }}>空闲</label>
                                 <br />
-                                <label id="id-default-node-label"></label>
+                                <label ref={this._nodeIsDefaultLabelRef}>默认</label>
                             </span>
                         </div>
                         {/* 图片浏览器 */}
                         {showImg && <div style={{
                             position: "absolute", left: "0px", top: "0px",
                             width: "100%",
                             height: "100%",
@@ -742,25 +763,28 @@
                             <div style={{
                                 width: "100%",
                                 height: "100%",
                             }}
                                 ref={codeEditorRef}
                             ></div>
                             {
-                                codeEditorMenuOpen && <ContextMenu
-                                    x={menuCoordinates.x}
-                                    y={menuCoordinates.y}
-                                    options={codeEditorMenuOptions}
-                                    onRequestClose={closeContextMenu}
-                                    onOptionSelected={(option) => {
-                                        this._onSelectedCodeEditorOption(option)
-                                    }}
-                                    label="搜索cell"
-                                    from="codeEditor"
-                                />
+                                codeEditorMenuOpen &&
+                                <Portal>
+                                    <ContextMenu
+                                        x={menuCoordinates.x}
+                                        y={menuCoordinates.y}
+                                        options={codeEditorMenuOptions}
+                                        onRequestClose={closeContextMenu}
+                                        onOptionSelected={(option) => {
+                                            this._onSelectedCodeEditorOption(option)
+                                        }}
+                                        label="搜索cell"
+                                        from="codeEditor"
+                                    />
+                                </Portal>
                             }
                             <div style={{
                                 position: "absolute", right: "0px", top: "0px",
                                 zIndex: 100,
                                 display: "flex",
                                 alignItems: "center",
                             }}>
@@ -776,48 +800,56 @@
                                     />
                                 }
                                 <RunIcon onClick={() => {
                                     this._editorRun()
                                 }} width={codeEditorIconLength} height={codeEditorIconLength} />
                                 <DeleteIcon onClick={() => {
                                     setshowCodeEditor(false)
+                                    setUseDiffEditor(false)
                                     this._saveCode = null
                                     this._curEditingCellIndex = -1
                                 }} width={codeEditorIconLength} height={codeEditorIconLength}
                                 />
                             </div>
                             <div style={{
                                 position: "absolute", left: "0px", bottom: "0px",
                                 zIndex: 100,
                             }}>
-                                <label data-name="node-editor-kernel-state-label" style={{
-                                    height: "100%",
-                                    color: "white",
-                                }}>空闲</label>
+                                <label
+                                    ref={this._kernelStateLabelCodeEditorRef}
+                                    style={{
+                                        height: "100%",
+                                        color: "white",
+                                    }}>空闲</label>
                                 <br />
                                 {!useDiffEditor && <span>
                                     <label style={{
                                         height: "100%",
                                         color: "white",
                                     }}>当前索引:</label>
                                     <input
                                         ref={cellIndexInputRef}
                                         type="number"
                                         onChange={e => {
                                             let value = Number(e.target.value)
-                                            if (value < 0) {
-                                                e.target.value = "0"
-                                                value = 0
+                                            let index = undefined
+                                            if (value < this._curEditingCellIndex) {
+                                                index = this._getCodeCell(this._curEditingCellIndex - 1, 0, -1)
+                                            } else if (value > this._curEditingCellIndex) {
+                                                index = this._getCodeCell(
+                                                    this._curEditingCellIndex + 1,
+                                                    this._context.model.cells.length,
+                                                    1
+                                                )
                                             }
-                                            const maxValue = this._context.model.cells.length - 1
-                                            if (value > maxValue) {
-                                                value = maxValue
-                                                e.target.value = `${maxValue}`
+                                            if (index != undefined) {
+                                                this._editCell(value)
+                                            } else {
+                                                e.target.value = `${this._curEditingCellIndex}`
                                             }
-                                            this._editCell(value)
                                         }}
                                     /></span>
                                 }
                             </div>
                         </div>}
                     </div>
                 </div>
@@ -830,14 +862,26 @@
 
         // 刷新选择表现
         this.refreshNodeBoxShadow()
 
         return this._renderCache
     }
 
+
+    onInterval() {
+        if (this.node.clientWidth != this._sizeCache.width
+            || this.node.clientHeight != this._sizeCache.height) {
+            this._onResize()
+            this._sizeCache = {
+                width: this.node.clientWidth,
+                height: this.node.clientHeight
+            }
+        }
+    }
+
     async onKeyDown(e: KeyboardEvent) {
         if (this.keyEventFilter.has(e.key)) {
             return
         }
         // console.log(e)
         switch (e.key) {
             case " ": {
@@ -888,27 +932,31 @@
         }
 
         // this._initPython() 必须在 this._loadNodesFromAllCell()之前
         if (!await this._initPython()) {
             return false
         }
 
+        // 加载所有的保存的类型
+        let options = this._loadNodesAsList()
+        for (const option of options) {
+            this._buildNodeTypesFromSaved(option.data)
+        }
+
         // 加载第一个节点
-        let nodes = this._loadNodesFromAllCell()
-        if (nodes.length > 0) {
-            if (!await this._loadNodes(nodes[0].data)) {
-                showDialog({
-                    title: "加载节点失败",
-                    body: "加载节点失败，请重新加载节点",
-                    buttons: [Dialog.okButton({ label: 'Ok' })]
-                });
-                return false
-            }
+        if (!await this._tryLoadNodes()) {
+            showDialog({
+                title: "加载节点失败",
+                body: "加载节点失败，请重新加载节点",
+                buttons: [Dialog.okButton({ label: 'Ok' })]
+            });
+            return false
         }
 
+
         this._isReady = true
         return true
     }
 
 
     async runAllCells() {
         for (let index = 0; index < this._context.model.cells.length; index++) {
@@ -916,24 +964,37 @@
             if (cell.type == "code") {
                 await this._runCell(cell as CodeCellModel, nullTranslator)
             }
         }
         this._context.save()
     }
 
-    async createNewNodes() {
-        this._isSaveNodes = false
-        this._curNodesId = ""
+    async createNewNodes(addRedo = true) {
+        this._curNodesId = uuidv4()
+        if (addRedo) {
+            this._addRedo({
+                action: {
+                    type: "CREATE_NODES",
+                    from: "nodes"
+                },
+                redoAction: {
+                    type: "DELETE_NODES",
+                    id: this._curNodesId,
+                    from: "nodes"
+                },
+            })
+        }
+        this._needSaveNodes = false
         this.setCurNodeName("未命名")
         this._clearNodes()
-        this._isSaveNodes = true
+        this._needSaveNodes = true
     }
 
     async onConnectToSpace(e, nodeId, portName) {
-        // let node = this.editorNodes[nodeId]
+        // let node = this._getNode(nodeId)
         // if (!node) {
         //     return
         // }
 
         // let outVarName = this._get_out_var_name(nodeId)
         // switch (node.type) {
         //     case "image":
@@ -950,17 +1011,15 @@
         // }
 
         // this._setMenuOpen(`${outVarName}`)
     }
 
     async runNode(id, clearCache = false) {
         this._interruptingKernel = false
-        this._showMsgToNotebook = true
         this._stopCreateNodeType = true
-        this._clearCurOutput()
         let removeList = [id]
         let exceptIds: any = []
         if (clearCache) {
             for (const nodeId in this._runCache) {
                 if (this._lockedNodes.has(nodeId)) {
                     exceptIds = [
                         ...await this._getNodeInputLinkedNodes(nodeId),
@@ -974,87 +1033,109 @@
         exceptIds = new Set(exceptIds)
         for (const nodeId of removeList) {
             if (exceptIds.has(nodeId) && nodeId != id) {
                 continue
             }
             delete this._runCache[nodeId]
         }
-
         this._setRunningNode(id)
         this.refreshNodeBoxShadow()
         this._runCache[id] = await this._runNode(id)
         this._saveNodes(this.editorNodes)
         this._setRunningNode(0)
         this.refreshNodeBoxShadow()
     }
 
-    async deleteNodes() {
-        let ret = await showDialog({
-            title: "确定要删除吗？",
-            body: "确定要删除吗？删除就没了哦",
-            buttons: [Dialog.cancelButton({ label: "取消" }),
-            Dialog.okButton({ label: '确定' })]
-        });
+    async deleteNodes(targetId = null, needAuthorization = true, addRedo = true) {
+        if (needAuthorization) {
+            let ret = await showDialog({
+                title: "确定要删除吗？",
+                body: "确定要删除吗？删除就没了哦",
+                buttons: [Dialog.cancelButton({ label: "取消" }),
+                Dialog.okButton({ label: '确定' })]
+            });
 
-        if (ret.button.label != "确定") {
-            return
+            if (ret.button.label != "确定") {
+                return
+            }
         }
 
+        let allNodes = this.getAllNodes()
+
         this._clearNodes()
         setTimeout(() => {
-            let index = this._getNodesCellIndex(this._curNodesId)
-            if (index == null) {
-                return
-            }
-            console.log("_deleteNodes", this._curNodesId)
-            this._context.model.sharedModel.deleteCell(index)
-            let nodes = this._loadNodesFromAllCell()
-            if (nodes.length > 0) {
-                this._loadNodes(nodes[0].data)
+            let id = targetId || this._curNodesId
+            if (addRedo) {
+                this._addRedo({
+                    action: {
+                        type: "DELETE_NODES",
+                        id,
+                        from: "nodes"
+                    },
+                    redoAction: {
+                        type: "RESTORE_NODES",
+                        data: allNodes[id],
+                        from: "nodes"
+                    },
+                })
             }
-        }, 50);
+
+            delete allNodes[id]
+            this.setAllNodes(allNodes)
+            this._tryLoadNodes()
+        });
     }
 
     async save() {
         await this._context.save()
     }
 
     async redo(direct) {
         // 检测是否有历史
         if (this._redoList.length == 0) {
             return
         }
 
         // 获取目标index
         let target_index = this._redoListIndex + direct
+        if (direct > 0) {
+            target_index = this._redoListIndex
+        }
+
         if (target_index < 0 || target_index >= this._redoList.length) {
             return
         }
-        this._redoListIndex = target_index
-        let action = this._redoList[this._redoListIndex]
-        if (direct > 0) {
-            action = action.action
-        } else {
-            action = action.redoAction
+
+        this._redoListIndex = this._redoListIndex + direct
+
+        let action = this._redoList[target_index]
+        this._redoing = direct > 0 ? action.action : action.redoAction
+
+
+        console.log("redo", this._redoing, this._redoListIndex)
+        switch (this._redoing.from) {
+            case "comment": {
+                this.dispatchComments(this._redoing)
+            } break;
+            case "node": {
+                this.dispatchNodes(this._redoing)
+            } break
+            case "nodes": {
+                await this._dispatchNodesAction(this._redoing)
+            } break
         }
-        this._redoing = action
-        console.log("redo", action, this._redoListIndex)
-        this.dispatchNodes(action)
     }
 
 
-
     refreshNodeBoxShadow() {
         // 刷新选择表现
-        let element: HTMLElement | null
         for (const id in this.editorNodes) {
-            element = document.getElementById(id)
-            if (!element) {
-                continue
-            }
+            this._setNodeBoxShadow(id, nodeInitBoxShadow)
+        }
+        for (const id in this.editorComments) {
             this._setNodeBoxShadow(id, nodeInitBoxShadow)
         }
         this._refreshSelectedNodes()
         this._refreshRunningNode()
     }
 
     async onNodeStartDrag(id, nodeElement: HTMLElement) {
@@ -1124,14 +1205,22 @@
     async onStageStartDrag(e: MouseEvent) {
         this._stageDragging = true
     }
 
     onSaveState() {
     }
 
+    onCommentsChange(comments) {
+        this.editorComments = comments
+        if (this._redoing) {
+            this._redoing = null
+        }
+        this.onNodesChange(this.editorNodes)
+    }
+
     onNodesChange(nodes: NodeMap) {
         console.log("onNodesChange", nodes)
         if (!this._checkReady(false)) {
             return
         }
         refreshImageUrls(this)
         this._saveNodes(nodes)
@@ -1144,40 +1233,138 @@
                     this._setNodePortControlInputValue(
                         this._redoing.nodeId,
                         this._redoing.portName,
                         this._redoing.controlName,
                         this._redoing.data
                     )
                 } break
+                case "ADD_CONNECTION":
+                case "REMOVE_CONNECTION": {
+                    this._triggerRecalculation()
+                } break
             }
             this._redoing = null
         }
 
         // 执行一些后处理
         setTimeout(() => {
             this._updateHeaderCache()
         });
     }
 
+    onCommentsAction(comments, action, nanoid) {
+        console.log(comments, action)
+        if (this._redoing != null) {
+            this._needSaveNodes = true
+            return
+        }
+
+        if (this._preAction == action) {
+            return
+        }
+
+        this._preAction = action
+        let redoAction
+        action.from = "comment"
+        switch (action.type) {
+            case "CLEAR":
+            case "RE_INIT":
+                return
+            case "ADD_COMMENT": {
+                action.id = action.id || nanoid(commentIdLength)
+                redoAction = {
+                    type: "DELETE_COMMENT",
+                    id: action.id,
+                }
+            } break
+            case "ADD_COMMENTS": {
+                redoAction = {
+                    type: "DELETE_COMMENTS",
+                    ids: Object.keys(action.comments)
+                }
+            } break
+            case "REMOVE_COMMENT_NEW": {
+
+            } break
+            case "SET_COMMENT_COORDINATES": {
+                const comment = comments[action.id]
+                redoAction = {
+                    type: "SET_COMMENT_COORDINATES",
+                    ...comment,
+                }
+            } break
+            case "SET_COMMENT_DIMENSIONS": {
+                const comment = comments[action.id]
+                redoAction = {
+                    type: "SET_COMMENT_DIMENSIONS",
+                    ...comment,
+                }
+            } break
+            case "SET_COMMENT_TEXT": {
+                const comment = comments[action.id]
+                redoAction = {
+                    type: "SET_COMMENT_TEXT",
+                    ...comment,
+                }
+            } break
+            case "SET_COMMENT_COLOR": {
+                const comment = comments[action.id]
+                redoAction = {
+                    type: "SET_COMMENT_COLOR",
+                    ...comment,
+                }
+            } break
+            case "DELETE_COMMENT": {
+                const comment = comments[action.id]
+                redoAction = {
+                    type: "ADD_COMMENT",
+                    comment,
+                }
+            } break
+            case "DELETE_COMMENTS": {
+                const add_comments = {}
+                for (const id of action.ids) {
+                    add_comments[id] = this._getNode(id)
+                }
+                redoAction = {
+                    type: "ADD_COMMENTS",
+                    comments: add_comments,
+                }
+            } break
+            default: {
+            } break
+        }
+        if (redoAction) {
+            redoAction.from = "comment"
+            this._addRedo({
+                action,
+                redoAction
+            })
+            this._needSaveNodes = true
+        }
+    }
+
     onNodeAction(nodes, action, nanoid) {
         if (this._redoing != null) {
+            this._needSaveNodes = true
             return
         }
 
         if (this._preAction == action) {
             return
         }
         this._preAction = action
 
         let redoAction
+        action.from = "node"
         switch (action.type) {
             case "CLEAR":
             case "RE_INIT":
-                this._redoList = []
-                this._redoListIndex = 0
+                // this._redoList = []
+                // this._redoListIndex = 0
                 let draggableRef = this.editorOptions["draggableRef"]
                 if (document.activeElement != draggableRef.current)
                     draggableRef.current.focus()
                 return
             case "SET_NODE_COORDINATES": {
                 const node = nodes[action.nodeId]
                 if (!node) return
@@ -1218,18 +1405,22 @@
                 redoAction = {
                     type: "ADD_NODES",
                     nodes: removed_nodes
                 }
 
             } break
             case "ADD_NODE": {
-                action.id = action.id || nanoid(10)
+                action.id = action.id || nanoid(nodeIdLength)
+                let nodeId = action.id
+                if (action.node) {
+                    nodeId = action.node.id
+                }
                 redoAction = {
                     type: "REMOVE_NODE",
-                    nodeId: action.id
+                    nodeId
                 }
             } break
             case "ADD_NODES": {
                 const nodeIds: any[] = []
                 for (const node of action.nodes) {
                     nodeIds.push(node.id)
                 }
@@ -1246,19 +1437,26 @@
             } break
             case "REMOVE_CONNECTION": {
                 redoAction = {
                     ...action,
                     type: "ADD_CONNECTION",
                 }
             } break
+            default: {
+
+            } break
+        }
+        if (redoAction) {
+            redoAction.from = "node"
+            this._addRedo({
+                action,
+                redoAction
+            })
+            this._needSaveNodes = true
         }
-        this._addRedo({
-            action,
-            redoAction
-        })
     }
 
     onNodeLockChange(nodeId, isLock) {
         if (isLock) {
             this._lockedNodes.add(nodeId)
         } else {
             this._lockedNodes.delete(nodeId)
@@ -1277,20 +1475,23 @@
         closeMenu: closeContextMenu,
         deleteNode
     }, id) {
         const Ret = () => {
             const [fontSize, setFontSize] = useState(headerFontsize);
             const instanceBackgroundColor = "#d9822b"
             const functionBackgroundColor = "#5F41FF"
+            const combineBackgroundColor = "rgb(0 81 255 / 80%)"
             const defaultBackGroundColor = "rgba(248, 28, 149, 0.8)"
             let backgroundColor
             if (/instance@/g.exec(currentNodeType.type)) {
                 backgroundColor = instanceBackgroundColor
             } else if (/function@/g.exec(currentNodeType.type)) {
                 backgroundColor = functionBackgroundColor
+            } else if (/combine@/g.exec(currentNodeType.type)) {
+                backgroundColor = combineBackgroundColor
             } else {
                 backgroundColor = defaultBackGroundColor
             }
             let HeaderDeleteIcon = () => {
                 return <DeleteIcon
                     onClick={e => {
                         e.preventDefault()
@@ -1346,41 +1547,31 @@
             let HeaderExportIcon = () => {
                 if (backgroundColor == instanceBackgroundColor)
                     return null
                 return <ExportIcon
                     width={fontSize}
                     height={fontSize}
                     onClick={async e => {
-                        let preCheckCache = this._runCheckCache
-                        try {
-                            this._exportRet = []
-                            this._exportingCodeNodeId = id
-                            this._runCheckCache = false
-                            this._exportIndent = ""
-                            await this.runNode(id)
-                            this._codeEditorValueCache = this._getExportedCodeText()
-                            this._outputText(this._codeEditorValueCache)
-                            let nodeId = this._exportingCodeNodeId
-                            this._saveCode = () => {
-                                this._writeToExportCell(nodeId)
-                            }
-                            let preValue = this._readExportedData(nodeId) || ""
-                            this._setUseDiffEditor(true)
-                            this._setshowCodeEditor(true)
-                            setTimeout(() => {
-                                let firstLineEndIndex = preValue.indexOf("\n")
-                                if (firstLineEndIndex >= 0) {
-                                    preValue = preValue.slice(firstLineEndIndex + 1, preValue.length)
-                                }
-                                this._setDiffCodeEditorValue(preValue, this._codeEditorValueCache)
-                            }, 0);
-                        } finally {
-                            this._exportingCodeNodeId = null
-                            this._runCheckCache = preCheckCache
+                        if (!await this._buildNodeCode(id)) {
+                            return
+                        }
+                        this._outputText(this._codeEditorValueCache)
+                        this._saveCode = () => {
+                            this._writeToExportCell(id)
                         }
+                        let preValue = this._readExportedData(id) || ""
+                        this._setUseDiffEditor(true)
+                        this._setshowCodeEditor(true)
+                        setTimeout(() => {
+                            let firstLineEndIndex = preValue.indexOf("\n")
+                            if (firstLineEndIndex >= 0) {
+                                preValue = preValue.slice(firstLineEndIndex + 1, preValue.length)
+                            }
+                            this._setDiffCodeEditorValue(preValue, this._codeEditorValueCache)
+                        }, 0);
                     }}
                 />
             }
 
             return <div style={{
                 backgroundColor,
                 display: "flex",
@@ -1456,14 +1647,32 @@
         }
     }
 
     cellGet(index) {
         return this._context.model.cells.get(index)
     }
 
+    getAllNodes() {
+        return this._context.model.getMetadata("nodes") || {}
+    }
+
+    setAllNodes(data) {
+        this._context.model.setMetadata("nodes", data)
+    }
+
+    getNodes(id) {
+        return this.getAllNodes()[id]
+    }
+
+    setNodes(id, data) {
+        let allNodes = this.getAllNodes()
+        allNodes[id] = data
+        this.setAllNodes(allNodes)
+    }
+
     async onContextMenuFilter(
         filter: string,
         options: any[] = [],
         setOptions,
         filterOptions,
         from
     ) {
@@ -1560,16 +1769,18 @@
         switch (match.type) {
             case "instance": {
                 let target_type = ""
                 let target_value = "None"
                 try {
                     // 1.获取instance的数据类型和值
                     await this._getInstanceInfo(node_type_name, (msg) => {
-                        if (KernelMessage.isStreamMsg(msg)) {
-                            let info = JSON.parse(msg.content.text as string)
+                        if (KernelMessage.isExecuteResultMsg(msg)) {
+                            let data = msg.content.data as any
+                            data = eval(data["text/plain"].trim())
+                            let info = JSON.parse(data as string)
                             let getTypeRet = /<class '(.*)'>/g.exec(info.type)
                             if (getTypeRet) {
                                 target_type = getTypeRet[1]
                                 if (info.value === null) {
                                     info.value = "None"
                                 }
                                 target_value = info.value
@@ -1593,15 +1804,15 @@
                     }
                 } catch (error) { }
             } break;
             case "function": {
                 // 1.解析signature (a:int, b, c:str= "123", *args, **kwargs)
                 let in_ports: any[] = this._buildInputPortsFromSignature(match.signature)
                 // 2.构建nodeType
-                node_types = this._buildFunctionNodeTypes(node_type_name, in_ports)
+                node_types = this._buildCommonNodeTypes(node_type_name, in_ports)
                 // 3.记录下来
                 this._nodeTypes[node_type_name] = {
                     type: "function",
                     node_type_name,
                     in_ports,
                 }
             } break;
@@ -1680,16 +1891,16 @@
                 })
             }
         }
 
         return in_ports
     }
 
-    private _buildFunctionNodeTypes(node_type_name, in_ports) {
-        let type_name = "function@" + node_type_name
+    private _buildCommonNodeTypes(node_type_name, in_ports, prefix = "function") {
+        let type_name = prefix + "@" + node_type_name
         let node_types: any[] = []
         let nodetype = {
             type: type_name,
             label: node_type_name,
             description: node_type_name,
             initialWidth: buildNodeWidth(node_type_name, headerFontsize, nodeMinWidth, nodeMaxWidth),
             inputs: ports => (inputData, connections, executionContext: NodeEditorWidget, nodeId) => {
@@ -1699,15 +1910,15 @@
                 for (const in_port of in_ports) {
                     if (in_port.arg_name == "/") {
                         continue
                     }
                     let f = get_port_func(in_port.arg_type)
                     let port = f(
                         ports,
-                        in_port.arg_name,
+                        in_port.arg_label || in_port.arg_name,
                         in_port.arg_name,
                         in_port.arg_default
                     )
                     ret.push(port)
                 }
                 return ret
             },
@@ -1718,57 +1929,96 @@
     }
 
     private _buildInstanceNodeTypes(node_type_name, target_type, target_value): any[] {
         let node_types: any[] = []
         if (target_type == "") {
             return node_types
         }
-        let port_func: any = null
-        let type_name = "instance@set@" + node_type_name
-        let label = node_type_name + "@set"
-        port_func = get_port_func(target_type)
-        let nodetype = {
-            type: type_name,
-            label,
-            description: node_type_name + "@" + target_type,
-            initialWidth: buildNodeWidth(label, headerFontsize, nodeMinWidth, nodeMaxWidth),
-            inputs: ports => (inputData, connections, executionContext: NodeEditorWidget, nodeId) => {
-                let port = port_func(ports, node_type_name, node_type_name, target_value)
-                return [get_port_func("control")(ports), port]
-            },
-            outputs: ports => (inputData, connections, executionContext: NodeEditorWidget, nodeId) => {
-                let port = port_func(ports, node_type_name, node_type_name, target_value)
-                return [get_port_func("control")(ports), port]
-            }
-        }
-        node_types.push(nodetype)
-        type_name = "instance@get@" + node_type_name
-        label = node_type_name + "@get"
-        nodetype = {
-            type: "instance@get@" + node_type_name,
-            label,
-            description: node_type_name + "@" + target_type,
-            initialWidth: buildNodeWidth(label, headerFontsize, nodeMinWidth, nodeMaxWidth),
-            inputs: ports => (inputData, connections, executionContext: NodeEditorWidget, nodeId) => {
-                return []
-            },
-            outputs: ports => (inputData, connections, executionContext: NodeEditorWidget, nodeId) => {
-                let port = port_func(ports, node_type_name, node_type_name, target_value)
-                return [port]
-            }
+        let extra_label = ""
+        let type_prefix: String = ""
+        switch (target_type) {
+            case "jupyterlab_nodeeditor.select.mselect":
+                extra_label = "[Select an option]"
+                type_prefix = "instance_mselect"
+            case "jupyterlab_nodeeditor.select.select": {
+                let nodetype
+                if (type_prefix.length == 0) {
+                    type_prefix = "instance_select"
+                }
+                let type_name = type_prefix + "@get@" + node_type_name
+                let label = node_type_name + "@get"
+                let port_func = get_port_func(target_type)
+                let width = 0
+                for (const option of target_value) {
+                    width = Math.max(width, buildNodeWidth(label + option.label + extra_label, headerFontsize, nodeMinWidth, nodeMaxWidth))
+                }
+                nodetype = {
+                    type: type_name,
+                    label,
+                    description: node_type_name + "@" + target_type,
+                    initialWidth: width,
+                    inputs: ports => (inputData, connections, executionContext: NodeEditorWidget, nodeId) => {
+                        let port = port_func(ports, node_type_name, node_type_name, target_value)
+                        port.hidePort = true
+                        return [port]
+                    },
+                    outputs: common_out
+                }
+                node_types.push(nodetype)
+            } break
+            default: {
+                let nodetype
+                let type_name = "instance@set@" + node_type_name
+                let label = node_type_name + "@set"
+                let port_func: any = get_port_func(target_type)
+                nodetype = {
+                    type: type_name,
+                    label,
+                    description: node_type_name + "@" + target_type,
+                    initialWidth: buildNodeWidth(label, headerFontsize, nodeMinWidth, nodeMaxWidth),
+                    inputs: ports => (inputData, connections, executionContext: NodeEditorWidget, nodeId) => {
+                        let port = port_func(ports, node_type_name, node_type_name, target_value)
+                        return [get_port_func("control")(ports), port]
+                    },
+                    outputs: common_out
+                }
+                node_types.push(nodetype)
+                type_name = "instance@get@" + node_type_name
+                label = node_type_name + "@get"
+                nodetype = {
+                    type: type_name,
+                    label,
+                    description: node_type_name + "@" + target_type,
+                    initialWidth: buildNodeWidth(label, headerFontsize, nodeMinWidth, nodeMaxWidth),
+                    inputs: ports => (inputData, connections, executionContext: NodeEditorWidget, nodeId) => {
+                        return []
+                    },
+                    outputs: ports => (inputData, connections, executionContext: NodeEditorWidget, nodeId) => {
+                        let port = port_func(ports, "输出", "out", target_value)
+                        return [port]
+                    }
+                }
+                node_types.push(nodetype)
+            } break
         }
-        node_types.push(nodetype)
+
         return node_types
     }
 
     private async _getInputValue(input, node) {
         // 分两种情况
         let connection = node.connections.inputs[input.name]
         // 1.没有对应的连接，需要解析control的值
         if (!connection) {
+            if (node.inputValues) {
+                let ret = node.inputValues[input.name]
+                if (ret) {
+                    return ret
+                }
+            }
             return await this._getPortValue(
                 input.type, node.inputData[input.name] || {}, input.name)
         }
         // 2.有连接，需要递归解析连接的节点
         else {
             // 1.获取该连接的信息
             let { nodeId, portName } = connection[0]
@@ -1784,15 +2034,15 @@
             // 3.根据返回的值，提取结果
             this._runCache[nodeId] = target_node_ret
             return target_node_ret[portName]
         }
     }
 
     private async _getPythonValueIsTrue(value) {
-        await this._runCode(`______jupyterlab_get_boolean_value__(${value})`, (msg) => {
+        await this._runCode(`jupyterlab_nodeeditor.get_boolean_value(${value})`, (msg) => {
             if (KernelMessage.isExecuteResultMsg(msg)) {
                 let data = msg.content.data as any
                 data = data["text/plain"].trim()
                 value = data == "True"
             }
         })
         return value
@@ -1802,14 +2052,18 @@
         let inputs = this.editorConfig.nodeTypes[node.type].inputs;
         if (typeof inputs === 'function') {
             inputs = inputs(node.inputData, node.connections, this, node.id);
         }
         return inputs
     }
 
+    private async _getNodeOutputs(node) {
+
+    }
+
     private async _getNodeInputValue(node, inputs, input_name) {
         for (const input of inputs) {
             if (input.name == input_name)
                 return await this._getInputValue(input, node)
         }
     }
 
@@ -1819,15 +2073,15 @@
             this.refreshNodeBoxShadow()
             const errorMsg = "内核中断"
             this._outputText(errorMsg)
             throw errorMsg
         }
 
         // 1.获取该节点
-        let node = this.editorNodes[id]
+        let node = this._getNode(id)
         if (!node) {
             console.error("节点不存在")
             return
         }
 
         if (this._runCheckCache) {
             let ret = this._runCache[id]
@@ -1841,15 +2095,15 @@
 
         // 3.判断是否是分支节点
         let inputValues = {}
         if (node.type == "if") {
             // 1.解析value的真值
             let condition_ret = await this._getNodeInputValue(node, inputs, "value")
             if (this._exportingCodeNodeId) {
-                let out_var_name = this._get_out_var_name(id)
+                let out_var_name = this._getOutVarName(id)
                 this._exportCode(`if ${condition_ret}:`)
                 this._exportAddIndent()
                 let ret = await this._getNodeInputValue(node, inputs, "true")
                 this._exportCode(`${out_var_name}=${ret}`)
                 this._exportRemoveIndent()
                 this._exportCode(`else:`)
                 this._exportAddIndent()
@@ -1939,15 +2193,15 @@
                                     this._exportCode(code)
                                 } else {
                                     await this._runCode(code)
                                 }
                             }
                         // 2.如果是get，直接返回该变量的名称
                         case "get":
-                            return { [match_ret[2]]: match_ret[2] }
+                            return { out: match_ret[2] }
                     }
                     return inputValues
                 // 2.节点是函数
                 case "function":
                     let no_keyword_arguments = false
                     let type_cache = this._nodeTypes[match_ret[2]]
                     if (type_cache) {
@@ -1978,55 +2232,100 @@
                                 args_string += `, ${inputValues[name]}`
                             }
                         }
                     }
                     // 2.去除开头的,
                     args_string = args_string.slice(1, args_string.length)
                     // 3.构建代码
-                    let out_var_name = this._get_out_var_name(id)
+                    let out_var_name = this._getOutVarName(id)
                     let code = `${out_var_name} = ${match_ret[2]}(${args_string})`
                     // 4.运行代码
                     if (this._exportingCodeNodeId) {
                         this._exportCode(code)
                     } else {
                         await this._runCode(code)
                     }
                     return {
                         out: out_var_name
                     }
+                // 3.是select
+                case "instance_select": {
+                    let out_var_name = this._getOutVarName(id)
+                    // 1.根据输入的值，执行代码
+                    for (const varName in inputValues) {
+                        let code = `${out_var_name} = ${varName}.get_option_value(${inputValues[varName]})`
+                        if (this._exportingCodeNodeId) {
+                            this._exportCode(code)
+                        } else {
+                            await this._runCode(code)
+                        }
+                    }
+                    return { out: out_var_name }
+                }
+                case "instance_mselect": {
+                    let out_var_name = this._getOutVarName(id)
+                    // 1.根据输入的值，执行代码
+                    for (const varName in inputValues) {
+                        let code = `${out_var_name} = ${varName}.get_option_value([${inputValues[varName]}])`
+                        if (this._exportingCodeNodeId) {
+                            this._exportCode(code)
+                        } else {
+                            await this._runCode(code)
+                        }
+                    }
+                    return { out: out_var_name }
+                }
+                case "combine": {
+                    let out_var_name = this._getOutVarName(id)
+                    let savedNodeType = this._nodeTypes[match_ret[2]]
+                    if (!savedNodeType) {
+                        throw new Error(`${node.type}不存在`);
+                    }
+                    let code = savedNodeType.code as string
+                    for (const portName in inputValues) {
+                        code = code.replace(portName, inputValues[portName])
+                    }
+                    if (this._exportingCodeNodeId) {
+                        let codelines = code.split("\n")
+                        for (const line of codelines) {
+                            this._exportCode(line)
+                        }
+                    } else {
+                        await this._runCode(code)
+                    }
+                    return { out: out_var_name }
+                }
                 default: break
             }
         } else {
             switch (node.type) {
                 case "video":
                 case "image": {
-                    let out_var_name = this._get_out_var_name(id)
-
+                    let out_var_name = this._getOutVarName(id)
                     if (this._exportingCodeNodeId) {
                         this._exportRet.push(`${out_var_name}=${inputValues["urls"]}`)
                     } else {
                         let code = `
-                        ${out_var_name}=${inputValues["urls"]}
-                        ______jupyterlab_node_editor_get_urls_(${out_var_name})
-                        `
+${out_var_name}=${inputValues["urls"]}
+jupyterlab_nodeeditor.get_urls(${out_var_name})
+                    `
                         await this._runCode(code, (msg) => {
                             if (KernelMessage.isExecuteResultMsg(msg)) {
                                 let data = msg.content.data as any
                                 data = eval(data["text/plain"])
                                 let urls = JSON.parse(data)
                                 setImageUrls(id, urls)
                             }
                         })
                     }
 
-                    let ret = { urls: out_var_name }
-                    return ret
+                    return { out: out_var_name }
                 }
                 case "tuple": {
-                    let out_var_name = this._get_out_var_name(id)
+                    let out_var_name = this._getOutVarName(id)
                     let code = ""
                     let maxV = get_tuple_max_index(inputValues)
                     for (let index = 0; index <= maxV; index++) {
                         code += `${inputValues[tuple_value_name(index)]},`
                     }
                     code = `${out_var_name} = (${code})`
 
@@ -2037,15 +2336,15 @@
                     }
 
                     return {
                         out: out_var_name
                     }
                 }
                 case "dict": {
-                    let out_var_name = this._get_out_var_name(id)
+                    let out_var_name = this._getOutVarName(id)
                     let code = ""
                     for (const key in inputValues) {
                         let ret = parse_dict_name(key)
                         if (ret) {
                             code += `'${ret[1]}':${inputValues[key]},`
                         }
                     }
@@ -2060,64 +2359,64 @@
                     return {
                         out: out_var_name
                     }
                 }
                 case "bool":
                 case "string":
                 case "any": {
-                    let out_var_name = this._get_out_var_name(id)
+                    let out_var_name = this._getOutVarName(id)
                     let code = `${out_var_name} = ${inputValues["value"]}`
                     if (this._exportingCodeNodeId) {
                         this._exportCode(code)
                     } else {
                         await this._runCode(code)
                     }
                     return {
                         out: out_var_name
                     }
                 }
                 case "int": {
-                    let out_var_name = this._get_out_var_name(id)
+                    let out_var_name = this._getOutVarName(id)
                     let code = `${out_var_name} = int(${inputValues["value"]})`
                     if (this._exportingCodeNodeId) {
                         this._exportCode(code)
                     } else {
                         await this._runCode(code)
                     }
                     return {
                         out: out_var_name
                     }
                 }
                 case "float": {
-                    let out_var_name = this._get_out_var_name(id)
+                    let out_var_name = this._getOutVarName(id)
                     let code = `${out_var_name} = float(${inputValues["value"]})`
                     if (this._exportingCodeNodeId) {
                         this._exportCode(code)
                     } else {
                         await this._runCode(code)
                     }
                     return {
                         out: out_var_name
                     }
                 }
                 case "if": {
-                    let out_var_name = this._get_out_var_name(id)
+                    let out_var_name = this._getOutVarName(id)
                     let code = `${out_var_name} = ${inputValues["out"]}`
                     await this._runCode(code)
                     return {
                         out: out_var_name
                     }
                 }
                 case "loop": {
                     return {
                         out: "None"
                     }
                 }
                 case "operator": {
-                    let out_var_name = this._get_out_var_name(id)
+                    let out_var_name = this._getOutVarName(id)
                     let yiyuan_operator = ["not", "~"]
                     let operator = inputValues["operator"]["operator"]
                     let code
                     if (!yiyuan_operator.includes(operator)) {
                         code = `${out_var_name} = ${inputValues["value1"]} ${operator} ${inputValues["value2"]}`
                     } else {
                         code = `${out_var_name} = ${operator} ${inputValues["value1"]}`
@@ -2245,119 +2544,121 @@
             }
         }
         catch (e) {
             throw e;
         }
     }
 
-    private _loadNodesFromAllCell() {
+    private _loadNodesAsList() {
         let ret: any[] = []
-        for (let index = 0; index < this._context.model.cells.length; index++) {
-            const cell = this.cellGet(index);
-            if (cell.type == "code") {
-                let data: any = this._get_node_data(cell as CodeCellModel)
-                if (!data) {
-                    continue
-                }
-                ret.push(data)
-            }
-        }
-
-        if (ret.length > 0) {
-            ret[0].data.default = true
+        let records = this.getAllNodes()
+        for (const nodesId in records) {
+            let record = records[nodesId]
+            ret.push({
+                id: record.id,
+                name: record.name,
+                data: record
+            })
         }
-
         return ret
     }
 
-    private async _saveNodes(nodes: NodeMap) {
-        if (!this._isSaveNodes) return
+    private async _saveNodes(nodes: NodeMap = this.editorNodes) {
+        if (!this._needSaveNodes) {
+            return
+        }
+        this._needSaveNodes = false
+
         if (this._curNodesId == "") {
             this._curNodesId = uuidv4()
         }
+
         let save_data = {
             id: this._curNodesId,
             name: this.curNodeName,
             nodes,
             nodeTypes: {},
             locked: [...this._lockedNodes],
-            runCache: this._runCache
+            runCache: this._runCache,
+            comments: this.editorComments,
+            default: this._curNodesIsDefault,
         }
 
-        // 检查并保存所有用到的nodetypes
-        for (const key in nodes) {
-            let type_name = nodes[key].type
+        const saveNodeType = (type_name) => {
             // 1.判断是instance 还是 function
-            let ret = /instance@(get|set)@(.*)/g.exec(type_name)
+            let ret = /instance.*?@(get|set)@(.*)/g.exec(type_name)
             if (ret) {
                 save_data.nodeTypes[ret[2]] = this._nodeTypes[ret[2]]
             }
             else {
                 ret = /function@(.*)/g.exec(type_name)
                 if (ret) {
                     save_data.nodeTypes[ret[1]] = this._nodeTypes[ret[1]]
                 }
+                else {
+                    ret = /combine@(.*)/g.exec(type_name)
+                    if (ret) {
+                        save_data.nodeTypes[ret[1]] = this._nodeTypes[ret[1]]
+                    }
+                }
             }
         }
 
-        this.setEditorNodes(nodes)
-        let nodes_string = JSON.stringify(save_data)
-        let nodes_reg_exp = new RegExp(`#\\[nodes_${this._curNodesId}\\]`, "g")
-        let data = `#[nodes_${this._curNodesId}][${this.curNodeName}]${nodes_string}`
-        this._writeDataToCell(nodes_reg_exp, data)
-    }
-
-    private _get_node_data(cell: CodeCellModel) {
-        let nodes_reg_exp = /#\[nodes_(.*?)\]\[(.*?)\]([\s\S]*)/g
-        let ret = nodes_reg_exp.exec(cell.sharedModel.getSource())
-        if (!ret) {
-            return null
+        // 检查并保存所有用到的nodetypes
+        for (const key in nodes) {
+            saveNodeType(nodes[key].type)
         }
-        return {
-            id: ret[1].trim(),
-            name: ret[2].trim(),
-            data: JSON.parse(ret[3])
+        for (const typeName in this._nodeTypes) {
+            let record = this._nodeTypes[typeName]
+            if (record.nodes) {
+                for (const id in record.nodes) {
+                    saveNodeType(record.nodes[id].type)
+                }
+            }
         }
+
+        this.editorNodes = nodes
+
+        // 保存数据到metedata
+        this.setNodes(this._curNodesId, save_data)
     }
 
-    private async _loadNodes(data) {
+    private async _loadNodes(data, addRedo = true) {
+        let activate = this.node.getAttribute("data-node-editor-activate")
+        if (activate == "false" || !activate) {
+            this._needLoadData = {
+                data,
+                addRedo
+            }
+            return true
+        }
+
         if (this._curNodesId == data.id) {
             return
         }
+
+        if (addRedo) {
+            this._addRedo({
+                action: {
+                    type: "LOAD_NODES",
+                    id: data.id,
+                    from: "nodes"
+                },
+                redoAction: {
+                    type: "LOAD_NODES",
+                    id: this._curNodesId,
+                    from: "nodes"
+                },
+            })
+        }
+
         this._loadingNodes = true
-        this._isSaveNodes = false
         try {
             // 1.读取保存的nodetypes
-            this._nodeTypes = {
-                ...this._nodeTypes,
-                ...data.nodeTypes
-            }
-            for (const name in data.nodeTypes) {
-                let type_data = data.nodeTypes[name]
-                let node_types: any[] = []
-                if (type_data.type == "instance") {
-                    node_types = this._buildInstanceNodeTypes(
-                        type_data.node_type_name,
-                        type_data.target_type,
-                        type_data.target_value)
-                }
-                else if (type_data.type == "function") {
-                    node_types = this._buildFunctionNodeTypes(
-                        type_data.node_type_name,
-                        type_data.in_ports)
-                }
-
-                for (const node_type of node_types) {
-                    try {
-                        if (this.editorConfig[node_type.type])
-                            this.editorConfig.removeNodeType(node_type.type)
-                        this.editorConfig.addNodeType(node_type)
-                    } catch (error) { }
-                }
-            }
+            this._buildNodeTypesFromSaved(data)
 
             // 2.根据保存的nodes构建nodetypes
             for (const node_id in data.nodes) {
                 const node = data.nodes[node_id];
                 if (this.editorConfig.nodeTypes[node.type]) {
                     continue
                 }
@@ -2379,50 +2680,69 @@
                 }
 
                 if (!got_node_type) {
                     return false
                 }
             }
 
-            // 3.锁定的节点
+            // 3.读取锁定的节点
             if (data.locked) {
                 this._lockedNodes = new Set([...data.locked])
             }
 
-            // 4.运行缓存
+            // 4.读取运行缓存
             await this._readRunCache(data)
-            this._curNodesIsDefault = data.default
-            this.setEditorConfig(this.editorConfig)
-            // 清除当前数据
-            this._clearNodes()
-            // 加载node数据
-            this.dispatchNodes({ type: "RE_INIT", nodes: data.nodes })
-            this.setEditorNodes(data.nodes)
-            this.setCurNodeName(data.name)
+
+            // 5.读取node数据
             this._curNodesId = data.id
-            this._isSaveNodes = true
-            // 清除redolist
-            this._clearRedoList()
+            this.editorNodes = data.nodes
+            this.editorComments = data.comments || {}
+            this.setCurNodeName(data.name)
+            this._curNodesIsDefault = data.default
+
+            // 6.清除当前数据
+            this._refreshNodeEditorCache()
+
+            // 7.将数据同步到节点编辑器
+            this.dispatchNodes({ type: "RE_INIT", nodes: this.editorNodes })
+            this.dispatchComments({ type: "RE_INIT", comments: this.editorComments })
+            this._updateNodesDefaultShow()
 
+            // 8.调整视角
             setTimeout(() => {
                 this._focusToAllNodes()
-                this._updateNodesDefaultShow()
-            })
+                this._triggerRecalculation()
+                this._loadingNodes = false
+            }, 50)
+
             return true
         } catch (error) {
+            console.error(error)
         } finally {
-            this._loadingNodes = false
+            setTimeout(() => { this._loadingNodes = false }, 1000)
+
         }
         return false
     }
 
+    private _triggerRecalculation() {
+        let triggerRecalculation = this.editorOptions["triggerRecalculation"]
+        if (triggerRecalculation) {
+            triggerRecalculation()
+        }
+    }
+
+    private _getIsDefaultText() {
+        return this._curNodesIsDefault ? "默认" : "非默认"
+    }
+
     private _updateNodesDefaultShow() {
-        const element = document.getElementById("id-default-node-label")
-        if (element) {
-            element.innerText = this._curNodesIsDefault ? "默认" : "非默认"
+        if (this._nodeIsDefaultLabelRef.current) {
+            const element = this._nodeIsDefaultLabelRef.current as unknown as HTMLLabelElement
+            element.innerText = this._getIsDefaultText()
         }
     }
 
     private async _checkSessionAndKernel(translator: ITranslator | null) {
         translator = translator || nullTranslator;
         const trans = translator.load('jupyterlab');
         let sessionContext = this._context.sessionContext
@@ -2463,15 +2783,14 @@
             return false;
         }
 
         return true
     }
 
     private async _requestCompleter(code: string, cursor_pos: number) {
-        this._showMsgToNotebook = false
         return await this._context.sessionContext.session?.kernel?.requestComplete({
             code,
             cursor_pos
         })
     }
 
     private async _inspectRequest(code: string, cursor_pos: number) {
@@ -2493,64 +2812,24 @@
             }
             return false
         }
         return true
     }
 
     private async _initPython() {
-        let code = `
-import json
-def ______jupyterlab_node_editor_get_instance_info(v):
-    t = type(v)
-    d = None
-    if isinstance(v,int) or isinstance(v,float) or isinstance(v,str) or isinstance(v, bool):
-        d = v
-    return json.dumps({"type":str(t), "value":d})
-
-def ______jupyterlab_node_editor_get_urls_(urls):
-    if isinstance(urls, str):
-        try:
-            ret = json.loads(urls)
-            if not isinstance(ret, list):
-                raise TypeError('Expecting a list') 
-            return json.dumps(ret)
-        except ValueError as e:
-            return json.dumps([urls])
-        except TypeError as e:
-            raise TypeError('Invalid input type')
-    elif isinstance(urls, list):
-        return json.dumps(urls)
-    elif isinstance(urls, dict):
-        return json.dumps(list(urls.values()))
-    else:
-        raise TypeError('Invalid input type')
-
-def ______jupyterlab_get_boolean_value__(v):           
-    if v:
-        return True
-    else:
-        return False
-
-def ______jupyterlab_node_editor_hasVars(vars):
-    vars = json.loads(vars)
-    print(vars)
-    ret = {}
-    for v in vars:
-        ret[v] = v in globals()
-    return json.dumps(ret)
-`
+        let code = `import jupyterlab_nodeeditor`
         return await this._runCode(code)
     }
 
     private async _getInstanceInfo(
         instanceName,
         onIOPub: (
             msg: KernelMessage.IIOPubMessage<KernelMessage.IOPubMessageType>) => void
             | PromiseLike<void>) {
-        let code = `print(______jupyterlab_node_editor_get_instance_info(${instanceName}))`
+        let code = `jupyterlab_nodeeditor.get_instance_info(${instanceName})`
         return await this._runCode(code, onIOPub)
     }
 
     private async _getPortValue(portType: String, data: Object, name) {
         switch (portType) {
             case "any":
                 for (const key in data) {
@@ -2585,14 +2864,24 @@
                 return data["image"]
             case "tuple":
                 return "()"
             case "dict":
                 return "{}"
             case "control":
                 return ""
+            case "select": {
+                for (const key in data) {
+                    return `${data[key]}`
+                }
+            }
+            case "mselect": {
+                for (const key in data) {
+                    return `${data[key]}`
+                }
+            }
             default:
                 return data
         }
     }
 
 
     private _getCellIndex(reg: RegExp) {
@@ -2603,21 +2892,21 @@
                     return index
                 reg.lastIndex = 0
             }
         }
         return null
     }
 
-    private _getNodesCellIndex(id) {
-        let nodes_reg_exp = new RegExp(`nodes_${id}`, 'g');
-        return this._getCellIndex(nodes_reg_exp)
+    private _clearNodes() {
+        this.dispatchNodes({ type: "CLEAR" })
+        this.dispatchComments({ type: "CLEAR" })
+        this._refreshNodeEditorCache()
     }
 
-    private _clearNodes() {
-        this.dispatchNodes({ type: "CLEAR", nodes: this.editorNodes })
+    private _refreshNodeEditorCache() {
         let refreshCache = this.editorOptions["refreshCache"]
         if (refreshCache) refreshCache()
     }
 
     private _outputText(text) {
         this._outputArea.model.add({
             output_type: "stream",
@@ -2664,30 +2953,23 @@
             let state = kernelStateMap[msg.content.execution_state]
             if (state) {
                 this._setKernelState(state)
             }
         }
 
         if (outputMsg) {
-            let curCellModel = this._getCurNodeCellModel()
-            if (this._showMsgToNotebook
-                && curCellModel
-                && !KernelMessage.isExecuteInputMsg(msg)) {
-                curCellModel.outputs.add(outputMsg)
-            }
-
             if (this._outputArea) {
                 this._outputArea.model.add(outputMsg)
             }
         }
     }
 
-    private _get_out_var_name(nodeId) {
+    private _getOutVarName(nodeId) {
         let out_var_name = `_${nodeId}_out`
-        return out_var_name.replace(/-/g, "")
+        return out_var_name.replace(/-/g, "_")
     }
 
     private _addRedo(action) {
         // 1.将this._redoListIndex以后的全部删除
         this._redoList.splice(this._redoListIndex, this._redoList.length - this._redoListIndex)
         this._redoList.push(action)
         // 2.检测redolist是否超长
@@ -2703,22 +2985,22 @@
         let setMenuCoordinates = this.editorOptions["setMenuCoordinates"]
         let setMenuOpen = this.editorOptions["setMenuOpen"]
         let pos = { x: this._mouseMove.clientX, y: this._mouseMove.clientY }
         setTimeout(() => {
             setMenuCoordinates(pos);
             setMenuOpen(true);
             setTimeout(() => {
-                let inputElement = document.querySelector('[data-flume-component="ctx-menu-input"]') as HTMLInputElement
+                let inputElement = this.editorOptions['menuInputRef'].current as HTMLInputElement
                 inputElement.value = filter
                 inputElement.selectionEnd = inputElement.value.length;
                 setTimeout(() => {
                     let setFilter = this.editorOptions["setFilter"]
                     setFilter(inputElement.value)
-                }, 100);
-            })
+                });
+            }, 50)
         })
     }
 
     private _startDrag() {
         if (!this._dragging) {
             let draggableRef = this.editorOptions["draggableRef"]
             if (this._isDraggableFocus()) {
@@ -2880,72 +3162,100 @@
             translate: {
                 x: 0,
                 y: 0
             }
         });
     }
 
-    private _focusToNodes(nodeIds) {
+    private _nodeXY2ClientXY(x, y) {
+        let nodeXY2ClientXY = this.editorOptions["nodeXY2ClientXY"]
+        if (!nodeXY2ClientXY) {
+            throw new Error("nodeXY2ClientXY是空的");
+        }
+
+        return nodeXY2ClientXY(x, y)
+    }
+
+    private _getNodesCenter(nodeIds) {
         // 计算最小的X，最大的X，最小的y，最大的y
         let minX = Number.MAX_SAFE_INTEGER
         let minY = Number.MAX_SAFE_INTEGER
         let maxX = Number.MIN_SAFE_INTEGER
         let maxY = Number.MIN_SAFE_INTEGER
         let node
         let element: HTMLDivElement
+
         for (const nodeId of nodeIds) {
-            node = this.editorNodes[nodeId]
-            if (minX >= node.x) {
-                minX = node.x
-            }
-            if (minY >= node.y) {
-                minY = node.y
-            }
+            node = this._getNode(nodeId)
+            if (node) {
+                element = this.editorOptions[`nodeDraggable_${nodeId}`].current as HTMLDivElement
+                if (!element) {
+                    continue
+                }
 
-            element = this.editorOptions[`nodeDraggable_${nodeId}`].current as HTMLDivElement
-            if (maxX <= node.x + element.clientWidth) {
-                maxX = node.x + element.clientWidth
-            }
+                if (minX >= node.x) {
+                    minX = node.x
+                }
+                if (minY >= node.y) {
+                    minY = node.y
+                }
+
+                if (maxX <= node.x + element.clientWidth) {
+                    maxX = node.x + element.clientWidth
+                }
 
-            if (maxY <= node.y + element.clientHeight) {
-                maxY = node.y + element.clientHeight
+                if (maxY <= node.y + element.clientHeight) {
+                    maxY = node.y + element.clientHeight
+                }
             }
         }
 
         // 计算节点的宽高
         const width = maxX - minX
         const height = maxY - minY
 
         // 计算中心点
         const centerX = width / 2 + minX
         const centerY = height / 2 + minY
+        return {
+            width,
+            height,
+            centerX,
+            centerY
+        }
+    }
 
+    private _focusToNodes(nodeIds) {
+        let ret = this._getNodesCenter(nodeIds)
         // 计算应该缩放的大小
         const container = this._editorContainerRef.current
         let rect = container.getBoundingClientRect()
-        let scale = Math.min(rect.width / width, rect.height / height)
+        let scale = Math.min(rect.width / ret.width, rect.height / ret.height)
         scale = Math.min(1, scale)
 
         // 更新位移和缩放
         const dispatchStageState = this.editorOptions["dispatchStageState"]
         dispatchStageState({
             type: "SET_TRANSLATE_SCALE",
             scale: scale,
             translate: {
-                x: centerX * scale,
-                y: centerY * scale,
+                x: ret.centerX * scale,
+                y: ret.centerY * scale,
             }
         });
     }
 
     private _focusToAllNodes() {
         const nodeIds: any[] = []
         for (const nodeId in this.editorNodes) {
             nodeIds.push(nodeId)
         }
+        for (const commentId in this.editorComments) {
+            nodeIds.push(commentId)
+        }
         if (nodeIds.length == 0) {
             return
         }
         this._focusToNodes(nodeIds)
     }
 
     private _focusToSelectedNodes() {
@@ -2961,38 +3271,47 @@
             || this._containerRef.current == document.activeElement
             || this._containerRef.current.parentElement == document.activeElement
 
     }
 
     private _removeSelectedNodes() {
         if (this._isDraggableFocus() && this.selectedNodes.size > 0) {
-            this.dispatchNodes({
-                type: "REMOVE_NODES",
-                nodeIds: this.selectedNodes
-            })
+            const filteredIds = this._classifySelectedNodes()
+            if (filteredIds.nodeIds.length > 0) {
+                this.dispatchNodes({
+                    type: "REMOVE_NODES",
+                    nodeIds: filteredIds.nodeIds
+                })
+            }
+            if (filteredIds.commentIds.length > 0) {
+                this.dispatchComments({
+                    type: "DELETE_COMMENTS",
+                    ids: filteredIds.commentIds
+                })
+            }
         }
     }
 
-    private _genNodeId() {
+    private _genNodeId(length = nodeIdLength) {
         const nanoid = this.editorOptions["nanoid"]
-        if (nanoid) return nanoid(10)
+        if (nanoid) return nanoid(length)
     }
 
     private _copySelectedNodes() {
         if (!this._isDraggableFocus() || this.selectedNodes.size == 0) {
             return
         }
 
         const nodes = {}
         // 创建副本
         for (const id of this.selectedNodes) {
-            const node = this.editorNodes[id]
+            const node = this._getNode(id)
             if (!node) continue
             const newNode = cloneDeep(node)
-            newNode.newId = this._genNodeId()
+            newNode.newId = this._genNodeId(newNode.id.length)
             nodes[id] = newNode
         }
 
         // 重新构建连接
         const refreshConnection = (node, target) => {
             let puts = node.connections[target]
             for (const portName in puts) {
@@ -3004,52 +3323,351 @@
                     } else {
                         delete puts[portName]
                     }
                 }
             }
         }
 
-
         let node
         this._copyedNodes = []
         for (const oldId in nodes) {
             node = nodes[oldId]
-            // 替换连接中的ID为新的ID
-            refreshConnection(node, "inputs")
-            refreshConnection(node, "outputs")
+            if (oldId.length == nodeIdLength) {
+                // 替换连接中的ID为新的ID
+                refreshConnection(node, "inputs")
+                refreshConnection(node, "outputs")
+            }
             node.id = node.newId
             // delete node.newId
             this._copyedNodes.push(node)
         }
     }
 
     private _pasteSelectedNodes() {
         if (!this._copyedNodes || !this._mouseMove) {
             return
         }
 
+        const classifiedNodes = this._classifyCopyedNodes()
+
         this.dispatchNodes({
             type: "ADD_NODES",
-            nodes: this._copyedNodes
+            nodes: classifiedNodes.nodes
+        })
+        this.dispatchComments({
+            type: "ADD_COMMENTS",
+            comments: classifiedNodes.comments
         })
 
         // 选择所有粘贴的节点
         setTimeout(() => {
             this.selectedNodes.clear()
             for (const node of this._copyedNodes) {
                 this.selectedNodes.add(node.id)
             }
             this.refreshNodeBoxShadow()
         });
     }
 
+    private _addNodeTypes(nodeTypes) {
+        for (const nodeType of nodeTypes) {
+            // 添加节点类型
+            try {
+                if (this.editorConfig[nodeType.type])
+                    this.editorConfig.removeNodeType(nodeType.type)
+                this.editorConfig.addNodeType(nodeType)
+            } catch (error) { }
+        }
+    }
+
+    private async _combineSelectedNodes() {
+        const classifiedNodes = this._classifySelectedNodes()
+        if (classifiedNodes.nodeIds.length == 0) {
+            showErrorMessage("错误", "没有选中节点!")
+            return
+        }
+
+        let nodesCache = {}
+        let newNodeId = this._genNodeId(nodeIdLength)
+
+        // 筛选出端口节点
+        let outNodes: any[] = []
+        let node
+        let connection
+        for (const id of classifiedNodes.nodeIds) {
+            node = this._getNode(id)
+            if (!node) {
+                showErrorMessage("错误", "节点不存在，请重新加载节点!")
+                return
+            }
+
+            // 缓存节点
+            nodesCache[id] = cloneDeep(node)
+
+            let flag = true
+            for (const portName in node.connections.outputs) {
+                connection = node.connections.outputs[portName][0]
+                if (connection
+                    && classifiedNodes.nodeIds.findIndex((value, index) => {
+                        return connection.nodeId == value
+                    }) != -1) {
+                    flag = false
+                    break
+                }
+            }
+            if (flag) {
+                outNodes.push(id)
+            }
+
+        }
+
+        // 如果输出节点多于一个，要提示
+        if (outNodes.length > 1) {
+            showErrorMessage("错误", "只能选中一个输出节点")
+            return
+        }
+
+        // 向前递归获取链上的所有节点
+        let linkedNodeIds = await this._getNodeInputLinkedNodes(outNodes[0])
+
+        // 扫描查看有没有不在linkedNodeIds中的节点被选中了
+        for (const id of classifiedNodes.nodeIds) {
+            if (id == outNodes[0]) {
+                continue
+            }
+
+            if (linkedNodeIds.findIndex((value, index) => id == value) == -1) {
+                showErrorMessage("错误", "不要选择不在输出节点链上的节点")
+                return
+            }
+        }
+
+        let typeName = ""
+        const ret = await showDialog({
+            title: "请输入名称",
+            body: <input type="text" onChange={e => {
+                typeName = e.target.value
+            }}></input>,
+            buttons: [Dialog.cancelButton({ label: "取消" }),
+            Dialog.okButton({ label: '确定' })]
+        })
+
+        if (ret.button.label != "确定") {
+            return
+        }
+
+        // 选出输入节点数据
+        let connectionData = {}
+        const in_ports: any[] = []
+        for (const id of classifiedNodes.nodeIds) {
+            if (id == outNodes[0]) {
+                continue
+            }
+            node = this._getNode(id)
+            let inputs = await this._getNodeInputs(node)
+            for (const input of inputs) {
+                if (input.type == "control" || input.hidePort) {
+                    continue
+                }
+
+                connection = node.connections.inputs[input.name]
+                if (!connection || classifiedNodes.nodeIds.findIndex((value, index) => {
+                    return value == connection[0].nodeId
+                }) == -1) {
+                    // 为节点的输入添加替代值，以便在生成代码的时候可以用来替换端口的值
+                    node.inputValues = node.inputValues || {}
+                    delete node.inputValues[input.name]
+                    let arg_default: any = null
+                    if (connection) {
+                        connectionData[id] = connectionData[id] || []
+                        connectionData[id].push(connection[0])
+                        let cacheNode = nodesCache[id]
+                        delete cacheNode.connections.inputs[input.name]
+                    }
+                    else {
+                        arg_default = await this._getInputValue(input, node)
+                    }
+                    in_ports.push({
+                        arg_name: `${id}@${input.name}`,
+                        arg_label: input.label,
+                        arg_type: input.type,
+                        arg_default,
+                    })
+                    node.inputValues[input.name] = `${id}@${input.name}`
+                }
+            }
+        }
+
+        let record = {
+            type: "combine",
+            node_type_name: typeName,
+            in_ports,
+            code: "",
+            nodes: nodesCache,
+        }
+
+        // 断开节点与外部的链接
+        let newConnections: any[] = []
+        for (const nodeId in connectionData) {
+            let connections = connectionData[nodeId]
+            for (const connection of connections) {
+                let fromNode = this._getNode(connection.nodeId)
+                let inputs = fromNode.connections.outputs[connection.portName]
+                for (const input of inputs) {
+                    if (input.nodeId == nodeId) {
+                        this.dispatchNodes({
+                            type: "REMOVE_CONNECTION",
+                            input,
+                            output: connection,
+                        })
+                        // 创建新的connection用于创建combine节点后添加链接
+                        newConnections.push({
+                            input: {
+                                nodeId: newNodeId,
+                                portName: `${nodeId}@${input.portName}`
+                            },
+                            output: connection,
+                        })
+                    }
+                }
+            }
+        }
+
+        // 生成代码
+        record.code = await new Promise((resolve, reject) => {
+            setTimeout(() => {
+                this._buildNodeCode(outNodes[0]).then(ret => {
+                    resolve(this._getExportedCodeText())
+                })
+            });
+        })
+
+        record.code = record.code.replace(this._getOutVarName(outNodes[0]), this._getOutVarName(newNodeId))
+
+        // 清除inputsCache
+        for (const id of classifiedNodes.nodeIds) {
+            node = this._getNode(id)
+            delete node.inputValues
+        }
+
+        // 保存记录
+        this._nodeTypes[typeName] = record
+
+        // 构建nodeType并添加到配置
+        const nodeTypes = this._buildCommonNodeTypes(
+            record.node_type_name,
+            record.in_ports,
+            record.type)
+        this._addNodeTypes(nodeTypes)
+
+        // 移除选中的节点
+        this._removeSelectedNodes()
+
+        // 计算一个中心点用于添加新的节点
+        let centerRet = this._getNodesCenter(classifiedNodes.nodeIds)
+
+        // 添加新节点
+        this.dispatchNodes({
+            type: "ADD_NODE",
+            id: newNodeId,
+            nodeType: nodeTypes[0].type,
+            x: centerRet.centerX,
+            y: centerRet.centerY,
+        })
+
+        // 添加连接
+        for (const action of newConnections) {
+            this.dispatchNodes({
+                type: "ADD_CONNECTION",
+                ...action
+            })
+        }
+
+        let outNode = nodesCache[outNodes[0]]
+        for (const portName in outNode.connections.outputs) {
+            connection = outNode.connections.outputs[portName]
+            if (connection) {
+                this.dispatchNodes({
+                    type: "ADD_CONNECTION",
+                    input: connection[0],
+                    output: { nodeId: newNodeId, portName }
+                })
+                delete outNode.connections.outputs[portName]
+            }
+        }
+    }
+
+    private _separateSelectedNode() {
+        if (this.selectedNodes.size == 0) {
+            return
+        }
+        if (this.selectedNodes.size > 1) {
+            showErrorMessage("错误", "只能选择一个节点")
+            return
+        }
+
+        let targetNodeId = ""
+        for (const id of this.selectedNodes) {
+            targetNodeId = id
+        }
+
+        let node = this._getNode(targetNodeId)
+        let matchRet = /combine@(.*)/g.exec(node.type)
+        if (!matchRet) {
+            showErrorMessage("错误", "该节点不是一个组合节点")
+            return
+        }
+
+        // 获取记录
+        let record = this._nodeTypes[matchRet[1]]
+        if (!record) {
+            showErrorMessage("错误", "没找到类型记录")
+            return
+        }
+
+        // 移除当前的节点
+        this._removeSelectedNodes()
+
+        // 添加记录的节点
+        let nodes: any[] = []
+        for (const id in record.nodes) {
+            let node = record.nodes[id]
+            node.inputValues = {}
+            nodes.push(node)
+        }
+
+        this.dispatchNodes({
+            type: "ADD_NODES",
+            nodes
+        })
+
+        setTimeout(() => {
+            let nodeIds = Object.keys(record.nodes)
+            let center = this._getNodesCenter(nodeIds)
+            let directX = node.x - center.centerX
+            let directY = node.y - center.centerY
+            for (const nodeId of nodeIds) {
+                let tmpNode = this._getNode(nodeId)
+                this.dispatchNodes({
+                    type: "SET_NODE_COORDINATES",
+                    x: tmpNode.x + directX,
+                    y: tmpNode.y + directY,
+                    nodeId
+                })
+            }
+        });
+    }
+
     private _selectAllNodes() {
         for (const id in this.editorNodes) {
             this.selectedNodes.add(id)
         }
+        for (const id in this.editorComments) {
+            this.selectedNodes.add(id)
+        }
         this.refreshNodeBoxShadow()
     }
 
     private _getStageDraggableZuobiao(clientX, clientY) {
         const translateWrapper = this.editorOptions["translateWrapper"]
         const rect = translateWrapper.current.getBoundingClientRect()
         const scale = this.editorOptions["stagetScale"]
@@ -3123,96 +3741,83 @@
     }
 
     private _stopDrawSelect() {
         if (!this._showSelectRect) {
             return
         }
 
-        function getDuiJiaoZuoBiao(rect) {
-            let x1 = Math.min(rect.x, rect.x + rect.width);
-            let y1 = Math.min(rect.y, rect.y + rect.height);
-            let x2 = Math.max(rect.x, rect.x + rect.width);
-            let y2 = Math.max(rect.y, rect.y + rect.height);
-            return { x1, x2, y1, y2 }
-        }
-
-        function rectsIntersect(rect1, rect2) {
-            let duijiao1 = getDuiJiaoZuoBiao(rect1)
-            let duijiao2 = getDuiJiaoZuoBiao(rect2)
-            return duijiao1.x1 < duijiao2.x2
-                && duijiao1.x2 > duijiao2.x1
-                && duijiao1.y1 < duijiao2.y2
-                && duijiao1.y2 > duijiao2.y1
-        }
-
         // 获取矩形数据
         const d = this._calcSelctRect(this._mouseMove)
 
-        // 根据矩形数据，选择nodes
-        this.selectedNodes.clear()
-        for (const nodeId in this.editorNodes) {
-            const node = this.editorNodes[nodeId]
-            const element = document.getElementById(nodeId)
+        const processNode = (nodeId) => {
+            const node = this._getNode(nodeId)
+            const element = this._getNodeElement(nodeId)
             if (element) {
                 let rect = element.getBoundingClientRect()
                 if (rectsIntersect(d, {
                     x: node.x,
                     y: node.y,
                     width: rect.width,
                     height: rect.height
                 })) {
                     this.selectedNodes.add(nodeId)
                 }
             }
         }
 
+        // 根据矩形数据，选择nodes
+        this.selectedNodes.clear()
+        for (const nodeId in this.editorNodes) {
+            processNode(nodeId)
+        }
+        for (const nodeId in this.editorComments) {
+            processNode(nodeId)
+        }
+
         // 刷新选择
         this.refreshNodeBoxShadow()
 
-
         // 清除矩形
         const element = this._selectRectRef as SVGPathElement
         element.setAttribute("d", ``)
         this._showSelectRect = false
         this._drawStartPos = null
     }
 
+
     private _refreshSelectedNodes() {
         // 刷新选择
         const remove_list: any[] = []
         for (const id of this.selectedNodes) {
-            if (!this.editorNodes[id]) {
+            if (!this._getNode(id)) {
                 remove_list.push(id)
             }
         }
 
         // 删除已经移除的节点
         for (const id of remove_list) {
             this.selectedNodes.delete(id)
         }
 
         // 刷新选择表现
-        let element: HTMLElement | null
         for (const id in this.editorNodes) {
-            if (!this.selectedNodes.has(id)) {
-                continue
+            if (this.selectedNodes.has(id)) {
+                this._setNodeBoxShadow(id, nodeSelectedBoxShadow)
             }
-
-            element = document.getElementById(id)
-            if (!element) {
-                continue
+        }
+        for (const id in this.editorComments) {
+            if (this.selectedNodes.has(id)) {
+                this._setNodeBoxShadow(id, nodeSelectedBoxShadow)
             }
-
-            this._setNodeBoxShadow(id, nodeSelectedBoxShadow)
         }
     }
 
     private async _setNodePortControlInputValue(nodeId, portName, controlName, value) {
         // 获取NODE
-        const node = this.editorNodes[nodeId]
+        const node = this._getNode(nodeId)
         if (!node) {
             return
         }
 
         // 获取inputs数据
         let inputs = await this._getNodeInputs(node)
         let portType: any = null
@@ -3225,30 +3830,30 @@
             break
         }
 
         switch (portType) {
             case "number": {
                 const ret = document.evaluate(
                     `//input[@data-node-id="${nodeId}"][@data-port-name="${portName}"][@data-name="${controlName}"]`,
-                    document,
+                    this.node,
                     null,
                     XPathResult.FIRST_ORDERED_NODE_TYPE,
                     null)
                 let element = ret.singleNodeValue
                 if (!element) {
                     return
                 }
                 (element as HTMLInputElement).value = value
             } break
             case "jsstring":
             case "string":
             case "any": {
                 const ret = document.evaluate(
                     `//textarea[@data-node-id="${nodeId}"][@data-port-name="${portName}"][@data-name="${controlName}"]`,
-                    document,
+                    this.node,
                     null,
                     XPathResult.FIRST_ORDERED_NODE_TYPE,
                     null)
                 let element = ret.singleNodeValue
                 if (!element) {
                     return
                 }
@@ -3257,45 +3862,32 @@
             default: return
         }
     }
 
     private _updateHeaderCache() {
         const remove_list: any[] = []
         for (const nodeId in this._headRenderCache) {
-            if (!this.editorNodes[nodeId]) {
+            if (!this._getNode(nodeId)) {
                 remove_list.push(nodeId)
             }
         }
         for (const nodeId of remove_list) {
             delete this._headRenderCache[nodeId]
         }
     }
 
-    private _lockSelectedNodes() {
-        if (this.selectedNodes.size == 0) {
-            return
-        }
-
-        for (const nodeId of this.selectedNodes) {
-            // 如果已经锁住了
-            if (this._lockedNodes.has(nodeId)) {
-
-            }
-        }
-    }
-
-    private async _getNodeInputLinkedNodes(nodeId, exceptNames = new Set()) {
-        let node = this.editorNodes[nodeId]
+    private async _getNodeInputLinkedNodes(nodeId, exceptInputNames = new Set()) {
+        let node = this._getNode(nodeId)
         if (!node) {
             return []
         }
         let ret: any[] = []
         let inputs = await this._getNodeInputs(node)
         for (const input of inputs) {
-            if (exceptNames.has(input.name)) {
+            if (exceptInputNames.has(input.name)) {
                 continue
             }
 
             let connection = node.connections.inputs[input.name]
             if (!connection) {
                 continue
             }
@@ -3304,27 +3896,24 @@
             let tmpret = await this._getNodeInputLinkedNodes(connectionData.nodeId)
             ret = [...ret, ...tmpret]
         }
         return ret
     }
 
     private _getCellModelByregExp(exp: RegExp) {
-        let target_cell: null | CodeCellModel = null
         for (let index = 0; index < this._context.model.cells.length; index++) {
             const cell = this.cellGet(index);
             if (cell.type == "code") {
+                exp.lastIndex = 0
                 let ret = exp.exec(cell.sharedModel.getSource())
                 if (ret) {
-                    target_cell = cell as CodeCellModel
-                    break
+                    return cell as CodeCellModel
                 }
-                exp.lastIndex = 0
             }
         }
-        return target_cell
     }
 
     private _writeDataToCell(exp, data) {
         // 查找nodes保存的cell
         let target_cell = this._getCellModelByregExp(exp)
 
         // 如果没有找到，添加一个cell用于保存节点
@@ -3332,31 +3921,23 @@
             this.cellInsert(0)
             target_cell = this.cellGet(0) as CodeCellModel
         }
 
         target_cell.sharedModel.setSource(data)
     }
 
-    private _getCurNodeCellModel() {
-        let nodes_reg_exp = new RegExp(`#\\[nodes_${this._curNodesId}\\]`, "g")
-        return this._getCellModelByregExp(nodes_reg_exp)
-    }
-
-    private _clearCurOutput() {
-        let model = this._getCurNodeCellModel()
-        if (model) {
-            model.outputs.clear()
-        }
-    }
 
     private _clearRunCache() {
         if (!this._isDraggableFocus()) {
             return
         }
         this._runCache = {}
+        this._runningError = false
+        this._runningNodeId = 0
+        this.refreshNodeBoxShadow()
         this._saveNodes(this.editorNodes)
     }
 
     private async _readRunCache(data) {
         this._runCache = data.runCache || {}
 
         let cache
@@ -3366,15 +3947,15 @@
             for (const portName in cache) {
                 args.push(cache[portName])
             }
         }
 
         let argsStr = JSON.stringify(args)
         let ret: any = null
-        await this._runCode(`______jupyterlab_node_editor_hasVars('${argsStr}')`, msg => {
+        await this._runCode(`jupyterlab_nodeeditor.has_var('${argsStr}')`, msg => {
             if (KernelMessage.isExecuteResultMsg(msg)) {
                 let retString = eval(msg.content.data["text/plain"] as string)
                 ret = JSON.parse(retString)
             }
         })
 
         if (!ret) {
@@ -3396,51 +3977,49 @@
         for (const nodeId of removeList) {
             delete this._runCache[nodeId]
         }
     }
 
 
     private _toggleOutputArea() {
-        if (this._showOutputArea) {
-            ReactWidget.detach(this._outputArea)
-        }
         this._setShowOutputArea(!this._showOutputArea)
-
     }
 
     private _onOutputModelChanged() {
         if (!this._outputAreaContainerRef.current) {
             return
         }
 
         if (this._showOutputArea && this._outputAreaAutoScroll) {
             const element = this._outputAreaContainerRef.current as unknown as HTMLElement
             element.scrollTop = element.scrollHeight - element.clientHeight;
         }
     }
 
+    private _getNodeElement(nodeId) {
+        let ret = this.node.querySelector(`[id='${nodeId}']`)
+        if (!ret) {
+            return null
+        }
+        return ret as HTMLDivElement
+    }
+
     private _setNodeBoxShadow(nodeId, boxShadow) {
-        const element = document.getElementById(nodeId)
+        const element = this._getNodeElement(nodeId)
         if (!element) {
             return
         }
         element.style.boxShadow = boxShadow
     }
 
     private _refreshRunningNode() {
-        let element: HTMLElement | null
         for (const id in this.editorNodes) {
             if (this._runningNodeId != id) {
                 continue
             }
-            element = document.getElementById(id)
-            if (!element) {
-                continue
-            }
-
             this._setNodeBoxShadow(id,
                 this._runningError ? nodeErrorBoxShadow : nodeRunningBoxShadow
             )
         }
     }
 
     private _setRunningNode(nodeId, error = false) {
@@ -3492,17 +4071,18 @@
         if (!cell) {
             return null
         }
         return cell.sharedModel.getSource()
     }
 
     private _onCodeEditorChange(value: string | undefined, event: monaco.editor.IModelContentChangedEvent) {
-        if (value == undefined) {
+        if (!this._codeEditorNeedSave || value == undefined) {
             return
         }
+
         this._codeEditorValueCache = value
         if (this._curEditingCellIndex >= 0) {
             let cell = this.cellGet(this._curEditingCellIndex)
             if (!cell) {
                 this.cellInsert(this._curEditingCellIndex)
                 cell = this.cellGet(this._curEditingCellIndex)
             }
@@ -3510,29 +4090,37 @@
         }
     }
 
     private _openCellEditor() {
         this._setUseDiffEditor(false)
         this._setshowCodeEditor(true)
         setTimeout(() => {
-            this._editCell(0)
+            let index = this._getCodeCell(0, this._context.model.cells.length, 1)
+            if (index != undefined) {
+                this._editCell(index)
+            } else {
+                this.cellInsert(0)
+                this._editCell(0)
+            }
         }, 0);
     }
 
     private _editCell(index) {
         this._curEditingCellIndex = index
         const cell = this.cellGet(index)
         let text = ""
         if (cell) {
             text = cell.sharedModel.getSource()
         }
 
         if (this._codeEditor) {
+            this._codeEditorNeedSave = false
             this._codeEditor.setValue(text)
             this._codeEditor.pushUndoStop()
+            this._codeEditorNeedSave = true
         }
 
         if (this._cellIndexInputRef.current) {
             const element = this._cellIndexInputRef.current as unknown as HTMLInputElement
             element.value = `${this._curEditingCellIndex}`
         }
     }
@@ -3541,15 +4129,15 @@
         options: any[] = [],
         setOptions,
         filterOptions) {
         filter = filter.trim()
         if (!filter.trim()) return
         filter = filter.replace(/。/g, ".")
         if (filter.charAt(0) == ".") {
-            let nodes = this._loadNodesFromAllCell()
+            let nodes = this._loadNodesAsList()
             let options = filterOptions(filter, this._internal_options)
             for (const node of nodes) {
                 options.push({
                     label: "." + node.name,
                     description: "加载节点" + node.name + node.id,
                     ...node
                 })
@@ -3816,144 +4404,402 @@
             buttons: [Dialog.cancelButton({ label: "取消" }),
             Dialog.okButton({ label: '确定' })]
         }).then(ret => {
             if (ret.button.label != "确定") {
                 return
             }
             this.setCurNodeName(this._renameCache)
+            this._needSaveNodes = true
             setTimeout(() => { this.onNodesChange(this.editorNodes) })
         })
     }
 
+    private _copyNodes() {
+        // 先保存当前的
+        this._needSaveNodes = true
+        this.onNodesChange(this.editorNodes)
+        this._curNodesId = uuidv4()
+        this.setCurNodeName(`${this.curNodeName}_复制`)
+        setTimeout(() => {
+            this._needSaveNodes = true
+            this.onNodesChange(this.editorNodes)
+        })
+    }
+
     private _clearRedoList() {
         this._redoListIndex = 0
         this._redoList = []
     }
 
     private _createCommand(id, desc, execute) {
+        this._commandsMap[id] = execute
+
         const { commands } = this._app
         const category = "node-editor"
         if (commands.hasCommand(id)) {
             return
         }
 
         commands.addCommand(id, {
             label: `${id}(${desc})`,
-            execute
+            execute: () => {
+                const element = document.querySelector("[data-node-editor-activate=true]")
+                if (!element) {
+                    return
+                }
+                element.dispatchEvent(new CustomEvent("command", { detail: id }))
+            }
         })
+
         this._palette.addItem({
             command: id,
             category
         })
     }
 
     private _setKernelState(value) {
-        const elements = document.querySelectorAll("[data-name='node-editor-kernel-state-label']")
-        for (const element of elements) {
-            (element as HTMLLabelElement).innerText = value
+        if (this._kernelStateLabelNodeEditorRef.current) {
+            const element = this._kernelStateLabelNodeEditorRef.current as unknown as HTMLDivElement
+            element.innerText = value
+        }
+        if (this._kernelStateLabelCodeEditorRef.current) {
+            const element = this._kernelStateLabelCodeEditorRef.current as unknown as HTMLDivElement
+            element.innerText = value
+        }
+    }
+
+    private _getCodeCell(startIndex, endIndex, direct) {
+        try {
+            const cells = this._context.model.cells
+            for (let index = startIndex; direct > 0 ? index <= endIndex : index >= endIndex; index += direct) {
+                if (cells.get(index).type != "code") {
+                    continue
+                }
+                return index
+            }
+        } catch (error) {
+        }
+    }
+
+    private _getNode(nodeId) {
+        return this.editorNodes[nodeId] || this.editorComments[nodeId]
+    }
+
+    private _classifySelectedNodes() {
+        let nodeIds: any[] = []
+        let commentIds: any[] = []
+        for (const id of this.selectedNodes) {
+            if (id.length == commentIdLength) {
+                commentIds.push(id)
+            } else {
+                nodeIds.push(id)
+            }
+        }
+        return {
+            nodeIds,
+            commentIds
+        }
+    }
+
+    private _classifyCopyedNodes() {
+        let nodes: any[] = []
+        let comments = {}
+        for (const node of this._copyedNodes) {
+            if (node.id.length == commentIdLength) {
+                comments[node.id] = node
+            } else {
+                nodes.push(node)
+            }
+        }
+        return { nodes, comments }
+    }
+
+    private _openSelectedCommentsColorPicker() {
+        if (!this._isDraggableFocus()) {
+            return
+        }
+        const classifiedNodes = this._classifySelectedNodes()
+        for (const id of classifiedNodes.commentIds) {
+            let setOpenPickingColor = this.editorOptions[`commentSetIsPickingColor_${id}`]
+            if (setOpenPickingColor) {
+                setOpenPickingColor(true)
+            }
+        }
+    }
+
+    private _openLoadMenu() {
+        if (this._isDraggableFocus())
+            this._setMenuOpen(".")
+    }
+
+    private _clearOutput() {
+        this._clearOutputArea()
+    }
+
+    private _insertCellToCurrentIndex() {
+        this.cellInsert(this._curEditingCellIndex + 1)
+        this._editCell(this._curEditingCellIndex + 1)
+    }
+
+    private _deleteCurrentCell() {
+        this.cellRemove(this._curEditingCellIndex)
+        this._editPreCell()
+    }
+
+    private _undoCell() {
+        this.cellUndo()
+        this._editCell(this._curEditingCellIndex)
+    }
+
+    private _redoCell() {
+        this.cellRedo()
+        this._editCell(this._curEditingCellIndex)
+    }
+
+    private _editPreCell() {
+        if (this._codeEditor) {
+            let index = this._getCodeCell(this._curEditingCellIndex - 1, 0, -1)
+            if (index != undefined) {
+                this._editCell(index)
+            }
+        } else if (this.node.querySelector("[data-show-image-viewer=false][data-show-code-editor=false]")) {
+            const datas = this._loadNodesAsList()
+            for (let index = 0; index < datas.length; index++) {
+                if (this._curNodesId == datas[index].id) {
+                    this._loadNodes(datas[(index - 1 + datas.length) % datas.length].data)
+                }
+            }
+        }
+    }
+
+    private _editNextCell() {
+        if (this._codeEditor) {
+            const cells = this._context.model.cells
+            let index = this._getCodeCell(this._curEditingCellIndex + 1, cells.length - 1, 1)
+            if (index != undefined) {
+                this._editCell(index)
+            }
+        } else if (this.node.querySelector("[data-show-image-viewer=false][data-show-code-editor=false]")) {
+            const datas = this._loadNodesAsList()
+            for (let index = 0; index < datas.length; index++) {
+                if (this._curNodesId == datas[index].id) {
+                    this._loadNodes(datas[(index + 1) % datas.length].data)
+                }
+            }
+        }
+    }
+
+
+    private _CellMove(direct) {
+        if (this._curEditingCellIndex == -1 || !this._codeEditor) {
+            return
+        }
+
+        let targetIndex = this._curEditingCellIndex + direct
+
+        const cells = this._context.model.cells
+        if (targetIndex < 0 || targetIndex >= cells.length) {
+            return
+        }
+        let curModel = cells.get(this._curEditingCellIndex).sharedModel
+        let taregtModel = cells.get(targetIndex).sharedModel
+        let tmp = curModel.getSource()
+        curModel.setSource(taregtModel.getSource())
+        taregtModel.setSource(tmp)
+
+        this._editCell(targetIndex)
+    }
+
+    private _setCurrentNodesAsDefault() {
+        this._curNodesIsDefault = true
+        this._updateNodesDefaultShow()
+        this._needSaveNodes = true
+        this._saveNodes()
+    }
+
+    private async _buildNodeCode(id) {
+        let preCheckCache = this._runCheckCache
+        try {
+            this._exportRet = []
+            this._exportingCodeNodeId = id
+            this._runCheckCache = false
+            this._exportIndent = ""
+            await this.runNode(id)
+            this._codeEditorValueCache = this._getExportedCodeText()
+        } catch (e) {
+            showErrorMessage("错误", "将节点生成为代码发生错误！")
+            return false
+        }
+        finally {
+            this._exportingCodeNodeId = null
+            this._runCheckCache = preCheckCache
+        }
+
+        return true
+    }
+
+    private async _dispatchNodesAction(action) {
+        switch (action.type) {
+            case "CREATE_NODES": {
+                await this.createNewNodes(false)
+            } break
+            case "DELETE_NODES": {
+                await this.deleteNodes(action.id, false, false)
+            } break;
+            case "RESTORE_NODES": {
+                this.setNodes(action.data.id, action.data)
+                this._loadNodes(action.data, true)
+            } break
+            case "LOAD_NODES": {
+                let nodes = this.getNodes(action.id)
+                if (nodes) {
+                    await this._loadNodes(nodes, false)
+                }
+            } break
+            default:
+                break;
+        }
+    }
+
+    private _buildNodeTypesFromSaved(data) {
+        this._nodeTypes = {
+            ...this._nodeTypes,
+            ...data.nodeTypes
+        }
+        for (const name in data.nodeTypes) {
+            let type_data = data.nodeTypes[name]
+            let node_types: any[] = []
+            switch (type_data.type) {
+                case "instance": {
+                    node_types = this._buildInstanceNodeTypes(
+                        type_data.node_type_name,
+                        type_data.target_type,
+                        type_data.target_value)
+                } break
+                case "combine":
+                case "function": {
+                    node_types = this._buildCommonNodeTypes(
+                        type_data.node_type_name,
+                        type_data.in_ports,
+                        type_data.type)
+
+                } break
+            }
+            this._addNodeTypes(node_types)
+        }
+    }
+
+    private _onResize() {
+        let left = "0px"
+        let width = "100%"
+        if (this._showOutputArea) {
+            if (this._outputArea) {
+                this._outputArea.fit()
+            }
+            const element = this._outputAreaContainerRef.current as unknown as HTMLElement
+            const rect = element.getBoundingClientRect()
+            left = `${rect.width}px`
+            const container = this._containerRef.current as unknown as HTMLDivElement
+            const containerRect = container.getBoundingClientRect()
+            width = `${(containerRect.width - rect.width) / containerRect.width * 100}%`
+        }
+
+        // 设置编辑器的位置和宽度
+        if (this._editorContainerRef && this._editorContainerRef.current) {
+            let editor = this._editorContainerRef.current as unknown as HTMLElement
+            editor.style.left = left
+            editor.style.width = width
         }
+
+        if (this._codeEditor) {
+            this._codeEditor.layout()
+        }
+
+        if (this._codeDiffEditor) {
+            this._codeDiffEditor.layout()
+        }
+    }
+
+    private _onFocusIn() {
+        this.node.setAttribute("data-node-editor-activate", "true")
+        if (this._needLoadData) {
+            this._loadNodes(this._needLoadData.data, this._needLoadData.addRedo)
+            this._needLoadData = null
+        }
+    }
+
+    private _onFocusOut() {
+        this.node.setAttribute("data-node-editor-activate", "false")
+    }
+
+    private async _onCommand(e: CustomEvent) {
+        let fn = this._commandsMap[e.detail]
+        if (!fn) {
+            return
+        }
+        fn()
+    }
+
+
+    private async _tryLoadNodes() {
+        let allNodes = this.getAllNodes()
+        let targetNodes: any = null
+        for (const nodes of Object.values<any>(allNodes)) {
+            if (targetNodes == null) {
+                targetNodes = nodes
+            }
+            if (nodes.default) {
+                targetNodes = nodes
+            }
+        }
+
+        if (targetNodes == null) {
+            return true
+        }
+
+        return await this._loadNodes(targetNodes, false)
     }
 
     private _createCommands() {
         try {
-            this._createCommand("nd-load", "加载", () => {
-                if (this._isDraggableFocus())
-                    this._setMenuOpen(".")
-            })
+            this._createCommand("nd-load", "加载", () => { this._openLoadMenu() })
             this._createCommand("nd-create", "创建", () => this.createNewNodes())
             this._createCommand("nd-delete", "删除", () => this.deleteNodes())
             this._createCommand("nd-rename", "重命名", () => this._renameNodes())
+            this._createCommand("nd-copy", "复制", () => this._copyNodes())
             this._createCommand("nd-run-all-cells", "执行所有的cell", () => this.runAllCells())
-            this._createCommand("nd-clear-run-cache", "清楚运行缓存", () => this._clearRunCache())
+            this._createCommand("nd-clear-run-cache", "清除运行缓存", () => this._clearRunCache())
             this._createCommand("nd-undo", "恢复", () => this.redo(-1))
             this._createCommand("nd-redo", "重做", () => this.redo(1))
             this._createCommand("nd-reset-viewport", "重置视口", () => this._focusToAllNodes())
             this._createCommand("nd-toggle-output-area", "切换输出面板", () => this._toggleOutputArea())
-            this._createCommand("nd-clear-output-area", "清空输出面板", () => {
-                this._clearOutputArea()
-                this._clearCurOutput()
-            })
+            this._createCommand("nd-clear-output-area", "清空输出面板", () => { this._clearOutput() })
             this._createCommand("nd-open-code-editor", "打开编辑器", () => this._openCellEditor())
             this._createCommand("nd-kernel-interrupt", "中断内核", () => this._interuptKernel())
             this._createCommand("nd-kernel-restart", "重启内核", () => this._restartKernel())
             this._createCommand("nd-kernel-change", "更换内核", () => this._selectKernel())
             this._createCommand("nd-select-all", "选中所有节点", () => this._selectAllNodes())
             this._createCommand("nd-delete-selected-nodes", "删除选中的节点", () => this._removeSelectedNodes())
             this._createCommand("nd-copy-selected-nodes", "复制选中的节点", () => this._copySelectedNodes())
             this._createCommand("nd-paste-selected-nodes", "粘贴选中的节点", () => this._pasteSelectedNodes())
             this._createCommand("nd-focus-to-selected-nodes", "聚焦选中的节点", () => this._focusToSelectedNodes())
             this._createCommand("nd-close-image-viewer", "关闭图片浏览器", () => this.setShowImg(false))
-
-            this._createCommand("nd-run-cucrrent-cell", "nd-run-cucrrent-cell(运行当前的Cell)", () => this._editorRun())
-            this._createCommand("nd-insert-cell", "nd-insert-cell(插入Cell)", () => {
-                this.cellInsert(this._curEditingCellIndex)
-                this._editCell(this._curEditingCellIndex)
-            })
-            this._createCommand("nd-delete-cell", "nd-delete-cell(删除Cell)", () => {
-                this.cellRemove(this._curEditingCellIndex)
-                let index = this._curEditingCellIndex - 1
-                if (index < 0) {
-                    index = 0
-                }
-                this._editCell(this._curEditingCellIndex)
-            })
-
-            this._createCommand("nd-cell-undo", "nd-cell-undo(恢复Cell)", () => {
-                this.cellUndo()
-                this._editCell(this._curEditingCellIndex)
-            })
-
-            this._createCommand("nd-cell-redo", "nd-cell-redo(重做Cell)", () => {
-                this.cellRedo()
-                this._editCell(this._curEditingCellIndex)
-            })
-
-            this._createCommand("nd-edit-pre-cell", "nd-edit-pre-cell(编辑上一个Cell)", () => {
-                if (this._codeEditor) {
-                    this._editCell(Math.max(this._curEditingCellIndex - 1, 0))
-                } else if (document.querySelector("[data-show-image-viewer=false][data-show-code-editor=false]")) {
-                    const datas = this._loadNodesFromAllCell()
-                    for (let index = 0; index < datas.length; index++) {
-                        if (this._curNodesId == datas[index].id) {
-                            if (index > 0) {
-                                this._loadNodes(datas[index - 1].data)
-                            }
-                        }
-                    }
-                }
-            })
-
-            this._createCommand("nd-edit-next-cell", "nd-edit-next-cell(编辑下一个Cell)", () => {
-                if (this._codeEditor) {
-                    const cells = this._context.model.cells
-                    this._editCell(Math.min(this._curEditingCellIndex + 1, cells.length - 1))
-                } else if (document.querySelector("[data-show-image-viewer=false][data-show-code-editor=false]")) {
-                    const datas = this._loadNodesFromAllCell()
-                    for (let index = 0; index < datas.length; index++) {
-                        if (this._curNodesId == datas[index].id) {
-                            if (index < datas.length - 1) {
-                                this._loadNodes(datas[index + 1].data)
-                            }
-                        }
-                    }
-                }
-            })
-
-            this._createCommand("nd-set-as-default", "nd-set-as-default(设置为默认)", () => {
-                const curModel = this._getCurNodeCellModel()
-                if (curModel) {
-                    const firstModel = this.cellGet(0)
-                    const temp = curModel.sharedModel.getSource()
-                    curModel.sharedModel.setSource(firstModel.sharedModel.getSource())
-                    firstModel.sharedModel.setSource(temp)
-                    this._curNodesIsDefault = true
-                    this._updateNodesDefaultShow()
-                }
-            })
-
+            this._createCommand("nd-run-cucrrent-cell", "运行当前的Cell", () => this._editorRun())
+            this._createCommand("nd-insert-cell", "插入Cell", () => { this._insertCellToCurrentIndex() })
+            this._createCommand("nd-delete-cell", "删除Cell", () => { this._deleteCurrentCell() })
+            this._createCommand("nd-cell-undo", "恢复Cell", () => { this._undoCell() })
+            this._createCommand("nd-cell-redo", "重做Cell", () => { this._redoCell() })
+            this._createCommand("nd-edit-pre-cell", "编辑上一个Cell", () => { this._editPreCell() })
+            this._createCommand("nd-edit-next-cell", "编辑下一个Cell", () => { this._editNextCell() })
+            this._createCommand("nd-cell-up", "Cell上移", () => { this._CellMove(-1) })
+            this._createCommand("nd-cell-down", "Cell下移", () => { this._CellMove(1) })
+            this._createCommand("nd-set-as-default", "设置为默认", () => { this._setCurrentNodesAsDefault() })
+            this._createCommand("nd-open-comment-color-picker", "打开注释颜色选择器", () => { this._openSelectedCommentsColorPicker() })
+            this._createCommand("nd-combine-selected-nodes", "组合节点", () => { this._combineSelectedNodes() })
+            this._createCommand("nd-separate-selected-node", "拆分节点", () => { this._separateSelectedNode() })
         } catch (error) {
 
         }
     }
 }
 
 const NOTEBOOK_PANEL_TOOLBAR_CLASS = 'jp-NotebookPanel-toolbar';
```

### Comparing `jupyterlab_nodeeditor-1.0.3/src/yesIcon.tsx` & `jupyterlab_nodeeditor-1.0.4/src/yesIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/.gitignore` & `jupyterlab_nodeeditor-1.0.4/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -114,10 +114,8 @@
 
 # End of https://www.gitignore.io/api/python
 
 # OSX files
 .DS_Store
 
 # Yarn cache
-.yarn/
-
-test_ext
+.yarn/
```

### Comparing `jupyterlab_nodeeditor-1.0.3/LICENSE` & `jupyterlab_nodeeditor-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/README.md` & `jupyterlab_nodeeditor-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/pyproject.toml` & `jupyterlab_nodeeditor-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.3/PKG-INFO` & `jupyterlab_nodeeditor-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_nodeeditor
-Version: 1.0.3
+Version: 1.0.4
 Summary: 一个节点编辑器
 Project-URL: Homepage, https://github.com/github_username/jupyterlab_nodeeditor
 Project-URL: Bug Tracker, https://github.com/github_username/jupyterlab_nodeeditor/issues
 Project-URL: Repository, https://github.com/github_username/jupyterlab_nodeeditor.git
 Author-email: l0n0l <cenlan@hotmail.com>
 License: BSD 3-Clause License
```

