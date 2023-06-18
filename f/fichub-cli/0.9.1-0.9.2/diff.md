# Comparing `tmp/fichub-cli-0.9.1.tar.gz` & `tmp/fichub-cli-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Projects\Personal\Projects\Python\Others\fichub\fichub-cli\fichub-cli\dist\.tmp-hx578pc6\fichub-cli-0.9.1.tar", last modified: Sun Jan 29 07:21:55 2023, max compression
+gzip compressed data, was "D:\Projects\Personal\Projects\Langs\Python\Others\fichub\fichub-cli\fichub-cli\dist\.tmp-2wum0ush\fichub-cli-0.9.2.tar", last modified: Sun Jun 18 20:25:30 2023, max compression
```

## Comparing `fichub-cli-0.9.1.tar` & `fichub-cli-0.9.2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-01-29 07:21:55.043554 fichub-cli-0.9.1/
--rw-rw-rw-   0        0        0    11357 2022-04-28 17:27:29.000000 fichub-cli-0.9.1/LICENSE.txt
--rw-rw-rw-   0        0        0     5262 2023-01-29 07:21:55.043554 fichub-cli-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     4802 2023-01-28 09:21:49.000000 fichub-cli-0.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-29 07:21:55.008810 fichub-cli-0.9.1/fichub_cli/
--rw-rw-rw-   0        0        0       23 2023-01-29 07:15:45.000000 fichub-cli-0.9.1/fichub_cli/__init__.py
--rw-rw-rw-   0        0        0     7791 2023-01-28 09:37:39.000000 fichub-cli-0.9.1/fichub_cli/cli.py
-drwxrwxrwx   0        0        0        0 2023-01-29 07:21:55.042551 fichub-cli-0.9.1/fichub_cli/utils/
--rw-rw-rw-   0        0        0        0 2022-04-28 17:27:29.000000 fichub-cli-0.9.1/fichub_cli/utils/__init__.py
--rw-rw-rw-   0        0        0    11811 2023-01-28 09:21:49.000000 fichub-cli-0.9.1/fichub_cli/utils/fetch_data.py
--rw-rw-rw-   0        0        0     6123 2023-01-28 09:21:49.000000 fichub-cli-0.9.1/fichub_cli/utils/fichub.py
--rw-rw-rw-   0        0        0     2320 2022-05-02 15:35:09.000000 fichub-cli-0.9.1/fichub_cli/utils/logging.py
--rw-rw-rw-   0        0        0    14639 2023-01-29 07:14:45.000000 fichub-cli-0.9.1/fichub_cli/utils/processing.py
-drwxrwxrwx   0        0        0        0 2023-01-29 07:21:55.027159 fichub-cli-0.9.1/fichub_cli.egg-info/
--rw-rw-rw-   0        0        0     5262 2023-01-29 07:21:54.000000 fichub-cli-0.9.1/fichub_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-01-29 07:21:54.000000 fichub-cli-0.9.1/fichub_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-29 07:21:54.000000 fichub-cli-0.9.1/fichub_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-01-29 07:21:54.000000 fichub-cli-0.9.1/fichub_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      115 2023-01-29 07:21:54.000000 fichub-cli-0.9.1/fichub_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-01-29 07:21:54.000000 fichub-cli-0.9.1/fichub_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      229 2022-04-28 17:27:29.000000 fichub-cli-0.9.1/pyproject.toml
--rw-rw-rw-   0        0        0      114 2023-01-29 07:21:55.045553 fichub-cli-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1101 2023-01-29 07:15:45.000000 fichub-cli-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:25:30.635617 fichub-cli-0.9.2/
+-rw-rw-rw-   0        0        0    11558 2023-06-04 18:06:14.000000 fichub-cli-0.9.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     5262 2023-06-18 20:25:30.635617 fichub-cli-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4802 2023-06-04 18:06:14.000000 fichub-cli-0.9.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 20:25:30.613620 fichub-cli-0.9.2/fichub_cli/
+-rw-rw-rw-   0        0        0       23 2023-06-18 20:19:24.000000 fichub-cli-0.9.2/fichub_cli/__init__.py
+-rw-rw-rw-   0        0        0     7791 2023-06-04 18:06:14.000000 fichub-cli-0.9.2/fichub_cli/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:25:30.633616 fichub-cli-0.9.2/fichub_cli/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 18:06:14.000000 fichub-cli-0.9.2/fichub_cli/utils/__init__.py
+-rw-rw-rw-   0        0        0    11811 2023-06-04 18:06:14.000000 fichub-cli-0.9.2/fichub_cli/utils/fetch_data.py
+-rw-rw-rw-   0        0        0     6194 2023-06-18 20:24:03.000000 fichub-cli-0.9.2/fichub_cli/utils/fichub.py
+-rw-rw-rw-   0        0        0     2384 2023-06-04 18:06:14.000000 fichub-cli-0.9.2/fichub_cli/utils/logging.py
+-rw-rw-rw-   0        0        0    14639 2023-06-04 18:06:14.000000 fichub-cli-0.9.2/fichub_cli/utils/processing.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:25:30.629616 fichub-cli-0.9.2/fichub_cli.egg-info/
+-rw-rw-rw-   0        0        0     5262 2023-06-18 20:25:30.000000 fichub-cli-0.9.2/fichub_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-06-18 20:25:30.000000 fichub-cli-0.9.2/fichub_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 20:25:30.000000 fichub-cli-0.9.2/fichub_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-18 20:25:30.000000 fichub-cli-0.9.2/fichub_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      115 2023-06-18 20:25:30.000000 fichub-cli-0.9.2/fichub_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-18 20:25:30.000000 fichub-cli-0.9.2/fichub_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      233 2023-06-04 18:06:14.000000 fichub-cli-0.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0      114 2023-06-18 20:25:30.640616 fichub-cli-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     1101 2023-06-18 20:19:24.000000 fichub-cli-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:25:30.634618 fichub-cli-0.9.2/tests/
+-rw-rw-rw-   0        0        0     2227 2023-06-18 20:19:24.000000 fichub-cli-0.9.2/tests/test_cli.py
```

### Comparing `fichub-cli-0.9.1/LICENSE.txt` & `fichub-cli-0.9.2/LICENSE.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `fichub-cli-0.9.1/PKG-INFO` & `fichub-cli-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fichub-cli
-Version: 0.9.1
+Version: 0.9.2
 Summary: A CLI for the fichub.net API
 Home-page: https://github.com/FicHub/fichub-cli
 Author: Arbaaz Laskar
 Author-email: arzkar.dev@gmail.com
 License: Apache License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fichub-cli-0.9.1/README.md` & `fichub-cli-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `fichub-cli-0.9.1/fichub_cli/cli.py` & `fichub-cli-0.9.2/fichub_cli/cli.py`

 * *Files identical despite different names*

### Comparing `fichub-cli-0.9.1/fichub_cli/utils/fetch_data.py` & `fichub-cli-0.9.2/fichub_cli/utils/fetch_data.py`

 * *Files identical despite different names*

### Comparing `fichub-cli-0.9.1/fichub_cli/utils/fichub.py` & `fichub-cli-0.9.2/fichub_cli/utils/fichub.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import requests
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
-
+import traceback
 import re
 import time
 from colorama import Fore, Style
 from tqdm import tqdm
 from loguru import logger
 from fichub_cli import __version__
 
