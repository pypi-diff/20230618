# Comparing `tmp/pydicom-2.4.0.tar.gz` & `tmp/pydicom-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydicom-2.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pydicom-2.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pydicom-2.4.0.tar` & `pydicom-2.4.1.tar`

### file list

```diff
@@ -1,440 +1,440 @@
--rw-r--r--   0        0        0      588 2023-06-13 16:06:05.695394 pydicom-2.4.0/.circleci/config.yml
--rw-r--r--   0        0        0      114 2023-06-13 16:06:05.695394 pydicom-2.4.0/.codespellrc
--rw-r--r--   0        0        0       58 2023-06-13 16:06:05.695394 pydicom-2.4.0/.coveragerc
--rw-r--r--   0        0        0       18 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      678 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      387 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0        0        0      519 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      195 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/ISSUE_TEMPLATE/other_issues.md
--rw-r--r--   0        0        0     1398 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/ISSUE_TEMPLATE/pixel_issue.md
--rw-r--r--   0        0        0      626 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0       19 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/codespell_ignore_words.txt
--rw-r--r--   0        0        0     3351 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/workflows/merge-pytest.yml
--rw-r--r--   0        0        0      743 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/workflows/merge-typing.yml
--rw-r--r--   0        0        0     5501 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/workflows/pr-pytest.yml
--rw-r--r--   0        0        0      360 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/workflows/pr-run-linters.yml
--rw-r--r--   0        0        0      916 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/workflows/pr-type-spell.yml
--rw-r--r--   0        0        0     1220 2023-06-13 16:06:05.695394 pydicom-2.4.0/.github/workflows/publish-pypi-deploy.yml
--rw-r--r--   0        0        0      714 2023-06-13 16:06:05.695394 pydicom-2.4.0/.gitignore
--rw-r--r--   0        0        0      197 2023-06-13 16:06:05.695394 pydicom-2.4.0/.lgtm.yml
--rw-r--r--   0        0        0       62 2023-06-13 16:06:05.695394 pydicom-2.4.0/.pep8speaks.yml
--rw-r--r--   0        0        0     9179 2023-06-13 16:06:05.695394 pydicom-2.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     3196 2023-06-13 16:06:05.695394 pydicom-2.4.0/LICENSE
--rw-r--r--   0        0        0      163 2023-06-13 16:06:05.695394 pydicom-2.4.0/MANIFEST.in
--rw-r--r--   0        0        0      684 2023-06-13 16:06:05.695394 pydicom-2.4.0/Makefile
--rw-r--r--   0        0        0     6055 2023-06-13 16:06:05.695394 pydicom-2.4.0/README.md
--rw-r--r--   0        0        0     2488 2023-06-13 16:06:05.695394 pydicom-2.4.0/asv.conf.json
--rw-r--r--   0        0        0        0 2023-06-13 16:06:05.695394 pydicom-2.4.0/benchmarks/__init__.py
--rw-r--r--   0        0        0     2962 2023-06-13 16:06:05.695394 pydicom-2.4.0/benchmarks/bench_encaps.py
--rw-r--r--   0        0        0     7943 2023-06-13 16:06:05.695394 pydicom-2.4.0/benchmarks/bench_handler_numpy.py
--rw-r--r--   0        0        0     2989 2023-06-13 16:06:05.695394 pydicom-2.4.0/benchmarks/bench_nested_seq.py
--rw-r--r--   0        0        0     2080 2023-06-13 16:06:05.695394 pydicom-2.4.0/benchmarks/bench_pixel_util.py
--rw-r--r--   0        0        0     4160 2023-06-13 16:06:05.695394 pydicom-2.4.0/benchmarks/bench_rle_decode.py
--rw-r--r--   0        0        0     3310 2023-06-13 16:06:05.695394 pydicom-2.4.0/benchmarks/bench_rle_encode.py
--rwxr-xr-x   0        0        0     3049 2023-06-13 16:06:05.695394 pydicom-2.4.0/build_tools/circle/build_doc.sh
--rwxr-xr-x   0        0        0     3520 2023-06-13 16:06:05.695394 pydicom-2.4.0/build_tools/circle/push_doc.sh
--rw-r--r--   0        0        0     2811 2023-06-13 16:06:05.695394 pydicom-2.4.0/build_tools/sphinx/github_link.py
--rw-r--r--   0        0        0      466 2023-06-13 16:06:05.695394 pydicom-2.4.0/dicom.py
--rw-r--r--   0        0        0     7153 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/Makefile
--rw-r--r--   0        0        0     1209 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/README.md
--rw-r--r--   0        0        0     1751 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/_static/css/pydicom.css
--rw-r--r--   0        0        0      290 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/_templates/class.rst
--rw-r--r--   0        0        0      229 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/_templates/function.rst
--rw-r--r--   0        0        0     1150 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/assets/img/favicon.ico
--rw-r--r--   0        0        0     5693 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/assets/img/logo.png
--rw-r--r--   0        0        0    33703 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/assets/img/pydicom_blue_light.png
--rw-r--r--   0        0        0    12643 2023-06-13 16:06:05.695394 pydicom-2.4.0/doc/assets/img/pydicom_blue_light.svg
--rw-r--r--   0        0        0    33283 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/assets/img/pydicom_flat_black.png
--rw-r--r--   0        0        0    12173 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/assets/img/pydicom_flat_black.svg
--rw-r--r--   0        0        0    29209 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/assets/img/pydicom_flat_black_alpha.png
--rw-r--r--   0        0        0    10529 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/conf.py
--rw-r--r--   0        0        0     3262 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/faq/index.rst
--rw-r--r--   0        0        0     5015 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/cli/cli_codify.rst
--rw-r--r--   0        0        0     2886 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/cli/cli_dev.rst
--rw-r--r--   0        0        0      410 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/cli/cli_guide.rst
--rw-r--r--   0        0        0     7729 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/cli/cli_intro.rst
--rw-r--r--   0        0        0     5852 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/cli/cli_show.rst
--rw-r--r--   0        0        0    11425 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/element_value_types.rst
--rw-r--r--   0        0        0     1932 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/encoding/encoder_plugin_options.rst
--rw-r--r--   0        0        0     5137 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/encoding/encoder_plugins.rst
--rw-r--r--   0        0        0      270 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/encoding/index.rst
--rw-r--r--   0        0        0     7283 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/encoding/rle_lossless.rst
--rw-r--r--   0        0        0     5283 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/glossary.rst
--rw-r--r--   0        0        0      245 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/index.rst
--rw-r--r--   0        0        0     3998 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/guides/writing_documentation.rst
--rw-r--r--   0        0        0     1742 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/index.rst
--rw-r--r--   0        0        0     3073 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/make.bat
--rw-r--r--   0        0        0    11081 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/base_element.rst
--rw-r--r--   0        0        0     4599 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/best_practices.rst
--rw-r--r--   0        0        0     2854 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/getting_started.rst
--rw-r--r--   0        0        0     5612 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/image_data_compression.rst
--rw-r--r--   0        0        0     7357 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/image_data_handlers.rst
--rw-r--r--   0        0        0     5176 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/private_data_elements.rst
--rw-r--r--   0        0        0      337 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/pydicom_user_guide.rst
--rw-r--r--   0        0        0      524 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/python2_support.rst
--rw-r--r--   0        0        0     1090 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/ref_guide.rst
--rw-r--r--   0        0        0     5049 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/transition_to_pydicom1.rst
--rw-r--r--   0        0        0     2644 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/viewing_images.rst
--rw-r--r--   0        0        0     3614 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/working_with_overlays.rst
--rw-r--r--   0        0        0     8221 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/working_with_pixel_data.rst
--rw-r--r--   0        0        0     3235 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/working_with_waveforms.rst
--rw-r--r--   0        0        0     3779 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/old/writing_files.rst
--rw-r--r--   0        0        0      327 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/charset.rst
--rw-r--r--   0        0        0      774 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/config.rst
--rw-r--r--   0        0        0      314 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/data.rst
--rw-r--r--   0        0        0      802 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/datadict.rst
--rw-r--r--   0        0        0      341 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/dataset.rst
--rw-r--r--   0        0        0      233 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/dicomdir.rst
--rw-r--r--   0        0        0      280 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/elem.dataelem.rst
--rw-r--r--   0        0        0      301 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/elem.multival.rst
--rw-r--r--   0        0        0      224 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/elem.rst
--rw-r--r--   0        0        0      335 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/elem.sequence.rst
--rw-r--r--   0        0        0      267 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/elem.tag.rst
--rw-r--r--   0        0        0      495 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/elem.valuerep.rst
--rw-r--r--   0        0        0      589 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/elem.values.rst
--rw-r--r--   0        0        0      723 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/encaps.rst
--rw-r--r--   0        0        0      574 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/encoders.rst
--rw-r--r--   0        0        0      186 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/errors.rst
--rw-r--r--   0        0        0      275 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/fileio.base.rst
--rw-r--r--   0        0        0      480 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/fileio.read.rst
--rw-r--r--   0        0        0      221 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/fileio.rst
--rw-r--r--   0        0        0      331 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/fileio.util.rst
--rw-r--r--   0        0        0      632 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/fileio.write.rst
--rw-r--r--   0        0        0      325 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/fileset.rst
--rw-r--r--   0        0        0      285 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/handlers.overlay_data.rst
--rw-r--r--   0        0        0      398 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/handlers.pixel_data.rst
--rw-r--r--   0        0        0      615 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/handlers.rst
--rw-r--r--   0        0        0      276 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/handlers.waveform_data.rst
--rw-r--r--   0        0        0      399 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/index.rst
--rw-r--r--   0        0        0      218 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/misc.rst
--rw-r--r--   0        0        0     7525 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/reference/uid.rst
--rw-r--r--   0        0        0      523 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/index.rst
--rw-r--r--   0        0        0     1959 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v0.9.2.rst
--rw-r--r--   0        0        0     1625 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v0.9.3.rst
--rw-r--r--   0        0        0     3132 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v0.9.4.rst
--rw-r--r--   0        0        0     1320 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v0.9.5.rst
--rw-r--r--   0        0        0      708 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v0.9.6.rst
--rw-r--r--   0        0        0     2522 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v0.9.7.rst
--rw-r--r--   0        0        0     1736 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v0.9.8.rst
--rw-r--r--   0        0        0     1261 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v0.9.9.rst
--rw-r--r--   0        0        0     3448 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v1.0.0.rst
--rw-r--r--   0        0        0     2043 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v1.1.0.rst
--rw-r--r--   0        0        0     3570 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v1.2.0.rst
--rw-r--r--   0        0        0     3069 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v1.3.0.rst
--rw-r--r--   0        0        0     4371 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v1.4.0.rst
--rw-r--r--   0        0        0      358 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v1.4.1.rst
--rw-r--r--   0        0        0     2806 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v2.0.0.rst
--rw-r--r--   0        0        0     7542 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v2.1.0.rst
--rw-r--r--   0        0        0      219 2023-06-13 16:06:05.699394 pydicom-2.4.0/doc/release_notes/v2.1.1.rst
--rw-r--r--   0        0        0     6511 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/release_notes/v2.2.0.rst
--rw-r--r--   0        0        0     2893 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/release_notes/v2.3.0.rst
--rw-r--r--   0        0        0     2155 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/release_notes/v2.4.0.rst
--rw-r--r--   0        0        0     1081 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/contributing.rst
--rw-r--r--   0        0        0    10607 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/contributing_code.rst
--rw-r--r--   0        0        0     9568 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/contributing_docs.rst
--rw-r--r--   0        0        0    22994 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/dataset_basics.rst
--rw-r--r--   0        0        0     4390 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/dicom_json.rst
--rw-r--r--   0        0        0    19523 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/filesets.rst
--rw-r--r--   0        0        0      311 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/index.rst
--rw-r--r--   0        0        0     5487 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/installation.rst
--rw-r--r--   0        0        0     7747 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/pixel_data/compressing.rst
--rw-r--r--   0        0        0     2153 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/sr_basics.rst
--rw-r--r--   0        0        0     9581 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/virtualenvs.rst
--rw-r--r--   0        0        0     9195 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/waveforms.rst
--rw-r--r--   0        0        0   135332 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/waveforms_assets/waveforms_decode.png
--rw-r--r--   0        0        0    90122 2023-06-13 16:06:05.703394 pydicom-2.4.0/doc/tutorials/waveforms_assets/waveforms_encode.png
--rw-r--r--   0        0        0       77 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/README.txt
--rw-r--r--   0        0        0     3481 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/dicomtree.py
--rw-r--r--   0        0        0      173 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/image_processing/README.txt
--rw-r--r--   0        0        0     1377 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/image_processing/plot_downsize_image.py
--rw-r--r--   0        0        0     1541 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/image_processing/plot_waveforms.py
--rw-r--r--   0        0        0     2126 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/image_processing/reslice.py
--rw-r--r--   0        0        0      119 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/input_output/README.txt
--rw-r--r--   0        0        0     1563 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/input_output/plot_printing_dataset.py
--rw-r--r--   0        0        0     1165 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/input_output/plot_read_dicom.py
--rw-r--r--   0        0        0     2794 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/input_output/plot_read_dicom_directory.py
--rw-r--r--   0        0        0     4465 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/input_output/plot_read_fileset.py
--rw-r--r--   0        0        0     1123 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/input_output/plot_read_rtplan.py
--rw-r--r--   0        0        0     2401 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/input_output/plot_write_dicom.py
--rw-r--r--   0        0        0     2392 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/memory_dataset.py
--rw-r--r--   0        0        0      177 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/metadata_processing/README.txt
--rw-r--r--   0        0        0     1410 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/metadata_processing/plot_add_dict_entries.py
--rw-r--r--   0        0        0     2787 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/metadata_processing/plot_anonymize.py
--rw-r--r--   0        0        0     1071 2023-06-13 16:06:05.703394 pydicom-2.4.0/examples/metadata_processing/plot_sequences.py
--rw-r--r--   0        0        0     1033 2023-06-13 16:06:05.707394 pydicom-2.4.0/examples/plot_dicom_difference.py
--rw-r--r--   0        0        0     1286 2023-06-13 16:06:05.707394 pydicom-2.4.0/examples/show_charset_name.py
--rw-r--r--   0        0        0      330 2023-06-13 16:06:05.707394 pydicom-2.4.0/mypy.ini
--rw-r--r--   0        0        0     1577 2023-06-13 16:06:05.707394 pydicom-2.4.0/pydicom/__init__.py
--rw-r--r--   0        0        0   509435 2023-06-13 16:06:05.707394 pydicom-2.4.0/pydicom/_dicom_dict.py
--rw-r--r--   0        0        0   613172 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/_private_dict.py
--rw-r--r--   0        0        0      130 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/_storage_sopclass_uids.py
--rw-r--r--   0        0        0    65890 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/_uid_dict.py
--rw-r--r--   0        0        0      379 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/_version.py
--rw-r--r--   0        0        0    31107 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/charset.py
--rw-r--r--   0        0        0        0 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/cli/__init__.py
--rw-r--r--   0        0        0     1001 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/cli/codify.py
--rw-r--r--   0        0        0     7670 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/cli/main.py
--rw-r--r--   0        0        0     5323 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/cli/show.py
--rw-r--r--   0        0        0      607 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/compat.py
--rw-r--r--   0        0        0    18738 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/config.py
--rw-r--r--   0        0        0      403 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/__init__.py
--rw-r--r--   0        0        0     1896 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/FileInfo.txt
--rw-r--r--   0        0        0     1892 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrArab.dcm
--rw-r--r--   0        0        0     1890 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrFren.dcm
--rw-r--r--   0        0        0     1938 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrFrenMulti.dcm
--rw-r--r--   0        0        0     1894 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrGerm.dcm
--rw-r--r--   0        0        0     1890 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrGreek.dcm
--rw-r--r--   0        0        0     1950 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrH31.dcm
--rw-r--r--   0        0        0     1960 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrH32.dcm
--rw-r--r--   0        0        0     1890 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrHbrw.dcm
--rw-r--r--   0        0        0     1934 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrI2.dcm
--rw-r--r--   0        0        0     1918 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrJapMulti.dcm
--rw-r--r--   0        0        0     1940 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrJapMultiExplicitIR6.dcm
--rw-r--r--   0        0        0     1898 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrKoreanMulti.dcm
--rw-r--r--   0        0        0     1890 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrRuss.dcm
--rw-r--r--   0        0        0      520 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrSQEncoding.dcm
--rw-r--r--   0        0        0      520 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrSQEncoding1.dcm
--rw-r--r--   0        0        0     1910 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrX1.dcm
--rw-r--r--   0        0        0     1904 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/charset_files/chrX2.dcm
--rw-r--r--   0        0        0    11895 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/data_manager.py
--rw-r--r--   0        0        0     8205 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/download.py
--rw-r--r--   0        0        0     6297 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/hashes.json
--rw-r--r--   0        0        0     1725 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/palettes/README.md
--rw-r--r--   0        0        0     4078 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/palettes/fall.dcm
--rw-r--r--   0        0        0     4754 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/palettes/hotiron.dcm
--rw-r--r--   0        0        0     4776 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/palettes/hotmetalblue.dcm
--rw-r--r--   0        0        0     4732 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/palettes/pet.dcm
--rw-r--r--   0        0        0     4790 2023-06-13 16:06:05.711394 pydicom-2.4.0/pydicom/data/palettes/pet20step.dcm
--rw-r--r--   0        0        0     4104 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/palettes/spring.dcm
--rw-r--r--   0        0        0     4100 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/palettes/summer.dcm
--rw-r--r--   0        0        0     4112 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/palettes/winter.dcm
--rw-r--r--   0        0        0     2057 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/retry.py
--rw-r--r--   0        0        0     3590 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/693_J2KI.dcm
--rw-r--r--   0        0        0    39206 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/CT_small.dcm
--rw-r--r--   0        0        0    15412 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/ExplVR_BigEnd.dcm
--rw-r--r--   0        0        0      434 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/ExplVR_BigEndNoMeta.dcm
--rw-r--r--   0        0        0      434 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/ExplVR_LitEndNoMeta.dcm
--rw-r--r--   0        0        0    30706 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/GDCMJ2K_TextGBR.dcm
--rw-r--r--   0        0        0   138518 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/J2K_pixelrep_mismatch.dcm
--rw-r--r--   0        0        0     9844 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/JPEG-lossy.dcm
--rw-r--r--   0        0        0     3308 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/JPEG2000-embedded-sequence-delimiter.dcm
--rw-r--r--   0        0        0     3308 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/JPEG2000.dcm
--rw-r--r--   0        0        0     9844 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/JPGExtended.dcm
--rw-r--r--   0        0        0     9830 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_small.dcm
--rw-r--r--   0        0        0     7790 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_small_RLE.dcm
--rw-r--r--   0        0        0     9708 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_small_bigendian.dcm
--rw-r--r--   0        0        0     9846 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_small_expb.dcm
--rw-r--r--   0        0        0     9702 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_small_implicit.dcm
--rw-r--r--   0        0        0     6008 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_small_jp2klossless.dcm
--rw-r--r--   0        0        0     6124 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_small_jpeg_ls_lossless.dcm
--rw-r--r--   0        0        0     9958 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_small_padded.dcm
--rw-r--r--   0        0        0     9630 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/MR_truncated.dcm
--rw-r--r--   0        0        0    15439 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/README.txt
--rw-r--r--   0        0        0     4316 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_jpeg_no_color_transform.dcm
--rw-r--r--   0        0        0     4310 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_jpeg_no_color_transform_2.dcm
--rw-r--r--   0        0        0     3626 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cr.dcm
--rw-r--r--   0        0        0     3136 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+n1.dcm
--rw-r--r--   0        0        0     3090 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+n2.dcm
--rw-r--r--   0        0        0     3140 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+np.dcm
--rw-r--r--   0        0        0     3094 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+s2.dcm
--rw-r--r--   0        0        0     3420 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+s4.dcm
--rw-r--r--   0        0        0     2998 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_gdcm_KY.dcm
--rw-r--r--   0        0        0     4464 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg.dcm
--rw-r--r--   0        0        0     4310 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_app14_dcmd.dcm
--rw-r--r--   0        0        0   197506 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_dcmd.dcm
--rw-r--r--   0        0        0     3424 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_dcmtk.dcm
--rw-r--r--   0        0        0     5204 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_gdcm.dcm
--rw-r--r--   0        0        0     5042 2023-06-13 16:06:05.715394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_lossy_gdcm.dcm
--rw-r--r--   0        0        0     2006 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle.dcm
--rw-r--r--   0        0        0     2606 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_16bit.dcm
--rw-r--r--   0        0        0     3896 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_16bit_2frame.dcm
--rw-r--r--   0        0        0     2696 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_2frame.dcm
--rw-r--r--   0        0        0     3760 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_32bit.dcm
--rw-r--r--   0        0        0     6246 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_32bit_2frame.dcm
--rw-r--r--   0        0        0     1444 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_small_odd.dcm
--rw-r--r--   0        0        0     1444 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_small_odd_big_endian.dcm
--rw-r--r--   0        0        0     2044 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_rgb_small_odd_jpeg.dcm
--rw-r--r--   0        0        0    21686 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/SC_ybr_full_422_uncompressed.dcm
--rw-r--r--   0        0        0      674 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/UN_sequence.dcm
--rw-r--r--   0        0        0     7618 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/badVR.dcm
--rw-r--r--   0        0        0     2300 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CR1/6154
--rw-r--r--   0        0        0     2298 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CR2/6247
--rw-r--r--   0        0        0     2298 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CR3/6278
--rw-r--r--   0        0        0     3810 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CT2/17106
--rw-r--r--   0        0        0     3812 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CT2/17136
--rw-r--r--   0        0        0     3812 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CT2/17166
--rw-r--r--   0        0        0     3812 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CT2/17196
--rw-r--r--   0        0        0     3920 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT2N/6293
--rw-r--r--   0        0        0     3908 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT2N/6924
--rw-r--r--   0        0        0     3936 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2062
--rw-r--r--   0        0        0     3936 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2392
--rw-r--r--   0        0        0     3936 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2693
--rw-r--r--   0        0        0     3936 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/3023
--rw-r--r--   0        0        0     3938 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/3353
--rw-r--r--   0        0        0     2336 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR1/15820
--rw-r--r--   0        0        0     2336 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR1/4919
--rw-r--r--   0        0        0     2330 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR1/5641
--rw-r--r--   0        0        0     2336 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/15970
--rw-r--r--   0        0        0     2356 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/4950
--rw-r--r--   0        0        0     2354 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/4981
--rw-r--r--   0        0        0     2354 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/5011
--rw-r--r--   0        0        0     2348 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/6273
--rw-r--r--   0        0        0     2348 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/6605
--rw-r--r--   0        0        0     2350 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/6935
--rw-r--r--   0        0        0     2350 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4467
--rw-r--r--   0        0        0     2348 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4528
--rw-r--r--   0        0        0     2348 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4558
--rw-r--r--   0        0        0     2350 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4588
--rw-r--r--   0        0        0     2350 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4618
--rw-r--r--   0        0        0     2350 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4648
--rw-r--r--   0        0        0     2350 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4678
--rw-r--r--   0        0        0    11116 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR
--rw-r--r--   0        0        0    11116 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-bigEnd
--rw-r--r--   0        0        0      396 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-empty.dcm
--rw-r--r--   0        0        0    11110 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-implicit
--rw-r--r--   0        0        0    11092 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-nooffset
--rw-r--r--   0        0        0    11116 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-nopatient
--rw-r--r--   0        0        0    11116 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-reordered
--rw-r--r--   0        0        0      719 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/README.txt
--rw-r--r--   0        0        0    13066 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/DICOMDIR
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000000
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000001
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000002
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000003
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000004
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000005
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000006
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000007
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000008
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000009
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000A
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000B
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000C
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000D
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000E
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000F
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.719394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000G
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000H
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000I
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000J
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000K
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000L
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000M
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000N
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000O
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000P
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Q
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000R
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000S
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000T
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000U
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000V
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000W
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000X
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Y
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Z
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000010
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000011
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000012
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000013
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000014
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000015
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000016
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000017
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000018
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000019
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001A
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001B
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001C
--rw-r--r--   0        0        0      740 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001D
--rw-r--r--   0        0        0     1206 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/README
--rw-r--r--   0        0        0      276 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/empty_charset_LEI.dcm
--rw-r--r--   0        0        0     4637 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/image_dfl.dcm
--rw-r--r--   0        0        0    37084 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/liver_1frame.dcm
--rw-r--r--   0        0        0    36532 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/liver_expb_1frame.dcm
--rw-r--r--   0        0        0      317 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/meta_missing_tsyntax.dcm
--rw-r--r--   0        0        0      343 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/nested_priv_SQ.dcm
--rw-r--r--   0        0        0    38871 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/no_meta.dcm
--rw-r--r--   0        0        0      408 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/no_meta_group_length.dcm
--rw-r--r--   0        0        0      546 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/priv_SQ.dcm
--rw-r--r--   0        0        0     2968 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/reportsi.dcm
--rw-r--r--   0        0        0     2700 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/reportsi_with_empty_number_tags.dcm
--rw-r--r--   0        0        0     7568 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtdose.dcm
--rwxr-xr-x   0        0        0     1958 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtdose_1frame.dcm
--rw-r--r--   0        0        0     7618 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtdose_expb.dcm
--rw-r--r--   0        0        0     2008 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtdose_expb_1frame.dcm
--rw-r--r--   0        0        0     6816 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtdose_rle.dcm
--rw-r--r--   0        0        0     2122 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtdose_rle_1frame.dcm
--rw-r--r--   0        0        0     2672 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtplan.dcm
--rw-r--r--   0        0        0    14474 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtplan.dump
--rw-r--r--   0        0        0     2129 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtplan_truncated.dcm
--rw-r--r--   0        0        0     2534 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtstruct.dcm
--rw-r--r--   0        0        0     7935 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/rtstruct.dump
--rw-r--r--   0        0        0     6796 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/test-SR.dcm
--rw-r--r--   0        0        0    20965 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/test1.json
--rw-r--r--   0        0        0     1841 2023-06-13 16:06:05.723394 pydicom-2.4.0/pydicom/data/test_files/test_PN.json
--rwxr-xr-x   0        0        0   291088 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/data/test_files/waveform_ecg.dcm
--rw-r--r--   0        0        0     6958 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/data/test_files/zipMR.gz
--rw-r--r--   0        0        0     9485 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/data/urls.json
--rw-r--r--   0        0        0    18650 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/datadict.py
--rw-r--r--   0        0        0    31098 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/dataelem.py
--rw-r--r--   0        0        0   109590 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/dataset.py
--rw-r--r--   0        0        0     5676 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/dicomdir.py
--rw-r--r--   0        0        0      403 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/dicomio.py
--rw-r--r--   0        0        0    26824 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/encaps.py
--rw-r--r--   0        0        0       66 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/encoders/__init__.py
--rw-r--r--   0        0        0    36135 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/encoders/base.py
--rw-r--r--   0        0        0     5901 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/encoders/gdcm.py
--rw-r--r--   0        0        0     5374 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/encoders/native.py
--rw-r--r--   0        0        0     1125 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/encoders/pylibjpeg.py
--rw-r--r--   0        0        0     1714 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/env_info.py
--rw-r--r--   0        0        0      771 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/errors.py
--rw-r--r--   0        0        0     7794 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/filebase.py
--rw-r--r--   0        0        0    44662 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/filereader.py
--rw-r--r--   0        0        0   102357 2023-06-13 16:06:05.727394 pydicom-2.4.0/pydicom/fileset.py
--rw-r--r--   0        0        0    14625 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/fileutil.py
--rw-r--r--   0        0        0    44151 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/filewriter.py
--rw-r--r--   0        0        0    12252 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/jsonrep.py
--rw-r--r--   0        0        0     1644 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/misc.py
--rw-r--r--   0        0        0     5140 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/multival.py
--rw-r--r--   0        0        0      108 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/overlay_data_handlers/__init__.py
--rw-r--r--   0        0        0       61 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/overlays/__init__.py
--rw-r--r--   0        0        0     9951 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/overlays/numpy_handler.py
--rw-r--r--   0        0        0      262 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/pixel_data_handlers/__init__.py
--rw-r--r--   0        0        0     9761 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/pixel_data_handlers/gdcm_handler.py
--rw-r--r--   0        0        0     3396 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/pixel_data_handlers/jpeg_ls_handler.py
--rw-r--r--   0        0        0    12284 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/pixel_data_handlers/numpy_handler.py
--rw-r--r--   0        0        0     8695 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/pixel_data_handlers/pillow_handler.py
--rw-r--r--   0        0        0    11053 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/pixel_data_handlers/pylibjpeg_handler.py
--rw-r--r--   0        0        0    16581 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/pixel_data_handlers/rle_handler.py
--rw-r--r--   0        0        0    54722 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/pixel_data_handlers/util.py
--rw-r--r--   0        0        0        0 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/py.typed
--rw-r--r--   0        0        0     7573 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/sequence.py
--rw-r--r--   0        0        0       38 2023-06-13 16:06:05.731394 pydicom-2.4.0/pydicom/sr/__init__.py
--rw-r--r--   0        0        0   788696 2023-06-13 16:06:05.735394 pydicom-2.4.0/pydicom/sr/_cid_dict.py
--rw-r--r--   0        0        0  2725654 2023-06-13 16:06:05.747394 pydicom-2.4.0/pydicom/sr/_concepts_dict.py
--rw-r--r--   0        0        0   424515 2023-06-13 16:06:05.751395 pydicom-2.4.0/pydicom/sr/_snomed_dict.py
--rw-r--r--   0        0        0    11035 2023-06-13 16:06:05.751395 pydicom-2.4.0/pydicom/sr/codedict.py
--rw-r--r--   0        0        0     2026 2023-06-13 16:06:05.751395 pydicom-2.4.0/pydicom/sr/coding.py
--rw-r--r--   0        0        0     8541 2023-06-13 16:06:05.751395 pydicom-2.4.0/pydicom/tag.py
--rw-r--r--   0        0        0    34984 2023-06-13 16:06:05.755395 pydicom-2.4.0/pydicom/uid.py
--rw-r--r--   0        0        0        0 2023-06-13 16:06:05.755395 pydicom-2.4.0/pydicom/util/__init__.py
--rw-r--r--   0        0        0    17459 2023-06-13 16:06:05.755395 pydicom-2.4.0/pydicom/util/codify.py
--rw-r--r--   0        0        0     3956 2023-06-13 16:06:05.755395 pydicom-2.4.0/pydicom/util/dump.py
--rw-r--r--   0        0        0     4259 2023-06-13 16:06:05.755395 pydicom-2.4.0/pydicom/util/fixer.py
--rw-r--r--   0        0        0     1576 2023-06-13 16:06:05.755395 pydicom-2.4.0/pydicom/util/hexutil.py
--rw-r--r--   0        0        0     6465 2023-06-13 16:06:05.755395 pydicom-2.4.0/pydicom/util/leanread.py
--rw-r--r--   0        0        0    73466 2023-06-13 16:06:05.759395 pydicom-2.4.0/pydicom/valuerep.py
--rw-r--r--   0        0        0    26630 2023-06-13 16:06:05.759395 pydicom-2.4.0/pydicom/values.py
--rw-r--r--   0        0        0       88 2023-06-13 16:06:05.759395 pydicom-2.4.0/pydicom/waveforms/__init__.py
--rw-r--r--   0        0        0     8580 2023-06-13 16:06:05.759395 pydicom-2.4.0/pydicom/waveforms/numpy_handler.py
--rw-r--r--   0        0        0     2829 2023-06-13 16:06:05.759395 pydicom-2.4.0/pyproject.toml
--rw-r--r--   0        0        0       48 2023-06-13 16:06:05.759395 pydicom-2.4.0/setup.cfg
--rw-r--r--   0        0        0     2744 2023-06-13 16:06:05.759395 pydicom-2.4.0/setup.py
--rwxr-xr-x   0        0        0    14008 2023-06-13 16:06:05.759395 pydicom-2.4.0/source/generate_cids/generate_concept_dicts.py
--rwxr-xr-x   0        0        0    11894 2023-06-13 16:06:05.759395 pydicom-2.4.0/source/generate_dict/generate_dicom_dict.py
--rwxr-xr-x   0        0        0     3769 2023-06-13 16:06:05.759395 pydicom-2.4.0/source/generate_dict/generate_private_dict.py
--rwxr-xr-x   0        0        0     7710 2023-06-13 16:06:05.759395 pydicom-2.4.0/source/generate_dict/generate_uid_dict.py
--rwxr-xr-x   0        0        0     2450 2023-06-13 16:06:05.759395 pydicom-2.4.0/source/generate_uids/generate_storage_sopclass_uids.py
--rw-r--r--   0        0        0     1708 2023-06-13 16:06:05.759395 pydicom-2.4.0/source/scripts/charlist.py
--rw-r--r--   0        0        0     7808 1970-01-01 00:00:00.000000 pydicom-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0      588 2023-06-18 21:37:24.962689 pydicom-2.4.1/.circleci/config.yml
+-rw-r--r--   0        0        0      114 2023-06-18 21:37:24.962689 pydicom-2.4.1/.codespellrc
+-rw-r--r--   0        0        0       58 2023-06-18 21:37:24.962689 pydicom-2.4.1/.coveragerc
+-rw-r--r--   0        0        0       18 2023-06-18 21:37:24.962689 pydicom-2.4.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      678 2023-06-18 21:37:24.962689 pydicom-2.4.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      387 2023-06-18 21:37:24.962689 pydicom-2.4.1/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0        0        0      519 2023-06-18 21:37:24.962689 pydicom-2.4.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      195 2023-06-18 21:37:24.962689 pydicom-2.4.1/.github/ISSUE_TEMPLATE/other_issues.md
+-rw-r--r--   0        0        0     1398 2023-06-18 21:37:24.962689 pydicom-2.4.1/.github/ISSUE_TEMPLATE/pixel_issue.md
+-rw-r--r--   0        0        0      626 2023-06-18 21:37:24.962689 pydicom-2.4.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0       19 2023-06-18 21:37:24.962689 pydicom-2.4.1/.github/codespell_ignore_words.txt
+-rw-r--r--   0        0        0     3351 2023-06-18 21:37:24.962689 pydicom-2.4.1/.github/workflows/merge-pytest.yml
+-rw-r--r--   0        0        0      743 2023-06-18 21:37:24.962689 pydicom-2.4.1/.github/workflows/merge-typing.yml
+-rw-r--r--   0        0        0     5501 2023-06-18 21:37:24.962689 pydicom-2.4.1/.github/workflows/pr-pytest.yml
+-rw-r--r--   0        0        0      360 2023-06-18 21:37:24.962689 pydicom-2.4.1/.github/workflows/pr-run-linters.yml
+-rw-r--r--   0        0        0      916 2023-06-18 21:37:24.962689 pydicom-2.4.1/.github/workflows/pr-type-spell.yml
+-rw-r--r--   0        0        0     1220 2023-06-18 21:37:24.962689 pydicom-2.4.1/.github/workflows/publish-pypi-deploy.yml
+-rw-r--r--   0        0        0      714 2023-06-18 21:37:24.962689 pydicom-2.4.1/.gitignore
+-rw-r--r--   0        0        0      197 2023-06-18 21:37:24.962689 pydicom-2.4.1/.lgtm.yml
+-rw-r--r--   0        0        0       62 2023-06-18 21:37:24.962689 pydicom-2.4.1/.pep8speaks.yml
+-rw-r--r--   0        0        0     9179 2023-06-18 21:37:24.962689 pydicom-2.4.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     3196 2023-06-18 21:37:24.962689 pydicom-2.4.1/LICENSE
+-rw-r--r--   0        0        0      163 2023-06-18 21:37:24.962689 pydicom-2.4.1/MANIFEST.in
+-rw-r--r--   0        0        0      684 2023-06-18 21:37:24.962689 pydicom-2.4.1/Makefile
+-rw-r--r--   0        0        0     6055 2023-06-18 21:37:24.962689 pydicom-2.4.1/README.md
+-rw-r--r--   0        0        0     2488 2023-06-18 21:37:24.962689 pydicom-2.4.1/asv.conf.json
+-rw-r--r--   0        0        0        0 2023-06-18 21:37:24.962689 pydicom-2.4.1/benchmarks/__init__.py
+-rw-r--r--   0        0        0     2962 2023-06-18 21:37:24.962689 pydicom-2.4.1/benchmarks/bench_encaps.py
+-rw-r--r--   0        0        0     7943 2023-06-18 21:37:24.962689 pydicom-2.4.1/benchmarks/bench_handler_numpy.py
+-rw-r--r--   0        0        0     2989 2023-06-18 21:37:24.962689 pydicom-2.4.1/benchmarks/bench_nested_seq.py
+-rw-r--r--   0        0        0     2080 2023-06-18 21:37:24.962689 pydicom-2.4.1/benchmarks/bench_pixel_util.py
+-rw-r--r--   0        0        0     4160 2023-06-18 21:37:24.962689 pydicom-2.4.1/benchmarks/bench_rle_decode.py
+-rw-r--r--   0        0        0     3310 2023-06-18 21:37:24.962689 pydicom-2.4.1/benchmarks/bench_rle_encode.py
+-rwxr-xr-x   0        0        0     3049 2023-06-18 21:37:24.962689 pydicom-2.4.1/build_tools/circle/build_doc.sh
+-rwxr-xr-x   0        0        0     3520 2023-06-18 21:37:24.962689 pydicom-2.4.1/build_tools/circle/push_doc.sh
+-rw-r--r--   0        0        0     2811 2023-06-18 21:37:24.962689 pydicom-2.4.1/build_tools/sphinx/github_link.py
+-rw-r--r--   0        0        0      466 2023-06-18 21:37:24.962689 pydicom-2.4.1/dicom.py
+-rw-r--r--   0        0        0     7153 2023-06-18 21:37:24.962689 pydicom-2.4.1/doc/Makefile
+-rw-r--r--   0        0        0     1209 2023-06-18 21:37:24.962689 pydicom-2.4.1/doc/README.md
+-rw-r--r--   0        0        0     1751 2023-06-18 21:37:24.962689 pydicom-2.4.1/doc/_static/css/pydicom.css
+-rw-r--r--   0        0        0      290 2023-06-18 21:37:24.962689 pydicom-2.4.1/doc/_templates/class.rst
+-rw-r--r--   0        0        0      229 2023-06-18 21:37:24.962689 pydicom-2.4.1/doc/_templates/function.rst
+-rw-r--r--   0        0        0     1150 2023-06-18 21:37:24.962689 pydicom-2.4.1/doc/assets/img/favicon.ico
+-rw-r--r--   0        0        0     5693 2023-06-18 21:37:24.962689 pydicom-2.4.1/doc/assets/img/logo.png
+-rw-r--r--   0        0        0    33703 2023-06-18 21:37:24.962689 pydicom-2.4.1/doc/assets/img/pydicom_blue_light.png
+-rw-r--r--   0        0        0    12643 2023-06-18 21:37:24.962689 pydicom-2.4.1/doc/assets/img/pydicom_blue_light.svg
+-rw-r--r--   0        0        0    33283 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/assets/img/pydicom_flat_black.png
+-rw-r--r--   0        0        0    12173 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/assets/img/pydicom_flat_black.svg
+-rw-r--r--   0        0        0    29209 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/assets/img/pydicom_flat_black_alpha.png
+-rw-r--r--   0        0        0    10529 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/conf.py
+-rw-r--r--   0        0        0     3262 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/faq/index.rst
+-rw-r--r--   0        0        0     5015 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/guides/cli/cli_codify.rst
+-rw-r--r--   0        0        0     2886 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/guides/cli/cli_dev.rst
+-rw-r--r--   0        0        0      410 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/guides/cli/cli_guide.rst
+-rw-r--r--   0        0        0     7729 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/guides/cli/cli_intro.rst
+-rw-r--r--   0        0        0     5852 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/guides/cli/cli_show.rst
+-rw-r--r--   0        0        0    11425 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/guides/element_value_types.rst
+-rw-r--r--   0        0        0     1932 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/guides/encoding/encoder_plugin_options.rst
+-rw-r--r--   0        0        0     5137 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/guides/encoding/encoder_plugins.rst
+-rw-r--r--   0        0        0      270 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/guides/encoding/index.rst
+-rw-r--r--   0        0        0     7283 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/guides/encoding/rle_lossless.rst
+-rw-r--r--   0        0        0     5283 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/guides/glossary.rst
+-rw-r--r--   0        0        0      245 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/guides/index.rst
+-rw-r--r--   0        0        0     3998 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/guides/writing_documentation.rst
+-rw-r--r--   0        0        0     1742 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/index.rst
+-rw-r--r--   0        0        0     3073 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/make.bat
+-rw-r--r--   0        0        0    11081 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/old/base_element.rst
+-rw-r--r--   0        0        0     4599 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/old/best_practices.rst
+-rw-r--r--   0        0        0     2854 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/old/getting_started.rst
+-rw-r--r--   0        0        0     5612 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/old/image_data_compression.rst
+-rw-r--r--   0        0        0     7357 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/old/image_data_handlers.rst
+-rw-r--r--   0        0        0     5176 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/old/private_data_elements.rst
+-rw-r--r--   0        0        0      337 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/old/pydicom_user_guide.rst
+-rw-r--r--   0        0        0      524 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/old/python2_support.rst
+-rw-r--r--   0        0        0     1090 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/old/ref_guide.rst
+-rw-r--r--   0        0        0     5049 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/old/transition_to_pydicom1.rst
+-rw-r--r--   0        0        0     2644 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/old/viewing_images.rst
+-rw-r--r--   0        0        0     3614 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/old/working_with_overlays.rst
+-rw-r--r--   0        0        0     8221 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/old/working_with_pixel_data.rst
+-rw-r--r--   0        0        0     3235 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/old/working_with_waveforms.rst
+-rw-r--r--   0        0        0     3779 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/old/writing_files.rst
+-rw-r--r--   0        0        0      327 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/charset.rst
+-rw-r--r--   0        0        0      774 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/config.rst
+-rw-r--r--   0        0        0      314 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/data.rst
+-rw-r--r--   0        0        0      802 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/datadict.rst
+-rw-r--r--   0        0        0      341 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/dataset.rst
+-rw-r--r--   0        0        0      233 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/dicomdir.rst
+-rw-r--r--   0        0        0      280 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/elem.dataelem.rst
+-rw-r--r--   0        0        0      301 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/elem.multival.rst
+-rw-r--r--   0        0        0      224 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/elem.rst
+-rw-r--r--   0        0        0      335 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/elem.sequence.rst
+-rw-r--r--   0        0        0      267 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/elem.tag.rst
+-rw-r--r--   0        0        0      495 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/elem.valuerep.rst
+-rw-r--r--   0        0        0      589 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/elem.values.rst
+-rw-r--r--   0        0        0      723 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/encaps.rst
+-rw-r--r--   0        0        0      574 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/encoders.rst
+-rw-r--r--   0        0        0      186 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/errors.rst
+-rw-r--r--   0        0        0      275 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/fileio.base.rst
+-rw-r--r--   0        0        0      480 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/fileio.read.rst
+-rw-r--r--   0        0        0      221 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/fileio.rst
+-rw-r--r--   0        0        0      331 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/fileio.util.rst
+-rw-r--r--   0        0        0      632 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/fileio.write.rst
+-rw-r--r--   0        0        0      325 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/fileset.rst
+-rw-r--r--   0        0        0      285 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/handlers.overlay_data.rst
+-rw-r--r--   0        0        0      398 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/handlers.pixel_data.rst
+-rw-r--r--   0        0        0      615 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/handlers.rst
+-rw-r--r--   0        0        0      276 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/handlers.waveform_data.rst
+-rw-r--r--   0        0        0      399 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/index.rst
+-rw-r--r--   0        0        0      218 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/misc.rst
+-rw-r--r--   0        0        0     7525 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/reference/uid.rst
+-rw-r--r--   0        0        0      523 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/index.rst
+-rw-r--r--   0        0        0     1959 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v0.9.2.rst
+-rw-r--r--   0        0        0     1625 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v0.9.3.rst
+-rw-r--r--   0        0        0     3132 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v0.9.4.rst
+-rw-r--r--   0        0        0     1320 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v0.9.5.rst
+-rw-r--r--   0        0        0      708 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v0.9.6.rst
+-rw-r--r--   0        0        0     2522 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v0.9.7.rst
+-rw-r--r--   0        0        0     1736 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v0.9.8.rst
+-rw-r--r--   0        0        0     1261 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v0.9.9.rst
+-rw-r--r--   0        0        0     3448 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v1.0.0.rst
+-rw-r--r--   0        0        0     2043 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v1.1.0.rst
+-rw-r--r--   0        0        0     3570 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v1.2.0.rst
+-rw-r--r--   0        0        0     3069 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v1.3.0.rst
+-rw-r--r--   0        0        0     4371 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v1.4.0.rst
+-rw-r--r--   0        0        0      358 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v1.4.1.rst
+-rw-r--r--   0        0        0     2806 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v2.0.0.rst
+-rw-r--r--   0        0        0     7542 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v2.1.0.rst
+-rw-r--r--   0        0        0      219 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v2.1.1.rst
+-rw-r--r--   0        0        0     6511 2023-06-18 21:37:24.966689 pydicom-2.4.1/doc/release_notes/v2.2.0.rst
+-rw-r--r--   0        0        0     2893 2023-06-18 21:37:24.970689 pydicom-2.4.1/doc/release_notes/v2.3.0.rst
+-rw-r--r--   0        0        0     2155 2023-06-18 21:37:24.970689 pydicom-2.4.1/doc/release_notes/v2.4.0.rst
+-rw-r--r--   0        0        0     1081 2023-06-18 21:37:24.970689 pydicom-2.4.1/doc/tutorials/contributing.rst
+-rw-r--r--   0        0        0    10607 2023-06-18 21:37:24.970689 pydicom-2.4.1/doc/tutorials/contributing_code.rst
+-rw-r--r--   0        0        0     9568 2023-06-18 21:37:24.970689 pydicom-2.4.1/doc/tutorials/contributing_docs.rst
+-rw-r--r--   0        0        0    22994 2023-06-18 21:37:24.970689 pydicom-2.4.1/doc/tutorials/dataset_basics.rst
+-rw-r--r--   0        0        0     4390 2023-06-18 21:37:24.970689 pydicom-2.4.1/doc/tutorials/dicom_json.rst
+-rw-r--r--   0        0        0    19523 2023-06-18 21:37:24.970689 pydicom-2.4.1/doc/tutorials/filesets.rst
+-rw-r--r--   0        0        0      311 2023-06-18 21:37:24.970689 pydicom-2.4.1/doc/tutorials/index.rst
+-rw-r--r--   0        0        0     5487 2023-06-18 21:37:24.970689 pydicom-2.4.1/doc/tutorials/installation.rst
+-rw-r--r--   0        0        0     7747 2023-06-18 21:37:24.970689 pydicom-2.4.1/doc/tutorials/pixel_data/compressing.rst
+-rw-r--r--   0        0        0     2153 2023-06-18 21:37:24.970689 pydicom-2.4.1/doc/tutorials/sr_basics.rst
+-rw-r--r--   0        0        0     9581 2023-06-18 21:37:24.970689 pydicom-2.4.1/doc/tutorials/virtualenvs.rst
+-rw-r--r--   0        0        0     9195 2023-06-18 21:37:24.970689 pydicom-2.4.1/doc/tutorials/waveforms.rst
+-rw-r--r--   0        0        0   135332 2023-06-18 21:37:24.970689 pydicom-2.4.1/doc/tutorials/waveforms_assets/waveforms_decode.png
+-rw-r--r--   0        0        0    90122 2023-06-18 21:37:24.970689 pydicom-2.4.1/doc/tutorials/waveforms_assets/waveforms_encode.png
+-rw-r--r--   0        0        0       77 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/README.txt
+-rw-r--r--   0        0        0     3481 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/dicomtree.py
+-rw-r--r--   0        0        0      173 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/image_processing/README.txt
+-rw-r--r--   0        0        0     1377 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/image_processing/plot_downsize_image.py
+-rw-r--r--   0        0        0     1541 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/image_processing/plot_waveforms.py
+-rw-r--r--   0        0        0     2126 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/image_processing/reslice.py
+-rw-r--r--   0        0        0      119 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/input_output/README.txt
+-rw-r--r--   0        0        0     1563 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/input_output/plot_printing_dataset.py
+-rw-r--r--   0        0        0     1165 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/input_output/plot_read_dicom.py
+-rw-r--r--   0        0        0     2794 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/input_output/plot_read_dicom_directory.py
+-rw-r--r--   0        0        0     4465 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/input_output/plot_read_fileset.py
+-rw-r--r--   0        0        0     1123 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/input_output/plot_read_rtplan.py
+-rw-r--r--   0        0        0     2401 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/input_output/plot_write_dicom.py
+-rw-r--r--   0        0        0     2392 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/memory_dataset.py
+-rw-r--r--   0        0        0      177 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/metadata_processing/README.txt
+-rw-r--r--   0        0        0     1410 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/metadata_processing/plot_add_dict_entries.py
+-rw-r--r--   0        0        0     2787 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/metadata_processing/plot_anonymize.py
+-rw-r--r--   0        0        0     1071 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/metadata_processing/plot_sequences.py
+-rw-r--r--   0        0        0     1033 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/plot_dicom_difference.py
+-rw-r--r--   0        0        0     1286 2023-06-18 21:37:24.970689 pydicom-2.4.1/examples/show_charset_name.py
+-rw-r--r--   0        0        0      330 2023-06-18 21:37:24.970689 pydicom-2.4.1/mypy.ini
+-rw-r--r--   0        0        0     1577 2023-06-18 21:37:24.970689 pydicom-2.4.1/pydicom/__init__.py
+-rw-r--r--   0        0        0   509435 2023-06-18 21:37:24.974689 pydicom-2.4.1/pydicom/_dicom_dict.py
+-rw-r--r--   0        0        0   613172 2023-06-18 21:37:24.974689 pydicom-2.4.1/pydicom/_private_dict.py
+-rw-r--r--   0        0        0      130 2023-06-18 21:37:24.974689 pydicom-2.4.1/pydicom/_storage_sopclass_uids.py
+-rw-r--r--   0        0        0    65890 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/_uid_dict.py
+-rw-r--r--   0        0        0      379 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/_version.py
+-rw-r--r--   0        0        0    31107 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/charset.py
+-rw-r--r--   0        0        0        0 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/cli/__init__.py
+-rw-r--r--   0        0        0     1001 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/cli/codify.py
+-rw-r--r--   0        0        0     7670 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/cli/main.py
+-rw-r--r--   0        0        0     5323 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/cli/show.py
+-rw-r--r--   0        0        0      607 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/compat.py
+-rw-r--r--   0        0        0    18738 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/config.py
+-rw-r--r--   0        0        0      403 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/__init__.py
+-rw-r--r--   0        0        0     1896 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/FileInfo.txt
+-rw-r--r--   0        0        0     1892 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/chrArab.dcm
+-rw-r--r--   0        0        0     1890 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/chrFren.dcm
+-rw-r--r--   0        0        0     1938 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/chrFrenMulti.dcm
+-rw-r--r--   0        0        0     1894 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/chrGerm.dcm
+-rw-r--r--   0        0        0     1890 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/chrGreek.dcm
+-rw-r--r--   0        0        0     1950 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/chrH31.dcm
+-rw-r--r--   0        0        0     1960 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/chrH32.dcm
+-rw-r--r--   0        0        0     1890 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/chrHbrw.dcm
+-rw-r--r--   0        0        0     1934 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/chrI2.dcm
+-rw-r--r--   0        0        0     1918 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/chrJapMulti.dcm
+-rw-r--r--   0        0        0     1940 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/chrJapMultiExplicitIR6.dcm
+-rw-r--r--   0        0        0     1898 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/chrKoreanMulti.dcm
+-rw-r--r--   0        0        0     1890 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/chrRuss.dcm
+-rw-r--r--   0        0        0      520 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/chrSQEncoding.dcm
+-rw-r--r--   0        0        0      520 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/chrSQEncoding1.dcm
+-rw-r--r--   0        0        0     1910 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/chrX1.dcm
+-rw-r--r--   0        0        0     1904 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/charset_files/chrX2.dcm
+-rw-r--r--   0        0        0    11895 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/data_manager.py
+-rw-r--r--   0        0        0     8205 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/download.py
+-rw-r--r--   0        0        0     6297 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/hashes.json
+-rw-r--r--   0        0        0     1725 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/palettes/README.md
+-rw-r--r--   0        0        0     4078 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/palettes/fall.dcm
+-rw-r--r--   0        0        0     4754 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/palettes/hotiron.dcm
+-rw-r--r--   0        0        0     4776 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/palettes/hotmetalblue.dcm
+-rw-r--r--   0        0        0     4732 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/palettes/pet.dcm
+-rw-r--r--   0        0        0     4790 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/palettes/pet20step.dcm
+-rw-r--r--   0        0        0     4104 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/palettes/spring.dcm
+-rw-r--r--   0        0        0     4100 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/palettes/summer.dcm
+-rw-r--r--   0        0        0     4112 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/palettes/winter.dcm
+-rw-r--r--   0        0        0     2057 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/retry.py
+-rw-r--r--   0        0        0     3590 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/693_J2KI.dcm
+-rw-r--r--   0        0        0    39206 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/CT_small.dcm
+-rw-r--r--   0        0        0    15412 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/ExplVR_BigEnd.dcm
+-rw-r--r--   0        0        0      434 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/ExplVR_BigEndNoMeta.dcm
+-rw-r--r--   0        0        0      434 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/ExplVR_LitEndNoMeta.dcm
+-rw-r--r--   0        0        0    30706 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/GDCMJ2K_TextGBR.dcm
+-rw-r--r--   0        0        0   138518 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/J2K_pixelrep_mismatch.dcm
+-rw-r--r--   0        0        0     9844 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/JPEG-lossy.dcm
+-rw-r--r--   0        0        0     3308 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/JPEG2000-embedded-sequence-delimiter.dcm
+-rw-r--r--   0        0        0     3308 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/JPEG2000.dcm
+-rw-r--r--   0        0        0     9844 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/JPGExtended.dcm
+-rw-r--r--   0        0        0     9830 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/MR_small.dcm
+-rw-r--r--   0        0        0     7790 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/MR_small_RLE.dcm
+-rw-r--r--   0        0        0     9708 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/MR_small_bigendian.dcm
+-rw-r--r--   0        0        0     9846 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/MR_small_expb.dcm
+-rw-r--r--   0        0        0     9702 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/MR_small_implicit.dcm
+-rw-r--r--   0        0        0     6008 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/MR_small_jp2klossless.dcm
+-rw-r--r--   0        0        0     6124 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/MR_small_jpeg_ls_lossless.dcm
+-rw-r--r--   0        0        0     9958 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/MR_small_padded.dcm
+-rw-r--r--   0        0        0     9630 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/MR_truncated.dcm
+-rw-r--r--   0        0        0    15439 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/README.txt
+-rw-r--r--   0        0        0     4316 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/SC_jpeg_no_color_transform.dcm
+-rw-r--r--   0        0        0     4310 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/SC_jpeg_no_color_transform_2.dcm
+-rw-r--r--   0        0        0     3626 2023-06-18 21:37:24.978689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cr.dcm
+-rw-r--r--   0        0        0     3136 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+n1.dcm
+-rw-r--r--   0        0        0     3090 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+n2.dcm
+-rw-r--r--   0        0        0     3140 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+np.dcm
+-rw-r--r--   0        0        0     3094 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+s2.dcm
+-rw-r--r--   0        0        0     3420 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+s4.dcm
+-rw-r--r--   0        0        0     2998 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_gdcm_KY.dcm
+-rw-r--r--   0        0        0     4464 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_jpeg.dcm
+-rw-r--r--   0        0        0     4310 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_jpeg_app14_dcmd.dcm
+-rw-r--r--   0        0        0   197506 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_jpeg_dcmd.dcm
+-rw-r--r--   0        0        0     3424 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_jpeg_dcmtk.dcm
+-rw-r--r--   0        0        0     5204 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_jpeg_gdcm.dcm
+-rw-r--r--   0        0        0     5042 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_jpeg_lossy_gdcm.dcm
+-rw-r--r--   0        0        0     2006 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_rle.dcm
+-rw-r--r--   0        0        0     2606 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_rle_16bit.dcm
+-rw-r--r--   0        0        0     3896 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_rle_16bit_2frame.dcm
+-rw-r--r--   0        0        0     2696 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_rle_2frame.dcm
+-rw-r--r--   0        0        0     3760 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_rle_32bit.dcm
+-rw-r--r--   0        0        0     6246 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_rle_32bit_2frame.dcm
+-rw-r--r--   0        0        0     1444 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_small_odd.dcm
+-rw-r--r--   0        0        0     1444 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_small_odd_big_endian.dcm
+-rw-r--r--   0        0        0     2044 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_rgb_small_odd_jpeg.dcm
+-rw-r--r--   0        0        0    21686 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/SC_ybr_full_422_uncompressed.dcm
+-rw-r--r--   0        0        0      674 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/UN_sequence.dcm
+-rw-r--r--   0        0        0     7618 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/badVR.dcm
+-rw-r--r--   0        0        0     2300 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/77654033/CR1/6154
+-rw-r--r--   0        0        0     2298 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/77654033/CR2/6247
+-rw-r--r--   0        0        0     2298 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/77654033/CR3/6278
+-rw-r--r--   0        0        0     3810 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/77654033/CT2/17106
+-rw-r--r--   0        0        0     3812 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/77654033/CT2/17136
+-rw-r--r--   0        0        0     3812 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/77654033/CT2/17166
+-rw-r--r--   0        0        0     3812 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/77654033/CT2/17196
+-rw-r--r--   0        0        0     3920 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892001/CT2N/6293
+-rw-r--r--   0        0        0     3908 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892001/CT2N/6924
+-rw-r--r--   0        0        0     3936 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2062
+-rw-r--r--   0        0        0     3936 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2392
+-rw-r--r--   0        0        0     3936 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2693
+-rw-r--r--   0        0        0     3936 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/3023
+-rw-r--r--   0        0        0     3938 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/3353
+-rw-r--r--   0        0        0     2336 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR1/15820
+-rw-r--r--   0        0        0     2336 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR1/4919
+-rw-r--r--   0        0        0     2330 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR1/5641
+-rw-r--r--   0        0        0     2336 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/15970
+-rw-r--r--   0        0        0     2356 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/4950
+-rw-r--r--   0        0        0     2354 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/4981
+-rw-r--r--   0        0        0     2354 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/5011
+-rw-r--r--   0        0        0     2348 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/6273
+-rw-r--r--   0        0        0     2348 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/6605
+-rw-r--r--   0        0        0     2350 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/6935
+-rw-r--r--   0        0        0     2350 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4467
+-rw-r--r--   0        0        0     2348 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4528
+-rw-r--r--   0        0        0     2348 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4558
+-rw-r--r--   0        0        0     2350 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4588
+-rw-r--r--   0        0        0     2350 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4618
+-rw-r--r--   0        0        0     2350 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4648
+-rw-r--r--   0        0        0     2350 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4678
+-rw-r--r--   0        0        0    11116 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/DICOMDIR
+-rw-r--r--   0        0        0    11116 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-bigEnd
+-rw-r--r--   0        0        0      396 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-empty.dcm
+-rw-r--r--   0        0        0    11110 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-implicit
+-rw-r--r--   0        0        0    11092 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-nooffset
+-rw-r--r--   0        0        0    11116 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-nopatient
+-rw-r--r--   0        0        0    11116 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-reordered
+-rw-r--r--   0        0        0      719 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/README.txt
+-rw-r--r--   0        0        0    13066 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/DICOMDIR
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000000
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000001
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000002
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000003
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000004
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000005
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000006
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000007
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000008
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000009
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000A
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000B
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000C
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.982689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000D
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000E
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000F
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000G
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000H
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000I
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000J
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000K
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000L
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000M
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000N
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000O
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000P
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Q
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000R
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000S
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000T
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000U
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000V
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000W
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000X
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Y
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Z
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000010
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000011
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000012
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000013
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000014
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000015
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000016
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000017
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000018
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000019
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001A
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001B
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001C
+-rw-r--r--   0        0        0      740 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001D
+-rw-r--r--   0        0        0     1206 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/README
+-rw-r--r--   0        0        0      276 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/empty_charset_LEI.dcm
+-rw-r--r--   0        0        0     4637 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/image_dfl.dcm
+-rw-r--r--   0        0        0    37084 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/liver_1frame.dcm
+-rw-r--r--   0        0        0    36532 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/liver_expb_1frame.dcm
+-rw-r--r--   0        0        0      317 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/meta_missing_tsyntax.dcm
+-rw-r--r--   0        0        0      343 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/nested_priv_SQ.dcm
+-rw-r--r--   0        0        0    38871 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/no_meta.dcm
+-rw-r--r--   0        0        0      408 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/no_meta_group_length.dcm
+-rw-r--r--   0        0        0      546 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/priv_SQ.dcm
+-rw-r--r--   0        0        0     2968 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/reportsi.dcm
+-rw-r--r--   0        0        0     2700 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/reportsi_with_empty_number_tags.dcm
+-rw-r--r--   0        0        0     7568 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/rtdose.dcm
+-rwxr-xr-x   0        0        0     1958 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/rtdose_1frame.dcm
+-rw-r--r--   0        0        0     7618 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/rtdose_expb.dcm
+-rw-r--r--   0        0        0     2008 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/rtdose_expb_1frame.dcm
+-rw-r--r--   0        0        0     6816 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/rtdose_rle.dcm
+-rw-r--r--   0        0        0     2122 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/rtdose_rle_1frame.dcm
+-rw-r--r--   0        0        0     2672 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/rtplan.dcm
+-rw-r--r--   0        0        0    14474 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/rtplan.dump
+-rw-r--r--   0        0        0     2129 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/rtplan_truncated.dcm
+-rw-r--r--   0        0        0     2534 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/rtstruct.dcm
+-rw-r--r--   0        0        0     7935 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/rtstruct.dump
+-rw-r--r--   0        0        0     6796 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/test-SR.dcm
+-rw-r--r--   0        0        0    20965 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/test1.json
+-rw-r--r--   0        0        0     1841 2023-06-18 21:37:24.986689 pydicom-2.4.1/pydicom/data/test_files/test_PN.json
+-rwxr-xr-x   0        0        0   291088 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/data/test_files/waveform_ecg.dcm
+-rw-r--r--   0        0        0     6958 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/data/test_files/zipMR.gz
+-rw-r--r--   0        0        0     9485 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/data/urls.json
+-rw-r--r--   0        0        0    18650 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/datadict.py
+-rw-r--r--   0        0        0    31098 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/dataelem.py
+-rw-r--r--   0        0        0   109626 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/dataset.py
+-rw-r--r--   0        0        0     5676 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/dicomdir.py
+-rw-r--r--   0        0        0      403 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/dicomio.py
+-rw-r--r--   0        0        0    26824 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/encaps.py
+-rw-r--r--   0        0        0       66 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/encoders/__init__.py
+-rw-r--r--   0        0        0    36135 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/encoders/base.py
+-rw-r--r--   0        0        0     5901 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/encoders/gdcm.py
+-rw-r--r--   0        0        0     5374 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/encoders/native.py
+-rw-r--r--   0        0        0     1125 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/encoders/pylibjpeg.py
+-rw-r--r--   0        0        0     1714 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/env_info.py
+-rw-r--r--   0        0        0      771 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/errors.py
+-rw-r--r--   0        0        0     7794 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/filebase.py
+-rw-r--r--   0        0        0    44662 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/filereader.py
+-rw-r--r--   0        0        0   102357 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/fileset.py
+-rw-r--r--   0        0        0    14625 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/fileutil.py
+-rw-r--r--   0        0        0    44151 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/filewriter.py
+-rw-r--r--   0        0        0    12252 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/jsonrep.py
+-rw-r--r--   0        0        0     1644 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/misc.py
+-rw-r--r--   0        0        0     5140 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/multival.py
+-rw-r--r--   0        0        0      108 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/overlay_data_handlers/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/overlays/__init__.py
+-rw-r--r--   0        0        0     9951 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/overlays/numpy_handler.py
+-rw-r--r--   0        0        0      262 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/pixel_data_handlers/__init__.py
+-rw-r--r--   0        0        0     9761 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/pixel_data_handlers/gdcm_handler.py
+-rw-r--r--   0        0        0     3396 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/pixel_data_handlers/jpeg_ls_handler.py
+-rw-r--r--   0        0        0    12284 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/pixel_data_handlers/numpy_handler.py
+-rw-r--r--   0        0        0     8695 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/pixel_data_handlers/pillow_handler.py
+-rw-r--r--   0        0        0    11053 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/pixel_data_handlers/pylibjpeg_handler.py
+-rw-r--r--   0        0        0    16581 2023-06-18 21:37:24.990690 pydicom-2.4.1/pydicom/pixel_data_handlers/rle_handler.py
+-rw-r--r--   0        0        0    54722 2023-06-18 21:37:24.994690 pydicom-2.4.1/pydicom/pixel_data_handlers/util.py
+-rw-r--r--   0        0        0        0 2023-06-18 21:37:24.994690 pydicom-2.4.1/pydicom/py.typed
+-rw-r--r--   0        0        0     7608 2023-06-18 21:37:24.994690 pydicom-2.4.1/pydicom/sequence.py
+-rw-r--r--   0        0        0       38 2023-06-18 21:37:24.994690 pydicom-2.4.1/pydicom/sr/__init__.py
+-rw-r--r--   0        0        0   788696 2023-06-18 21:37:24.998690 pydicom-2.4.1/pydicom/sr/_cid_dict.py
+-rw-r--r--   0        0        0  2725654 2023-06-18 21:37:25.006690 pydicom-2.4.1/pydicom/sr/_concepts_dict.py
+-rw-r--r--   0        0        0   424515 2023-06-18 21:37:25.010690 pydicom-2.4.1/pydicom/sr/_snomed_dict.py
+-rw-r--r--   0        0        0    11035 2023-06-18 21:37:25.010690 pydicom-2.4.1/pydicom/sr/codedict.py
+-rw-r--r--   0        0        0     2026 2023-06-18 21:37:25.010690 pydicom-2.4.1/pydicom/sr/coding.py
+-rw-r--r--   0        0        0     8541 2023-06-18 21:37:25.010690 pydicom-2.4.1/pydicom/tag.py
+-rw-r--r--   0        0        0    34984 2023-06-18 21:37:25.014690 pydicom-2.4.1/pydicom/uid.py
+-rw-r--r--   0        0        0        0 2023-06-18 21:37:25.014690 pydicom-2.4.1/pydicom/util/__init__.py
+-rw-r--r--   0        0        0    17459 2023-06-18 21:37:25.014690 pydicom-2.4.1/pydicom/util/codify.py
+-rw-r--r--   0        0        0     3956 2023-06-18 21:37:25.014690 pydicom-2.4.1/pydicom/util/dump.py
+-rw-r--r--   0        0        0     4259 2023-06-18 21:37:25.014690 pydicom-2.4.1/pydicom/util/fixer.py
+-rw-r--r--   0        0        0     1576 2023-06-18 21:37:25.014690 pydicom-2.4.1/pydicom/util/hexutil.py
+-rw-r--r--   0        0        0     6465 2023-06-18 21:37:25.014690 pydicom-2.4.1/pydicom/util/leanread.py
+-rw-r--r--   0        0        0    73466 2023-06-18 21:37:25.014690 pydicom-2.4.1/pydicom/valuerep.py
+-rw-r--r--   0        0        0    26630 2023-06-18 21:37:25.014690 pydicom-2.4.1/pydicom/values.py
+-rw-r--r--   0        0        0       88 2023-06-18 21:37:25.014690 pydicom-2.4.1/pydicom/waveforms/__init__.py
+-rw-r--r--   0        0        0     8580 2023-06-18 21:37:25.014690 pydicom-2.4.1/pydicom/waveforms/numpy_handler.py
+-rw-r--r--   0        0        0     2811 2023-06-18 21:37:25.014690 pydicom-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-06-18 21:37:25.014690 pydicom-2.4.1/setup.cfg
+-rw-r--r--   0        0        0     2744 2023-06-18 21:37:25.014690 pydicom-2.4.1/setup.py
+-rwxr-xr-x   0        0        0    14008 2023-06-18 21:37:25.014690 pydicom-2.4.1/source/generate_cids/generate_concept_dicts.py
+-rwxr-xr-x   0        0        0    11894 2023-06-18 21:37:25.014690 pydicom-2.4.1/source/generate_dict/generate_dicom_dict.py
+-rwxr-xr-x   0        0        0     3769 2023-06-18 21:37:25.014690 pydicom-2.4.1/source/generate_dict/generate_private_dict.py
+-rwxr-xr-x   0        0        0     7710 2023-06-18 21:37:25.014690 pydicom-2.4.1/source/generate_dict/generate_uid_dict.py
+-rwxr-xr-x   0        0        0     2450 2023-06-18 21:37:25.014690 pydicom-2.4.1/source/generate_uids/generate_storage_sopclass_uids.py
+-rw-r--r--   0        0        0     1708 2023-06-18 21:37:25.014690 pydicom-2.4.1/source/scripts/charlist.py
+-rw-r--r--   0        0        0     7808 1970-01-01 00:00:00.000000 pydicom-2.4.1/PKG-INFO
```