@@ -64,27 +64,27 @@
                 if self.debug:
                     logger.debug(
                         f"GET: {response.status_code}: {response.url}")
                     if self.automated:
                         logger.debug(
                             f"Headers: {response.request.headers}")
                 break
-            except (ConnectionError, TimeoutError, Exception) as e:
+            except (requests.exceptions.ConnectionError, requests.exceptions.Timeout) as e:
                 if self.debug:
                     logger.error(str(traceback.format_exc()))
                 tqdm.write("\n" + Fore.RED + str(e) + Style.RESET_ALL +
                            Fore.GREEN + "\nWill retry in 3s!" +
                            Style.RESET_ALL)
                 time.sleep(3)
 
         try:
             self.response = response.json()
-            self.file_format =[]
+            self.file_format = []
             self.cache_hash = {}
-            cache_urls= {}
+            cache_urls = {}
 
             for format in format_type:
                 if format == 0:
                     cache_urls['epub'] = self.response['urls']['epub']
                     self.cache_hash['epub'] = self.response['hashes']['epub']
                     self.file_format.append(".epub")
 
@@ -95,25 +95,25 @@
 
                 elif format == 2:
                     cache_urls['pdf'] = self.response['urls']['pdf']
                     self.cache_hash['pdf'] = self.response['hashes']['epub']
                     self.file_format.append(".pdf")
 
                 elif format == 3:
-                    cache_urls['zip'] =self.response['urls']['html']
+                    cache_urls['zip'] = self.response['urls']['html']
                     self.cache_hash['zip'] = self.response['hashes']['epub']
                     self.file_format.append(".zip")
-            
+
             self.files = {}
             self.files["meta"] = self.response['meta']
             for file_format in self.file_format:
                 self.files[self.response['urls']['epub'].split(
-                "/")[4].split("?")[0].replace(".epub", file_format)] = {
-                "hash": self.cache_hash[file_format.replace(".","")],
-                "download_url": "https://fichub.net"+cache_urls[file_format.replace(".","")]
+                    "/")[4].split("?")[0].replace(".epub", file_format)] = {
+                    "hash": self.cache_hash[file_format.replace(".", "")],
+                    "download_url": "https://fichub.net" + cache_urls[file_format.replace(".", "")]
                 }
         # Error: 'epub_url'
         # Reason: Unsupported URL
         except (KeyError, UnboundLocalError) as e:
             if self.debug:
                 logger.error(f"Error: {str(e)} not found!")
                 logger.error(
@@ -141,14 +141,14 @@
                 self.response_data = self.http.get(
                     download_url, allow_redirects=True, headers=headers,
                     params=params, timeout=(6.1, 300))
                 if self.debug:
                     logger.debug(
                         f"GET: {self.response_data.status_code}: {self.response_data.url}")
                 break
-            except (ConnectionError, TimeoutError, Exception) as e:
+            except (requests.exceptions.ConnectionError, requests.exceptions.Timeout) as e:
                 if self.debug:
                     logger.error(str(traceback.format_exc()))
                 tqdm.write("\n" + Fore.RED + str(e) + Style.RESET_ALL +
                            Fore.GREEN + "\nWill retry in 3s!" +
                            Style.RESET_ALL)
                 time.sleep(3)
```

### Comparing `fichub-cli-0.9.1/fichub_cli/utils/logging.py` & `fichub-cli-0.9.2/fichub_cli/utils/logging.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-# Copyright 2021 Arbaaz Laskar
-
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-
-#   http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from colorama import Fore
-from loguru import logger
-from tqdm import tqdm
-from datetime import datetime
-
-
-def init_log(debug: bool, force: bool):
-    if debug:
-        if force:
-            logger.warning(
-                "--force flag was passed. Files will be overwritten.")
-    if force:
-        tqdm.write(
-            Fore.YELLOW +
-            "WARNING: --force flag was passed. Files will be overwritten.")
-
-
-def downloaded_log(debug: bool, file_name: str):
-    if debug:
-        logger.info(f"Downloaded '{file_name}'")
-    tqdm.write(Fore.GREEN + f"Downloaded '{file_name}'")
-
-
-def download_processing_log(debug: bool, url: str):
-    if debug:
-        logger.info(f"Processing {url.strip()}")
-    tqdm.write(Fore.BLUE + f"\nProcessing {url.strip()}")
-
-
-def verbose_log(debug: bool, fic):
-    try:
-        if debug:
-            logger.info(" Title: " +
-                        str(fic.response['meta']['title'])
-                        + " | Total Chapters: " +
-                        str(fic.response['meta']['chapters'])
-                        + " | Last Scrape: " + datetime
-                        .strptime(str(fic.response['meta']['updated']), "%Y-%m-%dT%H:%M:%S")
-                        .strftime("%d %b, %Y at %H:%M:%S"))
-        tqdm.write(Fore.MAGENTA
-                   + "Title: " +
-                   str(fic.response['meta']['title'])
-                   + "\nTotal Chapters: " +
-                   str(fic.response['meta']['chapters'])
-                   + "\nLast Updated: " + datetime
-                   .strptime(str(fic.response['meta']['updated']), "%Y-%m-%dT%H:%M:%S")
-                   .strftime("%d %b, %Y at %H:%M:%S"))
-    # Error: KeyError: 'meta'
-    # Reason: Unsupported url
-    except KeyError:
+# Copyright 2021 Arbaaz Laskar
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from colorama import Fore
+from loguru import logger
+from tqdm import tqdm
+from datetime import datetime
+
+
+def init_log(debug: bool, force: bool):
+    if debug:
+        if force:
+            logger.warning(
+                "--force flag was passed. Files will be overwritten.")
+    if force:
+        tqdm.write(
+            Fore.YELLOW +
+            "WARNING: --force flag was passed. Files will be overwritten.")
+
+
+def downloaded_log(debug: bool, file_name: str):
+    if debug:
+        logger.info(f"Downloaded '{file_name}'")
+    tqdm.write(Fore.GREEN + f"Downloaded '{file_name}'")
+
+
+def download_processing_log(debug: bool, url: str):
+    if debug:
+        logger.info(f"Processing {url.strip()}")
+    tqdm.write(Fore.BLUE + f"\nProcessing {url.strip()}")
+
+
+def verbose_log(debug: bool, fic):
+    try:
+        if debug:
+            logger.info(" Title: " +
+                        str(fic.response['meta']['title'])
+                        + " | Total Chapters: " +
+                        str(fic.response['meta']['chapters'])
+                        + " | Last Scrape: " + datetime
+                        .strptime(str(fic.response['meta']['updated']), "%Y-%m-%dT%H:%M:%S")
+                        .strftime("%d %b, %Y at %H:%M:%S"))
+        tqdm.write(Fore.MAGENTA
+                   + "Title: " +
+                   str(fic.response['meta']['title'])
+                   + "\nTotal Chapters: " +
+                   str(fic.response['meta']['chapters'])
+                   + "\nLast Updated: " + datetime
+                   .strptime(str(fic.response['meta']['updated']), "%Y-%m-%dT%H:%M:%S")
+                   .strftime("%d %b, %Y at %H:%M:%S"))
+    # Error: KeyError: 'meta'
+    # Reason: Unsupported url
+    except KeyError:
         pass
```

### Comparing `fichub-cli-0.9.1/fichub_cli/utils/processing.py` & `fichub-cli-0.9.2/fichub_cli/utils/processing.py`

 * *Files identical despite different names*

### Comparing `fichub-cli-0.9.1/fichub_cli.egg-info/PKG-INFO` & `fichub-cli-0.9.2/fichub_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fichub-cli
-Version: 0.9.1
+Version: 0.9.2
 Summary: A CLI for the fichub.net API
 Home-page: https://github.com/FicHub/fichub-cli
 Author: Arbaaz Laskar
 Author-email: arzkar.dev@gmail.com
 License: Apache License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fichub-cli-0.9.1/setup.py` & `fichub-cli-0.9.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 setup(
     name='fichub-cli',
     author='Arbaaz Laskar',
     author_email="arzkar.dev@gmail.com",
     description="A CLI for the fichub.net API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.9.1",
+    version="0.9.2",
     license='Apache License',
     url="https://github.com/FicHub/fichub-cli",
     packages=find_packages(include=['fichub_cli', 'fichub_cli.*']),
     include_package_data=True,
     install_requires=[
         'typer>=0.4.0',
-        'requests>=2.25.1',
+        'requests>=2.31.0',
         'loguru>=0.6.0',
         'tqdm>=4.60.0',
         'BeautifulSoup4>=4.9.3',
         'colorama>=0.4.4',
         'platformdirs>=2.5.1'
     ],
     entry_points= {
```