### Comparing `pydicom-2.4.0/.circleci/config.yml` & `pydicom-2.4.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/.github/ISSUE_TEMPLATE/bug_report.md` & `pydicom-2.4.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/.github/ISSUE_TEMPLATE/feature_request.md` & `pydicom-2.4.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/.github/ISSUE_TEMPLATE/pixel_issue.md` & `pydicom-2.4.1/.github/ISSUE_TEMPLATE/pixel_issue.md`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/.github/PULL_REQUEST_TEMPLATE.md` & `pydicom-2.4.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/.github/workflows/merge-pytest.yml` & `pydicom-2.4.1/.github/workflows/merge-pytest.yml`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/.github/workflows/merge-typing.yml` & `pydicom-2.4.1/.github/workflows/merge-typing.yml`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/.github/workflows/pr-pytest.yml` & `pydicom-2.4.1/.github/workflows/pr-pytest.yml`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/.github/workflows/pr-type-spell.yml` & `pydicom-2.4.1/.github/workflows/pr-type-spell.yml`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/.github/workflows/publish-pypi-deploy.yml` & `pydicom-2.4.1/.github/workflows/publish-pypi-deploy.yml`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/.gitignore` & `pydicom-2.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/CONTRIBUTING.md` & `pydicom-2.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/LICENSE` & `pydicom-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/Makefile` & `pydicom-2.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/README.md` & `pydicom-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/asv.conf.json` & `pydicom-2.4.1/asv.conf.json`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/benchmarks/bench_encaps.py` & `pydicom-2.4.1/benchmarks/bench_encaps.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/benchmarks/bench_handler_numpy.py` & `pydicom-2.4.1/benchmarks/bench_handler_numpy.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/benchmarks/bench_nested_seq.py` & `pydicom-2.4.1/benchmarks/bench_nested_seq.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/benchmarks/bench_pixel_util.py` & `pydicom-2.4.1/benchmarks/bench_pixel_util.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/benchmarks/bench_rle_decode.py` & `pydicom-2.4.1/benchmarks/bench_rle_decode.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/benchmarks/bench_rle_encode.py` & `pydicom-2.4.1/benchmarks/bench_rle_encode.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/build_tools/circle/build_doc.sh` & `pydicom-2.4.1/build_tools/circle/build_doc.sh`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/build_tools/circle/push_doc.sh` & `pydicom-2.4.1/build_tools/circle/push_doc.sh`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/build_tools/sphinx/github_link.py` & `pydicom-2.4.1/build_tools/sphinx/github_link.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/Makefile` & `pydicom-2.4.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/README.md` & `pydicom-2.4.1/doc/README.md`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/_static/css/pydicom.css` & `pydicom-2.4.1/doc/_static/css/pydicom.css`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/assets/img/favicon.ico` & `pydicom-2.4.1/doc/assets/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/assets/img/logo.png` & `pydicom-2.4.1/doc/assets/img/logo.png`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/assets/img/pydicom_blue_light.png` & `pydicom-2.4.1/doc/assets/img/pydicom_blue_light.png`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/assets/img/pydicom_blue_light.svg` & `pydicom-2.4.1/doc/assets/img/pydicom_blue_light.svg`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/assets/img/pydicom_flat_black.png` & `pydicom-2.4.1/doc/assets/img/pydicom_flat_black.png`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/assets/img/pydicom_flat_black.svg` & `pydicom-2.4.1/doc/assets/img/pydicom_flat_black.svg`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/assets/img/pydicom_flat_black_alpha.png` & `pydicom-2.4.1/doc/assets/img/pydicom_flat_black_alpha.png`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/conf.py` & `pydicom-2.4.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/faq/index.rst` & `pydicom-2.4.1/doc/faq/index.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/guides/cli/cli_codify.rst` & `pydicom-2.4.1/doc/guides/cli/cli_codify.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/guides/cli/cli_dev.rst` & `pydicom-2.4.1/doc/guides/cli/cli_dev.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/guides/cli/cli_intro.rst` & `pydicom-2.4.1/doc/guides/cli/cli_intro.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/guides/cli/cli_show.rst` & `pydicom-2.4.1/doc/guides/cli/cli_show.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/guides/element_value_types.rst` & `pydicom-2.4.1/doc/guides/element_value_types.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/guides/encoding/encoder_plugin_options.rst` & `pydicom-2.4.1/doc/guides/encoding/encoder_plugin_options.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/guides/encoding/encoder_plugins.rst` & `pydicom-2.4.1/doc/guides/encoding/encoder_plugins.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/guides/encoding/rle_lossless.rst` & `pydicom-2.4.1/doc/guides/encoding/rle_lossless.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/guides/glossary.rst` & `pydicom-2.4.1/doc/guides/glossary.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/guides/writing_documentation.rst` & `pydicom-2.4.1/doc/guides/writing_documentation.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/index.rst` & `pydicom-2.4.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/make.bat` & `pydicom-2.4.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/old/base_element.rst` & `pydicom-2.4.1/doc/old/base_element.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/old/best_practices.rst` & `pydicom-2.4.1/doc/old/best_practices.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/old/getting_started.rst` & `pydicom-2.4.1/doc/old/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/old/image_data_compression.rst` & `pydicom-2.4.1/doc/old/image_data_compression.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/old/image_data_handlers.rst` & `pydicom-2.4.1/doc/old/image_data_handlers.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/old/private_data_elements.rst` & `pydicom-2.4.1/doc/old/private_data_elements.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/old/python2_support.rst` & `pydicom-2.4.1/doc/old/python2_support.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/old/ref_guide.rst` & `pydicom-2.4.1/doc/old/ref_guide.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/old/transition_to_pydicom1.rst` & `pydicom-2.4.1/doc/old/transition_to_pydicom1.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/old/viewing_images.rst` & `pydicom-2.4.1/doc/old/viewing_images.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/old/working_with_overlays.rst` & `pydicom-2.4.1/doc/old/working_with_overlays.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/old/working_with_pixel_data.rst` & `pydicom-2.4.1/doc/old/working_with_pixel_data.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/old/working_with_waveforms.rst` & `pydicom-2.4.1/doc/old/working_with_waveforms.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/old/writing_files.rst` & `pydicom-2.4.1/doc/old/writing_files.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/reference/config.rst` & `pydicom-2.4.1/doc/reference/config.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/reference/datadict.rst` & `pydicom-2.4.1/doc/reference/datadict.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/reference/elem.values.rst` & `pydicom-2.4.1/doc/reference/elem.values.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/reference/encaps.rst` & `pydicom-2.4.1/doc/reference/encaps.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/reference/encoders.rst` & `pydicom-2.4.1/doc/reference/encoders.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/reference/fileio.write.rst` & `pydicom-2.4.1/doc/reference/fileio.write.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/reference/handlers.rst` & `pydicom-2.4.1/doc/reference/handlers.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/reference/uid.rst` & `pydicom-2.4.1/doc/reference/uid.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/index.rst` & `pydicom-2.4.1/doc/release_notes/index.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v0.9.2.rst` & `pydicom-2.4.1/doc/release_notes/v0.9.2.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v0.9.3.rst` & `pydicom-2.4.1/doc/release_notes/v0.9.3.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v0.9.4.rst` & `pydicom-2.4.1/doc/release_notes/v0.9.4.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v0.9.5.rst` & `pydicom-2.4.1/doc/release_notes/v0.9.5.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v0.9.6.rst` & `pydicom-2.4.1/doc/release_notes/v0.9.6.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v0.9.7.rst` & `pydicom-2.4.1/doc/release_notes/v0.9.7.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v0.9.8.rst` & `pydicom-2.4.1/doc/release_notes/v0.9.8.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v0.9.9.rst` & `pydicom-2.4.1/doc/release_notes/v0.9.9.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v1.0.0.rst` & `pydicom-2.4.1/doc/release_notes/v1.0.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v1.1.0.rst` & `pydicom-2.4.1/doc/release_notes/v1.1.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v1.2.0.rst` & `pydicom-2.4.1/doc/release_notes/v1.2.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v1.3.0.rst` & `pydicom-2.4.1/doc/release_notes/v1.3.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v1.4.0.rst` & `pydicom-2.4.1/doc/release_notes/v1.4.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v2.0.0.rst` & `pydicom-2.4.1/doc/release_notes/v2.0.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v2.1.0.rst` & `pydicom-2.4.1/doc/release_notes/v2.1.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v2.2.0.rst` & `pydicom-2.4.1/doc/release_notes/v2.2.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v2.3.0.rst` & `pydicom-2.4.1/doc/release_notes/v2.3.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/release_notes/v2.4.0.rst` & `pydicom-2.4.1/doc/release_notes/v2.4.0.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/tutorials/contributing.rst` & `pydicom-2.4.1/doc/tutorials/contributing.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/tutorials/contributing_code.rst` & `pydicom-2.4.1/doc/tutorials/contributing_code.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/tutorials/contributing_docs.rst` & `pydicom-2.4.1/doc/tutorials/contributing_docs.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/tutorials/dataset_basics.rst` & `pydicom-2.4.1/doc/tutorials/dataset_basics.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/tutorials/dicom_json.rst` & `pydicom-2.4.1/doc/tutorials/dicom_json.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/tutorials/filesets.rst` & `pydicom-2.4.1/doc/tutorials/filesets.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/tutorials/installation.rst` & `pydicom-2.4.1/doc/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/tutorials/pixel_data/compressing.rst` & `pydicom-2.4.1/doc/tutorials/pixel_data/compressing.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/tutorials/sr_basics.rst` & `pydicom-2.4.1/doc/tutorials/sr_basics.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/tutorials/virtualenvs.rst` & `pydicom-2.4.1/doc/tutorials/virtualenvs.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/tutorials/waveforms.rst` & `pydicom-2.4.1/doc/tutorials/waveforms.rst`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/tutorials/waveforms_assets/waveforms_decode.png` & `pydicom-2.4.1/doc/tutorials/waveforms_assets/waveforms_decode.png`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/doc/tutorials/waveforms_assets/waveforms_encode.png` & `pydicom-2.4.1/doc/tutorials/waveforms_assets/waveforms_encode.png`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/examples/dicomtree.py` & `pydicom-2.4.1/examples/dicomtree.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/examples/image_processing/plot_downsize_image.py` & `pydicom-2.4.1/examples/image_processing/plot_downsize_image.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/examples/image_processing/plot_waveforms.py` & `pydicom-2.4.1/examples/image_processing/plot_waveforms.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/examples/image_processing/reslice.py` & `pydicom-2.4.1/examples/image_processing/reslice.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/examples/input_output/plot_printing_dataset.py` & `pydicom-2.4.1/examples/input_output/plot_printing_dataset.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/examples/input_output/plot_read_dicom.py` & `pydicom-2.4.1/examples/input_output/plot_read_dicom.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/examples/input_output/plot_read_dicom_directory.py` & `pydicom-2.4.1/examples/input_output/plot_read_dicom_directory.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/examples/input_output/plot_read_fileset.py` & `pydicom-2.4.1/examples/input_output/plot_read_fileset.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/examples/input_output/plot_read_rtplan.py` & `pydicom-2.4.1/examples/input_output/plot_read_rtplan.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/examples/input_output/plot_write_dicom.py` & `pydicom-2.4.1/examples/input_output/plot_write_dicom.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/examples/memory_dataset.py` & `pydicom-2.4.1/examples/memory_dataset.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/examples/metadata_processing/plot_add_dict_entries.py` & `pydicom-2.4.1/examples/metadata_processing/plot_add_dict_entries.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/examples/metadata_processing/plot_anonymize.py` & `pydicom-2.4.1/examples/metadata_processing/plot_anonymize.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/examples/metadata_processing/plot_sequences.py` & `pydicom-2.4.1/examples/metadata_processing/plot_sequences.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/examples/plot_dicom_difference.py` & `pydicom-2.4.1/examples/plot_dicom_difference.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/examples/show_charset_name.py` & `pydicom-2.4.1/examples/show_charset_name.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/__init__.py` & `pydicom-2.4.1/pydicom/__init__.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/_dicom_dict.py` & `pydicom-2.4.1/pydicom/_dicom_dict.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/_private_dict.py` & `pydicom-2.4.1/pydicom/_private_dict.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/_uid_dict.py` & `pydicom-2.4.1/pydicom/_uid_dict.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/charset.py` & `pydicom-2.4.1/pydicom/charset.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/cli/codify.py` & `pydicom-2.4.1/pydicom/cli/codify.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/cli/main.py` & `pydicom-2.4.1/pydicom/cli/main.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/cli/show.py` & `pydicom-2.4.1/pydicom/cli/show.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/compat.py` & `pydicom-2.4.1/pydicom/compat.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/config.py` & `pydicom-2.4.1/pydicom/config.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/FileInfo.txt` & `pydicom-2.4.1/pydicom/data/charset_files/FileInfo.txt`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/chrArab.dcm` & `pydicom-2.4.1/pydicom/data/charset_files/chrArab.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/chrFren.dcm` & `pydicom-2.4.1/pydicom/data/charset_files/chrFren.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/chrFrenMulti.dcm` & `pydicom-2.4.1/pydicom/data/charset_files/chrFrenMulti.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/chrGerm.dcm` & `pydicom-2.4.1/pydicom/data/charset_files/chrGerm.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/chrGreek.dcm` & `pydicom-2.4.1/pydicom/data/charset_files/chrGreek.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/chrH31.dcm` & `pydicom-2.4.1/pydicom/data/charset_files/chrH31.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/chrH32.dcm` & `pydicom-2.4.1/pydicom/data/charset_files/chrH32.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/chrHbrw.dcm` & `pydicom-2.4.1/pydicom/data/charset_files/chrHbrw.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/chrI2.dcm` & `pydicom-2.4.1/pydicom/data/charset_files/chrI2.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/chrJapMulti.dcm` & `pydicom-2.4.1/pydicom/data/charset_files/chrJapMulti.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/chrJapMultiExplicitIR6.dcm` & `pydicom-2.4.1/pydicom/data/charset_files/chrJapMultiExplicitIR6.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/chrKoreanMulti.dcm` & `pydicom-2.4.1/pydicom/data/charset_files/chrKoreanMulti.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/chrRuss.dcm` & `pydicom-2.4.1/pydicom/data/charset_files/chrRuss.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/chrSQEncoding.dcm` & `pydicom-2.4.1/pydicom/data/charset_files/chrSQEncoding.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/chrSQEncoding1.dcm` & `pydicom-2.4.1/pydicom/data/charset_files/chrSQEncoding1.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/chrX1.dcm` & `pydicom-2.4.1/pydicom/data/charset_files/chrX1.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/charset_files/chrX2.dcm` & `pydicom-2.4.1/pydicom/data/charset_files/chrX2.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/data_manager.py` & `pydicom-2.4.1/pydicom/data/data_manager.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/download.py` & `pydicom-2.4.1/pydicom/data/download.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/hashes.json` & `pydicom-2.4.1/pydicom/data/hashes.json`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/palettes/README.md` & `pydicom-2.4.1/pydicom/data/palettes/README.md`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/palettes/fall.dcm` & `pydicom-2.4.1/pydicom/data/palettes/fall.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/palettes/hotiron.dcm` & `pydicom-2.4.1/pydicom/data/palettes/hotiron.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/palettes/hotmetalblue.dcm` & `pydicom-2.4.1/pydicom/data/palettes/hotmetalblue.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/palettes/pet.dcm` & `pydicom-2.4.1/pydicom/data/palettes/pet.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/palettes/pet20step.dcm` & `pydicom-2.4.1/pydicom/data/palettes/pet20step.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/palettes/spring.dcm` & `pydicom-2.4.1/pydicom/data/palettes/spring.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/palettes/summer.dcm` & `pydicom-2.4.1/pydicom/data/palettes/summer.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/palettes/winter.dcm` & `pydicom-2.4.1/pydicom/data/palettes/winter.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/retry.py` & `pydicom-2.4.1/pydicom/data/retry.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/693_J2KI.dcm` & `pydicom-2.4.1/pydicom/data/test_files/693_J2KI.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/CT_small.dcm` & `pydicom-2.4.1/pydicom/data/test_files/CT_small.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/ExplVR_BigEnd.dcm` & `pydicom-2.4.1/pydicom/data/test_files/ExplVR_BigEnd.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/GDCMJ2K_TextGBR.dcm` & `pydicom-2.4.1/pydicom/data/test_files/GDCMJ2K_TextGBR.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/J2K_pixelrep_mismatch.dcm` & `pydicom-2.4.1/pydicom/data/test_files/J2K_pixelrep_mismatch.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/JPEG-lossy.dcm` & `pydicom-2.4.1/pydicom/data/test_files/JPEG-lossy.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/JPEG2000-embedded-sequence-delimiter.dcm` & `pydicom-2.4.1/pydicom/data/test_files/JPEG2000-embedded-sequence-delimiter.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/JPEG2000.dcm` & `pydicom-2.4.1/pydicom/data/test_files/JPEG2000.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/JPGExtended.dcm` & `pydicom-2.4.1/pydicom/data/test_files/JPGExtended.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/MR_small.dcm` & `pydicom-2.4.1/pydicom/data/test_files/MR_small.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/MR_small_RLE.dcm` & `pydicom-2.4.1/pydicom/data/test_files/MR_small_RLE.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/MR_small_bigendian.dcm` & `pydicom-2.4.1/pydicom/data/test_files/MR_small_bigendian.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/MR_small_expb.dcm` & `pydicom-2.4.1/pydicom/data/test_files/MR_small_expb.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/MR_small_implicit.dcm` & `pydicom-2.4.1/pydicom/data/test_files/MR_small_implicit.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/MR_small_jp2klossless.dcm` & `pydicom-2.4.1/pydicom/data/test_files/MR_small_jp2klossless.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/MR_small_jpeg_ls_lossless.dcm` & `pydicom-2.4.1/pydicom/data/test_files/MR_small_jpeg_ls_lossless.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/MR_small_padded.dcm` & `pydicom-2.4.1/pydicom/data/test_files/MR_small_padded.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/MR_truncated.dcm` & `pydicom-2.4.1/pydicom/data/test_files/MR_truncated.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/README.txt` & `pydicom-2.4.1/pydicom/data/test_files/README.txt`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_jpeg_no_color_transform.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_jpeg_no_color_transform.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_jpeg_no_color_transform_2.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_jpeg_no_color_transform_2.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cr.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cr.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+n1.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+n1.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+n2.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+n2.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+np.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+np.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+s2.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+s2.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+s4.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_dcmtk_+eb+cy+s4.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_gdcm_KY.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_gdcm_KY.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_jpeg.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_app14_dcmd.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_jpeg_app14_dcmd.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_dcmd.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_jpeg_dcmd.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_dcmtk.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_jpeg_dcmtk.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_gdcm.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_jpeg_gdcm.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_jpeg_lossy_gdcm.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_jpeg_lossy_gdcm.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_rle.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_16bit.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_rle_16bit.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_16bit_2frame.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_rle_16bit_2frame.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_2frame.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_rle_2frame.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_32bit.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_rle_32bit.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_rle_32bit_2frame.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_rle_32bit_2frame.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_small_odd.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_small_odd.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_small_odd_big_endian.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_small_odd_big_endian.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_rgb_small_odd_jpeg.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_rgb_small_odd_jpeg.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/SC_ybr_full_422_uncompressed.dcm` & `pydicom-2.4.1/pydicom/data/test_files/SC_ybr_full_422_uncompressed.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/UN_sequence.dcm` & `pydicom-2.4.1/pydicom/data/test_files/UN_sequence.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/badVR.dcm` & `pydicom-2.4.1/pydicom/data/test_files/badVR.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CR1/6154` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/77654033/CR1/6154`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CR2/6247` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/77654033/CR2/6247`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CR3/6278` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/77654033/CR3/6278`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CT2/17106` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/77654033/CT2/17106`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CT2/17136` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/77654033/CT2/17136`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CT2/17166` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/77654033/CT2/17166`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/77654033/CT2/17196` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/77654033/CT2/17196`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT2N/6293` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892001/CT2N/6293`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT2N/6924` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892001/CT2N/6924`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2062` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2062`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2392` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2392`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2693` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/2693`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/3023` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/3023`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892001/CT5N/3353` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892001/CT5N/3353`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR1/15820` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR1/15820`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR1/4919` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR1/4919`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR1/5641` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR1/5641`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/15970` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/15970`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/4950` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/4950`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/4981` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/4981`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/5011` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/5011`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/6273` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/6273`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/6605` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/6605`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR2/6935` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR2/6935`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4467` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4467`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4528` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4528`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4558` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4558`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4588` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4588`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4618` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4618`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4648` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4648`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/98892003/MR700/4678` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/98892003/MR700/4678`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/DICOMDIR`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-bigEnd` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-bigEnd`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-implicit` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-implicit`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-nooffset` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-nooffset`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-nopatient` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-nopatient`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/DICOMDIR-reordered` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/DICOMDIR-reordered`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/README.txt` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/README.txt`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/DICOMDIR` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/DICOMDIR`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000000` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000000`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000001` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000001`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000002` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000002`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000003` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000003`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000004` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000004`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000005` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000005`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000006` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000006`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000007` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000007`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000008` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000008`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000009` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000009`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000A` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000A`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000B` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000B`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000C` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000C`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000D` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000D`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000E` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000E`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000F` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000F`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000G` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000G`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000H` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000H`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000I` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000I`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000J` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000J`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000K` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000K`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000L` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000L`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000M` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000M`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000N` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000N`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000O` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000O`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000P` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000P`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Q` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Q`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000R` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000R`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000S` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000S`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000T` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000T`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000U` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000U`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000V` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000V`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000W` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000W`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000X` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000X`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Y` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Y`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Z` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00000Z`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000010` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000010`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000011` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000011`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000012` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000012`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000013` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000013`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000014` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000014`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000015` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000015`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000016` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000016`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000017` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000017`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000018` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000018`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000019` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM000019`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001A` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001A`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001B` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001B`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001C` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001C`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001D` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/PT000000/ST000000/SE000000/IM00001D`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/README` & `pydicom-2.4.1/pydicom/data/test_files/dicomdirtests/TINY_ALPHA/README`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/image_dfl.dcm` & `pydicom-2.4.1/pydicom/data/test_files/image_dfl.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/liver_1frame.dcm` & `pydicom-2.4.1/pydicom/data/test_files/liver_1frame.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/liver_expb_1frame.dcm` & `pydicom-2.4.1/pydicom/data/test_files/liver_expb_1frame.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/no_meta.dcm` & `pydicom-2.4.1/pydicom/data/test_files/no_meta.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/priv_SQ.dcm` & `pydicom-2.4.1/pydicom/data/test_files/priv_SQ.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/reportsi.dcm` & `pydicom-2.4.1/pydicom/data/test_files/reportsi.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/reportsi_with_empty_number_tags.dcm` & `pydicom-2.4.1/pydicom/data/test_files/reportsi_with_empty_number_tags.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/rtdose.dcm` & `pydicom-2.4.1/pydicom/data/test_files/rtdose.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/rtdose_1frame.dcm` & `pydicom-2.4.1/pydicom/data/test_files/rtdose_1frame.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/rtdose_expb.dcm` & `pydicom-2.4.1/pydicom/data/test_files/rtdose_expb.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/rtdose_expb_1frame.dcm` & `pydicom-2.4.1/pydicom/data/test_files/rtdose_expb_1frame.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/rtdose_rle.dcm` & `pydicom-2.4.1/pydicom/data/test_files/rtdose_rle.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/rtdose_rle_1frame.dcm` & `pydicom-2.4.1/pydicom/data/test_files/rtdose_rle_1frame.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/rtplan.dcm` & `pydicom-2.4.1/pydicom/data/test_files/rtplan.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/rtplan.dump` & `pydicom-2.4.1/pydicom/data/test_files/rtplan.dump`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/rtplan_truncated.dcm` & `pydicom-2.4.1/pydicom/data/test_files/rtplan_truncated.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/rtstruct.dcm` & `pydicom-2.4.1/pydicom/data/test_files/rtstruct.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/rtstruct.dump` & `pydicom-2.4.1/pydicom/data/test_files/rtstruct.dump`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/test-SR.dcm` & `pydicom-2.4.1/pydicom/data/test_files/test-SR.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/test1.json` & `pydicom-2.4.1/pydicom/data/test_files/test1.json`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/test_PN.json` & `pydicom-2.4.1/pydicom/data/test_files/test_PN.json`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/waveform_ecg.dcm` & `pydicom-2.4.1/pydicom/data/test_files/waveform_ecg.dcm`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/test_files/zipMR.gz` & `pydicom-2.4.1/pydicom/data/test_files/zipMR.gz`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/data/urls.json` & `pydicom-2.4.1/pydicom/data/urls.json`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/datadict.py` & `pydicom-2.4.1/pydicom/datadict.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/dataelem.py` & `pydicom-2.4.1/pydicom/dataelem.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/dataset.py` & `pydicom-2.4.1/pydicom/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,15 +465,16 @@
             warnings.warn(
                 "Dataset.parent will be removed in pydicom 3.0",
                 DeprecationWarning
             )
         self._parent = weakref.ref(value)
 
     def __deepcopy__(self, memo: Optional[Dict[int, Any]]) -> "Dataset":
-        copied = Dataset()
+        cls = self.__class__
+        copied = cls.__new__(cls)
         if memo:
             memo[id(self)] = copied   # add the new class to the memo
         # Insert a deepcopy of all instance attributes
         copied.__dict__.update(copy.deepcopy(self.__dict__, memo))
         # Manually update the weakref to be correct
         for elem in copied:  # DICOM elements
             if elem.VR == VR_.SQ:
```

### Comparing `pydicom-2.4.0/pydicom/dicomdir.py` & `pydicom-2.4.1/pydicom/dicomdir.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/encaps.py` & `pydicom-2.4.1/pydicom/encaps.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/encoders/base.py` & `pydicom-2.4.1/pydicom/encoders/base.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/encoders/gdcm.py` & `pydicom-2.4.1/pydicom/encoders/gdcm.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/encoders/native.py` & `pydicom-2.4.1/pydicom/encoders/native.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/encoders/pylibjpeg.py` & `pydicom-2.4.1/pydicom/encoders/pylibjpeg.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/env_info.py` & `pydicom-2.4.1/pydicom/env_info.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/errors.py` & `pydicom-2.4.1/pydicom/errors.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/filebase.py` & `pydicom-2.4.1/pydicom/filebase.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/filereader.py` & `pydicom-2.4.1/pydicom/filereader.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/fileset.py` & `pydicom-2.4.1/pydicom/fileset.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/fileutil.py` & `pydicom-2.4.1/pydicom/fileutil.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/filewriter.py` & `pydicom-2.4.1/pydicom/filewriter.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/jsonrep.py` & `pydicom-2.4.1/pydicom/jsonrep.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/misc.py` & `pydicom-2.4.1/pydicom/misc.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/multival.py` & `pydicom-2.4.1/pydicom/multival.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/overlays/numpy_handler.py` & `pydicom-2.4.1/pydicom/overlays/numpy_handler.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/pixel_data_handlers/gdcm_handler.py` & `pydicom-2.4.1/pydicom/pixel_data_handlers/gdcm_handler.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/pixel_data_handlers/jpeg_ls_handler.py` & `pydicom-2.4.1/pydicom/pixel_data_handlers/jpeg_ls_handler.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/pixel_data_handlers/numpy_handler.py` & `pydicom-2.4.1/pydicom/pixel_data_handlers/numpy_handler.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/pixel_data_handlers/pillow_handler.py` & `pydicom-2.4.1/pydicom/pixel_data_handlers/pillow_handler.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/pixel_data_handlers/pylibjpeg_handler.py` & `pydicom-2.4.1/pydicom/pixel_data_handlers/pylibjpeg_handler.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/pixel_data_handlers/rle_handler.py` & `pydicom-2.4.1/pydicom/pixel_data_handlers/rle_handler.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/pixel_data_handlers/util.py` & `pydicom-2.4.1/pydicom/pixel_data_handlers/util.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/sequence.py` & `pydicom-2.4.1/pydicom/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,16 @@
             raise TypeError("An iterable of 'Dataset' is required")
 
         super().extend(val)
         for ds in val:
             ds.parent_seq = self  # type: ignore
 
     def __deepcopy__(self, memo: Optional[Dict[int, Any]]) -> "Sequence":
-        copied = Sequence()
+        cls = self.__class__
+        copied = cls.__new__(cls)
         if memo is not None:
             memo[id(self)] = copied
         copied.__dict__.update(deepcopy(self.__dict__, memo))
         for ds in copied:
             ds.parent_seq = copied  # type:ignore
         return copied
```

### Comparing `pydicom-2.4.0/pydicom/sr/_cid_dict.py` & `pydicom-2.4.1/pydicom/sr/_cid_dict.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/sr/_concepts_dict.py` & `pydicom-2.4.1/pydicom/sr/_concepts_dict.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/sr/_snomed_dict.py` & `pydicom-2.4.1/pydicom/sr/_snomed_dict.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/sr/codedict.py` & `pydicom-2.4.1/pydicom/sr/codedict.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/sr/coding.py` & `pydicom-2.4.1/pydicom/sr/coding.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/tag.py` & `pydicom-2.4.1/pydicom/tag.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/uid.py` & `pydicom-2.4.1/pydicom/uid.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/util/codify.py` & `pydicom-2.4.1/pydicom/util/codify.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/util/dump.py` & `pydicom-2.4.1/pydicom/util/dump.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/util/fixer.py` & `pydicom-2.4.1/pydicom/util/fixer.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/util/hexutil.py` & `pydicom-2.4.1/pydicom/util/hexutil.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/util/leanread.py` & `pydicom-2.4.1/pydicom/util/leanread.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/valuerep.py` & `pydicom-2.4.1/pydicom/valuerep.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/values.py` & `pydicom-2.4.1/pydicom/values.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pydicom/waveforms/numpy_handler.py` & `pydicom-2.4.1/pydicom/waveforms/numpy_handler.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/pyproject.toml` & `pydicom-2.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 description = "A pure Python package for reading and writing DICOM data"
 #  dynamic = ["version"]  uncomment for pydicom v3.0
 keywords = ["dicom, python, medical, imaging"]
 license = {text = "MIT"}
 name = "pydicom"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "2.4.0" # remove for v3.0
+version = "2.4.1"
 
 
 [project.optional-dependencies]
 docs = [
         "numpy",
         "numpydoc",
         "matplotlib",
```

### Comparing `pydicom-2.4.0/setup.py` & `pydicom-2.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/source/generate_cids/generate_concept_dicts.py` & `pydicom-2.4.1/source/generate_cids/generate_concept_dicts.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/source/generate_dict/generate_dicom_dict.py` & `pydicom-2.4.1/source/generate_dict/generate_dicom_dict.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/source/generate_dict/generate_private_dict.py` & `pydicom-2.4.1/source/generate_dict/generate_private_dict.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/source/generate_dict/generate_uid_dict.py` & `pydicom-2.4.1/source/generate_dict/generate_uid_dict.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/source/generate_uids/generate_storage_sopclass_uids.py` & `pydicom-2.4.1/source/generate_uids/generate_storage_sopclass_uids.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/source/scripts/charlist.py` & `pydicom-2.4.1/source/scripts/charlist.py`

 * *Files identical despite different names*

### Comparing `pydicom-2.4.0/PKG-INFO` & `pydicom-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydicom
-Version: 2.4.0
+Version: 2.4.1
 Summary: A pure Python package for reading and writing DICOM data
 Keywords: dicom, python, medical, imaging
 Author-email: Darcy Mason and contributors <darcymason@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

