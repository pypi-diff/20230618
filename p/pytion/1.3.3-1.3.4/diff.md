# Comparing `tmp/pytion-1.3.3.tar.gz` & `tmp/pytion-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytion-1.3.3.tar", last modified: Wed Jan  4 16:17:58 2023, max compression
+gzip compressed data, was "pytion-1.3.4.tar", last modified: Sun Jun 18 19:28:11 2023, max compression
```

## Comparing `pytion-1.3.3.tar` & `pytion-1.3.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-01-04 16:17:58.355475 pytion-1.3.3/
--rw-rw-rw-   0        0        0    35802 2021-10-23 13:52:40.000000 pytion-1.3.3/LICENSE
--rw-rw-rw-   0        0        0    27058 2023-01-04 16:17:58.354476 pytion-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    26271 2023-01-04 15:55:17.000000 pytion-1.3.3/README.md
--rw-rw-rw-   0        0        0       84 2022-05-03 14:01:39.000000 pytion-1.3.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-01-04 16:17:58.303816 pytion-1.3.3/pytion/
--rw-rw-rw-   0        0        0     1565 2022-03-29 20:12:51.000000 pytion-1.3.3/pytion/__init__.py
--rw-rw-rw-   0        0        0    26375 2023-01-04 14:53:25.000000 pytion-1.3.3/pytion/api.py
--rw-rw-rw-   0        0        0      823 2022-07-28 09:30:54.000000 pytion-1.3.3/pytion/envs.py
--rw-rw-rw-   0        0        0     6376 2022-03-29 20:12:51.000000 pytion-1.3.3/pytion/exceptions.py
--rw-rw-rw-   0        0        0    42384 2023-01-04 16:00:35.000000 pytion-1.3.3/pytion/models.py
--rw-rw-rw-   0        0        0    10749 2023-01-02 18:09:24.000000 pytion-1.3.3/pytion/query.py
-drwxrwxrwx   0        0        0        0 2023-01-04 16:17:58.332563 pytion-1.3.3/pytion.egg-info/
--rw-rw-rw-   0        0        0    27058 2023-01-04 16:17:58.000000 pytion-1.3.3/pytion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-01-04 16:17:58.000000 pytion-1.3.3/pytion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-04 16:17:58.000000 pytion-1.3.3/pytion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-01-04 16:17:58.000000 pytion-1.3.3/pytion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-01-04 16:17:58.000000 pytion-1.3.3/pytion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-04 16:17:58.355475 pytion-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1113 2023-01-02 13:18:26.000000 pytion-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-04 16:17:58.353474 pytion-1.3.3/tests/
--rw-rw-rw-   0        0        0        0 2022-04-30 21:11:37.000000 pytion-1.3.3/tests/__init__.py
--rw-rw-rw-   0        0        0      260 2022-07-28 15:28:48.000000 pytion-1.3.3/tests/conftest.py
--rw-rw-rw-   0        0        0      789 2022-09-26 21:28:52.000000 pytion-1.3.3/tests/fixtures.py
--rw-rw-rw-   0        0        0    31791 2023-01-04 14:55:58.000000 pytion-1.3.3/tests/test_api.py
--rw-rw-rw-   0        0        0     4655 2023-01-04 15:49:39.000000 pytion-1.3.3/tests/test_models.py
--rw-rw-rw-   0        0        0     8511 2023-01-04 15:03:01.000000 pytion-1.3.3/tests/test_query.py
+drwxr-xr-x   0 petrpaluba   (501) staff       (20)        0 2023-06-18 19:28:11.383852 pytion-1.3.4/
+-rw-r--r--   0 petrpaluba   (501) staff       (20)    35129 2023-06-16 21:36:37.000000 pytion-1.3.4/LICENSE
+-rw-r--r--   0 petrpaluba   (501) staff       (20)    32545 2023-06-18 19:28:11.383716 pytion-1.3.4/PKG-INFO
+-rw-r--r--   0 petrpaluba   (501) staff       (20)    31726 2023-06-18 19:24:21.000000 pytion-1.3.4/README.md
+-rw-r--r--   0 petrpaluba   (501) staff       (20)       81 2023-06-16 21:36:37.000000 pytion-1.3.4/pyproject.toml
+drwxr-xr-x   0 petrpaluba   (501) staff       (20)        0 2023-06-18 19:28:11.381861 pytion-1.3.4/pytion/
+-rw-r--r--   0 petrpaluba   (501) staff       (20)     1520 2023-06-16 21:36:37.000000 pytion-1.3.4/pytion/__init__.py
+-rw-r--r--   0 petrpaluba   (501) staff       (20)    25773 2023-06-18 19:24:16.000000 pytion-1.3.4/pytion/api.py
+-rw-r--r--   0 petrpaluba   (501) staff       (20)      790 2023-06-16 21:36:37.000000 pytion-1.3.4/pytion/envs.py
+-rw-r--r--   0 petrpaluba   (501) staff       (20)     6192 2023-06-16 21:36:37.000000 pytion-1.3.4/pytion/exceptions.py
+-rw-r--r--   0 petrpaluba   (501) staff       (20)    43082 2023-06-18 19:24:21.000000 pytion-1.3.4/pytion/models.py
+-rw-r--r--   0 petrpaluba   (501) staff       (20)    10490 2023-06-16 21:36:37.000000 pytion-1.3.4/pytion/query.py
+drwxr-xr-x   0 petrpaluba   (501) staff       (20)        0 2023-06-18 19:28:11.382587 pytion-1.3.4/pytion.egg-info/
+-rw-r--r--   0 petrpaluba   (501) staff       (20)    32545 2023-06-18 19:28:11.000000 pytion-1.3.4/pytion.egg-info/PKG-INFO
+-rw-r--r--   0 petrpaluba   (501) staff       (20)      405 2023-06-18 19:28:11.000000 pytion-1.3.4/pytion.egg-info/SOURCES.txt
+-rw-r--r--   0 petrpaluba   (501) staff       (20)        1 2023-06-18 19:28:11.000000 pytion-1.3.4/pytion.egg-info/dependency_links.txt
+-rw-r--r--   0 petrpaluba   (501) staff       (20)       17 2023-06-18 19:28:11.000000 pytion-1.3.4/pytion.egg-info/requires.txt
+-rw-r--r--   0 petrpaluba   (501) staff       (20)       13 2023-06-18 19:28:11.000000 pytion-1.3.4/pytion.egg-info/top_level.txt
+-rw-r--r--   0 petrpaluba   (501) staff       (20)       38 2023-06-18 19:28:11.383890 pytion-1.3.4/setup.cfg
+-rw-r--r--   0 petrpaluba   (501) staff       (20)     1131 2023-06-18 19:24:21.000000 pytion-1.3.4/setup.py
+drwxr-xr-x   0 petrpaluba   (501) staff       (20)        0 2023-06-18 19:28:11.383482 pytion-1.3.4/tests/
+-rw-r--r--   0 petrpaluba   (501) staff       (20)        0 2023-06-16 21:36:37.000000 pytion-1.3.4/tests/__init__.py
+-rw-r--r--   0 petrpaluba   (501) staff       (20)      260 2023-06-16 21:43:38.000000 pytion-1.3.4/tests/conftest.py
+-rw-r--r--   0 petrpaluba   (501) staff       (20)      884 2023-06-18 19:24:21.000000 pytion-1.3.4/tests/fixtures.py
+-rw-r--r--   0 petrpaluba   (501) staff       (20)    31120 2023-06-16 21:36:37.000000 pytion-1.3.4/tests/test_api.py
+-rw-r--r--   0 petrpaluba   (501) staff       (20)     8485 2023-06-18 19:24:21.000000 pytion-1.3.4/tests/test_models.py
+-rw-r--r--   0 petrpaluba   (501) staff       (20)     8300 2023-06-18 19:24:21.000000 pytion-1.3.4/tests/test_query.py
```

### Comparing `pytion-1.3.3/LICENSE` & `pytion-1.3.4/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
+GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `pytion-1.3.3/PKG-INFO` & `pytion-1.3.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,482 +1,580 @@
-Metadata-Version: 2.1
-Name: pytion
-Version: 1.3.3
-Summary: Unofficial Python client for official Notion API
-Home-page: https://github.com/lastorel/pytion
-Author: Yegor Gomzin
-Author-email: slezycmex@mail.ru
-Project-URL: Bug Tracker, https://github.com/lastorel/pytion/issues
-Project-URL: Changelog, https://github.com/lastorel/pytion/blob/main/CHANGELOG.md
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pytion
-
-[![PyPI](https://img.shields.io/pypi/v/pytion.svg)](https://pypi.org/project/pytion)
-![PyVersion](https://img.shields.io/pypi/pyversions/pytion)
-![CodeSize](https://img.shields.io/github/languages/code-size/lastorel/pytion)
-[![LICENSE](https://img.shields.io/github/license/lastorel/pytion)](LICENSE)
-
-Independent unofficial **Python client** for the official **Notion API** (for internal integrations only)
-
-Client is built with its own object model based on API
-
-So if you are using **notion.so** and want to automate some stuff with the original API, you're welcome!  
-You can read any available data, create basic models, and even work with databases.
-
-Current Notion API version = **"2022-06-28"**
-
-_*does not use notion-sdk-py client_
-
-See [Change Log](./CHANGELOG.md)
-
-# Contents
-
-1. [Quick Start](#quick-start)
-2. [Pytion API](#pytion-api)
-   1. [Searching](#search)
-   2. [pytion.api.Element](#pytionapielement)
-3. [Models](#models)
-   1. [pytion.models](#pytionmodels)
-   2. [Supported Property types](#supported-property-types)
-   3. [Supported block types](#supported-block-types)
-      1. [Block creating examples](#block-creating-examples)
-      2. [Block deleting](#block-deleting)
-   4. [Database operations](#database-operations)
-      1. [Retrieving](#retrieving)
-4. [Logging](#logging)
-
-# Quick start
-
-```
-pip install pytion
-```
-
-Create new integration and get your Notion API Token at notion.so -> [here](https://www.notion.com/my-integrations).  
-Invite your new integration 'manager' to your pages or databases.
-
-```python
-from pytion import Notion; no = Notion(token=SOME_TOKEN)
-```
-
-Or put your token for Notion API into file `token` at script directory and use simple `no = Notion()`
-
-```python
-from pytion import Notion
-no = Notion(token=SOME_TOKEN)
-page = no.pages.get("PAGE ID")  # retrieve page data (not content) and create object
-blocks = page.get_block_children()  # retrieve page content and create list of objects
-database = no.databases.get("Database ID")  # retrieve database data (not content) and create object
-# retrieve database content by filtering with sorting
-pages = database.db_filter(property_name="Done", property_type="checkbox", value=False, descending="title")
-```
-
-```
-In [1]: from pytion import Notion
-
-In [2]: no = Notion(token=SOME_TOKEN)
-
-In [3]: page = no.pages.get("a458613160da45fa96367c8a594297c7")
-In [4]: print(page)
-Notion/pages/Page(Example page)
-
-In [5]: blocks = page.get_block_children_recursive()
-
-In [6]: print(blocks)
-Notion/blocks/BlockArray(## Migration planning [x] Rese)
-
-In [7]: print(blocks.obj)
-## Migration planning
-[x] Reset new switch 2022-05-12T00:00:00.000+03:00 → 2022-05-13T01:00:00.000+03:00 
-	- reboot
-	- hold reset button
-[x] Connect to console with baud rate 9600
-[ ] Skip default configuration dialog
-Use LinkTo(configs) 
-[Integration changes](https://developers.notion.com/changelog?page=2)
-
-In [8]: print(blocks.obj.simple)
-Migration planning
-Reset new switch 2022-05-12T00:00:00.000+03:00 → 2022-05-13T01:00:00.000+03:00 
-	reboot
-	hold reset button
-Connect to console with baud rate 9600
-Skip default configuration dialog
-Use https://api.notion.com/v1/pages/90ea1231865f4af28055b855c2fba267 
-https://developers.notion.com/changelog?page=2
-```
-
-# Pytion API
-
-Almost all operations are carried out through `Notion` or `Element` object:
-
-```python
-page = no.pages.get("a458613160da45fa96367c8a594297c7")
-
-# no -> Notion
-# pages -> URI in https://api.notion.com/v1/PAGES/a458613160da45fa96367c8a594297c7
-# get -> pytion API method
-# page -> Element
-# page.obj -> Page (main data structure)
-```
-
-so:
-
-- `isinstance(no, Notion) == True`
-- `isinstance(no.pages, Element) == True`
-- `isinstance(no.databases, Element) == True`
-- `isinstance(page, Element) == True`
-- `isinstance(page.obj, Page) == True`
-
-and if you want to retrieve a database - you must use _"databases"_ URI
-
-```python
-database = no.databases.get("123412341234")
-```
-
-and the same applies for _"blocks"_ and _"users"_. Valid URI-s are:
-
-- _pages_
-- _blocks_
-- _databases_
-- _users_
-
-When you work with existing `Element` object like `page` above, all [methods](#pytionapielement) below will be applied to this Page:
-
-```python
-new_page = page.page_update(title="new page name 2")
-
-# new_page is not a new page, it is updated page
-# new_page.obj is equal page.obj except title and last_edited properties
-```
-
-## Search
-
-There is a search example:
-```python
-no = Notion(token)
-
-r = no.search("updating", object_type="page")
-print(r.obj)
-# output:
-# Page for updating
-# Page to updating databases
-```
-
-
-## pytion.api.Element
-
-There is a list of available methods for communicate with **api.notion.com**. These methods are better structured in [next chapter](#pytionmodels).
-
-`.get(id_)` - Get Element by ID.
-
-`.get_parent(id_)` - Get parent object of current object if possible.
-
-`.get_block_children(id_, limit)` - Get children Block objects of current Block object (tabulated texts) if exist.
-
-`.get_block_children_recursive(id_, max_depth, limit, force)` - Get children Block objects of current Block object (tabulated texts) if exist recursive.
-
-`.get_page_property(property_id, id_, limit)` - Retrieve a page property item.
-
-`.get_page_properties(title_only, obj)` - Retrieve the title or all properties of current Page or Page `obj`
-*(deprecated, useful for v1.3.0 only)*
-
-`.db_query(id_, limit, filter_, sorts)` - Query Database.
-
-`.db_filter(...see desc...)` - Query Database.
-
-`.db_create(database_obj, parent, properties, title)` - Create Database.
-
-**_There is no way to delete a database object yet!_**
-
-`.db_update(id_, title, properties)` - Update Database.
-
-`.page_create(page_obj, parent, properties, title)` - Create Page.
-
-`.page_update(id_, properties, title, archived)` - Update Page.
-
-`.block_update(id_, block_obj, new_text, archived)` - Update text in Block.
-
-`.block_append(id_, block, blocks)` - Append block or blocks children.
-
-`.get_myself()` - Retrieve my bot User.
-
-`.from_linkto(linkto)` - Creates new Element object based on LinkTo information.
-
-`.from_object(model)` - Creates new Element object from Page, Block or Database object. Usable while Element object contains an Array.
-
-> More details and usage examples of these methods you can see into func descriptions.
-
-# Models
-
-### pytion.models
-
-There are classes **based on API** structures:
-
-- `RichText` based on [Rich text object](https://developers.notion.com/reference/rich-text)
-- `RichTextArray` is a list of RichText objects with useful methods
-  - You can create object by simple `RichTextArray.create("My title text")` and then use it in any methods
-  - Any Rich Text getting from API will be RichTextArray
-  - `str()` returns plain text of all "Rich Texts". ez
-  - `+` operator is available with `str` and `RichTextArray`
-  - `.simple` property returns stripped plain text without any markdown syntax. useful for URL
-- `Database` based on [Database object](https://developers.notion.com/reference/database)
-  - You can create object `Database.create(...)` and/or use `.db_create(...)` API method
-  - attrs represent API model. Complex structures like `created_by` are wrapped in internal objects
-  - use `.db_update()` API method for modify a real database (for ex. properties or title)
-  - use `.db_query()` to get all database content (it will be `PageArray`)
-  - use `.db_filter()` to get database content with filtering and/or sorting
-  - has `.description` attr
-  - has `.is_inline` attr with the value True if the database appears in the page as an inline block
-- `Page` based on [Page object](https://developers.notion.com/reference/page)
-  - You can create object `Page.create(...)` and/or use `.page_create(...)` API method
-  - use `.page_update()` method to modify attributes or delete the page
-  - use `.get_block_children()` to get page content (without nested blocks) (it will be `BlockArray`)
-  - use `.get_block_children_recursive()` to get page content with nested blocks
-  - use `.get_page_property()` to retrieve the specific `PropertyValue` of the page
-- `Block` based on [Block object](https://developers.notion.com/reference/block)
-  - You can create object `Block.create(...)` of specific type from [_support matrix_](#supported-block-types) below and then use it while creating pages or appending
-  - use `.block_update()` to replace content or change _extension attributes_ or delete the block
-  - use `.block_append()` to add a new block to a page or add a nested block to another block
-  - use `.get_block_children()` to get first level nested blocks
-  - use `.get_block_children_recursive()` to get all levels nested blocks
-- `User` based on [User object](https://developers.notion.com/reference/user)
-  - You can create object `User.create(...)` and use it in some properties like `people` type property
-  - You can retrieve more data about a User by his ID using `.get()`
-  - use `.get_myself()` to retrieve the current bot User
-  - has `.workspace_name` attr for `bot` type users
-- `Property` based on [Property object](https://developers.notion.com/reference/property-object)
-  - You can create object `Property.create(...)` while creating or editing database: `.db_create()` or `.db_update()`
-  - `formula`, `rollup` type properties configuration is not supported
-- `PropertyValue` based on [Property values](https://developers.notion.com/reference/property-value-object)
-  - You can create object `PropertyValue.create(...)` to set or edit page properties by `.page_create()` or `.page_update()`
-  - `files`, `formula`, `rollup` type properties are not editable
-
-There are also useful **internal** classes:
-
-- `BlockArray` is found when API returns page content in "list of blocks" format
-  - it is useful to represent all content by `str()`
-  - also it has `simple` property like `RichTextArray` object
-  - it automatically indents `str` output of nested blocks
-- `PageArray` is found when API returns the result of database query (list of pages)
-- `LinkTo` is basic internal model to link to any Notion object
-  - You can create object `LinkTo.create()` and use it in many places and methods
-  - use `LinkTo(from_object=my_page1)` to quickly create a link to any existing object of pytion.models
-  - `link` property of `LinkTo` returns expanded URL
-- `ElementArray` is found while using `.search()` endpoint. It's a parent of `PageArray`
-
-> And every model has a `.get()` method that returns API friendly JSON.
- 
-### Supported Property types
-
-| Property type            | value type          | read (DB) | read value (Page) | create (DB) | create value (Page) | Oper attrs                          | Config attrs                        |
-|--------------------------|---------------------|-----------|-------------------|-------------|---------------------|-------------------------------------|-------------------------------------|
-| `title`                  | `RichTextArray`     | +         | +                 | +           | +                   |                                     |                                     |
-| `rich_text`              | `RichTextArray`     | +         | +                 | +           | +                   |                                     |                                     |
-| `number`                 | `int`/`float`       | +         | +                 | +           | +                   |                                     | ~~format~~                          |
-| `select`                 | `str`               | +         | +                 | +           | +                   |                                     | ~~options~~                         |
-| `multi_select`           | `List[str]`         | +         | +                 | +           | +                   |                                     | ~~options~~                         |
-| `status`                 | `str`               | +         | +                 | +           | +\*\*\*\*           |                                     | `options`, `groups` (read-only)     |
-| `date`                   | `str`               | +         | +                 | +           | +                   | `start: datetime` `end: datetime`\* |                                     |
-| `people`                 | `List[User]`        | +         | +                 | +           | +\*\*               |                                     |                                     |
-| `files`                  |                     | +         | -                 | +           | -                   |                                     |                                     |
-| `checkbox`               | `bool`              | +         | +                 | +           | +                   |                                     |                                     |
-| `url`                    | `str`               | +         | +                 | +           | +                   |                                     |                                     |
-| `email`                  | `str`               | +         | +                 | +           | +                   |                                     |                                     |
-| `phone_number`           | `str`               | +         | +                 | +           | +                   |                                     |                                     |
-| `formula`                |                     | -         | +                 | -           | -                   |                                     |                                     |
-| `relation`               | `List[LinkTo]`      | +         | +                 | +           | +                   | `has_more: bool`                    | `single_property` / `dual_property` |
-| `rollup`                 | depends on relation | -         | +                 | -           | -                   |                                     |                                     |
-| `created_time`\*\*\*     | `datetime`          | +         | +                 | +           | -                   |                                     |                                     |
-| `created_by`\*\*\*       | `User`              | +         | +                 | +           | -                   |                                     |                                     |
-| `last_edited_time`\*\*\* | `datetime`          | +         | +                 | +           | -                   |                                     |                                     |
-| `last_edited_by`\*\*\*   | `User`              | +         | +                 | +           | -                   |                                     |                                     |
-
-> [\*] - Create examples:  
-> `pv = PropertyValue.create(type_="date", value=datetime.now())`  
-> `pv = PropertyValue.create(type_="date", date={"start": str(datetime(2022, 2, 1, 5)), "end": str(datetime.now())})`  
-> [\*\*] - Create example:  
-> `user = User.create('1d393ffb5efd4d09adfc2cb6738e4812')`  
-> `pv = PropertyValue.create(type_="people", value=[user])`  
-> [\*\*\*] - Every Base model like Page already has mandatory attributes created/last_edited returned by API  
-> [\*\*\*\*] - Status type is not configurable. API doesn't support NEW options added via Property modify or updating a Page
-
-
-## Supported block types
-
-At present the API only supports the block types which are listed in the reference below. Any unsupported block types will continue to appear in the structure, but only contain a `type` set to `"unsupported"`.
-Colors are not yet supported.
-
-Every Block has mandatory attributes and extension attributes. There are mandatory:
-
-- `id: str` - UUID-64 without hyphens
-- `object: str` - always `"block"` (from API)
-- `created_time: datetime` - from API
-- `created_by: User` - from API
-- `last_edited_time: datetime` - from API
-- `last_edited_by: User` - from API
-- `type: str` - the type of block (from API)
-- `has_children: bool` - does the block have children blocks (from API)
-- `archived: bool` - does the block marked as deleted (from API)
-- `text: Union[str, RichTextArray]` - **main content**
-- `simple: str` - only simple text string (url expanded)
-
-Extension attributes are listed below in support matrix:
-
-| Block Type           | Description                               | Read support | Create support | Can have children | Extension attributes                              |
-|----------------------|-------------------------------------------|--------------|----------------|-------------------|---------------------------------------------------|
-| `paragraph`          | Simple Block with text                    | +            | +              | +                 |                                                   |
-| `heading_1`          | Heading Block with text highest level     | +            | +              | -/+\*             | `is_toggleable: bool`                             |
-| `heading_2`          | Heading Block with text medium level      | +            | +              | -/+\*             | `is_toggleable: bool`                             |
-| `heading_3`          | Heading Block with text lowest level      | +            | +              | -/+\*             | `is_toggleable: bool`                             |
-| `bulleted_list_item` | Text Block with bullet                    | +            | -              | +                 |                                                   |
-| `numbered_list_item` | Text Block with number                    | +            | -              | +                 |                                                   |
-| `to_do`              | Text Block with checkbox                  | +            | +              | +                 | `checked: bool`                                   |
-| `toggle`             | Text Block with toggle to children blocks | +            | -              | +                 |                                                   |
-| `code`               | Text Block with code style                | +            | +              | +                 | `language: str`, `caption: RichTextArray`         |
-| `child_page`         | Page inside                               | +            | -              | +                 |                                                   |
-| `child_database`     | Database inside                           | +            | -              | +                 |                                                   |
-| `embed`              | Embed online content                      | +            | -              | -                 | `caption: RichTextArray`                          |
-| `image`              | Embed image content                       | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
-| `video`              | Embed video content                       | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
-| `file`               | Embed file content                        | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
-| `pdf`                | Embed pdf content                         | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
-| `bookmark`           | Block for URL Link                        | +            | -              | -                 | `caption: RichTextArray`                          |
-| `callout`            | Highlighted footnote text Block           | +            | -              | +                 | `icon: dict`                                      |
-| `quote`              | Text Block with quote style               | +            | -              | +                 |                                                   |
-| `equation`           | KaTeX compatible text Block               | +            | -              | -                 |                                                   |
-| `divider`            | Simple line to divide the page            | +            | -              | -                 |                                                   |
-| `table_of_contents`  | Block with content structure in the page  | +            | -              | -                 |                                                   |
-| `column`             |                                           | -            | -              | +                 |                                                   |
-| `column_list`        |                                           | -            | -              | -                 |                                                   |
-| `link_preview`       | Same as `bookmark`                        | +            | -              | -                 |                                                   |
-| `synced_block`       | Block for synced content aka parent       | +            | -              | +                 | `synced_from: LinkTo`                             |
-| `template`           | Template Block title                      | +            | -              | +                 |                                                   |
-| `link_to_page`       | Block with link to particular page `@...` | +            | -              | -                 | `link: LinkTo`                                    |
-| `table`              | Table Block with some attrs               | +            | -              | +                 | `table_width: int`                                |
-| `table_row`          | Children Blocks with table row content    | +            | -              | -                 |                                                   |
-| `breadcrumb`         | Empty Block actually                      | +            | -              | -                 |                                                   |
-| `unsupported`        | Blocks unsupported by API                 | +            | -              | -                 |                                                   |
-
-> [\*] - `heading_X` blocks can have children if `is_toggleable` is True 
-
-### Block creating examples
-
-Create `paragraph` block object and add it to Notion:
-
-```python
-from pytion.models import Block
-my_text_block = Block.create("Hello World!")
-my_text_block = Block.create(text="Hello World!", type_="paragraph")  # the same
-
-# indented append my block to other known block:
-no.blocks.block_append("5f60073a9dda4a9c93a212a74a107359", block=my_text_block)
-
-# append my block to a known page (in the end)
-no.blocks.block_append("9796f2525016128d9af4bf12b236b555", block=my_text_block)  # the same operation actually
-
-# another way to append:
-my_page = no.pages.get("9796f2525016128d9af4bf12b236b555")
-my_page.block_append(block=my_text_block)
-```
-
-Create `to_do` block object:
-
-```python
-from pytion.models import Block
-my_todo_block = Block.create("create readme documentation", type_="to_do")
-my_todo_block2 = Block.create("add 'create' method", type_="to_do", checked=True)
-```
-
-Create `code` block object:
-
-```python
-from pytion.models import Block
-my_code_block = Block.create("code example here", type_="code", language="javascript")
-my_code_block2 = Block.create("another code example", type_="code", caption="it will be plain text code block with caption")
-```
-
-Create `heading` block object:
-
-```python
-from pytion.models import Block
-my_code_block = Block.create("Title 1 example here", type_="heading_1")
-my_code_block2 = Block.create("Toggle Title 2", type_="heading_2", is_toggleable=True)
-```
-
-### Block deleting
-
-```python
-no.blocks.block_update("3d4af9f0f98641dea8c44e3864eed4d0", archived=True)
-# or if you have Element with Block object already
-block.block_update(archived=True)
-```
-
-## Database operations
-
-### Retrieving
-
-```python
-from pytion import Notion
-no = Notion(token=TOKEN)
-
-# get all pages from Database
-# example 1
-pages = no.databases.db_query("114f1ef1f1241e2f12f41fe2f")
-# example 2
-db = no.databases.get("114f1ef1f1241e2f12f41fe2f")
-pages = db.db_query()
-print(pages.obj)
-
-# get pages with "task" in title
-pages = db.db_filter("task")
-
-# get all pages with sorting by property name "Tags"
-pages = db.db_filter("", ascending="Tags")
-pages = db.db_filter("", descending="Tags")
-
-# get pages with Status property equals Done
-pages = db.db_filter(property_name="Status", property_type="status", value="Done")
-
-# get pages with Price property greater than 150
-pages = db.db_filter(property_name="Price", property_type="number", condition="greater_than", value=150)
-
-# complex query
-pages = db.db_filter(
-    property_name="WorkTime", property_type="date", condition="before",
-    value=datetime.now(), descending="Deadline", limit=25
-)
-```
-
-> Queries with multifiltering and multisorting are not supported  
-> But you can compose your custom filter dict from API reference and call `db.db_filter(raw={...})` 
-
-Filter conditions and types combination -> [Official API reference](https://developers.notion.com/reference/post-database-query-filter)
-
-After you got `pages` which is `Element` object, you can not call API methods directly on `pages`
-because there is `PageArray` object with List of Pages.
-If you need to change a Page or something else, you can follow these steps:
-
-```python
-# 1. create new Element object with non-list object type
-page = no.pages.from_object(pages.obj[14])  # choosed page from the PageArray
-# 2. call the desired API method on this page
-page.page_update(archived=True)  # delete Page example
-```
-
-# Logging
-
-Logging is muted by default. To enable to stdout and/or to file:
-
-```python
-from pytion import setup_logging
-
-setup_logging(level="debug", to_console=True, filename="pytion.log")
-```
+Metadata-Version: 2.1
+Name: pytion
+Version: 1.3.4
+Summary: Unofficial Python client for official Notion API
+Home-page: https://github.com/lastorel/pytion
+Author: Yegor Gomzin
+Author-email: slezycmex@mail.ru
+Project-URL: Bug Tracker, https://github.com/lastorel/pytion/issues
+Project-URL: Changelog, https://github.com/lastorel/pytion/blob/main/CHANGELOG.md
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pytion
+
+[![PyPI](https://img.shields.io/pypi/v/pytion.svg)](https://pypi.org/project/pytion)
+![PyVersion](https://img.shields.io/pypi/pyversions/pytion)
+![CodeSize](https://img.shields.io/github/languages/code-size/lastorel/pytion)
+[![LICENSE](https://img.shields.io/github/license/lastorel/pytion)](LICENSE)
+
+Independent unofficial **Python client** for the official **Notion API** (for internal integrations only)
+
+Client is built with its own object model based on API
+
+So if you are using **notion.so** and want to automate some stuff with the original API, you're welcome!  
+You can read any available data, create basic models, and even work with databases.
+
+Current Notion API version = **"2022-06-28"**
+
+_*does not use notion-sdk-py client_
+
+See [Change Log](./CHANGELOG.md)
+
+# Contents
+
+1. [Quick Start](#quick-start)
+2. [Pytion API](#pytion-api)
+   1. [Searching](#search)
+   2. [pytion.api.Element](#pytionapielement)
+3. [Models](#models)
+   1. [pytion.models](#pytionmodels)
+   2. [Supported Property types](#supported-property-types)
+   3. [Supported block types](#supported-block-types)
+      1. [Block creating examples](#block-creating-examples)
+      2. [Block deleting](#block-deleting)
+   4. [Database operations](#database-operations)
+      1. [Retrieving](#retrieving)
+      2. [Appending (creating a Page)](#appending-creating-a-page)
+      3. [Property Values](#property-values)
+4. [Logging](#logging)
+
+# Quick start
+
+```
+pip install pytion
+```
+
+Create new integration and get your Notion API Token at notion.so -> [here](https://www.notion.com/my-integrations).  
+Add your new integration 'manager' to your pages or databases by going to the page's menu (three dots), at the bottom of the menu clicking on Add connections and then searching for you new Integration.
+
+```python
+from pytion import Notion; no = Notion(token=SOME_TOKEN)
+```
+
+Or put your token for Notion API into file `token` at script directory and use simple `no = Notion()`
+
+```python
+from pytion import Notion
+no = Notion(token=SOME_TOKEN)
+page = no.pages.get("PAGE ID")  # retrieve page data (not content) and create object
+blocks = page.get_block_children()  # retrieve page content and create list of objects
+database = no.databases.get("Database ID")  # retrieve database data (not content) and create object
+# retrieve database content by filtering with sorting
+pages = database.db_filter(property_name="Done", property_type="checkbox", value=False, descending="title")
+```
+
+```
+In [1]: from pytion import Notion
+
+In [2]: no = Notion(token=SOME_TOKEN)
+
+In [3]: page = no.pages.get("a458613160da45fa96367c8a594297c7")
+In [4]: print(page)
+Notion/pages/Page(Example page)
+
+In [5]: blocks = page.get_block_children_recursive()
+
+In [6]: print(blocks)
+Notion/blocks/BlockArray(## Migration planning [x] Rese)
+
+In [7]: print(blocks.obj)
+## Migration planning
+[x] Reset new switch 2022-05-12T00:00:00.000+03:00 → 2022-05-13T01:00:00.000+03:00 
+	- reboot
+	- hold reset button
+[x] Connect to console with baud rate 9600
+[ ] Skip default configuration dialog
+Use LinkTo(configs) 
+[Integration changes](https://developers.notion.com/changelog?page=2)
+
+In [8]: print(blocks.obj.simple)
+Migration planning
+Reset new switch 2022-05-12T00:00:00.000+03:00 → 2022-05-13T01:00:00.000+03:00 
+	reboot
+	hold reset button
+Connect to console with baud rate 9600
+Skip default configuration dialog
+Use https://api.notion.com/v1/pages/90ea1231865f4af28055b855c2fba267 
+https://developers.notion.com/changelog?page=2
+```
+
+# Pytion API
+
+Almost all operations are carried out through `Notion` or `Element` object:
+
+```python
+page = no.pages.get("a458613160da45fa96367c8a594297c7")
+
+# no -> Notion
+# pages -> URI in https://api.notion.com/v1/PAGES/a458613160da45fa96367c8a594297c7
+# get -> pytion API method
+# page -> Element
+# page.obj -> Page (main data structure)
+```
+
+so:
+
+- `isinstance(no, Notion) == True`
+- `isinstance(no.pages, Element) == True`
+- `isinstance(no.databases, Element) == True`
+- `isinstance(page, Element) == True`
+- `isinstance(page.obj, Page) == True`
+
+and if you want to retrieve a database - you must use _"databases"_ URI
+
+```python
+database = no.databases.get("123412341234")
+```
+
+and the same applies for _"blocks"_ and _"users"_. Valid URI-s are:
+
+- _pages_
+- _blocks_
+- _databases_
+- _users_
+
+When you work with existing `Element` object like `page` above, all [methods](#pytionapielement) below will be applied to this Page:
+
+```python
+new_page = page.page_update(title="new page name 2")
+
+# new_page is not a new page, it is updated page
+# new_page.obj is equal page.obj except title and last_edited properties
+```
+
+## Search
+
+There is a search example:
+```python
+no = Notion(token)
+
+r = no.search("updating", object_type="page")
+print(r.obj)
+# output:
+# Page for updating
+# Page to updating databases
+```
+
+
+## pytion.api.Element
+
+There is a list of available methods for communicate with **api.notion.com**. These methods are better structured in [next chapter](#pytionmodels).
+
+`.get(id_)` - Get Element by ID.
+
+`.get_parent(id_)` - Get parent object of current object if possible.
+
+`.get_block_children(id_, limit)` - Get children Block objects of current Block object (tabulated texts) if exist.
+
+`.get_block_children_recursive(id_, max_depth, limit, force)` - Get children Block objects of current Block object (tabulated texts) if exist recursive.
+
+`.get_page_property(property_id, id_, limit)` - Retrieve a page property item.
+
+`.get_page_properties(title_only, obj)` - Retrieve the title or all properties of current Page or Page `obj`
+*(deprecated, useful for v1.3.0 only)*
+
+`.db_query(id_, limit, filter_, sorts)` - Query Database.
+
+`.db_filter(...see desc...)` - Query Database.
+
+`.db_create(database_obj, parent, properties, title)` - Create Database.
+
+**_There is no way to delete a database object yet!_**
+
+`.db_update(id_, title, properties)` - Update Database.
+
+`.page_create(page_obj, parent, properties, title)` - Create Page.
+
+`.page_update(id_, properties, title, archived)` - Update Page.
+
+`.block_update(id_, block_obj, new_text, archived)` - Update text in Block.
+
+`.block_append(id_, block, blocks)` - Append block or blocks children.
+
+`.get_myself()` - Retrieve my bot User.
+
+`.from_linkto(linkto)` - Creates new Element object based on LinkTo information.
+
+`.from_object(model)` - Creates new Element object from Page, Block or Database object. Usable while Element object contains an Array.
+
+> More details and usage examples of these methods you can see into func descriptions.
+
+# Models
+
+### pytion.models
+
+There are classes **based on API** structures:
+
+- `RichText` based on [Rich text object](https://developers.notion.com/reference/rich-text)
+- `RichTextArray` is a list of RichText objects with useful methods
+  - You can create object by simple `RichTextArray.create("My title text")` and then use it in any methods
+  - Any Rich Text getting from API will be RichTextArray
+  - `str()` returns plain text of all "Rich Texts". ez
+  - `+` operator is available with `str` and `RichTextArray`
+  - `.simple` property returns stripped plain text without any markdown syntax. useful for URL
+- `Database` based on [Database object](https://developers.notion.com/reference/database)
+  - You can create object `Database.create(...)` and/or use `.db_create(...)` API method
+  - attrs represent API model. Complex structures like `created_by` are wrapped in internal objects
+  - use `.db_update()` API method for modify a real database (for ex. properties or title)
+  - use `.db_query()` to get all database content (it will be `PageArray`)
+  - use `.db_filter()` to get database content with filtering and/or sorting
+  - has `.description` attr
+  - has `.is_inline` attr with the value True if the database appears in the page as an inline block
+- `Page` based on [Page object](https://developers.notion.com/reference/page)
+  - You can create object `Page.create(...)` and/or use `.page_create(...)` API method
+  - use `.page_update()` method to modify attributes or delete the page
+  - use `.get_block_children()` to get page content (without nested blocks) (it will be `BlockArray`)
+  - use `.get_block_children_recursive()` to get page content with nested blocks
+  - use `.get_page_property()` to retrieve the specific `PropertyValue` of the page
+- `Block` based on [Block object](https://developers.notion.com/reference/block)
+  - You can create object `Block.create(...)` of specific type from [_support matrix_](#supported-block-types) below and then use it while creating pages or appending
+  - use `.block_update()` to replace content or change _extension attributes_ or delete the block
+  - use `.block_append()` to add a new block to a page or add a nested block to another block
+  - use `.get_block_children()` to get first level nested blocks
+  - use `.get_block_children_recursive()` to get all levels nested blocks
+- `User` based on [User object](https://developers.notion.com/reference/user)
+  - You can create object `User.create(...)` and use it in some properties like `people` type property
+  - You can retrieve more data about a User by his ID using `.get()`
+  - use `.get_myself()` to retrieve the current bot User
+  - has `.workspace_name` attr for `bot` type users
+- `Property` based on [Property object](https://developers.notion.com/reference/property-object)
+  - You can create object `Property.create(...)` while creating or editing database: `.db_create()` or `.db_update()`
+  - `formula` type properties configuration is not supported
+- `PropertyValue` based on [Property values](https://developers.notion.com/reference/property-value-object)
+  - You can create object `PropertyValue.create(...)` to set or edit page properties by `.page_create()` or `.page_update()`
+  - `files`, `formula`, `rollup` type properties are not editable
+
+There are also useful **internal** classes:
+
+- `BlockArray` is found when API returns page content in "list of blocks" format
+  - it is useful to represent all content by `str()`
+  - also it has `simple` property like `RichTextArray` object
+  - it automatically indents `str` output of nested blocks
+- `PageArray` is found when API returns the result of database query (list of pages)
+- `LinkTo` is basic internal model to link to any Notion object
+  - You can create object `LinkTo.create()` and use it in many places and methods
+  - use `LinkTo(from_object=my_page1)` to quickly create a link to any existing object of pytion.models
+  - `link` property of `LinkTo` returns expanded URL
+- `ElementArray` is found while using `.search()` endpoint. It's a parent of `PageArray`
+
+> And every model has a `.get()` method that returns API friendly JSON.
+ 
+### Supported Property types
+
+| Property type            | value type                       | read (DB) | read value (Page) | create (DB) | create value (Page) | Oper attrs                          | Config attrs                                                                                                 |
+|--------------------------|----------------------------------|-----------|-------------------|-------------|---------------------|-------------------------------------|--------------------------------------------------------------------------------------------------------------|
+| `title`                  | `RichTextArray`                  | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `rich_text`              | `RichTextArray`                  | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `number`                 | `int`/`float`                    | +         | +                 | +           | +                   |                                     | ~~format~~                                                                                                   |
+| `select`                 | `str`                            | +         | +                 | +           | +                   |                                     | ~~options~~                                                                                                  |
+| `multi_select`           | `List[str]`                      | +         | +                 | +           | +                   |                                     | ~~options~~                                                                                                  |
+| `status`                 | `str`                            | +         | +                 | +           | +\*\*\*\*           |                                     | `options`, `groups` (read-only)                                                                              |
+| `date`                   | `str`                            | +         | +                 | +           | +                   | `start: datetime` `end: datetime`\* |                                                                                                              |
+| `people`                 | `List[User]`                     | +         | +                 | +           | +\*\*               |                                     |                                                                                                              |
+| `files`                  |                                  | +         | -                 | +           | -                   |                                     |                                                                                                              |
+| `checkbox`               | `bool`                           | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `url`                    | `str`                            | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `email`                  | `str`                            | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `phone_number`           | `str`                            | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `formula`                |                                  | -         | +                 | -           | n/a                 |                                     |                                                                                                              |
+| `relation`               | `List[LinkTo]`                   | +         | +                 | +           | +                   | `has_more: bool`                    | `single_property` / `dual_property`                                                                          |
+| `rollup`                 | depends on relation and function | +         | +                 | +           | n/a                 | ~~has_more~~\*\*\*\*\*              | `function`, `relation_property_id` / `relation_property_name`, `rollup_property_id` / `rollup_property_name` |
+| `created_time`\*\*\*     | `datetime`                       | +         | +                 | +           | n/a                 |                                     |                                                                                                              |
+| `created_by`\*\*\*       | `User`                           | +         | +                 | +           | n/a                 |                                     |                                                                                                              |
+| `last_edited_time`\*\*\* | `datetime`                       | +         | +                 | +           | n/a                 |                                     |                                                                                                              |
+| `last_edited_by`\*\*\*   | `User`                           | +         | +                 | +           | n/a                 |                                     |                                                                                                              |
+
+> [\*] - Create examples:  
+> `pv = PropertyValue.create(type_="date", value=datetime.now())`  
+> `pv = PropertyValue.create(type_="date", date={"start": str(datetime(2022, 2, 1, 5)), "end": str(datetime.now())})`  
+> [\*\*] - Create example:  
+> `user = User.create('1d393ffb5efd4d09adfc2cb6738e4812')`  
+> `pv = PropertyValue.create(type_="people", value=[user])`  
+> [\*\*\*] - Every Base model like Page already has mandatory attributes created/last_edited returned by API  
+> [\*\*\*\*] - Status type is not configurable. API doesn't support NEW options added via Property modify or updating a Page
+> [\*\*\*\*\*] - Notion API hasn't `has_more` attr. Only 25 references can be shown in the array
+
+More details and examples can be found in Database [section](#property-values)
+
+More details and examples can be found in Database [section](#property-values)
+
+
+## Supported block types
+
+At present the API only supports the block types which are listed in the reference below. Any unsupported block types will continue to appear in the structure, but only contain a `type` set to `"unsupported"`.
+Colors are not yet supported.
+
+Every Block has mandatory attributes and extension attributes. There are mandatory:
+
+- `id: str` - UUID-64 without hyphens
+- `object: str` - always `"block"` (from API)
+- `created_time: datetime` - from API
+- `created_by: User` - from API
+- `last_edited_time: datetime` - from API
+- `last_edited_by: User` - from API
+- `type: str` - the type of block (from API)
+- `has_children: bool` - does the block have children blocks (from API)
+- `archived: bool` - does the block marked as deleted (from API)
+- `text: Union[str, RichTextArray]` - **main content**
+- `simple: str` - only simple text string (url expanded)
+
+Extension attributes are listed below in support matrix:
+
+| Block Type           | Description                               | Read support | Create support | Can have children | Extension attributes                              |
+|----------------------|-------------------------------------------|--------------|----------------|-------------------|---------------------------------------------------|
+| `paragraph`          | Simple Block with text                    | +            | +              | +                 |                                                   |
+| `heading_1`          | Heading Block with text highest level     | +            | +              | -/+\*             | `is_toggleable: bool`                             |
+| `heading_2`          | Heading Block with text medium level      | +            | +              | -/+\*             | `is_toggleable: bool`                             |
+| `heading_3`          | Heading Block with text lowest level      | +            | +              | -/+\*             | `is_toggleable: bool`                             |
+| `bulleted_list_item` | Text Block with bullet                    | +            | -              | +                 |                                                   |
+| `numbered_list_item` | Text Block with number                    | +            | -              | +                 |                                                   |
+| `to_do`              | Text Block with checkbox                  | +            | +              | +                 | `checked: bool`                                   |
+| `toggle`             | Text Block with toggle to children blocks | +            | -              | +                 |                                                   |
+| `code`               | Text Block with code style                | +            | +              | +                 | `language: str`, `caption: RichTextArray`         |
+| `child_page`         | Page inside                               | +            | -              | +                 |                                                   |
+| `child_database`     | Database inside                           | +            | -              | +                 |                                                   |
+| `embed`              | Embed online content                      | +            | -              | -                 | `caption: RichTextArray`                          |
+| `image`              | Embed image content                       | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
+| `video`              | Embed video content                       | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
+| `file`               | Embed file content                        | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
+| `pdf`                | Embed pdf content                         | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
+| `bookmark`           | Block for URL Link                        | +            | -              | -                 | `caption: RichTextArray`                          |
+| `callout`            | Highlighted footnote text Block           | +            | -              | +                 | `icon: dict`                                      |
+| `quote`              | Text Block with quote style               | +            | -              | +                 |                                                   |
+| `equation`           | KaTeX compatible text Block               | +            | -              | -                 |                                                   |
+| `divider`            | Simple line to divide the page            | +            | -              | -                 |                                                   |
+| `table_of_contents`  | Block with content structure in the page  | +            | -              | -                 |                                                   |
+| `column`             |                                           | -            | -              | +                 |                                                   |
+| `column_list`        |                                           | -            | -              | -                 |                                                   |
+| `link_preview`       | Same as `bookmark`                        | +            | -              | -                 |                                                   |
+| `synced_block`       | Block for synced content aka parent       | +            | -              | +                 | `synced_from: LinkTo`                             |
+| `template`           | Template Block title                      | +            | -              | +                 |                                                   |
+| `link_to_page`       | Block with link to particular page `@...` | +            | -              | -                 | `link: LinkTo`                                    |
+| `table`              | Table Block with some attrs               | +            | -              | +                 | `table_width: int`                                |
+| `table_row`          | Children Blocks with table row content    | +            | -              | -                 |                                                   |
+| `breadcrumb`         | Empty Block actually                      | +            | -              | -                 |                                                   |
+| `unsupported`        | Blocks unsupported by API                 | +            | -              | -                 |                                                   |
+
+> [\*] - `heading_X` blocks can have children if `is_toggleable` is True 
+
+### Block creating examples
+
+Create `paragraph` block object and add it to Notion:
+
+```python
+from pytion.models import Block
+my_text_block = Block.create("Hello World!")
+my_text_block = Block.create(text="Hello World!", type_="paragraph")  # the same
+
+# indented append my block to other known block:
+no.blocks.block_append("5f60073a9dda4a9c93a212a74a107359", block=my_text_block)
+
+# append my block to a known page (in the end)
+no.blocks.block_append("9796f2525016128d9af4bf12b236b555", block=my_text_block)  # the same operation actually
+
+# another way to append:
+my_page = no.pages.get("9796f2525016128d9af4bf12b236b555")
+my_page.block_append(block=my_text_block)
+```
+
+Create `to_do` block object:
+
+```python
+from pytion.models import Block
+my_todo_block = Block.create("create readme documentation", type_="to_do")
+my_todo_block2 = Block.create("add 'create' method", type_="to_do", checked=True)
+```
+
+Create `code` block object:
+
+```python
+from pytion.models import Block
+my_code_block = Block.create("code example here", type_="code", language="javascript")
+my_code_block2 = Block.create("another code example", type_="code", caption="it will be plain text code block with caption")
+```
+
+Create `heading` block object:
+
+```python
+from pytion.models import Block
+my_code_block = Block.create("Title 1 example here", type_="heading_1")
+my_code_block2 = Block.create("Toggle Title 2", type_="heading_2", is_toggleable=True)
+```
+
+### Block deleting
+
+```python
+no.blocks.block_update("3d4af9f0f98641dea8c44e3864eed4d0", archived=True)
+# or if you have Element with Block object already
+block.block_update(archived=True)
+```
+
+## Database operations
+
+### Retrieving
+
+```python
+from pytion import Notion
+no = Notion(token=TOKEN)
+
+# get all pages from Database
+# example 1
+pages = no.databases.db_query("114f1ef1f1241e2f12f41fe2f")
+# example 2
+db = no.databases.get("114f1ef1f1241e2f12f41fe2f")
+pages = db.db_query()
+print(pages.obj)
+
+# get pages with "task" in title
+pages = db.db_filter("task")
+
+# get all pages with sorting by property name "Tags"
+pages = db.db_filter("", ascending="Tags")
+pages = db.db_filter("", descending="Tags")
+
+# get pages with Status property equals Done
+pages = db.db_filter(property_name="Status", property_type="status", value="Done")
+
+# get pages with Price property greater than 150
+pages = db.db_filter(property_name="Price", property_type="number", condition="greater_than", value=150)
+
+# complex query
+pages = db.db_filter(
+    property_name="WorkTime", property_type="date", condition="before",
+    value=datetime.now(), descending="Deadline", limit=25
+)
+```
+
+> Queries with multifiltering and multisorting are not supported  
+> But you can compose your custom filter dict from API reference and call `db.db_filter(raw={...})` 
+
+Filter conditions and types combination -> [Official API reference](https://developers.notion.com/reference/post-database-query-filter)
+
+After you got `pages` which is `Element` object, you can not call API methods directly on `pages`
+because there is `PageArray` object with List of Pages.
+If you need to change a Page or something else, you can follow these steps:
+
+```python
+# 1. create new Element object with non-list object type
+page = no.pages.from_object(pages.obj[14])  # choosed page from the PageArray
+# 2. call the desired API method on this page
+page.page_update(archived=True)  # delete Page example
+```
+
+### Appending (creating a Page)
+
+There is a way to create a row into database. The same method is used to create any Page.
+The difference is in only in `parent` argument which can be the Page or the Database.
+
+```python
+from pytion.models import LinkTo
+
+# choose the parent target
+# it can be the database
+parent = LinkTo.create(database_id="043cb52491a44b80a5e5006237a4278f")
+# or the page
+parent2 = LinkTo.create(page_id="043cb52491a44b80a5e5006237a4278f")
+
+# if you need to set Properties
+from pytion.models import PropertyValue
+props = {
+            "Tags": PropertyValue.create(type_="multi_select", value=["tag1", "tag2"]),
+            "done": PropertyValue.create("checkbox", True),
+            "AnotherPropertyNAME": PropertyValue.create("date", datetime.now()),
+        }
+
+# create the Page
+page = no.pages.page_create(parent=parent, title="Page 2")  # without properties (will be empty)
+# or
+page2 = no.pages.page_create(parent=parent, properties=props, title="Page 2")  # with properties
+```
+
+### Property Values
+
+Pytion Properties support table is described [above](#supported-property-types)
+
+There are Properties that are used in Database operations and PropertyValues that are used in Page operations.
+
+It's necessary to choose the type (`type_` arg) and value (`value`) of property.
+The table shows the mapping between Property type and value (python) type.
+
+The `type_` must correspond to your database schema in Notion.
+
+```python
+from datetime import datetime
+from pytion.models import PropertyValue, LinkTo, RichTextArray, User
+
+# + relation type:
+pv = PropertyValue.create("relation", value=[LinkTo.create(page_id="04262843082a478d97f741948a32613b")])
+# + people type:
+pv = PropertyValue.create(type_="people", value=[User.create('1d393ffb5efd4d09adfc2cb6738e4812')])
+# + date type:
+pv = PropertyValue.create(type_="date", value=datetime.now())
+pv = PropertyValue.create(type_="date", date={"start": str(datetime(2022, 2, 1, 5)), "end": str(datetime.now())})
+# + rich_text (text or title field)
+pv = PropertyValue.create(type_="rich_text", value="Something Interesting")
+pv = PropertyValue.create("rich_text", value=RichTextArray.create("Something Interesting"))
+# + nubmer
+pv = PropertyValue.create(type_="number", value=156.2)
+# + status
+pv = PropertyValue.create("status", value="Done")
+
+# update needed property values
+new_props = {
+    "Tags": PropertyValue.create("multi_select", ["tag2"]),
+    "done": PropertyValue.create("checkbox", False),
+    "when": PropertyValue.create("date", datetime.now()),
+}
+page = page_for_updates.page_update(properties=new_props)
+page = no.pages.page_update(page_for_updates_id, properties=new_props)  # the same
+
+# rename (edit title property)
+page = page_for_updates.page_update(title=new_name)
+```
+
+Pytion also provides the ways to change database schema - create/update/rename/delete properties:
+
+```python
+from pytion.models import Property
+
+# rename property
+properties = {"Name": Property.create(type_="title", name="Subject")}
+database = database_for_updates.db_update(properties=properties)
+database = no.databases.db_update(database_for_updates_id, properties=properties)  # the same
+# change property type
+properties = {"Tags": Property.create("select")}
+database = database_for_updates.db_update(properties=properties)
+# delete property from database
+properties = {"Old property name": Property.create(None)}
+database = database_for_updates.db_update(properties=properties)
+# rename database
+database = database_for_updates.db_update(title="Refactoring")
+```
+
+# Logging
+
+Logging is muted by default. To enable to stdout and/or to file:
+
+```python
+from pytion import setup_logging
+
+setup_logging(level="debug", to_console=True, filename="pytion.log")
+```
```

### Comparing `pytion-1.3.3/README.md` & `pytion-1.3.4/pytion.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,463 +1,580 @@
-# pytion
-
-[![PyPI](https://img.shields.io/pypi/v/pytion.svg)](https://pypi.org/project/pytion)
-![PyVersion](https://img.shields.io/pypi/pyversions/pytion)
-![CodeSize](https://img.shields.io/github/languages/code-size/lastorel/pytion)
-[![LICENSE](https://img.shields.io/github/license/lastorel/pytion)](LICENSE)
-
-Independent unofficial **Python client** for the official **Notion API** (for internal integrations only)
-
-Client is built with its own object model based on API
-
-So if you are using **notion.so** and want to automate some stuff with the original API, you're welcome!  
-You can read any available data, create basic models, and even work with databases.
-
-Current Notion API version = **"2022-06-28"**
-
-_*does not use notion-sdk-py client_
-
-See [Change Log](./CHANGELOG.md)
-
-# Contents
-
-1. [Quick Start](#quick-start)
-2. [Pytion API](#pytion-api)
-   1. [Searching](#search)
-   2. [pytion.api.Element](#pytionapielement)
-3. [Models](#models)
-   1. [pytion.models](#pytionmodels)
-   2. [Supported Property types](#supported-property-types)
-   3. [Supported block types](#supported-block-types)
-      1. [Block creating examples](#block-creating-examples)
-      2. [Block deleting](#block-deleting)
-   4. [Database operations](#database-operations)
-      1. [Retrieving](#retrieving)
-4. [Logging](#logging)
-
-# Quick start
-
-```
-pip install pytion
-```
-
-Create new integration and get your Notion API Token at notion.so -> [here](https://www.notion.com/my-integrations).  
-Invite your new integration 'manager' to your pages or databases.
-
-```python
-from pytion import Notion; no = Notion(token=SOME_TOKEN)
-```
-
-Or put your token for Notion API into file `token` at script directory and use simple `no = Notion()`
-
-```python
-from pytion import Notion
-no = Notion(token=SOME_TOKEN)
-page = no.pages.get("PAGE ID")  # retrieve page data (not content) and create object
-blocks = page.get_block_children()  # retrieve page content and create list of objects
-database = no.databases.get("Database ID")  # retrieve database data (not content) and create object
-# retrieve database content by filtering with sorting
-pages = database.db_filter(property_name="Done", property_type="checkbox", value=False, descending="title")
-```
-
-```
-In [1]: from pytion import Notion
-
-In [2]: no = Notion(token=SOME_TOKEN)
-
-In [3]: page = no.pages.get("a458613160da45fa96367c8a594297c7")
-In [4]: print(page)
-Notion/pages/Page(Example page)
-
-In [5]: blocks = page.get_block_children_recursive()
-
-In [6]: print(blocks)
-Notion/blocks/BlockArray(## Migration planning [x] Rese)
-
-In [7]: print(blocks.obj)
-## Migration planning
-[x] Reset new switch 2022-05-12T00:00:00.000+03:00 → 2022-05-13T01:00:00.000+03:00 
-	- reboot
-	- hold reset button
-[x] Connect to console with baud rate 9600
-[ ] Skip default configuration dialog
-Use LinkTo(configs) 
-[Integration changes](https://developers.notion.com/changelog?page=2)
-
-In [8]: print(blocks.obj.simple)
-Migration planning
-Reset new switch 2022-05-12T00:00:00.000+03:00 → 2022-05-13T01:00:00.000+03:00 
-	reboot
-	hold reset button
-Connect to console with baud rate 9600
-Skip default configuration dialog
-Use https://api.notion.com/v1/pages/90ea1231865f4af28055b855c2fba267 
-https://developers.notion.com/changelog?page=2
-```
-
-# Pytion API
-
-Almost all operations are carried out through `Notion` or `Element` object:
-
-```python
-page = no.pages.get("a458613160da45fa96367c8a594297c7")
-
-# no -> Notion
-# pages -> URI in https://api.notion.com/v1/PAGES/a458613160da45fa96367c8a594297c7
-# get -> pytion API method
-# page -> Element
-# page.obj -> Page (main data structure)
-```
-
-so:
-
-- `isinstance(no, Notion) == True`
-- `isinstance(no.pages, Element) == True`
-- `isinstance(no.databases, Element) == True`
-- `isinstance(page, Element) == True`
-- `isinstance(page.obj, Page) == True`
-
-and if you want to retrieve a database - you must use _"databases"_ URI
-
-```python
-database = no.databases.get("123412341234")
-```
-
-and the same applies for _"blocks"_ and _"users"_. Valid URI-s are:
-
-- _pages_
-- _blocks_
-- _databases_
-- _users_
-
-When you work with existing `Element` object like `page` above, all [methods](#pytionapielement) below will be applied to this Page:
-
-```python
-new_page = page.page_update(title="new page name 2")
-
-# new_page is not a new page, it is updated page
-# new_page.obj is equal page.obj except title and last_edited properties
-```
-
-## Search
-
-There is a search example:
-```python
-no = Notion(token)
-
-r = no.search("updating", object_type="page")
-print(r.obj)
-# output:
-# Page for updating
-# Page to updating databases
-```
-
-
-## pytion.api.Element
-
-There is a list of available methods for communicate with **api.notion.com**. These methods are better structured in [next chapter](#pytionmodels).
-
-`.get(id_)` - Get Element by ID.
-
-`.get_parent(id_)` - Get parent object of current object if possible.
-
-`.get_block_children(id_, limit)` - Get children Block objects of current Block object (tabulated texts) if exist.
-
-`.get_block_children_recursive(id_, max_depth, limit, force)` - Get children Block objects of current Block object (tabulated texts) if exist recursive.
-
-`.get_page_property(property_id, id_, limit)` - Retrieve a page property item.
-
-`.get_page_properties(title_only, obj)` - Retrieve the title or all properties of current Page or Page `obj`
-*(deprecated, useful for v1.3.0 only)*
-
-`.db_query(id_, limit, filter_, sorts)` - Query Database.
-
-`.db_filter(...see desc...)` - Query Database.
-
-`.db_create(database_obj, parent, properties, title)` - Create Database.
-
-**_There is no way to delete a database object yet!_**
-
-`.db_update(id_, title, properties)` - Update Database.
-
-`.page_create(page_obj, parent, properties, title)` - Create Page.
-
-`.page_update(id_, properties, title, archived)` - Update Page.
-
-`.block_update(id_, block_obj, new_text, archived)` - Update text in Block.
-
-`.block_append(id_, block, blocks)` - Append block or blocks children.
-
-`.get_myself()` - Retrieve my bot User.
-
-`.from_linkto(linkto)` - Creates new Element object based on LinkTo information.
-
-`.from_object(model)` - Creates new Element object from Page, Block or Database object. Usable while Element object contains an Array.
-
-> More details and usage examples of these methods you can see into func descriptions.
-
-# Models
-
-### pytion.models
-
-There are classes **based on API** structures:
-
-- `RichText` based on [Rich text object](https://developers.notion.com/reference/rich-text)
-- `RichTextArray` is a list of RichText objects with useful methods
-  - You can create object by simple `RichTextArray.create("My title text")` and then use it in any methods
-  - Any Rich Text getting from API will be RichTextArray
-  - `str()` returns plain text of all "Rich Texts". ez
-  - `+` operator is available with `str` and `RichTextArray`
-  - `.simple` property returns stripped plain text without any markdown syntax. useful for URL
-- `Database` based on [Database object](https://developers.notion.com/reference/database)
-  - You can create object `Database.create(...)` and/or use `.db_create(...)` API method
-  - attrs represent API model. Complex structures like `created_by` are wrapped in internal objects
-  - use `.db_update()` API method for modify a real database (for ex. properties or title)
-  - use `.db_query()` to get all database content (it will be `PageArray`)
-  - use `.db_filter()` to get database content with filtering and/or sorting
-  - has `.description` attr
-  - has `.is_inline` attr with the value True if the database appears in the page as an inline block
-- `Page` based on [Page object](https://developers.notion.com/reference/page)
-  - You can create object `Page.create(...)` and/or use `.page_create(...)` API method
-  - use `.page_update()` method to modify attributes or delete the page
-  - use `.get_block_children()` to get page content (without nested blocks) (it will be `BlockArray`)
-  - use `.get_block_children_recursive()` to get page content with nested blocks
-  - use `.get_page_property()` to retrieve the specific `PropertyValue` of the page
-- `Block` based on [Block object](https://developers.notion.com/reference/block)
-  - You can create object `Block.create(...)` of specific type from [_support matrix_](#supported-block-types) below and then use it while creating pages or appending
-  - use `.block_update()` to replace content or change _extension attributes_ or delete the block
-  - use `.block_append()` to add a new block to a page or add a nested block to another block
-  - use `.get_block_children()` to get first level nested blocks
-  - use `.get_block_children_recursive()` to get all levels nested blocks
-- `User` based on [User object](https://developers.notion.com/reference/user)
-  - You can create object `User.create(...)` and use it in some properties like `people` type property
-  - You can retrieve more data about a User by his ID using `.get()`
-  - use `.get_myself()` to retrieve the current bot User
-  - has `.workspace_name` attr for `bot` type users
-- `Property` based on [Property object](https://developers.notion.com/reference/property-object)
-  - You can create object `Property.create(...)` while creating or editing database: `.db_create()` or `.db_update()`
-  - `formula`, `rollup` type properties configuration is not supported
-- `PropertyValue` based on [Property values](https://developers.notion.com/reference/property-value-object)
-  - You can create object `PropertyValue.create(...)` to set or edit page properties by `.page_create()` or `.page_update()`
-  - `files`, `formula`, `rollup` type properties are not editable
-
-There are also useful **internal** classes:
-
-- `BlockArray` is found when API returns page content in "list of blocks" format
-  - it is useful to represent all content by `str()`
-  - also it has `simple` property like `RichTextArray` object
-  - it automatically indents `str` output of nested blocks
-- `PageArray` is found when API returns the result of database query (list of pages)
-- `LinkTo` is basic internal model to link to any Notion object
-  - You can create object `LinkTo.create()` and use it in many places and methods
-  - use `LinkTo(from_object=my_page1)` to quickly create a link to any existing object of pytion.models
-  - `link` property of `LinkTo` returns expanded URL
-- `ElementArray` is found while using `.search()` endpoint. It's a parent of `PageArray`
-
-> And every model has a `.get()` method that returns API friendly JSON.
- 
-### Supported Property types
-
-| Property type            | value type          | read (DB) | read value (Page) | create (DB) | create value (Page) | Oper attrs                          | Config attrs                        |
-|--------------------------|---------------------|-----------|-------------------|-------------|---------------------|-------------------------------------|-------------------------------------|
-| `title`                  | `RichTextArray`     | +         | +                 | +           | +                   |                                     |                                     |
-| `rich_text`              | `RichTextArray`     | +         | +                 | +           | +                   |                                     |                                     |
-| `number`                 | `int`/`float`       | +         | +                 | +           | +                   |                                     | ~~format~~                          |
-| `select`                 | `str`               | +         | +                 | +           | +                   |                                     | ~~options~~                         |
-| `multi_select`           | `List[str]`         | +         | +                 | +           | +                   |                                     | ~~options~~                         |
-| `status`                 | `str`               | +         | +                 | +           | +\*\*\*\*           |                                     | `options`, `groups` (read-only)     |
-| `date`                   | `str`               | +         | +                 | +           | +                   | `start: datetime` `end: datetime`\* |                                     |
-| `people`                 | `List[User]`        | +         | +                 | +           | +\*\*               |                                     |                                     |
-| `files`                  |                     | +         | -                 | +           | -                   |                                     |                                     |
-| `checkbox`               | `bool`              | +         | +                 | +           | +                   |                                     |                                     |
-| `url`                    | `str`               | +         | +                 | +           | +                   |                                     |                                     |
-| `email`                  | `str`               | +         | +                 | +           | +                   |                                     |                                     |
-| `phone_number`           | `str`               | +         | +                 | +           | +                   |                                     |                                     |
-| `formula`                |                     | -         | +                 | -           | -                   |                                     |                                     |
-| `relation`               | `List[LinkTo]`      | +         | +                 | +           | +                   | `has_more: bool`                    | `single_property` / `dual_property` |
-| `rollup`                 | depends on relation | -         | +                 | -           | -                   |                                     |                                     |
-| `created_time`\*\*\*     | `datetime`          | +         | +                 | +           | -                   |                                     |                                     |
-| `created_by`\*\*\*       | `User`              | +         | +                 | +           | -                   |                                     |                                     |
-| `last_edited_time`\*\*\* | `datetime`          | +         | +                 | +           | -                   |                                     |                                     |
-| `last_edited_by`\*\*\*   | `User`              | +         | +                 | +           | -                   |                                     |                                     |
-
-> [\*] - Create examples:  
-> `pv = PropertyValue.create(type_="date", value=datetime.now())`  
-> `pv = PropertyValue.create(type_="date", date={"start": str(datetime(2022, 2, 1, 5)), "end": str(datetime.now())})`  
-> [\*\*] - Create example:  
-> `user = User.create('1d393ffb5efd4d09adfc2cb6738e4812')`  
-> `pv = PropertyValue.create(type_="people", value=[user])`  
-> [\*\*\*] - Every Base model like Page already has mandatory attributes created/last_edited returned by API  
-> [\*\*\*\*] - Status type is not configurable. API doesn't support NEW options added via Property modify or updating a Page
-
-
-## Supported block types
-
-At present the API only supports the block types which are listed in the reference below. Any unsupported block types will continue to appear in the structure, but only contain a `type` set to `"unsupported"`.
-Colors are not yet supported.
-
-Every Block has mandatory attributes and extension attributes. There are mandatory:
-
-- `id: str` - UUID-64 without hyphens
-- `object: str` - always `"block"` (from API)
-- `created_time: datetime` - from API
-- `created_by: User` - from API
-- `last_edited_time: datetime` - from API
-- `last_edited_by: User` - from API
-- `type: str` - the type of block (from API)
-- `has_children: bool` - does the block have children blocks (from API)
-- `archived: bool` - does the block marked as deleted (from API)
-- `text: Union[str, RichTextArray]` - **main content**
-- `simple: str` - only simple text string (url expanded)
-
-Extension attributes are listed below in support matrix:
-
-| Block Type           | Description                               | Read support | Create support | Can have children | Extension attributes                              |
-|----------------------|-------------------------------------------|--------------|----------------|-------------------|---------------------------------------------------|
-| `paragraph`          | Simple Block with text                    | +            | +              | +                 |                                                   |
-| `heading_1`          | Heading Block with text highest level     | +            | +              | -/+\*             | `is_toggleable: bool`                             |
-| `heading_2`          | Heading Block with text medium level      | +            | +              | -/+\*             | `is_toggleable: bool`                             |
-| `heading_3`          | Heading Block with text lowest level      | +            | +              | -/+\*             | `is_toggleable: bool`                             |
-| `bulleted_list_item` | Text Block with bullet                    | +            | -              | +                 |                                                   |
-| `numbered_list_item` | Text Block with number                    | +            | -              | +                 |                                                   |
-| `to_do`              | Text Block with checkbox                  | +            | +              | +                 | `checked: bool`                                   |
-| `toggle`             | Text Block with toggle to children blocks | +            | -              | +                 |                                                   |
-| `code`               | Text Block with code style                | +            | +              | +                 | `language: str`, `caption: RichTextArray`         |
-| `child_page`         | Page inside                               | +            | -              | +                 |                                                   |
-| `child_database`     | Database inside                           | +            | -              | +                 |                                                   |
-| `embed`              | Embed online content                      | +            | -              | -                 | `caption: RichTextArray`                          |
-| `image`              | Embed image content                       | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
-| `video`              | Embed video content                       | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
-| `file`               | Embed file content                        | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
-| `pdf`                | Embed pdf content                         | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
-| `bookmark`           | Block for URL Link                        | +            | -              | -                 | `caption: RichTextArray`                          |
-| `callout`            | Highlighted footnote text Block           | +            | -              | +                 | `icon: dict`                                      |
-| `quote`              | Text Block with quote style               | +            | -              | +                 |                                                   |
-| `equation`           | KaTeX compatible text Block               | +            | -              | -                 |                                                   |
-| `divider`            | Simple line to divide the page            | +            | -              | -                 |                                                   |
-| `table_of_contents`  | Block with content structure in the page  | +            | -              | -                 |                                                   |
-| `column`             |                                           | -            | -              | +                 |                                                   |
-| `column_list`        |                                           | -            | -              | -                 |                                                   |
-| `link_preview`       | Same as `bookmark`                        | +            | -              | -                 |                                                   |
-| `synced_block`       | Block for synced content aka parent       | +            | -              | +                 | `synced_from: LinkTo`                             |
-| `template`           | Template Block title                      | +            | -              | +                 |                                                   |
-| `link_to_page`       | Block with link to particular page `@...` | +            | -              | -                 | `link: LinkTo`                                    |
-| `table`              | Table Block with some attrs               | +            | -              | +                 | `table_width: int`                                |
-| `table_row`          | Children Blocks with table row content    | +            | -              | -                 |                                                   |
-| `breadcrumb`         | Empty Block actually                      | +            | -              | -                 |                                                   |
-| `unsupported`        | Blocks unsupported by API                 | +            | -              | -                 |                                                   |
-
-> [\*] - `heading_X` blocks can have children if `is_toggleable` is True 
-
-### Block creating examples
-
-Create `paragraph` block object and add it to Notion:
-
-```python
-from pytion.models import Block
-my_text_block = Block.create("Hello World!")
-my_text_block = Block.create(text="Hello World!", type_="paragraph")  # the same
-
-# indented append my block to other known block:
-no.blocks.block_append("5f60073a9dda4a9c93a212a74a107359", block=my_text_block)
-
-# append my block to a known page (in the end)
-no.blocks.block_append("9796f2525016128d9af4bf12b236b555", block=my_text_block)  # the same operation actually
-
-# another way to append:
-my_page = no.pages.get("9796f2525016128d9af4bf12b236b555")
-my_page.block_append(block=my_text_block)
-```
-
-Create `to_do` block object:
-
-```python
-from pytion.models import Block
-my_todo_block = Block.create("create readme documentation", type_="to_do")
-my_todo_block2 = Block.create("add 'create' method", type_="to_do", checked=True)
-```
-
-Create `code` block object:
-
-```python
-from pytion.models import Block
-my_code_block = Block.create("code example here", type_="code", language="javascript")
-my_code_block2 = Block.create("another code example", type_="code", caption="it will be plain text code block with caption")
-```
-
-Create `heading` block object:
-
-```python
-from pytion.models import Block
-my_code_block = Block.create("Title 1 example here", type_="heading_1")
-my_code_block2 = Block.create("Toggle Title 2", type_="heading_2", is_toggleable=True)
-```
-
-### Block deleting
-
-```python
-no.blocks.block_update("3d4af9f0f98641dea8c44e3864eed4d0", archived=True)
-# or if you have Element with Block object already
-block.block_update(archived=True)
-```
-
-## Database operations
-
-### Retrieving
-
-```python
-from pytion import Notion
-no = Notion(token=TOKEN)
-
-# get all pages from Database
-# example 1
-pages = no.databases.db_query("114f1ef1f1241e2f12f41fe2f")
-# example 2
-db = no.databases.get("114f1ef1f1241e2f12f41fe2f")
-pages = db.db_query()
-print(pages.obj)
-
-# get pages with "task" in title
-pages = db.db_filter("task")
-
-# get all pages with sorting by property name "Tags"
-pages = db.db_filter("", ascending="Tags")
-pages = db.db_filter("", descending="Tags")
-
-# get pages with Status property equals Done
-pages = db.db_filter(property_name="Status", property_type="status", value="Done")
-
-# get pages with Price property greater than 150
-pages = db.db_filter(property_name="Price", property_type="number", condition="greater_than", value=150)
-
-# complex query
-pages = db.db_filter(
-    property_name="WorkTime", property_type="date", condition="before",
-    value=datetime.now(), descending="Deadline", limit=25
-)
-```
-
-> Queries with multifiltering and multisorting are not supported  
-> But you can compose your custom filter dict from API reference and call `db.db_filter(raw={...})` 
-
-Filter conditions and types combination -> [Official API reference](https://developers.notion.com/reference/post-database-query-filter)
-
-After you got `pages` which is `Element` object, you can not call API methods directly on `pages`
-because there is `PageArray` object with List of Pages.
-If you need to change a Page or something else, you can follow these steps:
-
-```python
-# 1. create new Element object with non-list object type
-page = no.pages.from_object(pages.obj[14])  # choosed page from the PageArray
-# 2. call the desired API method on this page
-page.page_update(archived=True)  # delete Page example
-```
-
-# Logging
-
-Logging is muted by default. To enable to stdout and/or to file:
-
-```python
-from pytion import setup_logging
-
-setup_logging(level="debug", to_console=True, filename="pytion.log")
-```
+Metadata-Version: 2.1
+Name: pytion
+Version: 1.3.4
+Summary: Unofficial Python client for official Notion API
+Home-page: https://github.com/lastorel/pytion
+Author: Yegor Gomzin
+Author-email: slezycmex@mail.ru
+Project-URL: Bug Tracker, https://github.com/lastorel/pytion/issues
+Project-URL: Changelog, https://github.com/lastorel/pytion/blob/main/CHANGELOG.md
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pytion
+
+[![PyPI](https://img.shields.io/pypi/v/pytion.svg)](https://pypi.org/project/pytion)
+![PyVersion](https://img.shields.io/pypi/pyversions/pytion)
+![CodeSize](https://img.shields.io/github/languages/code-size/lastorel/pytion)
+[![LICENSE](https://img.shields.io/github/license/lastorel/pytion)](LICENSE)
+
+Independent unofficial **Python client** for the official **Notion API** (for internal integrations only)
+
+Client is built with its own object model based on API
+
+So if you are using **notion.so** and want to automate some stuff with the original API, you're welcome!  
+You can read any available data, create basic models, and even work with databases.
+
+Current Notion API version = **"2022-06-28"**
+
+_*does not use notion-sdk-py client_
+
+See [Change Log](./CHANGELOG.md)
+
+# Contents
+
+1. [Quick Start](#quick-start)
+2. [Pytion API](#pytion-api)
+   1. [Searching](#search)
+   2. [pytion.api.Element](#pytionapielement)
+3. [Models](#models)
+   1. [pytion.models](#pytionmodels)
+   2. [Supported Property types](#supported-property-types)
+   3. [Supported block types](#supported-block-types)
+      1. [Block creating examples](#block-creating-examples)
+      2. [Block deleting](#block-deleting)
+   4. [Database operations](#database-operations)
+      1. [Retrieving](#retrieving)
+      2. [Appending (creating a Page)](#appending-creating-a-page)
+      3. [Property Values](#property-values)
+4. [Logging](#logging)
+
+# Quick start
+
+```
+pip install pytion
+```
+
+Create new integration and get your Notion API Token at notion.so -> [here](https://www.notion.com/my-integrations).  
+Add your new integration 'manager' to your pages or databases by going to the page's menu (three dots), at the bottom of the menu clicking on Add connections and then searching for you new Integration.
+
+```python
+from pytion import Notion; no = Notion(token=SOME_TOKEN)
+```
+
+Or put your token for Notion API into file `token` at script directory and use simple `no = Notion()`
+
+```python
+from pytion import Notion
+no = Notion(token=SOME_TOKEN)
+page = no.pages.get("PAGE ID")  # retrieve page data (not content) and create object
+blocks = page.get_block_children()  # retrieve page content and create list of objects
+database = no.databases.get("Database ID")  # retrieve database data (not content) and create object
+# retrieve database content by filtering with sorting
+pages = database.db_filter(property_name="Done", property_type="checkbox", value=False, descending="title")
+```
+
+```
+In [1]: from pytion import Notion
+
+In [2]: no = Notion(token=SOME_TOKEN)
+
+In [3]: page = no.pages.get("a458613160da45fa96367c8a594297c7")
+In [4]: print(page)
+Notion/pages/Page(Example page)
+
+In [5]: blocks = page.get_block_children_recursive()
+
+In [6]: print(blocks)
+Notion/blocks/BlockArray(## Migration planning [x] Rese)
+
+In [7]: print(blocks.obj)
+## Migration planning
+[x] Reset new switch 2022-05-12T00:00:00.000+03:00 → 2022-05-13T01:00:00.000+03:00 
+	- reboot
+	- hold reset button
+[x] Connect to console with baud rate 9600
+[ ] Skip default configuration dialog
+Use LinkTo(configs) 
+[Integration changes](https://developers.notion.com/changelog?page=2)
+
+In [8]: print(blocks.obj.simple)
+Migration planning
+Reset new switch 2022-05-12T00:00:00.000+03:00 → 2022-05-13T01:00:00.000+03:00 
+	reboot
+	hold reset button
+Connect to console with baud rate 9600
+Skip default configuration dialog
+Use https://api.notion.com/v1/pages/90ea1231865f4af28055b855c2fba267 
+https://developers.notion.com/changelog?page=2
+```
+
+# Pytion API
+
+Almost all operations are carried out through `Notion` or `Element` object:
+
+```python
+page = no.pages.get("a458613160da45fa96367c8a594297c7")
+
+# no -> Notion
+# pages -> URI in https://api.notion.com/v1/PAGES/a458613160da45fa96367c8a594297c7
+# get -> pytion API method
+# page -> Element
+# page.obj -> Page (main data structure)
+```
+
+so:
+
+- `isinstance(no, Notion) == True`
+- `isinstance(no.pages, Element) == True`
+- `isinstance(no.databases, Element) == True`
+- `isinstance(page, Element) == True`
+- `isinstance(page.obj, Page) == True`
+
+and if you want to retrieve a database - you must use _"databases"_ URI
+
+```python
+database = no.databases.get("123412341234")
+```
+
+and the same applies for _"blocks"_ and _"users"_. Valid URI-s are:
+
+- _pages_
+- _blocks_
+- _databases_
+- _users_
+
+When you work with existing `Element` object like `page` above, all [methods](#pytionapielement) below will be applied to this Page:
+
+```python
+new_page = page.page_update(title="new page name 2")
+
+# new_page is not a new page, it is updated page
+# new_page.obj is equal page.obj except title and last_edited properties
+```
+
+## Search
+
+There is a search example:
+```python
+no = Notion(token)
+
+r = no.search("updating", object_type="page")
+print(r.obj)
+# output:
+# Page for updating
+# Page to updating databases
+```
+
+
+## pytion.api.Element
+
+There is a list of available methods for communicate with **api.notion.com**. These methods are better structured in [next chapter](#pytionmodels).
+
+`.get(id_)` - Get Element by ID.
+
+`.get_parent(id_)` - Get parent object of current object if possible.
+
+`.get_block_children(id_, limit)` - Get children Block objects of current Block object (tabulated texts) if exist.
+
+`.get_block_children_recursive(id_, max_depth, limit, force)` - Get children Block objects of current Block object (tabulated texts) if exist recursive.
+
+`.get_page_property(property_id, id_, limit)` - Retrieve a page property item.
+
+`.get_page_properties(title_only, obj)` - Retrieve the title or all properties of current Page or Page `obj`
+*(deprecated, useful for v1.3.0 only)*
+
+`.db_query(id_, limit, filter_, sorts)` - Query Database.
+
+`.db_filter(...see desc...)` - Query Database.
+
+`.db_create(database_obj, parent, properties, title)` - Create Database.
+
+**_There is no way to delete a database object yet!_**
+
+`.db_update(id_, title, properties)` - Update Database.
+
+`.page_create(page_obj, parent, properties, title)` - Create Page.
+
+`.page_update(id_, properties, title, archived)` - Update Page.
+
+`.block_update(id_, block_obj, new_text, archived)` - Update text in Block.
+
+`.block_append(id_, block, blocks)` - Append block or blocks children.
+
+`.get_myself()` - Retrieve my bot User.
+
+`.from_linkto(linkto)` - Creates new Element object based on LinkTo information.
+
+`.from_object(model)` - Creates new Element object from Page, Block or Database object. Usable while Element object contains an Array.
+
+> More details and usage examples of these methods you can see into func descriptions.
+
+# Models
+
+### pytion.models
+
+There are classes **based on API** structures:
+
+- `RichText` based on [Rich text object](https://developers.notion.com/reference/rich-text)
+- `RichTextArray` is a list of RichText objects with useful methods
+  - You can create object by simple `RichTextArray.create("My title text")` and then use it in any methods
+  - Any Rich Text getting from API will be RichTextArray
+  - `str()` returns plain text of all "Rich Texts". ez
+  - `+` operator is available with `str` and `RichTextArray`
+  - `.simple` property returns stripped plain text without any markdown syntax. useful for URL
+- `Database` based on [Database object](https://developers.notion.com/reference/database)
+  - You can create object `Database.create(...)` and/or use `.db_create(...)` API method
+  - attrs represent API model. Complex structures like `created_by` are wrapped in internal objects
+  - use `.db_update()` API method for modify a real database (for ex. properties or title)
+  - use `.db_query()` to get all database content (it will be `PageArray`)
+  - use `.db_filter()` to get database content with filtering and/or sorting
+  - has `.description` attr
+  - has `.is_inline` attr with the value True if the database appears in the page as an inline block
+- `Page` based on [Page object](https://developers.notion.com/reference/page)
+  - You can create object `Page.create(...)` and/or use `.page_create(...)` API method
+  - use `.page_update()` method to modify attributes or delete the page
+  - use `.get_block_children()` to get page content (without nested blocks) (it will be `BlockArray`)
+  - use `.get_block_children_recursive()` to get page content with nested blocks
+  - use `.get_page_property()` to retrieve the specific `PropertyValue` of the page
+- `Block` based on [Block object](https://developers.notion.com/reference/block)
+  - You can create object `Block.create(...)` of specific type from [_support matrix_](#supported-block-types) below and then use it while creating pages or appending
+  - use `.block_update()` to replace content or change _extension attributes_ or delete the block
+  - use `.block_append()` to add a new block to a page or add a nested block to another block
+  - use `.get_block_children()` to get first level nested blocks
+  - use `.get_block_children_recursive()` to get all levels nested blocks
+- `User` based on [User object](https://developers.notion.com/reference/user)
+  - You can create object `User.create(...)` and use it in some properties like `people` type property
+  - You can retrieve more data about a User by his ID using `.get()`
+  - use `.get_myself()` to retrieve the current bot User
+  - has `.workspace_name` attr for `bot` type users
+- `Property` based on [Property object](https://developers.notion.com/reference/property-object)
+  - You can create object `Property.create(...)` while creating or editing database: `.db_create()` or `.db_update()`
+  - `formula` type properties configuration is not supported
+- `PropertyValue` based on [Property values](https://developers.notion.com/reference/property-value-object)
+  - You can create object `PropertyValue.create(...)` to set or edit page properties by `.page_create()` or `.page_update()`
+  - `files`, `formula`, `rollup` type properties are not editable
+
+There are also useful **internal** classes:
+
+- `BlockArray` is found when API returns page content in "list of blocks" format
+  - it is useful to represent all content by `str()`
+  - also it has `simple` property like `RichTextArray` object
+  - it automatically indents `str` output of nested blocks
+- `PageArray` is found when API returns the result of database query (list of pages)
+- `LinkTo` is basic internal model to link to any Notion object
+  - You can create object `LinkTo.create()` and use it in many places and methods
+  - use `LinkTo(from_object=my_page1)` to quickly create a link to any existing object of pytion.models
+  - `link` property of `LinkTo` returns expanded URL
+- `ElementArray` is found while using `.search()` endpoint. It's a parent of `PageArray`
+
+> And every model has a `.get()` method that returns API friendly JSON.
+ 
+### Supported Property types
+
+| Property type            | value type                       | read (DB) | read value (Page) | create (DB) | create value (Page) | Oper attrs                          | Config attrs                                                                                                 |
+|--------------------------|----------------------------------|-----------|-------------------|-------------|---------------------|-------------------------------------|--------------------------------------------------------------------------------------------------------------|
+| `title`                  | `RichTextArray`                  | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `rich_text`              | `RichTextArray`                  | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `number`                 | `int`/`float`                    | +         | +                 | +           | +                   |                                     | ~~format~~                                                                                                   |
+| `select`                 | `str`                            | +         | +                 | +           | +                   |                                     | ~~options~~                                                                                                  |
+| `multi_select`           | `List[str]`                      | +         | +                 | +           | +                   |                                     | ~~options~~                                                                                                  |
+| `status`                 | `str`                            | +         | +                 | +           | +\*\*\*\*           |                                     | `options`, `groups` (read-only)                                                                              |
+| `date`                   | `str`                            | +         | +                 | +           | +                   | `start: datetime` `end: datetime`\* |                                                                                                              |
+| `people`                 | `List[User]`                     | +         | +                 | +           | +\*\*               |                                     |                                                                                                              |
+| `files`                  |                                  | +         | -                 | +           | -                   |                                     |                                                                                                              |
+| `checkbox`               | `bool`                           | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `url`                    | `str`                            | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `email`                  | `str`                            | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `phone_number`           | `str`                            | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `formula`                |                                  | -         | +                 | -           | n/a                 |                                     |                                                                                                              |
+| `relation`               | `List[LinkTo]`                   | +         | +                 | +           | +                   | `has_more: bool`                    | `single_property` / `dual_property`                                                                          |
+| `rollup`                 | depends on relation and function | +         | +                 | +           | n/a                 | ~~has_more~~\*\*\*\*\*              | `function`, `relation_property_id` / `relation_property_name`, `rollup_property_id` / `rollup_property_name` |
+| `created_time`\*\*\*     | `datetime`                       | +         | +                 | +           | n/a                 |                                     |                                                                                                              |
+| `created_by`\*\*\*       | `User`                           | +         | +                 | +           | n/a                 |                                     |                                                                                                              |
+| `last_edited_time`\*\*\* | `datetime`                       | +         | +                 | +           | n/a                 |                                     |                                                                                                              |
+| `last_edited_by`\*\*\*   | `User`                           | +         | +                 | +           | n/a                 |                                     |                                                                                                              |
+
+> [\*] - Create examples:  
+> `pv = PropertyValue.create(type_="date", value=datetime.now())`  
+> `pv = PropertyValue.create(type_="date", date={"start": str(datetime(2022, 2, 1, 5)), "end": str(datetime.now())})`  
+> [\*\*] - Create example:  
+> `user = User.create('1d393ffb5efd4d09adfc2cb6738e4812')`  
+> `pv = PropertyValue.create(type_="people", value=[user])`  
+> [\*\*\*] - Every Base model like Page already has mandatory attributes created/last_edited returned by API  
+> [\*\*\*\*] - Status type is not configurable. API doesn't support NEW options added via Property modify or updating a Page
+> [\*\*\*\*\*] - Notion API hasn't `has_more` attr. Only 25 references can be shown in the array
+
+More details and examples can be found in Database [section](#property-values)
+
+More details and examples can be found in Database [section](#property-values)
+
+
+## Supported block types
+
+At present the API only supports the block types which are listed in the reference below. Any unsupported block types will continue to appear in the structure, but only contain a `type` set to `"unsupported"`.
+Colors are not yet supported.
+
+Every Block has mandatory attributes and extension attributes. There are mandatory:
+
+- `id: str` - UUID-64 without hyphens
+- `object: str` - always `"block"` (from API)
+- `created_time: datetime` - from API
+- `created_by: User` - from API
+- `last_edited_time: datetime` - from API
+- `last_edited_by: User` - from API
+- `type: str` - the type of block (from API)
+- `has_children: bool` - does the block have children blocks (from API)
+- `archived: bool` - does the block marked as deleted (from API)
+- `text: Union[str, RichTextArray]` - **main content**
+- `simple: str` - only simple text string (url expanded)
+
+Extension attributes are listed below in support matrix:
+
+| Block Type           | Description                               | Read support | Create support | Can have children | Extension attributes                              |
+|----------------------|-------------------------------------------|--------------|----------------|-------------------|---------------------------------------------------|
+| `paragraph`          | Simple Block with text                    | +            | +              | +                 |                                                   |
+| `heading_1`          | Heading Block with text highest level     | +            | +              | -/+\*             | `is_toggleable: bool`                             |
+| `heading_2`          | Heading Block with text medium level      | +            | +              | -/+\*             | `is_toggleable: bool`                             |
+| `heading_3`          | Heading Block with text lowest level      | +            | +              | -/+\*             | `is_toggleable: bool`                             |
+| `bulleted_list_item` | Text Block with bullet                    | +            | -              | +                 |                                                   |
+| `numbered_list_item` | Text Block with number                    | +            | -              | +                 |                                                   |
+| `to_do`              | Text Block with checkbox                  | +            | +              | +                 | `checked: bool`                                   |
+| `toggle`             | Text Block with toggle to children blocks | +            | -              | +                 |                                                   |
+| `code`               | Text Block with code style                | +            | +              | +                 | `language: str`, `caption: RichTextArray`         |
+| `child_page`         | Page inside                               | +            | -              | +                 |                                                   |
+| `child_database`     | Database inside                           | +            | -              | +                 |                                                   |
+| `embed`              | Embed online content                      | +            | -              | -                 | `caption: RichTextArray`                          |
+| `image`              | Embed image content                       | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
+| `video`              | Embed video content                       | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
+| `file`               | Embed file content                        | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
+| `pdf`                | Embed pdf content                         | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
+| `bookmark`           | Block for URL Link                        | +            | -              | -                 | `caption: RichTextArray`                          |
+| `callout`            | Highlighted footnote text Block           | +            | -              | +                 | `icon: dict`                                      |
+| `quote`              | Text Block with quote style               | +            | -              | +                 |                                                   |
+| `equation`           | KaTeX compatible text Block               | +            | -              | -                 |                                                   |
+| `divider`            | Simple line to divide the page            | +            | -              | -                 |                                                   |
+| `table_of_contents`  | Block with content structure in the page  | +            | -              | -                 |                                                   |
+| `column`             |                                           | -            | -              | +                 |                                                   |
+| `column_list`        |                                           | -            | -              | -                 |                                                   |
+| `link_preview`       | Same as `bookmark`                        | +            | -              | -                 |                                                   |
+| `synced_block`       | Block for synced content aka parent       | +            | -              | +                 | `synced_from: LinkTo`                             |
+| `template`           | Template Block title                      | +            | -              | +                 |                                                   |
+| `link_to_page`       | Block with link to particular page `@...` | +            | -              | -                 | `link: LinkTo`                                    |
+| `table`              | Table Block with some attrs               | +            | -              | +                 | `table_width: int`                                |
+| `table_row`          | Children Blocks with table row content    | +            | -              | -                 |                                                   |
+| `breadcrumb`         | Empty Block actually                      | +            | -              | -                 |                                                   |
+| `unsupported`        | Blocks unsupported by API                 | +            | -              | -                 |                                                   |
+
+> [\*] - `heading_X` blocks can have children if `is_toggleable` is True 
+
+### Block creating examples
+
+Create `paragraph` block object and add it to Notion:
+
+```python
+from pytion.models import Block
+my_text_block = Block.create("Hello World!")
+my_text_block = Block.create(text="Hello World!", type_="paragraph")  # the same
+
+# indented append my block to other known block:
+no.blocks.block_append("5f60073a9dda4a9c93a212a74a107359", block=my_text_block)
+
+# append my block to a known page (in the end)
+no.blocks.block_append("9796f2525016128d9af4bf12b236b555", block=my_text_block)  # the same operation actually
+
+# another way to append:
+my_page = no.pages.get("9796f2525016128d9af4bf12b236b555")
+my_page.block_append(block=my_text_block)
+```
+
+Create `to_do` block object:
+
+```python
+from pytion.models import Block
+my_todo_block = Block.create("create readme documentation", type_="to_do")
+my_todo_block2 = Block.create("add 'create' method", type_="to_do", checked=True)
+```
+
+Create `code` block object:
+
+```python
+from pytion.models import Block
+my_code_block = Block.create("code example here", type_="code", language="javascript")
+my_code_block2 = Block.create("another code example", type_="code", caption="it will be plain text code block with caption")
+```
+
+Create `heading` block object:
+
+```python
+from pytion.models import Block
+my_code_block = Block.create("Title 1 example here", type_="heading_1")
+my_code_block2 = Block.create("Toggle Title 2", type_="heading_2", is_toggleable=True)
+```
+
+### Block deleting
+
+```python
+no.blocks.block_update("3d4af9f0f98641dea8c44e3864eed4d0", archived=True)
+# or if you have Element with Block object already
+block.block_update(archived=True)
+```
+
+## Database operations
+
+### Retrieving
+
+```python
+from pytion import Notion
+no = Notion(token=TOKEN)
+
+# get all pages from Database
+# example 1
+pages = no.databases.db_query("114f1ef1f1241e2f12f41fe2f")
+# example 2
+db = no.databases.get("114f1ef1f1241e2f12f41fe2f")
+pages = db.db_query()
+print(pages.obj)
+
+# get pages with "task" in title
+pages = db.db_filter("task")
+
+# get all pages with sorting by property name "Tags"
+pages = db.db_filter("", ascending="Tags")
+pages = db.db_filter("", descending="Tags")
+
+# get pages with Status property equals Done
+pages = db.db_filter(property_name="Status", property_type="status", value="Done")
+
+# get pages with Price property greater than 150
+pages = db.db_filter(property_name="Price", property_type="number", condition="greater_than", value=150)
+
+# complex query
+pages = db.db_filter(
+    property_name="WorkTime", property_type="date", condition="before",
+    value=datetime.now(), descending="Deadline", limit=25
+)
+```
+
+> Queries with multifiltering and multisorting are not supported  
+> But you can compose your custom filter dict from API reference and call `db.db_filter(raw={...})` 
+
+Filter conditions and types combination -> [Official API reference](https://developers.notion.com/reference/post-database-query-filter)
+
+After you got `pages` which is `Element` object, you can not call API methods directly on `pages`
+because there is `PageArray` object with List of Pages.
+If you need to change a Page or something else, you can follow these steps:
+
+```python
+# 1. create new Element object with non-list object type
+page = no.pages.from_object(pages.obj[14])  # choosed page from the PageArray
+# 2. call the desired API method on this page
+page.page_update(archived=True)  # delete Page example
+```
+
+### Appending (creating a Page)
+
+There is a way to create a row into database. The same method is used to create any Page.
+The difference is in only in `parent` argument which can be the Page or the Database.
+
+```python
+from pytion.models import LinkTo
+
+# choose the parent target
+# it can be the database
+parent = LinkTo.create(database_id="043cb52491a44b80a5e5006237a4278f")
+# or the page
+parent2 = LinkTo.create(page_id="043cb52491a44b80a5e5006237a4278f")
+
+# if you need to set Properties
+from pytion.models import PropertyValue
+props = {
+            "Tags": PropertyValue.create(type_="multi_select", value=["tag1", "tag2"]),
+            "done": PropertyValue.create("checkbox", True),
+            "AnotherPropertyNAME": PropertyValue.create("date", datetime.now()),
+        }
+
+# create the Page
+page = no.pages.page_create(parent=parent, title="Page 2")  # without properties (will be empty)
+# or
+page2 = no.pages.page_create(parent=parent, properties=props, title="Page 2")  # with properties
+```
+
+### Property Values
+
+Pytion Properties support table is described [above](#supported-property-types)
+
+There are Properties that are used in Database operations and PropertyValues that are used in Page operations.
+
+It's necessary to choose the type (`type_` arg) and value (`value`) of property.
+The table shows the mapping between Property type and value (python) type.
+
+The `type_` must correspond to your database schema in Notion.
+
+```python
+from datetime import datetime
+from pytion.models import PropertyValue, LinkTo, RichTextArray, User
+
+# + relation type:
+pv = PropertyValue.create("relation", value=[LinkTo.create(page_id="04262843082a478d97f741948a32613b")])
+# + people type:
+pv = PropertyValue.create(type_="people", value=[User.create('1d393ffb5efd4d09adfc2cb6738e4812')])
+# + date type:
+pv = PropertyValue.create(type_="date", value=datetime.now())
+pv = PropertyValue.create(type_="date", date={"start": str(datetime(2022, 2, 1, 5)), "end": str(datetime.now())})
+# + rich_text (text or title field)
+pv = PropertyValue.create(type_="rich_text", value="Something Interesting")
+pv = PropertyValue.create("rich_text", value=RichTextArray.create("Something Interesting"))
+# + nubmer
+pv = PropertyValue.create(type_="number", value=156.2)
+# + status
+pv = PropertyValue.create("status", value="Done")
+
+# update needed property values
+new_props = {
+    "Tags": PropertyValue.create("multi_select", ["tag2"]),
+    "done": PropertyValue.create("checkbox", False),
+    "when": PropertyValue.create("date", datetime.now()),
+}
+page = page_for_updates.page_update(properties=new_props)
+page = no.pages.page_update(page_for_updates_id, properties=new_props)  # the same
+
+# rename (edit title property)
+page = page_for_updates.page_update(title=new_name)
+```
+
+Pytion also provides the ways to change database schema - create/update/rename/delete properties:
+
+```python
+from pytion.models import Property
+
+# rename property
+properties = {"Name": Property.create(type_="title", name="Subject")}
+database = database_for_updates.db_update(properties=properties)
+database = no.databases.db_update(database_for_updates_id, properties=properties)  # the same
+# change property type
+properties = {"Tags": Property.create("select")}
+database = database_for_updates.db_update(properties=properties)
+# delete property from database
+properties = {"Old property name": Property.create(None)}
+database = database_for_updates.db_update(properties=properties)
+# rename database
+database = database_for_updates.db_update(title="Refactoring")
+```
+
+# Logging
+
+Logging is muted by default. To enable to stdout and/or to file:
+
+```python
+from pytion import setup_logging
+
+setup_logging(level="debug", to_console=True, filename="pytion.log")
+```
```

### Comparing `pytion-1.3.3/pytion/__init__.py` & `pytion-1.3.4/pytion/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-import logging
-from typing import Optional, Union
-
-import pytion.envs as envs
-from pytion.api import Notion
-from pytion.exceptions import *
-
-
-def setup_logging(
-        level: Union[int, str] = logging.INFO, to_console: bool = True, filename: Optional[str] = None
-) -> None:
-    """
-
-    :param level:       "debug", "info", "warning", "error", "critical" or `logging.INFO` etc.
-    :param to_console:  True/False to output to stdout
-    :param filename:    filename to put logs into file. or None
-    :return:
-    """
-    log_levels = {
-        "debug": logging.DEBUG,
-        "info": logging.INFO,
-        "warning": logging.WARNING,
-        "error": logging.ERROR,
-        "critical": logging.CRITICAL,
-    }
-    if isinstance(level, str):
-        if level not in log_levels:
-            raise ValueError("Invalid log level")
-        level = log_levels[level]
-    logger = logging.getLogger(__name__)
-    logger.handlers.clear()
-    logger.addHandler(logging.NullHandler())
-    logger.setLevel(level)
-    formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-    if to_console:
-        console_handler = logging.StreamHandler()
-        console_handler.setFormatter(formatter)
-        logger.addHandler(console_handler)
-    if filename:
-        file_handler = logging.FileHandler(filename)
-        file_handler.setFormatter(formatter)
-        logger.addHandler(file_handler)
-
-
-setup_logging(level=envs.LOGGING_BASE_LEVEL, to_console=envs.LOGGING_TO_CONSOLE, filename=envs.LOGGING_FILE)
+import logging
+from typing import Optional, Union
+
+import pytion.envs as envs
+from pytion.api import Notion
+from pytion.exceptions import *
+
+
+def setup_logging(
+        level: Union[int, str] = logging.INFO, to_console: bool = True, filename: Optional[str] = None
+) -> None:
+    """
+
+    :param level:       "debug", "info", "warning", "error", "critical" or `logging.INFO` etc.
+    :param to_console:  True/False to output to stdout
+    :param filename:    filename to put logs into file. or None
+    :return:
+    """
+    log_levels = {
+        "debug": logging.DEBUG,
+        "info": logging.INFO,
+        "warning": logging.WARNING,
+        "error": logging.ERROR,
+        "critical": logging.CRITICAL,
+    }
+    if isinstance(level, str):
+        if level not in log_levels:
+            raise ValueError("Invalid log level")
+        level = log_levels[level]
+    logger = logging.getLogger(__name__)
+    logger.handlers.clear()
+    logger.addHandler(logging.NullHandler())
+    logger.setLevel(level)
+    formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+    if to_console:
+        console_handler = logging.StreamHandler()
+        console_handler.setFormatter(formatter)
+        logger.addHandler(console_handler)
+    if filename:
+        file_handler = logging.FileHandler(filename)
+        file_handler.setFormatter(formatter)
+        logger.addHandler(file_handler)
+
+
+setup_logging(level=envs.LOGGING_BASE_LEVEL, to_console=envs.LOGGING_TO_CONSOLE, filename=envs.LOGGING_FILE)
```

### Comparing `pytion-1.3.3/pytion/api.py` & `pytion-1.3.4/pytion/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,608 +1,608 @@
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-import logging
-from typing import Optional, Union, Dict, List
-
-import pytion.envs as envs
-from pytion.query import Request, Filter, Sort
-from pytion.models import Database, Page, Block, BlockArray, PropertyValue, PageArray, LinkTo, RichTextArray, Property
-from pytion.models import ElementArray, User
-
-
-Models = Union[Database, Page, Block, BlockArray, PropertyValue, PageArray, ElementArray]
-logger = logging.getLogger(__name__)
-
-
-class Notion(object):
-    def __init__(self, token: Optional[str] = None, version: Optional[str] = None):
-        """
-        Creates main API object.
-
-        :param token:   provide your integration API token. If None - find the file `token`
-        :param version: provide non hardcoded API version
-        """
-        self.version = version if version else envs.NOTION_VERSION
-        self.session = Request(api=self, token=token)
-        logger.debug(f"API object created. Version {envs.NOTION_VERSION}")
-
-    def search(
-            self, query: Optional[str] = None, limit: int = 0,
-            object_type: Optional[str] = None, sort_last_edited_time: Optional[str] = None
-    ) -> Optional[Element]:
-        """
-        Searches all original pages, databases, and child pages/databases that are shared with the integration.
-        It will not return linked databases, since these duplicate their source databases. (c)
-
-
-        :param query:                   search by page title
-        :param limit:                   0 < int < 100 - max number of items to be returned (0 = return all)
-        :param object_type:             filter by type: 'page' or 'database'
-        :param sort_last_edited_time:   sorting 'ascending' or 'descending'
-        :return:
-
-        `r = no.search("pytion", 10, sort_last_edited_time="ascending")`
-        `print(r.obj)`
-        """
-        data = {"query": query} if query else None
-        filter_ = Filter(raw={"property": "object", "value": object_type}) if object_type else None
-        if sort_last_edited_time:
-            sort_last_edited_time = Sort(property_name="last_edited_time", direction=sort_last_edited_time)
-        result = self.session.method(
-            "post", "search", sort=sort_last_edited_time, filter_=filter_, limit=limit, data=data
-        )
-        if "results" in result and isinstance(result["results"], list):
-            data = ElementArray(result["results"])
-            for item in data:
-                if isinstance(item, Page):
-                    self.pages.get_page_properties(title_only=True, obj=item)
-            return Element(api=self, name="search", obj=data)
-        else:
-            logger.warning("Results list is not found")
-            return None
-
-    def __len__(self):
-        return 1
-
-    def __repr__(self):
-        return "NotionAPI"
-
-    def __str__(self):
-        return self.__repr__()
-
-    def __getattr__(self, name):
-        if name in dir(self):
-            return self.name
-        return Element(self, name)
-
-
-class Element(object):
-    class_map = {"page": Page, "database": Database, "block": Block, "user": User}
-
-    def __init__(self, api: Notion, name: str, obj: Optional[Models] = None):
-        self.api = api
-        self.name = name
-        self.obj = obj
-        logger.debug(f"Element {self!r} created")
-
-    def get(self, id_: str, _after_path: str = None, limit: int = 0) -> Element:
-        """
-        Get Element by ID.
-        .exceptions.ObjectNotFound exception if not found
-
-        :return:    `Element.obj` may be `Page`, `Database`, `Block`
-
-        result = no.databases.get("1234123412341")
-        result = no.pages.get("123412341234")
-        result = no.blocks.get("123412341234")
-        result = no.users.get("123412341234")
-        print(result.obj)
-        """
-        if "-" in id_:
-            id_ = id_.replace("-", "")
-        if not _after_path:
-            raw_obj = self.api.session.method(method="get", path=self.name, id_=id_, limit=limit)
-        else:
-            raw_obj = self.api.session.method(
-                method="get", path=self.name, id_=id_, after_path=_after_path, limit=limit
-            )
-        if raw_obj["object"] == "list":
-            if self.name == "pages":
-                self.obj = PageArray(raw_obj["results"])
-            elif self.name == "blocks":
-                self.obj = BlockArray(raw_obj["results"])
-            else:
-                self.obj = ElementArray(raw_obj["results"])
-        else:
-            self.obj = self.class_map[raw_obj["object"]](**raw_obj)
-        return self
-
-    def get_parent(self, id_: Optional[str] = None) -> Optional[Element]:
-        """
-        Get parent object of current object if possible.
-
-        :param id_:
-        :return:    Element (parent object) or None. `.obj` may be `Page`, `Database`, `Block`
-
-        `result = no.blocks.get_parent("123412341234")`
-        `print(result)`
-        Notion/pages/Page(Page Title here)
-        `result = result.get_parent()`
-        `print(result)`
-        Notion/databases/Database(Some database name)
-        """
-        if not self.obj:
-            self.get(id_)
-        if getattr(self.obj, "parent", None):
-            return self.from_linkto(self.obj.parent)
-        logger.warning(f"Parent object can not be found")
-        return None
-
-    def get_block_children(
-            self, id_: Optional[str] = None, block: Optional[Block] = None, limit: int = 0
-    ) -> Optional[Element]:
-        """
-        Get children Block objects of current Block object (tabulated texts) if exist (else None)
-
-        :param id_:
-        :param block: you can provide a Block object instead to get his children
-        :param limit:   0 < int < 100 - max number of items to be returned (0 = return all)
-        :return:        `Element.obj` will be BlockArray object even nothing is found
-
-        `print(no.pages.get_block_children("PAGE ID"))`
-        None
-
-        `print(no.blocks.get_block_children("PAGE ID"))`
-        Notion/blocks/BlockArray(Heading 2 level Paragraph some)
-
-        `print(no.blocks.get_block_children("PAGE ID").obj)`
-        Heading 2 level
-        Paragraph
-        some text
-
-        BlockArray or Database object expected.
-        """
-        if self.name not in ("blocks", "pages"):
-            logger.warning("Only `blocks` or `pages` can have children")
-            return None
-        if isinstance(id_, str) and "-" in id_:
-            id_ = id_.replace("-", "")
-        obj = block if block else self.obj
-        if obj:
-            return self.from_linkto(obj.children, limit=limit)
-        child = self.api.session.method(
-            method="get", path="blocks", id_=id_, after_path="children", limit=limit
-        )
-        # children object returns list of Blocks
-        if child["object"] != "list":
-            logger.warning(f"List of Blocks expected. Received\n{child}")
-            return None
-        return Element(api=self.api, name="blocks", obj=BlockArray(child["results"]))
-
-    def get_block_children_recursive(
-        self, id_: Optional[str] = None, max_depth: int = 10, block: Optional[Block] = None,
-        _cur_depth: int = 0, limit: int = 0, force: bool = False
-    ) -> Optional[Element]:
-        """
-        Get children Block objects of current Block object (tabulated texts) if exist (else None) recursive
-
-        :param id_:
-        :param block:       you can provide a Block object instead to get his children
-        :param max_depth:   how deep use the recursion (block inside block inside block etc.)
-        :param limit:       0 < int < 100 - max number of items to be returned (0 = return all)
-        :param force:       get blocks in subpages too
-        :return:            `Element.obj` will be BlockArray object even nothing is found
-
-        `print(no.blocks.get_block_children_recursive("PAGE ID").obj)`
-        Heading 2 level
-        Paragraph
-            block inside block
-        some text
-        """
-        if self.name not in ("blocks", "pages"):
-            logger.warning("Only `blocks` or `pages` can have children")
-            return None
-        if isinstance(id_, str) and "-" in id_:
-            id_ = id_.replace("-", "")
-        obj = block if block else self.obj
-        if obj:
-            id_ = obj.id
-            if isinstance(obj, Block) and obj.type == "child_database":
-                return self.from_linkto(obj.children)
-        child = self.api.session.method(
-            method="get", path="blocks", id_=id_, after_path="children", limit=limit
-        )
-        ba = BlockArray([])
-        for b in child["results"]:
-            block_obj = Block(level=_cur_depth, **b)
-            ba.append(block_obj)
-            # Do not get subpages if not force
-            if block_obj.type == "child_page" and not force:
-                continue
-            if block_obj.has_children and _cur_depth < max_depth:
-                sub_element = Element(api=self.api, name="blocks").get_block_children_recursive(
-                    id_=block_obj.id, max_depth=max_depth, _cur_depth=_cur_depth + 1, limit=limit, force=force
-                )
-                ba.extend(sub_element.obj)
-
-        return Element(api=self.api, name="blocks", obj=ba)
-
-    def get_page_property(self, property_id: str, id_: Optional[str] = None, limit: int = 0) -> Optional[Element]:
-        """
-        DEPRECATED
-        Retrieve a page property item.
-
-        :param property_id: ID of property in current database
-        :param id_:         ID of page in that database (if not `self.obj`)
-        :param limit:       0 < int < 100 - max number of items to be returned (0 = return all)
-        :return:            `Element.obj` will be PropertyValue object
-
-        `db = no.databases.get("1232412341234")`
-        `property_id = db.obj.properties["Last edited time"].id`
-        `result = no.pages.get_page_property(property_id, 'PAGE ID 152f123a12344')`
-        `print(result.obj)`
-        2021-11-04 16:47:00+00:00
-        """
-        if self.name != "pages":
-            logger.warning("Only `pages` can have properties")
-            return None
-        if isinstance(id_, str) and "-" in id_:
-            id_ = id_.replace("-", "")
-        if self.obj and not id_:
-            id_ = self.obj.id
-        property_obj = self.api.session.method(
-            method="get", path=self.name, id_=id_, after_path="properties/"+property_id, limit=limit
-        )
-        return Element(api=self.api, name=f"pages/{id_}/properties", obj=PropertyValue(property_obj, property_id))
-
-    def get_page_properties(self, title_only: bool = False, obj: Optional[Page] = None) -> None:
-        """
-        Page properties must be retrieved using the page properties endpoint. (c)
-        after retrieving a Page object you can retrieve its properties
-
-        obj or self.obj must be a Page
-        :return:
-        """
-        if not obj:
-            obj = self.obj
-        if obj and isinstance(obj, Page):
-            for prop in obj.properties:
-                # Skip already retrieved properties
-                if isinstance(obj.properties[prop], PropertyValue):
-                    continue
-                prop_id = obj.properties[prop].id
-                if title_only and prop_id != "title":
-                    continue
-                result = self.get_page_property(prop_id, id_=obj.id)
-                obj.properties[prop] = result.obj
-                if prop_id == "title":
-                    obj.title = result.obj.value if result.obj.value else ""
-            return
-        logger.warning("You must provide a Page to retrieve properties")
-
-    def db_query(
-            self,
-            id_: Optional[str] = None,
-            limit: int = 0,
-            filter_: Optional[Filter] = None,
-            sorts: Optional[Sort] = None,
-            **kwargs,
-    ) -> Optional[Element]:
-        if self.name != "databases":
-            logger.warning("Only `databases` can be queried")
-            return None
-        if isinstance(id_, str) and "-" in id_:
-            id_ = id_.replace("-", "")
-        if self.obj:
-            id_ = self.obj.id
-        r = self.api.session.method(
-            method="post", path=self.name, id_=id_, after_path="query",
-            data={}, limit=limit, filter_=filter_, sorts=sorts
-        )
-        if r["object"] != "list":
-            return None
-        return Element(api=self.api, name="pages", obj=PageArray(r["results"]))
-
-    def db_filter(self, title: str = None, **kwargs) -> Optional[Element]:
-        """
-        :param title: filter by title contains + opt. attrs: condition, sort etc.
-        OR
-        :param property_name: mandatory - full name or ID of property to filter by
-        :param value: the value of this property to filter by (may be bool or datetime etc.)
-        :param property_type: mandatory field - `text`, `number`, `checkbox`, `date`, `select` etc.
-        :param condition: optional field - it depends on the type: `starts_with`, `contains`, `equals` etc.
-        :param raw: correctly formatted dict to pass direct to API (instead of all other params)
-        :param property_obj: Property or PropertyValue obj. instead of `property_name` and `property_type`,
-                             PropertyValue can put value in request, if `value` is not provided
-
-        :param ascending: property name to be sorted by
-        :param descending: property name to be sorted by
-
-        :param limit: 0 < int < 100 - max number of items to be returned (0 = return all)
-        :return:              self.obj -> PageArray
-
-        examples
-        `.db_filter("My Page Title")`
-        `.db_filter("", ascending="Tags")`
-        `.db_filter(property_name="Done", property_type="checkbox")`
-        `.db_filter(property_name="Done", property_type="checkbox", value=False, descending="title")`
-        `.db_filter(property_name="tags", property_type="multi_select", condition="is_not_empty")`
-        `.db_filter(raw=YOUR_BIG_DICT_FROM_NOTION_DOCS, limit=2)`
-
-        Filters combinations are not supported. (in `raw` param only)
-        """
-        if self.name == "databases" and self.obj:
-            sort = None
-            if kwargs.get("ascending"):
-                sort = Sort(property_name=kwargs["ascending"], direction="ascending")
-            elif kwargs.get("descending"):
-                sort = Sort(property_name=kwargs["descending"], direction="descending")
-            if isinstance(title, str):
-                filter_obj = Filter(property_name="title", value=title, property_type="title", **kwargs)
-            else:
-                filter_obj = Filter(**kwargs)
-            return self.db_query(filter_=filter_obj, sorts=sort, **kwargs)
-        logger.warning("Database must be provided. use .get() before")
-        return None
-
-    def db_create(
-            self,
-            database_obj: Optional[Database] = None,
-            parent: Optional[LinkTo] = None,
-            properties: Optional[Dict[str, Property]] = None,
-            title: Optional[Union[str, RichTextArray]] = None,
-            description: Optional[Union[str, RichTextArray]] = None,
-    ) -> Optional[Element]:
-        """
-        :param database_obj:  you can provide `Database` object or -
-                              provide the params for creating it:
-        :param parent:        parent object in LinkTo format. workspace can not be a parent
-        :param properties:    dict of properties. Property with `title` type is mandatory!
-        :param title:         your name of the Database
-        :param description:   optional description for new Database
-        :return:              self.obj -> Database
-
-        `parent = LinkTo.create(database_id="24512345125123421")`
-        `p1 = Property.create(name="renamed")`
-        `p2 = Property.create(type_="multi_select", name="multiselected")`
-        `props = {"Property1_name": p1, "Property2_name": p2}` OR
-        ```props = {
-            "Name": Property.create("title")
-            "Digit": Property.create("number"),
-            "Status": Property.create("select")
-        }```
-        `db = db.db_create(parent=parent, properties=props, title=RichTextArray.create("NEW DB"))`
-        """
-        if self.name != "databases":
-            logger.warning("Method supports `databases` only")
-            return None
-        if database_obj:
-            db = database_obj
-        else:
-            if isinstance(title, str):
-                title = RichTextArray.create(title)
-            db = Database.create(parent=parent, properties=properties, title=title, description=description)
-        created_db = self.api.session.method(method="post", path=self.name, data=db.get())
-        self.obj = Database(**created_db)
-        return self
-
-    def db_update(
-            self, id_: Optional[str] = None, title: Optional[Union[str, RichTextArray]] = None,
-            properties: Optional[Dict[str, Property]] = None
-    ) -> Optional[Element]:
-        """
-        :param id_:         provide id of database if `self.obj` is empty
-        :param title:       provide RichTextArray or text to rename database
-        :param properties:  provide dict of Property to update them
-        :return:            self.obj -> Database
-
-
-        `rename_prop = Property.create(name="renamed")`
-        `rename_retype_prop = Property.create(type_="multi_select", name="multiselected")`
-        `retype_prop = Property.create("checkbox")`
-        `props = {"Property1_name": rename_retype_prop, "Property2_ID": retype_prop}`
-        `db = db.db_update(properties=props, title=RichTextArray.create("NEW DB"))`
-        """
-        if self.name != "databases":
-            logger.warning("Method supports `databases` only")
-            return None
-        if isinstance(id_, str) and "-" in id_:
-            id_ = id_.replace("-", "")
-        if self.obj:
-            id_ = self.obj.id
-        patch = {}
-        if title:
-            if isinstance(title, str):
-                title = RichTextArray.create(title)
-            patch["title"] = title.get()
-        if properties:
-            patch["properties"] = {name: value.get() for name, value in properties.items()}
-        updated_db = self.api.session.method(method="patch", path=self.name, id_=id_, data=patch)
-        self.obj = Database(**updated_db)
-        return self
-
-    def page_create(
-            self,
-            page_obj: Optional[Page] = None,
-            parent: Optional[LinkTo] = None,
-            properties: Optional[Dict[str, PropertyValue]] = None,
-            title: Optional[Union[str, RichTextArray]] = None,
-            children: Optional[BlockArray, List[Block]] = None,
-    ) -> Optional[Element]:
-        """
-        :param page_obj:      you can provide `Page` object or -
-                              provide the params for creating it:
-        :param parent:        LinkTo object with ID of parent element. workspace can not be a parent
-        :param properties:    Dict of properties with values
-        :param title:         New title
-        :param children:      Content of new page in [Block] or BlockArray format
-        :return:              self.obj -> Page
-
-        `parent = LinkTo.create(database_id="24512345125123421")`
-        `p2 = PropertyValue.create("date", datetime.now())`
-        `r = no.pages.page_create(parent=parent, properties={"Count": p1, "Date": p2}, title="Extra PAGE")`
-
-        `props["Status"] = PropertyValue.create("select", "new select option")`
-        `props["Tags"] = PropertyValue.create("multi_select", ["new-option1", "new option2"])`
-        `no.pages.create(parent=parent, properties=props)`
-
-        `parent2 = LinkTo.create(page_id="123412341234")`
-        `no.pages.page_create(parent=parent2, title="New page 121")`
-        """
-        if self.name != "pages":
-            logger.warning("Method supports `pages` only")
-            return None
-        if page_obj:
-            page = page_obj
-        else:
-            if children and not isinstance(children, BlockArray):
-                children = BlockArray(children, create=True)
-            page = Page.create(parent=parent, properties=properties, title=title, children=children)
-        created_page = self.api.session.method(method="post", path=self.name, data=page.get())
-        self.obj = Page(**created_page)
-        return self
-
-    def page_update(
-            self, id_: Optional[str] = None, properties: Optional[Dict[str, PropertyValue]] = None,
-            title: Optional[Union[str, RichTextArray]] = None, archived: bool = False
-    ) -> Optional[Element]:
-        """
-        :param id_:         ID of page
-        :param properties:  dict of existing properties
-        :param title:
-        :param archived:    set to `True` for delete the page
-        :return:            self.obj -> Page
-        """
-        if self.name != "pages":
-            logger.warning("Method supports `pages` only")
-            return None
-        if isinstance(id_, str) and "-" in id_:
-            id_ = id_.replace("-", "")
-        if self.obj:
-            id_ = self.obj.id
-        patch = {}
-        if properties:
-            patch["properties"] = {name: p.get() for name, p in properties.items()}
-        if title:
-            patch.setdefault("properties", {})
-            patch["properties"]["title"] = PropertyValue.create("title", title).get()
-        # if archived:
-        patch["archived"] = archived
-        updated_page = self.api.session.method(method="patch", path=self.name, id_=id_, data=patch)
-        self.obj = Page(**updated_page)
-        return self
-
-    def block_update(
-            self, id_: Optional[str] = None, block_obj: Optional[Block] = None,
-            new_text: Optional[str] = None, archived: bool = False
-    ) -> Optional[Element]:
-        """
-        Updates text of Block.
-        `text`, `checked` (`to_do` type), `language` (`code` type) fields support only!
-        You can modify any attrs of existing block and provide it (Block object) to this func.
-        Changing the Block type is not supported.
-
-        :param id_:         ID of block to change text OR
-        :param block_obj:   modified Block (replace mode only)
-
-        :param new_text:    new text (replace mode only)
-        :param archived:    flag to delete that Block
-        :return:            self.obj -> Block
-
-        `blocks = no.blocks.get_block_children("PAGE ID")`
-        `for b in blocks.obj:`
-            `no.blocks.block_update(block_obj=b, new_text="OH YEEEAHH")`
-        `for b in blocks.obj:`
-            `b.text = "ALL IS DONE"`
-            `no.blocks.block_update(block_obj=b)`
-        """
-        if self.name != "blocks":
-            logger.warning("Method supports `blocks` only")
-            return None
-        if isinstance(id_, str) and "-" in id_:
-            id_ = id_.replace("-", "")
-        if self.obj:
-            id_ = self.obj.id
-        else:
-            self.get(id_)
-        if block_obj:
-            self.obj = block_obj
-        if not self.obj.get():
-            return None
-        if new_text:
-            self.obj.text = new_text
-        patch = {"archived": archived}
-        patch.update(self.obj.get())
-        updated_block = self.api.session.method(method="patch", path=self.name, id_=id_, data=patch)
-        self.obj = Block(**updated_block)
-        return self
-
-    def block_append(
-            self, id_: Optional[str] = None, block: Optional[Block] = None,
-            blocks: Optional[BlockArray, List[Block]] = None
-    ) -> Optional[Element]:
-        """
-        Append block or blocks children
-
-        :param id_:         provide id of block or page if `self.obj` is empty
-
-        :param block:       Block to append OR
-        :param blocks:          List[Block] or BlockArray to append
-
-        :return:            self.obj -> BlockArray
-
-        `p1 = no.pages.get("PAGE ID")`
-        `p1.block_append(block=Block.create("SOMETHING NEW YO"))`
-
-        `no.blocks.block_append("BLOCK OR PAGE ID", blocks=blocks)`
-        """
-        if self.name not in ["blocks", "pages"]:
-            logger.warning("Method supports `blocks` or `pages` only")
-            return None
-        if isinstance(id_, str) and "-" in id_:
-            id_ = id_.replace("-", "")
-        if self.obj:
-            id_ = self.obj.id
-        if isinstance(blocks, list):
-            blocks = BlockArray(blocks, create=True)
-        if isinstance(block, Block):
-            blocks = BlockArray([block], create=True)
-        data = {"children": blocks.get()}
-
-        new_blocks = self.api.session.method(
-            method="patch", path="blocks", id_=id_, after_path="children", data=data
-        )
-        return Element(api=self.api, name="blocks", obj=BlockArray(new_blocks["results"]))
-
-    def get_myself(self) -> Element:
-        """
-        Retrieves the bot User associated with the API token provided in the authorization header.
-
-        :return: Element with User obj
-
-        `me = no.users.get_myself()`
-        """
-        new_object = Element(self.api, name="users")
-        new_object.get("me")
-        return new_object
-
-    def from_linkto(self, linkto: LinkTo, limit: int = 0) -> Optional[Element]:
-        if not linkto:
-            logger.error("LinkTo must be provided!")
-            return None
-        if not linkto.uri:
-            logger.error("LinkTo.uri must be provided!")
-            return None
-        new_element = Element(self.api, name=linkto.uri)
-        return new_element.get(linkto.id, getattr(linkto, "after_path", None), limit)
-
-    def from_object(self, model: Union[Database, Page, Block]):
-        return Element(self.api, model.path, model)
-
-    def __repr__(self):
-        if not self.obj:
-            return f"Notion/{self.name}/"
-        return f"Notion/{self.name}/{self.obj!r}"
-
-    def __str__(self):
-        return self.__repr__()
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import logging
+from typing import Optional, Union, Dict, List
+
+import pytion.envs as envs
+from pytion.query import Request, Filter, Sort
+from pytion.models import Database, Page, Block, BlockArray, PropertyValue, PageArray, LinkTo, RichTextArray, Property
+from pytion.models import ElementArray, User
+
+
+Models = Union[Database, Page, Block, BlockArray, PropertyValue, PageArray, ElementArray]
+logger = logging.getLogger(__name__)
+
+
+class Notion(object):
+    def __init__(self, token: Optional[str] = None, version: Optional[str] = None):
+        """
+        Creates main API object.
+
+        :param token:   provide your integration API token. If None - find the file `token`
+        :param version: provide non hardcoded API version
+        """
+        self.version = version if version else envs.NOTION_VERSION
+        self.session = Request(api=self, token=token)
+        logger.debug(f"API object created. Version {envs.NOTION_VERSION}")
+
+    def search(
+            self, query: Optional[str] = None, limit: int = 0,
+            object_type: Optional[str] = None, sort_last_edited_time: Optional[str] = None
+    ) -> Optional[Element]:
+        """
+        Searches all original pages, databases, and child pages/databases that are shared with the integration.
+        It will not return linked databases, since these duplicate their source databases. (c)
+
+
+        :param query:                   search by page title
+        :param limit:                   0 < int < 100 - max number of items to be returned (0 = return all)
+        :param object_type:             filter by type: 'page' or 'database'
+        :param sort_last_edited_time:   sorting 'ascending' or 'descending'
+        :return:
+
+        `r = no.search("pytion", 10, sort_last_edited_time="ascending")`
+        `print(r.obj)`
+        """
+        data = {"query": query} if query else None
+        filter_ = Filter(raw={"property": "object", "value": object_type}) if object_type else None
+        if sort_last_edited_time:
+            sort_last_edited_time = Sort(property_name="last_edited_time", direction=sort_last_edited_time)
+        result = self.session.method(
+            "post", "search", sort=sort_last_edited_time, filter_=filter_, limit=limit, data=data
+        )
+        if "results" in result and isinstance(result["results"], list):
+            data = ElementArray(result["results"])
+            for item in data:
+                if isinstance(item, Page):
+                    self.pages.get_page_properties(title_only=True, obj=item)
+            return Element(api=self, name="search", obj=data)
+        else:
+            logger.warning("Results list is not found")
+            return None
+
+    def __len__(self):
+        return 1
+
+    def __repr__(self):
+        return "NotionAPI"
+
+    def __str__(self):
+        return self.__repr__()
+
+    def __getattr__(self, name):
+        if name in dir(self):
+            return self.name
+        return Element(self, name)
+
+
+class Element(object):
+    class_map = {"page": Page, "database": Database, "block": Block, "user": User}
+
+    def __init__(self, api: Notion, name: str, obj: Optional[Models] = None):
+        self.api = api
+        self.name = name
+        self.obj = obj
+        logger.debug(f"Element {self!r} created")
+
+    def get(self, id_: str, _after_path: str = None, limit: int = 0) -> Element:
+        """
+        Get Element by ID.
+        .exceptions.ObjectNotFound exception if not found
+
+        :return:    `Element.obj` may be `Page`, `Database`, `Block`
+
+        result = no.databases.get("1234123412341")
+        result = no.pages.get("123412341234")
+        result = no.blocks.get("123412341234")
+        result = no.users.get("123412341234")
+        print(result.obj)
+        """
+        if "-" in id_:
+            id_ = id_.replace("-", "")
+        if not _after_path:
+            raw_obj = self.api.session.method(method="get", path=self.name, id_=id_, limit=limit)
+        else:
+            raw_obj = self.api.session.method(
+                method="get", path=self.name, id_=id_, after_path=_after_path, limit=limit
+            )
+        if raw_obj["object"] == "list":
+            if self.name == "pages":
+                self.obj = PageArray(raw_obj["results"])
+            elif self.name == "blocks":
+                self.obj = BlockArray(raw_obj["results"])
+            else:
+                self.obj = ElementArray(raw_obj["results"])
+        else:
+            self.obj = self.class_map[raw_obj["object"]](**raw_obj)
+        return self
+
+    def get_parent(self, id_: Optional[str] = None) -> Optional[Element]:
+        """
+        Get parent object of current object if possible.
+
+        :param id_:
+        :return:    Element (parent object) or None. `.obj` may be `Page`, `Database`, `Block`
+
+        `result = no.blocks.get_parent("123412341234")`
+        `print(result)`
+        Notion/pages/Page(Page Title here)
+        `result = result.get_parent()`
+        `print(result)`
+        Notion/databases/Database(Some database name)
+        """
+        if not self.obj:
+            self.get(id_)
+        if getattr(self.obj, "parent", None):
+            return self.from_linkto(self.obj.parent)
+        logger.warning(f"Parent object can not be found")
+        return None
+
+    def get_block_children(
+            self, id_: Optional[str] = None, block: Optional[Block] = None, limit: int = 0
+    ) -> Optional[Element]:
+        """
+        Get children Block objects of current Block object (tabulated texts) if exist (else None)
+
+        :param id_:
+        :param block: you can provide a Block object instead to get his children
+        :param limit:   0 < int < 100 - max number of items to be returned (0 = return all)
+        :return:        `Element.obj` will be BlockArray object even nothing is found
+
+        `print(no.pages.get_block_children("PAGE ID"))`
+        None
+
+        `print(no.blocks.get_block_children("PAGE ID"))`
+        Notion/blocks/BlockArray(Heading 2 level Paragraph some)
+
+        `print(no.blocks.get_block_children("PAGE ID").obj)`
+        Heading 2 level
+        Paragraph
+        some text
+
+        BlockArray or Database object expected.
+        """
+        if self.name not in ("blocks", "pages"):
+            logger.warning("Only `blocks` or `pages` can have children")
+            return None
+        if isinstance(id_, str) and "-" in id_:
+            id_ = id_.replace("-", "")
+        obj = block if block else self.obj
+        if obj:
+            return self.from_linkto(obj.children, limit=limit)
+        child = self.api.session.method(
+            method="get", path="blocks", id_=id_, after_path="children", limit=limit
+        )
+        # children object returns list of Blocks
+        if child["object"] != "list":
+            logger.warning(f"List of Blocks expected. Received\n{child}")
+            return None
+        return Element(api=self.api, name="blocks", obj=BlockArray(child["results"]))
+
+    def get_block_children_recursive(
+        self, id_: Optional[str] = None, max_depth: int = 10, block: Optional[Block] = None,
+        _cur_depth: int = 0, limit: int = 0, force: bool = False
+    ) -> Optional[Element]:
+        """
+        Get children Block objects of current Block object (tabulated texts) if exist (else None) recursive
+
+        :param id_:
+        :param block:       you can provide a Block object instead to get his children
+        :param max_depth:   how deep use the recursion (block inside block inside block etc.)
+        :param limit:       0 < int < 100 - max number of items to be returned (0 = return all)
+        :param force:       get blocks in subpages too
+        :return:            `Element.obj` will be BlockArray object even nothing is found
+
+        `print(no.blocks.get_block_children_recursive("PAGE ID").obj)`
+        Heading 2 level
+        Paragraph
+            block inside block
+        some text
+        """
+        if self.name not in ("blocks", "pages"):
+            logger.warning("Only `blocks` or `pages` can have children")
+            return None
+        if isinstance(id_, str) and "-" in id_:
+            id_ = id_.replace("-", "")
+        obj = block if block else self.obj
+        if obj:
+            id_ = obj.id
+            if isinstance(obj, Block) and obj.type == "child_database":
+                return self.from_linkto(obj.children)
+        child = self.api.session.method(
+            method="get", path="blocks", id_=id_, after_path="children", limit=limit
+        )
+        ba = BlockArray([])
+        for b in child["results"]:
+            block_obj = Block(level=_cur_depth, **b)
+            ba.append(block_obj)
+            # Do not get subpages if not force
+            if block_obj.type == "child_page" and not force:
+                continue
+            if block_obj.has_children and _cur_depth < max_depth:
+                sub_element = Element(api=self.api, name="blocks").get_block_children_recursive(
+                    id_=block_obj.id, max_depth=max_depth, _cur_depth=_cur_depth + 1, limit=limit, force=force
+                )
+                ba.extend(sub_element.obj)
+
+        return Element(api=self.api, name="blocks", obj=ba)
+
+    def get_page_property(self, property_id: str, id_: Optional[str] = None, limit: int = 0) -> Optional[Element]:
+        """
+        DEPRECATED
+        Retrieve a page property item.
+
+        :param property_id: ID of property in current database
+        :param id_:         ID of page in that database (if not `self.obj`)
+        :param limit:       0 < int < 100 - max number of items to be returned (0 = return all)
+        :return:            `Element.obj` will be PropertyValue object
+
+        `db = no.databases.get("1232412341234")`
+        `property_id = db.obj.properties["Last edited time"].id`
+        `result = no.pages.get_page_property(property_id, 'PAGE ID 152f123a12344')`
+        `print(result.obj)`
+        2021-11-04 16:47:00+00:00
+        """
+        if self.name != "pages":
+            logger.warning("Only `pages` can have properties")
+            return None
+        if isinstance(id_, str) and "-" in id_:
+            id_ = id_.replace("-", "")
+        if self.obj and not id_:
+            id_ = self.obj.id
+        property_obj = self.api.session.method(
+            method="get", path=self.name, id_=id_, after_path="properties/"+property_id, limit=limit
+        )
+        return Element(api=self.api, name=f"pages/{id_}/properties", obj=PropertyValue(property_obj, property_id))
+
+    def get_page_properties(self, title_only: bool = False, obj: Optional[Page] = None) -> None:
+        """
+        Page properties must be retrieved using the page properties endpoint. (c)
+        after retrieving a Page object you can retrieve its properties
+
+        obj or self.obj must be a Page
+        :return:
+        """
+        if not obj:
+            obj = self.obj
+        if obj and isinstance(obj, Page):
+            for prop in obj.properties:
+                # Skip already retrieved properties
+                if isinstance(obj.properties[prop], PropertyValue):
+                    continue
+                prop_id = obj.properties[prop].id
+                if title_only and prop_id != "title":
+                    continue
+                result = self.get_page_property(prop_id, id_=obj.id)
+                obj.properties[prop] = result.obj
+                if prop_id == "title":
+                    obj.title = result.obj.value if result.obj.value else ""
+            return
+        logger.warning("You must provide a Page to retrieve properties")
+
+    def db_query(
+            self,
+            id_: Optional[str] = None,
+            limit: int = 0,
+            filter_: Optional[Filter] = None,
+            sorts: Optional[Sort] = None,
+            **kwargs,
+    ) -> Optional[Element]:
+        if self.name != "databases":
+            logger.warning("Only `databases` can be queried")
+            return None
+        if isinstance(id_, str) and "-" in id_:
+            id_ = id_.replace("-", "")
+        if self.obj:
+            id_ = self.obj.id
+        r = self.api.session.method(
+            method="post", path=self.name, id_=id_, after_path="query",
+            data={}, limit=limit, filter_=filter_, sorts=sorts
+        )
+        if r["object"] != "list":
+            return None
+        return Element(api=self.api, name="pages", obj=PageArray(r["results"]))
+
+    def db_filter(self, title: str = None, **kwargs) -> Optional[Element]:
+        """
+        :param title: filter by title contains + opt. attrs: condition, sort etc.
+        OR
+        :param property_name: mandatory - full name or ID of property to filter by
+        :param value: the value of this property to filter by (may be bool or datetime etc.)
+        :param property_type: mandatory field - `text`, `number`, `checkbox`, `date`, `select` etc.
+        :param condition: optional field - it depends on the type: `starts_with`, `contains`, `equals` etc.
+        :param raw: correctly formatted dict to pass direct to API (instead of all other params)
+        :param property_obj: Property or PropertyValue obj. instead of `property_name` and `property_type`,
+                             PropertyValue can put value in request, if `value` is not provided
+
+        :param ascending: property name to be sorted by
+        :param descending: property name to be sorted by
+
+        :param limit: 0 < int < 100 - max number of items to be returned (0 = return all)
+        :return:              self.obj -> PageArray
+
+        examples
+        `.db_filter("My Page Title")`
+        `.db_filter("", ascending="Tags")`
+        `.db_filter(property_name="Done", property_type="checkbox")`
+        `.db_filter(property_name="Done", property_type="checkbox", value=False, descending="title")`
+        `.db_filter(property_name="tags", property_type="multi_select", condition="is_not_empty")`
+        `.db_filter(raw=YOUR_BIG_DICT_FROM_NOTION_DOCS, limit=2)`
+
+        Filters combinations are not supported. (in `raw` param only)
+        """
+        if self.name == "databases" and self.obj:
+            sort = None
+            if kwargs.get("ascending"):
+                sort = Sort(property_name=kwargs["ascending"], direction="ascending")
+            elif kwargs.get("descending"):
+                sort = Sort(property_name=kwargs["descending"], direction="descending")
+            if isinstance(title, str):
+                filter_obj = Filter(property_name="title", value=title, property_type="title", **kwargs)
+            else:
+                filter_obj = Filter(**kwargs)
+            return self.db_query(filter_=filter_obj, sorts=sort, **kwargs)
+        logger.warning("Database must be provided. use .get() before")
+        return None
+
+    def db_create(
+            self,
+            database_obj: Optional[Database] = None,
+            parent: Optional[LinkTo] = None,
+            properties: Optional[Dict[str, Property]] = None,
+            title: Optional[Union[str, RichTextArray]] = None,
+            description: Optional[Union[str, RichTextArray]] = None,
+    ) -> Optional[Element]:
+        """
+        :param database_obj:  you can provide `Database` object or -
+                              provide the params for creating it:
+        :param parent:        parent object in LinkTo format. workspace can not be a parent
+        :param properties:    dict of properties. Property with `title` type is mandatory!
+        :param title:         your name of the Database
+        :param description:   optional description for new Database
+        :return:              self.obj -> Database
+
+        `parent = LinkTo.create(database_id="24512345125123421")`
+        `p1 = Property.create(name="renamed")`
+        `p2 = Property.create(type_="multi_select", name="multiselected")`
+        `props = {"Property1_name": p1, "Property2_name": p2}` OR
+        ```props = {
+            "Name": Property.create("title")
+            "Digit": Property.create("number"),
+            "Status": Property.create("select")
+        }```
+        `db = db.db_create(parent=parent, properties=props, title=RichTextArray.create("NEW DB"))`
+        """
+        if self.name != "databases":
+            logger.warning("Method supports `databases` only")
+            return None
+        if database_obj:
+            db = database_obj
+        else:
+            if isinstance(title, str):
+                title = RichTextArray.create(title)
+            db = Database.create(parent=parent, properties=properties, title=title, description=description)
+        created_db = self.api.session.method(method="post", path=self.name, data=db.get())
+        self.obj = Database(**created_db)
+        return self
+
+    def db_update(
+            self, id_: Optional[str] = None, title: Optional[Union[str, RichTextArray]] = None,
+            properties: Optional[Dict[str, Property]] = None
+    ) -> Optional[Element]:
+        """
+        :param id_:         provide id of database if `self.obj` is empty
+        :param title:       provide RichTextArray or text to rename database
+        :param properties:  provide dict of Property to update them
+        :return:            self.obj -> Database
+
+
+        `rename_prop = Property.create(name="renamed")`
+        `rename_retype_prop = Property.create(type_="multi_select", name="multiselected")`
+        `retype_prop = Property.create("checkbox")`
+        `props = {"Property1_name": rename_retype_prop, "Property2_ID": retype_prop}`
+        `db = db.db_update(properties=props, title=RichTextArray.create("NEW DB"))`
+        """
+        if self.name != "databases":
+            logger.warning("Method supports `databases` only")
+            return None
+        if isinstance(id_, str) and "-" in id_:
+            id_ = id_.replace("-", "")
+        if self.obj:
+            id_ = self.obj.id
+        patch = {}
+        if title:
+            if isinstance(title, str):
+                title = RichTextArray.create(title)
+            patch["title"] = title.get()
+        if properties:
+            patch["properties"] = {name: value.get() for name, value in properties.items()}
+        updated_db = self.api.session.method(method="patch", path=self.name, id_=id_, data=patch)
+        self.obj = Database(**updated_db)
+        return self
+
+    def page_create(
+            self,
+            page_obj: Optional[Page] = None,
+            parent: Optional[LinkTo] = None,
+            properties: Optional[Dict[str, PropertyValue]] = None,
+            title: Optional[Union[str, RichTextArray]] = None,
+            children: Union[BlockArray, List[Block], None] = None,
+    ) -> Optional[Element]:
+        """
+        :param page_obj:      you can provide `Page` object or -
+                              provide the params for creating it:
+        :param parent:        LinkTo object with ID of parent element. workspace can not be a parent
+        :param properties:    Dict of properties with values
+        :param title:         New title
+        :param children:      Content of new page in [Block] or BlockArray format
+        :return:              self.obj -> Page
+
+        `parent = LinkTo.create(database_id="24512345125123421")`
+        `p2 = PropertyValue.create("date", datetime.now())`
+        `r = no.pages.page_create(parent=parent, properties={"Count": p1, "Date": p2}, title="Extra PAGE")`
+
+        `props["Status"] = PropertyValue.create("select", "new select option")`
+        `props["Tags"] = PropertyValue.create("multi_select", ["new-option1", "new option2"])`
+        `no.pages.create(parent=parent, properties=props)`
+
+        `parent2 = LinkTo.create(page_id="123412341234")`
+        `no.pages.page_create(parent=parent2, title="New page 121")`
+        """
+        if self.name != "pages":
+            logger.warning("Method supports `pages` only")
+            return None
+        if page_obj:
+            page = page_obj
+        else:
+            if children and not isinstance(children, BlockArray):
+                children = BlockArray(children, create=True)
+            page = Page.create(parent=parent, properties=properties, title=title, children=children)
+        created_page = self.api.session.method(method="post", path=self.name, data=page.get())
+        self.obj = Page(**created_page)
+        return self
+
+    def page_update(
+            self, id_: Optional[str] = None, properties: Optional[Dict[str, PropertyValue]] = None,
+            title: Optional[Union[str, RichTextArray]] = None, archived: bool = False
+    ) -> Optional[Element]:
+        """
+        :param id_:         ID of page
+        :param properties:  dict of existing properties
+        :param title:
+        :param archived:    set to `True` for delete the page
+        :return:            self.obj -> Page
+        """
+        if self.name != "pages":
+            logger.warning("Method supports `pages` only")
+            return None
+        if isinstance(id_, str) and "-" in id_:
+            id_ = id_.replace("-", "")
+        if self.obj:
+            id_ = self.obj.id
+        patch = {}
+        if properties:
+            patch["properties"] = {name: p.get() for name, p in properties.items()}
+        if title:
+            patch.setdefault("properties", {})
+            patch["properties"]["title"] = PropertyValue.create("title", title).get()
+        # if archived:
+        patch["archived"] = archived
+        updated_page = self.api.session.method(method="patch", path=self.name, id_=id_, data=patch)
+        self.obj = Page(**updated_page)
+        return self
+
+    def block_update(
+            self, id_: Optional[str] = None, block_obj: Optional[Block] = None,
+            new_text: Optional[str] = None, archived: bool = False
+    ) -> Optional[Element]:
+        """
+        Updates text of Block.
+        `text`, `checked` (`to_do` type), `language` (`code` type) fields support only!
+        You can modify any attrs of existing block and provide it (Block object) to this func.
+        Changing the Block type is not supported.
+
+        :param id_:         ID of block to change text OR
+        :param block_obj:   modified Block (replace mode only)
+
+        :param new_text:    new text (replace mode only)
+        :param archived:    flag to delete that Block
+        :return:            self.obj -> Block
+
+        `blocks = no.blocks.get_block_children("PAGE ID")`
+        `for b in blocks.obj:`
+            `no.blocks.block_update(block_obj=b, new_text="OH YEEEAHH")`
+        `for b in blocks.obj:`
+            `b.text = "ALL IS DONE"`
+            `no.blocks.block_update(block_obj=b)`
+        """
+        if self.name != "blocks":
+            logger.warning("Method supports `blocks` only")
+            return None
+        if isinstance(id_, str) and "-" in id_:
+            id_ = id_.replace("-", "")
+        if self.obj:
+            id_ = self.obj.id
+        else:
+            self.get(id_)
+        if block_obj:
+            self.obj = block_obj
+        if not self.obj.get():
+            return None
+        if new_text:
+            self.obj.text = new_text
+        patch = {"archived": archived}
+        patch.update(self.obj.get())
+        updated_block = self.api.session.method(method="patch", path=self.name, id_=id_, data=patch)
+        self.obj = Block(**updated_block)
+        return self
+
+    def block_append(
+            self, id_: Optional[str] = None, block: Optional[Block] = None,
+            blocks: Union[BlockArray, List[Block], None] = None
+    ) -> Optional[Element]:
+        """
+        Append block or blocks children
+
+        :param id_:         provide id of block or page if `self.obj` is empty
+
+        :param block:       Block to append OR
+        :param blocks:          List[Block] or BlockArray to append
+
+        :return:            self.obj -> BlockArray
+
+        `p1 = no.pages.get("PAGE ID")`
+        `p1.block_append(block=Block.create("SOMETHING NEW YO"))`
+
+        `no.blocks.block_append("BLOCK OR PAGE ID", blocks=blocks)`
+        """
+        if self.name not in ["blocks", "pages"]:
+            logger.warning("Method supports `blocks` or `pages` only")
+            return None
+        if isinstance(id_, str) and "-" in id_:
+            id_ = id_.replace("-", "")
+        if self.obj:
+            id_ = self.obj.id
+        if isinstance(blocks, list):
+            blocks = BlockArray(blocks, create=True)
+        if isinstance(block, Block):
+            blocks = BlockArray([block], create=True)
+        data = {"children": blocks.get()}
+
+        new_blocks = self.api.session.method(
+            method="patch", path="blocks", id_=id_, after_path="children", data=data
+        )
+        return Element(api=self.api, name="blocks", obj=BlockArray(new_blocks["results"]))
+
+    def get_myself(self) -> Element:
+        """
+        Retrieves the bot User associated with the API token provided in the authorization header.
+
+        :return: Element with User obj
+
+        `me = no.users.get_myself()`
+        """
+        new_object = Element(self.api, name="users")
+        new_object.get("me")
+        return new_object
+
+    def from_linkto(self, linkto: LinkTo, limit: int = 0) -> Optional[Element]:
+        if not linkto:
+            logger.error("LinkTo must be provided!")
+            return None
+        if not linkto.uri:
+            logger.error("LinkTo.uri must be provided!")
+            return None
+        new_element = Element(self.api, name=linkto.uri)
+        return new_element.get(linkto.id, getattr(linkto, "after_path", None), limit)
+
+    def from_object(self, model: Union[Database, Page, Block]):
+        return Element(self.api, model.path, model)
+
+    def __repr__(self):
+        if not self.obj:
+            return f"Notion/{self.name}/"
+        return f"Notion/{self.name}/{self.obj!r}"
+
+    def __str__(self):
+        return self.__repr__()
```

### Comparing `pytion-1.3.3/pytion/exceptions.py` & `pytion-1.3.4/pytion/exceptions.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-# -*- coding: utf-8 -*-
-
-import logging
-import json
-from typing import Dict
-
-from requests import Response
-
-
-logger = logging.getLogger(__name__)
-
-
-class ClientError(Exception):
-    def __init__(self, message: Response):
-        req = message
-        message = f"Failed with code {req.status_code}. Raw: {req.content}"
-        super(ClientError, self).__init__(message)
-        self.req = req
-        self.request_body = req.request.body
-        self.base = req.url
-        self.error = message
-
-
-class ServerError(Exception):
-    def __init__(self, message: Response):
-        req = message
-        message = f"Failed with code {req.status_code}. Raw: {req.content}"
-        super(ServerError, self).__init__(message)
-        self.req = req
-        self.request_body = req.request.body
-        self.base = req.url
-        self.error = message
-
-
-class InvalidJSON(ClientError):
-    def __init__(self, req: Response):
-        message = f"Body could not be decoded as JSON: {req.request.body}"
-        Exception.__init__(self, message)
-
-
-class InvalidRequestURL(ClientError):
-    def __init__(self, req: Response):
-        message = f"The request URL is not valid: {req.url}"
-        Exception.__init__(self, message)
-
-
-class InvalidRequest(ClientError):
-    def __init__(self, req: Response):
-        message = f"This request is not supported: {req.url} {req.request.method}"
-        Exception.__init__(self, message)
-
-
-class ValidationError(ClientError):
-    def __init__(self, content: Dict):
-        message = content.get("message")
-        message = f"The request body does not match the schema: {message}"
-        Exception.__init__(self, message)
-
-
-class MissingVersion(ClientError):
-    def __init__(self, *args):
-        message = "The request is missing the required Notion-Version header."
-        Exception.__init__(self, message)
-
-
-class Unauthorized(ClientError):
-    def __init__(self, *args):
-        message = "The bearer token is not valid."
-        Exception.__init__(self, message)
-
-
-class RestrictedResource(ClientError):
-    def __init__(self, *args):
-        message = "Given the bearer token used, the client doesn't have permission to perform this operation."
-        Exception.__init__(self, message)
-
-
-class ObjectNotFound(ClientError):
-    def __init__(self, req: Response):
-        message = f"{req.url}" \
-                  "The resource does not exist or the resource has not been shared with owner of the bearer token."
-        Exception.__init__(self, message)
-
-
-class ConflictError(ClientError):
-    def __init__(self, *args):
-        message = "The transaction could not be completed, potentially due to a data collision. Make sure the " \
-                  "parameters are up to date and try again."
-        Exception.__init__(self, message)
-
-
-class RateLimited(ClientError):
-    def __init__(self, *args):
-        message = "This request exceeds the number of requests allowed. Slow down and try again."
-        Exception.__init__(self, message)
-
-
-class InternalServerError(ServerError):
-    def __init__(self, req: Response):
-        self.req = req
-        self.request_body = req.request.body
-        self.base = req.url
-        self.error = req.content
-        message = f"An unexpected error occurred. Reach out to Notion support. {req.status_code}: " \
-                  f"{req.request.method} {self.base} {self.request_body} -> {self.error}"
-        Exception.__init__(self, message)
-
-
-class ServiceUnavailable(ServerError):
-    def __init__(self, *args):
-        message = "Notion is unavailable. Try again later."
-        Exception.__init__(self, message)
-
-
-class DatabaseConnectionUnavailable(ServerError):
-    def __init__(self, *args):
-        message = "Notion's database is unavailable or in an unqueryable state. Try again later."
-        Exception.__init__(self, message)
-
-
-class ContentError(Exception):
-    """Content Exception
-    If the API URL does not point to a valid Notion API, the server may
-    return a valid response code, but the content is not json. This
-    exception is raised in those cases.
-    """
-
-    def __init__(self, message):
-        req = message
-
-        message = (
-            "The server returned invalid (non-json) data. Maybe not a Notion server?"
-        )
-
-        super(ContentError, self).__init__(message)
-        self.req = req
-        self.request_body = req.request.body
-        self.base = req.url
-        self.error = message
-
-
-def find_response_error(req: Response) -> Dict:
-    try:
-        content = req.json()
-    except json.JSONDecodeError:
-        logger.error(f"Result is not OK. JSON decoding fail\n{req.content}")
-        raise ContentError(req)
-    if req.ok:
-        return content
-    logger.error(f"Result is not OK. {req.status_code}\n{req.reason}")
-    status_code = int(req.status_code)
-    error_code = content.get("code")
-    if error_code:
-        if error_code == "invalid_json":
-            raise InvalidJSON(req)
-        elif error_code == "invalid_request_url":
-            raise InvalidRequestURL(req)
-        elif error_code == "invalid_request":
-            raise InvalidRequest(req)
-        elif error_code == "validation_error":
-            raise ValidationError(content)
-        elif error_code == "missing_version":
-            raise MissingVersion()
-        elif error_code == "unauthorized":
-            raise Unauthorized()
-        elif error_code == "restricted_resource":
-            raise RestrictedResource()
-        elif error_code == "object_not_found":
-            raise ObjectNotFound(req)
-        elif error_code == "conflict_error":
-            raise ConflictError()
-        elif error_code == "rate_limited":
-            raise RateLimited()
-        elif error_code == "internal_server_error":
-            raise InternalServerError(req)
-        elif error_code == "service_unavailable":
-            raise ServiceUnavailable()
-        elif error_code == "database_connection_unavailable":
-            raise DatabaseConnectionUnavailable()
-    if 400 <= status_code < 500:
-        raise ClientError(req)
-    elif 500 <= status_code < 600:
-        raise ServerError(req)
-    raise Exception(f"An unexpected error occurred. {req.status_code}: {req.content}")
+# -*- coding: utf-8 -*-
+
+import logging
+import json
+from typing import Dict
+
+from requests import Response
+
+
+logger = logging.getLogger(__name__)
+
+
+class ClientError(Exception):
+    def __init__(self, message: Response):
+        req = message
+        message = f"Failed with code {req.status_code}. Raw: {req.content}"
+        super(ClientError, self).__init__(message)
+        self.req = req
+        self.request_body = req.request.body
+        self.base = req.url
+        self.error = message
+
+
+class ServerError(Exception):
+    def __init__(self, message: Response):
+        req = message
+        message = f"Failed with code {req.status_code}. Raw: {req.content}"
+        super(ServerError, self).__init__(message)
+        self.req = req
+        self.request_body = req.request.body
+        self.base = req.url
+        self.error = message
+
+
+class InvalidJSON(ClientError):
+    def __init__(self, req: Response):
+        message = f"Body could not be decoded as JSON: {req.request.body}"
+        Exception.__init__(self, message)
+
+
+class InvalidRequestURL(ClientError):
+    def __init__(self, req: Response):
+        message = f"The request URL is not valid: {req.url}"
+        Exception.__init__(self, message)
+
+
+class InvalidRequest(ClientError):
+    def __init__(self, req: Response):
+        message = f"This request is not supported: {req.url} {req.request.method}"
+        Exception.__init__(self, message)
+
+
+class ValidationError(ClientError):
+    def __init__(self, content: Dict):
+        message = content.get("message")
+        message = f"The request body does not match the schema: {message}"
+        Exception.__init__(self, message)
+
+
+class MissingVersion(ClientError):
+    def __init__(self, *args):
+        message = "The request is missing the required Notion-Version header."
+        Exception.__init__(self, message)
+
+
+class Unauthorized(ClientError):
+    def __init__(self, *args):
+        message = "The bearer token is not valid."
+        Exception.__init__(self, message)
+
+
+class RestrictedResource(ClientError):
+    def __init__(self, *args):
+        message = "Given the bearer token used, the client doesn't have permission to perform this operation."
+        Exception.__init__(self, message)
+
+
+class ObjectNotFound(ClientError):
+    def __init__(self, req: Response):
+        message = f"{req.url}" \
+                  "The resource does not exist or the resource has not been shared with owner of the bearer token."
+        Exception.__init__(self, message)
+
+
+class ConflictError(ClientError):
+    def __init__(self, *args):
+        message = "The transaction could not be completed, potentially due to a data collision. Make sure the " \
+                  "parameters are up to date and try again."
+        Exception.__init__(self, message)
+
+
+class RateLimited(ClientError):
+    def __init__(self, *args):
+        message = "This request exceeds the number of requests allowed. Slow down and try again."
+        Exception.__init__(self, message)
+
+
+class InternalServerError(ServerError):
+    def __init__(self, req: Response):
+        self.req = req
+        self.request_body = req.request.body
+        self.base = req.url
+        self.error = req.content
+        message = f"An unexpected error occurred. Reach out to Notion support. {req.status_code}: " \
+                  f"{req.request.method} {self.base} {self.request_body} -> {self.error}"
+        Exception.__init__(self, message)
+
+
+class ServiceUnavailable(ServerError):
+    def __init__(self, *args):
+        message = "Notion is unavailable. Try again later."
+        Exception.__init__(self, message)
+
+
+class DatabaseConnectionUnavailable(ServerError):
+    def __init__(self, *args):
+        message = "Notion's database is unavailable or in an unqueryable state. Try again later."
+        Exception.__init__(self, message)
+
+
+class ContentError(Exception):
+    """Content Exception
+    If the API URL does not point to a valid Notion API, the server may
+    return a valid response code, but the content is not json. This
+    exception is raised in those cases.
+    """
+
+    def __init__(self, message):
+        req = message
+
+        message = (
+            "The server returned invalid (non-json) data. Maybe not a Notion server?"
+        )
+
+        super(ContentError, self).__init__(message)
+        self.req = req
+        self.request_body = req.request.body
+        self.base = req.url
+        self.error = message
+
+
+def find_response_error(req: Response) -> Dict:
+    try:
+        content = req.json()
+    except json.JSONDecodeError:
+        logger.error(f"Result is not OK. JSON decoding fail\n{req.content}")
+        raise ContentError(req)
+    if req.ok:
+        return content
+    logger.error(f"Result is not OK. {req.status_code}\n{req.reason}")
+    status_code = int(req.status_code)
+    error_code = content.get("code")
+    if error_code:
+        if error_code == "invalid_json":
+            raise InvalidJSON(req)
+        elif error_code == "invalid_request_url":
+            raise InvalidRequestURL(req)
+        elif error_code == "invalid_request":
+            raise InvalidRequest(req)
+        elif error_code == "validation_error":
+            raise ValidationError(content)
+        elif error_code == "missing_version":
+            raise MissingVersion()
+        elif error_code == "unauthorized":
+            raise Unauthorized()
+        elif error_code == "restricted_resource":
+            raise RestrictedResource()
+        elif error_code == "object_not_found":
+            raise ObjectNotFound(req)
+        elif error_code == "conflict_error":
+            raise ConflictError()
+        elif error_code == "rate_limited":
+            raise RateLimited()
+        elif error_code == "internal_server_error":
+            raise InternalServerError(req)
+        elif error_code == "service_unavailable":
+            raise ServiceUnavailable()
+        elif error_code == "database_connection_unavailable":
+            raise DatabaseConnectionUnavailable()
+    if 400 <= status_code < 500:
+        raise ClientError(req)
+    elif 500 <= status_code < 600:
+        raise ServerError(req)
+    raise Exception(f"An unexpected error occurred. {req.status_code}: {req.content}")
```

### Comparing `pytion-1.3.3/pytion/models.py` & `pytion-1.3.4/pytion/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1105 +1,1133 @@
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-from datetime import datetime
-from typing import Optional, Dict, Union, List, Any
-from collections.abc import MutableSequence
-
-from pytion.envs import NOTION_URL
-
-
-# I wanna use pydantic, but API provide variable names of property
-
-class RichText(object):
-    def __init__(self, **kwargs) -> None:
-        self.plain_text: str = kwargs.get("plain_text")
-        self.href: Optional[str] = kwargs.get("href")
-        self.annotations: Dict[str, Union[bool, str]] = kwargs.get("annotations")
-        # if not self.annotations:
-        #     self._create_default_annotations()
-        self.type: str = kwargs.get("type")
-        self.simple = ""
-        if self.type == "mention":
-            subtype = kwargs[self.type].get("type")
-            if subtype == "user":
-                self.data = User(**kwargs[self.type].get(subtype))
-                self.plain_text = str(self.data)
-                self.simple = LinkTo(from_object=self.data).link
-            elif subtype == "page":
-                sub_id = kwargs[self.type][subtype].get("id") if kwargs[self.type].get(subtype) else ""
-                self.data = LinkTo.create(page=sub_id)
-                if self.plain_text == "Untitled":
-                    self.plain_text = repr(self.data)
-                else:
-                    self.plain_text = "LinkTo(" + self.plain_text + ")"
-                self.simple = self.data.link
-            elif subtype == "database":
-                sub_id = kwargs[self.type][subtype].get("id") if kwargs[self.type].get(subtype) else ""
-                self.data = LinkTo.create(database_id=sub_id)
-                if self.plain_text == "Untitled":
-                    self.plain_text = repr(self.data)
-                else:
-                    self.plain_text = "LinkTo(" + self.plain_text + ")"
-                self.simple = self.data.link
-            elif subtype == "date":
-                self.data = {
-                    "start": Model.format_iso_time(kwargs[self.type][subtype].get("start")),
-                    "end": Model.format_iso_time(kwargs[self.type][subtype].get("end"))
-                }
-                self.simple = str(self.plain_text)
-            elif subtype == "link_preview":
-                self.simple = str(self.plain_text)
-                self.plain_text = f"<{self.plain_text}>"
-                self.data: Dict = kwargs[self.type]
-        else:
-            self.data: Dict = kwargs[self.type]
-            self.simple = str(self.plain_text)
-
-    def __str__(self):
-        return str(self.plain_text)
-
-    def __repr__(self):
-        return f"RichText({self.plain_text})"
-
-    def __bool__(self):
-        return bool(self.plain_text)
-
-    def _create_default_annotations(self):
-        self.annotations = {
-            "bold": False, "italic": False, "strikethrough": False,
-            "underline": False, "code": False, "color": "default"
-        }
-
-    # def __len__(self):
-    #     return len(self.plain_text)
-
-    def get(self) -> Dict[str, Any]:
-        """
-        Text type supported only
-        """
-        return {
-            "type": "text",
-            "text": {"content": self.plain_text, "link": None},
-            # "annotations": self.annotations,
-            # "plain_text": self.plain_text,
-        }
-
-
-class RichTextArray(MutableSequence):
-    def __init__(self, array: List[Dict]) -> None:
-        self.array = [RichText(**rt) for rt in array]
-
-    def __getitem__(self, item):
-        return self.array[item]
-
-    def __setitem__(self, key, value):
-        self.array[key] = value
-
-    def __delitem__(self, key):
-        del self.array[key]
-
-    def __len__(self):
-        return len(self.array)
-
-    def insert(self, index: int, value) -> None:
-        self.array.insert(index, value)
-
-    def __str__(self):
-        return "".join(str(rt) for rt in self)
-
-    def __repr__(self):
-        return f"RichTextArray({str(self)})"
-
-    def __bool__(self):
-        return any(map(bool, self.array))
-
-    def __add__(self, another: Union[RichTextArray, str]):
-        if isinstance(another, str):
-            another = RichTextArray.create(another)
-        self.array.extend(another)
-        return self
-
-    def get(self) -> List[Dict[str, Any]]:
-        return [item.get() for item in self]
-
-    @classmethod
-    def create(cls, text: str):
-        return cls([{"type": "text", "plain_text": text, "text": {}}])
-
-    @property
-    def simple(self) -> str:
-        return "".join(rt.simple for rt in self)
-
-
-class User(object):
-    """
-    The User object represents a user in a Notion workspace.
-    """
-    path = "users"
-
-    def __init__(self, **kwargs) -> None:
-        """
-        Create an User object by providing dict from API.
-
-        API attrs (from API docs):
-        Mandatory:
-        :param id: str
-        :param object: str
-
-        Optional:
-        :param type: str
-        :param name: str
-        :param avatar_url: str
-
-        Also Local attrs:
-        :param raw: dict from API
-        :param email: str if user is person
-        """
-        self.id = kwargs.get("id", "").replace("-", "")
-        self.object = kwargs.get("object")  # user
-        self.type = kwargs.get("type")
-        self.name = kwargs.get("name")
-        self.avatar_url = kwargs.get("avatar_url")
-        if self.type == "person" and kwargs.get(self.type):
-            self.email = kwargs[self.type].get("email")
-            self.workspace_name = None
-        elif self.type == "bot":
-            self.email = None
-            self.workspace_name = kwargs[self.type].get("workspace_name")
-        else:
-            self.email = None
-            self.workspace_name = None
-        self.raw = kwargs
-
-    def __str__(self):
-        if self.name and self.email:
-            name = f"{self.name}({self.email})"
-        else:
-            name = self.name
-        return name if name else self.id
-
-    def __repr__(self):
-        return f"User({self})"
-
-    def get(self) -> Dict[str, str]:
-        return {
-            "object": self.object,
-            "id": self.id
-        }
-
-    @classmethod
-    def create(cls, id: str):
-        return cls(object="user", id=id)
-
-
-class Model(object):
-    """
-    :param id:
-    :param object:
-    :param created_time:
-    :param last_edited_time:
-    :param created_by:
-    :param last_edited_by:
-    :param raw:
-    """
-
-    def __init__(self, **kwargs) -> None:
-        self.id = kwargs.get("id", "").replace("-", "")
-        self.object = kwargs.get("object")
-        self.created_time = self.format_iso_time(kwargs.get("created_time"))
-        self.last_edited_time = self.format_iso_time(kwargs.get("last_edited_time"))
-        self.created_by = User(**kwargs["created_by"]) if kwargs.get("created_by") else None
-        self.last_edited_by = User(**kwargs["last_edited_by"]) if kwargs.get("last_edited_by") else None
-        self.raw = kwargs
-
-    @classmethod
-    def format_iso_time(cls, time: str) -> Optional[datetime]:
-        if not time:
-            return None
-        return datetime.fromisoformat(time.replace("Z", "+00:00"))
-
-
-class Property(object):
-    def __init__(self, data: Dict[str, Any]):
-        self.to_delete = True if data.get("type", False) is None else False
-        self.id: str = data.get("id")
-        self.type: str = data.get("type", "")
-        self.name: str = data.get("name")
-        self.raw = data
-        self.subtype = None
-
-        if self.type == "relation":
-            if isinstance(data[self.type], dict):
-                self.subtype = data[self.type].get("type")
-                self.relation = LinkTo.create(database_id=data[self.type].get("database_id"))
-                if self.subtype == "single_property":
-                    pass
-                elif self.subtype == "dual_property":
-                    self.relation_property_id = data[self.type][self.subtype].get("synced_property_id")
-                    self.relation_property_name = data[self.type][self.subtype].get("synced_property_name")
-
-        if self.type == "status":
-            if isinstance(data[self.type], dict):
-                self.options = data[self.type].get("options", [])
-                self.groups = data[self.type].get("groups", [])
-
-    def __str__(self):
-        return self.name if self.name else self.type
-
-    def __repr__(self):
-        return f"Property({self})"
-
-    def get(self) -> Optional[Dict[str, Dict]]:
-        # property removing while patch
-        if self.to_delete:
-            return None
-        # property renaming while patch
-        data = {}
-        if self.name:
-            data["name"] = self.name
-        # property retyping while patch
-        if self.type:
-            # create relation type property with configuration
-            if self.type == "relation":
-                data[self.type] = {self.subtype: {}, "database_id": self.relation.id}
-            elif self.type == "status":
-                data[self.type] = {}
-                # not configurable
-                # if self.options:
-                #     data[self.type]["options"] = self.options
-                # if self.groups:
-                #     data[self.type]["groups"] = self.groups
-            else:
-                data[self.type] = {}
-        return data
-
-    @classmethod
-    def create(cls, type_: Optional[str] = "", **kwargs):
-        """
-        Property Schema Object (watch docs)
-        :param type_: see "create (DB)" column in "Supported Property types" matrix of README
-
-        + addons:
-        set type_ = `None` to delete this Property
-        set param `name` to rename this Property
-
-        + relation type:
-        set param `single_property` with `database_id` value OR
-        set param `dual_property` with `database_id` value
-        Property.create(type_="relation", dual_property="v111c132c12c1242341c41c")
-        """
-        if type_ == "relation":
-            subtype = next(kwarg for kwarg in kwargs if kwarg in ("single_property", "dual_property"))
-            kwargs["relation"] = {"type": subtype, subtype: {}, "database_id": kwargs[subtype]}
-        elif type_ == "status":
-            kwargs["status"] = {}
-        return cls({"type": type_, **kwargs})
-
-
-class PropertyValue(Property):
-    def __init__(self, data: Dict, name: str, **kwargs):
-        super().__init__(data)
-        # getting Paginated Properties (for retrieving property item)
-        # *Pagination
-        if data.get("object") and data["object"] == "list":
-            if data.get("results"):
-                self.type = data["results"][0].get("type")
-                data[self.type] = [sub_dict.get(sub_dict.get("type")) for sub_dict in data["results"]]
-
-        self.name = name
-        self.value = None
-
-        if self.type in ["title", "rich_text"]:
-            if isinstance(data[self.type], list):
-                self.value = RichTextArray(data[self.type])
-            elif isinstance(data[self.type], RichTextArray):
-                self.value = data[self.type]
-            else:
-                self.value = RichTextArray.create(data[self.type])
-
-        if self.type == "number":
-            self.value: Optional[int, float] = data["number"]
-
-        if self.type == "select":
-            if data["select"] and isinstance(data["select"], dict):
-                self.value: Optional[str] = data["select"].get("name")
-            elif data["select"] and isinstance(data["select"], str):
-                self.value = data["select"]
-            else:
-                self.value = None
-
-        if self.type == "multi_select":
-            self.value: List[str] = [(v.get("name") if isinstance(v, dict) else v) for v in data["multi_select"]]
-
-        if self.type == "checkbox":
-            self.value: bool = data["checkbox"]
-
-        if self.type == "date":
-            if isinstance(data["date"], datetime):
-                self.value = data["date"].isoformat()
-                self.start = data["date"]
-                self.end = None
-            elif data["date"]:
-                self.value: Optional[str] = data["date"].get("start")
-                self.start: Optional[datetime] = Model.format_iso_time(data["date"].get("start"))
-                self.end: Optional[datetime] = Model.format_iso_time(data["date"].get("end"))
-            else:
-                self.value = None
-                self.start = None
-                self.end = None
-
-        if "time" in self.type:
-            self.value: Optional[datetime] = Model.format_iso_time(data.get(self.type))
-
-        if self.type == "formula":
-            formula_type = data["formula"]["type"]
-            if formula_type == "date":
-                if data["formula"]["date"]:
-                    self.value: str = data["formula"]["date"].get("start")
-                    self.start: Optional[datetime] = Model.format_iso_time(data["formula"]["date"].get("start"))
-                    self.end: Optional[datetime] = Model.format_iso_time(data["formula"]["date"].get("end"))
-                else:
-                    self.value = None
-                    self.start = None
-                    self.end = None
-            else:
-                self.value: Union[str, int, float, bool] = data["formula"][formula_type]
-
-        if self.type == "created_by":
-            self.value = User(**data.get(self.type))
-
-        if self.type == "last_edited_by":
-            self.value = User(**data.get(self.type))
-
-        if self.type == "people":
-            self.value = [user if isinstance(user, User) else User(**user) for user in data[self.type]]
-
-        if self.type == "relation":
-            self.value: List[LinkTo] = [
-                LinkTo.create(page_id=item.get("id")) if not isinstance(item, LinkTo) else item
-                for item in data[self.type]
-            ]
-            self.has_more = data["has_more"] if "has_more" in data else False
-
-        if self.type == "status":
-            self.value = data[self.type].get("name") if isinstance(data[self.type], dict) else data[self.type]
-
-        if self.type == "rollup":
-            rollup_type = data["rollup"]["type"]
-            if rollup_type == "array":
-                if len(data["rollup"]["array"]) == 0:
-                    self.value = None
-                elif len(data["rollup"]["array"]) == 1:
-                    self.value = PropertyValue(data["rollup"]["array"][0], rollup_type)
-                else:
-                    self.value = [PropertyValue(element, rollup_type).value for element in data["rollup"]["array"]]
-
-            elif rollup_type == "number":
-                self.value: Optional[int, float] = data["rollup"]["number"]
-
-            elif rollup_type == "date":
-                if data["rollup"]["date"]:
-                    self.value: Optional[str] = data["rollup"]["date"].get("start")
-                    self.start: Optional[datetime] = Model.format_iso_time(data["rollup"]["date"].get("start"))
-                    self.end: Optional[datetime] = Model.format_iso_time(data["rollup"]["date"].get("end"))
-                else:
-                    self.value = None
-                    self.start = None
-                    self.end = None
-            else:
-                self.value = "unsupported rollup type"
-
-        if self.type == "files":
-            self.value = "unsupported"
-
-        if self.type == "url":
-            self.value: Optional[str] = data.get("url")
-
-        if self.type == "email":
-            self.value: Optional[str] = data.get("email")
-
-        if self.type == "phone_number":
-            self.value: Optional[str] = data.get("phone_number")
-
-    def __str__(self):
-        return str(self.value)
-
-    def __repr__(self):
-        return f"{self.name}({self})"
-
-    def get(self):
-        # checkbox can not be `None`
-        if self.type in ["checkbox"]:
-            return {self.type: self.value}
-
-        # empty values
-        elif not self.value:
-            if self.type in ["multi_select", "relation", "rich_text", "people", "files"]:
-                return {self.type: []}
-            return {self.type: None}
-
-        # RichTextArray
-        elif self.type in ["title", "rich_text"] and hasattr(self.value, "get"):
-            return {self.type: self.value.get()}
-
-        # simple values
-        elif self.type in ["number", "url", "email", "phone_number"]:
-            return {self.type: self.value}
-
-        # select type
-        elif self.type == "select":
-            return {self.type: {"name": self.value}}
-
-        # multi-select type
-        elif self.type == "multi_select":
-            return {self.type: [{"name": tag} for tag in self.value]}
-
-        # date type
-        elif self.type == "date" and hasattr(self, "start") and hasattr(self, "end"):
-            with_time = True if self.start.hour or self.start.minute else False
-            if self.start:
-                start = self.start.astimezone().isoformat() if with_time else str(self.start.date())
-            else:
-                start = None
-            if self.end:
-                end = self.end.astimezone().isoformat() if with_time else str(self.end.date())
-            else:
-                end = None
-            return {self.type: {"start": start, "end": end}}
-
-        # people type
-        elif self.type == "people":
-            return {self.type: [user.get() for user in self.value]}
-
-        # relation type
-        elif self.type == "relation":
-            return {self.type: [{"id": lt.id} for lt in self.value]}
-
-        # status type
-        elif self.type == "status":
-            return {self.type: {"name": self.value}}
-
-        # unsupported types:
-        elif self.type in ["files"]:
-            return {self.type: []}
-        elif self.type in ["created_time", "last_edited_by", "last_edited_time", "created_by"]:
-            return None
-        elif self.type in ["formula", "rollup"]:
-            return {self.type: {}}
-        return None
-
-    @classmethod
-    def create(cls, type_: str = "", value: Any = None, **kwargs):
-        """
-        PropertyValue Schema Object (watch docs)
-        :param type_: see "create value (Page)" column in "Supported Property types" matrix of README
-        :param value: see "value type" column in "Supported Property types" matrix of README
-
-        ~ examples:
-        + relation type:
-        pv = PropertyValue.create("relation", value=[LinkTo.create(page_id="04262843082a478d97f741948a32613b")])
-        + people type:
-        pv = PropertyValue.create(type_="people", value=[User.create('1d393ffb5efd4d09adfc2cb6738e4812')])
-        + date type:
-        pv = PropertyValue.create(type_="date", value=datetime.now())
-        pv = PropertyValue.create(type_="date", date={"start": str(datetime(2022, 2, 1, 5)), "end": str(datetime.now())})
-        """
-        return cls({"type": type_, type_: value, **kwargs}, name="")
-
-
-class Database(Model):
-    object = "database"
-    path = "databases"
-
-    def __init__(self, **kwargs) -> None:
-        """
-        params from Model +
-        :param cover:
-        :param icon:
-        :param title:
-        :param properties:
-        :param parent:
-        :param url:
-        :param is_inline:
-        """
-        super().__init__(**kwargs)
-        self.cover: Optional[Dict] = kwargs.get("cover")
-        self.icon: Optional[Dict] = kwargs.get("icon")
-        self.title = (kwargs.get("title")
-                      if isinstance(kwargs["title"], RichTextArray) or not kwargs.get("title")
-                      else RichTextArray(kwargs["title"])
-                      )
-        self.properties = {
-            name: (value if isinstance(value, Property) else Property(value))
-            for name, value in kwargs["properties"].items()
-        }
-        self.parent = kwargs["parent"] if isinstance(kwargs.get("parent"), LinkTo) else LinkTo(**kwargs["parent"])
-        self.url: str = kwargs.get("url")
-        self.description = None
-        if "description" in kwargs and kwargs["description"]:
-            if isinstance(kwargs["description"], RichTextArray):
-                self.description = kwargs["description"]
-            elif isinstance(kwargs["description"], str):
-                self.description = RichTextArray.create(kwargs["description"])
-            else:
-                self.description = RichTextArray(kwargs["description"])
-        self.is_inline: bool = kwargs.get("is_inline")
-
-    def __str__(self):
-        return str(self.title)
-
-    def __repr__(self):
-        return f"Database({self.title})"
-
-    def get(self) -> Dict[str, Dict]:
-        new_dict = {
-            "parent": self.parent.get(),
-            "properties": {name: value.get() for name, value in self.properties.items()}
-        }
-        if isinstance(self.title, RichTextArray):
-            new_dict["title"] = self.title.get()
-        if self.description:
-            new_dict["description"] = self.description.get()
-        return new_dict
-
-    @classmethod
-    def create(cls, parent: LinkTo, properties: Dict[str, Property], title: Optional[RichTextArray] = None, **kwargs):
-        return cls(parent=parent, properties=properties, title=title, **kwargs)
-
-
-class Page(Model):
-    object = "page"
-    path = "pages"
-
-    def __init__(self, **kwargs) -> None:
-        """
-        params from Model +
-        :param cover:
-        :param icon:
-        :param parent:
-        :param archived:
-        :param properties:
-        :param url:
-        """
-        super().__init__(**kwargs)
-        self.cover: Optional[Dict] = kwargs.get("cover")
-        self.icon: Optional[Dict] = kwargs.get("icon")
-        self.parent = kwargs["parent"] if isinstance(kwargs.get("parent"), LinkTo) else LinkTo(**kwargs["parent"])
-        self.archived: bool = kwargs.get("archived")
-        self.url: str = kwargs.get("url")
-        self.children = kwargs["children"] if "children" in kwargs else LinkTo(block=self)
-        self.properties = {
-            name: (PropertyValue(data, name) if not isinstance(data, PropertyValue) else data)
-            for name, data in kwargs["properties"].items()
-        }
-        for p in self.properties.values():
-            if "title" in p.type:
-                self.title = p.value
-                break
-        else:
-            self.title = None
-
-    def __str__(self):
-        return str(self.title)
-
-    def __repr__(self):
-        return f"Page({self.title})"
-
-    def get(self):
-        new_dict = {
-            "parent": self.parent.get(without_type=True),
-            "icon": self.icon,  # optional
-            "cover": self.cover,  # optional
-            "properties": {name: p.get() for name, p in self.properties.items()},
-        }
-        if getattr(self, "children", None):
-            new_dict["children"] = self.children.get()  # can not be None
-        return new_dict
-
-    @classmethod
-    def create(
-            cls, parent: LinkTo, properties: Optional[Dict[str, PropertyValue]] = None,
-            title: Optional[RichTextArray, str] = None, children: Optional[BlockArray] = None, **kwargs
-    ):
-        if not properties:
-            properties = {}
-        if title:
-            properties["title"] = PropertyValue.create("title", title)
-        return cls(parent=parent, properties=properties, children=children, **kwargs)
-
-
-class Block(Model):
-    object = "block"
-    path = "blocks"
-
-    def __init__(self, **kwargs):
-        """
-        params from Model +
-        :param has_children:
-        :param type:
-        :param archived:
-        :param create_mode:
-        """
-        super().__init__(**kwargs)
-        self.type: str = kwargs.get("type")
-        self.has_children: bool = kwargs.get("has_children")
-        self.archived: bool = kwargs.get("archived")
-        self.children = LinkTo(block=self)
-        self._level = kwargs["level"] if kwargs.get("level") else 0
-        self.create_mode: bool = kwargs["create_mode"] if "create_mode" in kwargs else False
-        self.parent = None
-        self._plain_text = ""
-
-        if self.create_mode:
-            self.text = kwargs[self.type]
-            if "checked" in kwargs:
-                self.checked = kwargs["checked"]
-            if "language" in kwargs:
-                self.language = kwargs["language"]
-            if "caption" in kwargs:
-                self.caption = kwargs["caption"]
-                if isinstance(self.caption, str):
-                    self.caption = RichTextArray.create(self.caption)
-            if "is_toggleable" in kwargs:
-                self.is_toggleable = kwargs["is_toggleable"]
-            return
-        self.parent = kwargs["parent"] if isinstance(kwargs.get("parent"), LinkTo) else LinkTo(**kwargs["parent"])
-
-        if self.type == "paragraph":
-            self.text = RichTextArray(kwargs[self.type].get("rich_text"))
-            self._plain_text = self.text.simple
-
-        elif "heading" in self.type:
-            indent = self.type.split("_")[-1]
-            indent_num = int(indent) if indent.isdigit() else 0
-            prefix = "#" * indent_num + " "
-            r_text = RichTextArray(kwargs[self.type].get("rich_text"))
-            self.text = RichTextArray.create(prefix) + r_text
-            self._plain_text = r_text.simple
-            self.is_toggleable: bool = kwargs[self.type].get("is_toggleable")
-
-        elif self.type == "callout":
-            self.text = RichTextArray(kwargs[self.type].get("rich_text"))
-            self._plain_text = self.text.simple
-            self.icon: Dict = kwargs[self.type].get("icon")
-
-        elif self.type == "quote":
-            r_text = RichTextArray(kwargs[self.type].get("rich_text"))
-            self.text = RichTextArray.create("| ") + r_text
-            self._plain_text = r_text.simple
-
-        elif "list_item" in self.type:
-            r_text = RichTextArray(kwargs[self.type].get("rich_text"))
-            self.text = RichTextArray.create("- ") + r_text
-            self._plain_text = r_text.simple
-            # Numbers does not support cause of lack of relativity
-
-        elif self.type == "to_do":
-            self.checked: bool = kwargs[self.type].get("checked")
-            prefix = "[x] " if self.checked else "[ ] "
-            r_text = RichTextArray(kwargs[self.type].get("rich_text"))
-            self.text = RichTextArray.create(prefix) + r_text
-            self._plain_text = r_text.simple
-
-        elif self.type == "toggle":
-            r_text = RichTextArray(kwargs[self.type].get("rich_text"))
-            self.text = RichTextArray.create("> ") + r_text
-            self._plain_text = r_text.simple
-
-        elif self.type == "code":
-            r_text = RichTextArray(kwargs[self.type].get("rich_text"))
-            self.language: str = kwargs[self.type].get("language")
-            prefix = RichTextArray.create(f"```{self.language}\n") if self.language else RichTextArray.create("```\n")
-            self.text = prefix + r_text + "\n```"
-            self._plain_text = r_text.simple
-            self.caption = RichTextArray(kwargs[self.type].get("caption"))
-
-        # when the block is child_page, parent will be the page object
-        # when the block is child_database, parent AND children will be the database object
-        elif "child" in self.type:
-            self.text: str = kwargs[self.type].get("title")
-            self._plain_text = str(self.text)
-            if self.type == "child_page":
-                # self.children is already set
-                self.parent = LinkTo(type="page", page=self.id)
-                self._plain_text = str(self.parent.link)
-            elif self.type == "child_database":
-                # well yes. parent and children are the same. parent of this database will be the page of this block
-                # and the database is children of this block
-                self.parent = LinkTo.create(database_id=self.id)
-                self.children = LinkTo.create(database_id=self.id)
-                self._plain_text = str(self.parent.link)
-                if not self.text:
-                    self.text = repr(self.children)
-            # page self.has_children is correct. checked.
-            # database self.has_children is false.
-            # database with custom source had no title!
-
-        # hello, markdown
-        elif self.type == "embed":
-            self.caption = RichTextArray(kwargs[self.type].get("caption"))
-            text = kwargs[self.type].get("url")
-            self._plain_text = str(text)
-            if self.caption:
-                self.text = f'[{self.caption}]({text})'
-            else:
-                self.text = f'<{text}>' if text else "*Empty embed*"
-
-        elif self.type == "image":
-            self.caption = RichTextArray(kwargs[self.type].get("caption"))
-            subtype = kwargs[self.type].get("type")
-            if subtype == "file":
-                # The file S3 URL will be valid for 1 hour
-                self.expiry_time = Model.format_iso_time(kwargs[self.type][subtype].get("expiry_time"))
-            else:
-                self.expiry_time = None
-            if subtype in ("file", "external"):
-                text = kwargs[self.type][subtype].get("url")
-                self._plain_text = str(text)
-                if self.caption:
-                    self.text = f'[{self.caption}]({text})'
-                else:
-                    self.text = f'<{text}>'
-            else:
-                self.text = "*Unknown image type*"
-                self._plain_text = "None"
-
-        elif self.type == "video":
-            self.caption = RichTextArray(kwargs[self.type].get("caption"))
-            subtype = kwargs[self.type].get("type")
-            if subtype == "file":
-                self.expiry_time = Model.format_iso_time(kwargs[self.type][subtype].get("expiry_time"))
-            else:
-                self.expiry_time = None
-            if subtype in ("file", "external"):
-                text = kwargs[self.type][subtype].get("url")
-                self._plain_text = str(text)
-                if self.caption:
-                    self.text = f'[{self.caption}]({text})'
-                else:
-                    self.text = f'<{text}>'
-            else:
-                self.text = "*Unknown video type*"
-                self._plain_text = "None"
-
-        elif self.type == "file":
-            self.caption = RichTextArray(kwargs[self.type].get("caption"))
-            subtype = kwargs[self.type].get("type")
-            if subtype == "file":
-                self.expiry_time = Model.format_iso_time(kwargs[self.type][subtype].get("expiry_time"))
-            else:
-                self.expiry_time = None
-            if subtype in ("file", "external"):
-                text = kwargs[self.type][subtype].get("url")
-                self._plain_text = str(text)
-                if self.caption:
-                    self.text = f'[{self.caption}]({text})'
-                else:
-                    self.text = f'<{text}>'
-            else:
-                self.text = "*Unknown file type*"
-                self._plain_text = "None"
-
-        elif self.type == "pdf":
-            self.caption = RichTextArray(kwargs[self.type].get("caption"))
-            subtype = kwargs[self.type].get("type")
-            if subtype == "file":
-                self.expiry_time = Model.format_iso_time(kwargs[self.type][subtype].get("expiry_time"))
-            else:
-                self.expiry_time = None
-            if subtype in ("file", "external"):
-                text = kwargs[self.type][subtype].get("url")
-                self._plain_text = str(text)
-                if self.caption:
-                    self.text = f'[{self.caption}]({text})'
-                else:
-                    self.text = f'<{text}>'
-            else:
-                self.text = "*Unknown pdf type*"
-                self._plain_text = "None"
-
-        elif self.type == "breadcrumb":
-            self.text = "*breadcrumb block*"
-            self._plain_text = "None"
-
-        elif self.type == "bookmark":
-            self.caption = RichTextArray(kwargs[self.type].get("caption"))
-            text = kwargs[self.type].get("url")
-            self._plain_text = str(text)
-            if self.caption:
-                self.text = f'[{self.caption}]({text})'
-            else:
-                self.text = f'<{text}>' if text else "*Empty bookmark*"
-
-        elif self.type == "link_preview":
-            text = kwargs[self.type].get("url")
-            self._plain_text = str(text)
-            self.text = f'<{text}>'
-
-        elif self.type == "link_to_page":
-            self.link = LinkTo(**kwargs[self.type])
-            self.text = repr(self.link)
-            self._plain_text = str(self.link.link)
-
-        elif self.type == "equation":
-            self.text: str = kwargs[self.type].get("expression")
-            self._plain_text = str(self.text)
-
-        elif self.type == "divider":
-            self.text = "---"
-            self._plain_text = "None"
-
-        elif self.type == "table_of_contents":
-            self.text = "*Table of contents*"
-            self._plain_text = "None"
-
-        elif self.type == "template":
-            r_text = RichTextArray(kwargs[self.type].get("rich_text"))
-            self.text = RichTextArray.create("Template: ") + r_text
-            self._plain_text = r_text.simple
-
-        elif self.type == "synced_block":
-            synced_from = kwargs[self.type].get("synced_from")
-            self.text = "*SYNCED BLOCK:*"
-            self._plain_text = "None"
-            self.synced_from = LinkTo(**synced_from) if synced_from else None
-
-        elif self.type == "table":
-            self.table_width: int = kwargs[self.type].get("table_width")
-            self.text = f"*Table {self.table_width}xN:*"
-            self._plain_text = "None"
-
-        elif self.type == "table_row":
-            cells = kwargs[self.type].get("cells")
-            self.text = RichTextArray.create("| ")
-            for cell in cells:
-                text_cell = RichTextArray(cell)
-                self._plain_text += f"\"{text_cell}\","
-                self.text += text_cell + " | "
-            self._plain_text = self._plain_text.strip(",")
-
-        elif self.type == "unsupported":
-            self.text = "*****"
-            self._plain_text = "None"
-
-        else:
-            self.text = "*UNKNOWN_BLOCK_TYPE*"
-            self._plain_text = "None"
-
-    def __str__(self):
-        return str(self.text)
-
-    def __repr__(self):
-        return f"Block({str(self.text)[:30]})"
-
-    def get(self, with_object_type: bool = False):
-        if self.type in [
-            "paragraph", "quote", "heading_1", "heading_2", "heading_3", "to_do",
-            "bulleted_list_item", "numbered_list_item", "toggle", "callout", "code", "child_database"
-        ]:
-
-            text = RichTextArray.create(self.text) if isinstance(self.text, str) else self.text
-
-            # base content
-            new_dict = {self.type: {"rich_text": text.get()}}
-
-            # to_do type attrs
-            if self.type == "to_do" and hasattr(self, "checked"):
-                new_dict[self.type]["checked"] = self.checked
-
-            # code type attrs
-            elif self.type == "code":
-                new_dict[self.type]["language"] = getattr(self, "language", "plain text")
-                if hasattr(self, "caption"):
-                    new_dict[self.type]["caption"] = self.caption.get()
-
-            # child_database type struct
-            elif self.type == "child_database":
-                new_dict = {self.type: {"title": str(text)}}
-
-            # heading_X types attrs
-            elif "heading" in self.type:
-                if hasattr(self, "is_toggleable") and isinstance(self.is_toggleable, bool):
-                    new_dict[self.type]["is_toggleable"] = self.is_toggleable
-                else:
-                    new_dict[self.type]["is_toggleable"] = False
-
-            if with_object_type:
-                new_dict["object"] = "block"
-                new_dict["type"] = self.type
-            return new_dict
-        return None
-
-    @property
-    def simple(self) -> str:
-        if self._plain_text:
-            return self._plain_text if self._plain_text != "None" else ""
-        if getattr(self, "text", None):
-            return str(self.text)
-        return self._plain_text
-
-    @classmethod
-    def create(cls, text: str, type_: str = "paragraph", **kwargs):
-        """
-        :param text:   Block content
-        :param type_:  Block types (API)
-        :param kwargs:
-            :kwargs param checked:          bool for to_do
-            :kwargs param language:         str for code
-            :kwargs param caption:          str or RichTextArray for code
-            :kwargs param is_toggleable:    bool for heading_1, heading_2, heading_3
-        :return:
-        """
-        new_dict = {
-            "type": type_,
-            type_: text,
-        }
-        return cls(**new_dict, create_mode=True, **kwargs)
-
-
-class ElementArray(MutableSequence):
-    class_map = {"page": Page, "database": Database, "block": Block}
-
-    def __init__(self, array, create: bool = False):
-        if create:
-            self.array = array
-            return
-
-        self.array = []
-        for ele in array:
-            if ele.get("object") and ele["object"] in self.class_map:
-                self.array.append(self.class_map[ele["object"]](**ele))
-
-    def __getitem__(self, item):
-        return self.array[item]
-
-    def __setitem__(self, key, value):
-        self.array[key] = value
-
-    def __delitem__(self, key):
-        del self.array[key]
-
-    def __len__(self):
-        return len(self.array)
-
-    def insert(self, index: int, value) -> None:
-        self.array.insert(index, value)
-
-    def __str__(self):
-        return "\n".join(str(b) for b in self)
-
-    def __repr__(self):
-        r = str(self)[:30].replace("\n", " ")
-        return f"ElementArray({r})"
-
-
-class BlockArray(ElementArray):
-    def __str__(self):
-        return "\n".join(b._level * "\t" + str(b) for b in self)
-
-    def __repr__(self):
-        r = str(self)[:30].replace("\n", " ")
-        return f"BlockArray({r})"
-
-    def get(self):
-        return [b.get() for b in self]
-
-    @property
-    def simple(self) -> str:
-        return "\n".join(b._level * "\t" + b.simple for b in self)
-
-
-class PageArray(ElementArray):
-    def __repr__(self):
-        r = str(self)[:30].replace("\n", " ")
-        return f"PageArray({r})"
-
-
-class LinkTo(object):
-    """
-    schema
-    .type = `element_type`
-    .id = `elementID`
-
-    .get() - return API like style
-    .create() - create in format `(page_id="123412341234")` or (database_id="13412341234")`
-    """
-
-    def __init__(
-            self, block: Optional[Model] = None, from_object: Optional[Block, Page, Database] = None, **kwargs
-    ):
-        """
-        Creates LinkTo object from API dict
-
-        :param block: Block object can be provided instead other attrs. Internal usage.
-        :param from_object: Any model object can be provided to create LinkTo to it.
-        :param kwargs: API attrs. Internal usage.
-        """
-        if block:
-            self.type = block.object
-            self.id = block.id
-            self.after_path = "children"
-            self.uri = "blocks"
-        # You can provide the object to create the LinkTo to it
-        elif from_object:
-            self.uri = from_object.path
-            self.id = from_object.id
-            if isinstance(from_object, Page):
-                self.type = "page_id"
-            elif isinstance(from_object, Database):
-                self.type = "database_id"
-            elif isinstance(from_object, Block):
-                self.type = "block_id"
-            elif isinstance(from_object, User):
-                self.type = "user_id"
-        else:
-            self.type: str = kwargs.get("type")
-            self.id: str = kwargs.get(self.type) if kwargs.get(self.type) else kwargs.get("id")
-            if self.type == "workspace":
-                self.id = ""
-            self.after_path = ""
-            if self.type == "page_id":
-                self.uri = "pages"
-            elif self.type == "database_id":
-                self.uri = "databases"
-            # when type is set manually
-            elif self.type == "page":  # deprecated.
-                self.uri = "pages"
-            elif self.type == "block_id":
-                self.uri = "blocks"
-            elif self.type == "user_id":
-                self.uri = "users"
-            else:
-                self.uri = None
-
-        if isinstance(self.id, str):
-            self.id = self.id.replace("-", "")
-
-    def __str__(self):
-        prefix = self.uri if self.uri else self.type
-        if getattr(self, "after_path", ""):
-            return f"{prefix}/{self.id}/{self.after_path}"
-        return f"{prefix}/{self.id}"
-
-    def __repr__(self):
-        return f"LinkTo({self})"
-
-    @property
-    def link(self) -> str:
-        return NOTION_URL + str(self)
-
-    def get(self, without_type: bool = False):
-        if self.type == "workspace":
-            return {"type": "workspace", "workspace": True}
-        if without_type:
-            return {self.type: self.id}
-        return {"type": self.type, self.type: self.id}
-
-    @classmethod
-    def create(cls, **kwargs):
-        """
-        `.create(page_id="123412341234")`
-        `.create(database_id="13412341234")`
-        `.create(workspace=True)`
-        """
-        for key, value in kwargs.items():
-            return cls(type=key, id=value)
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+from datetime import datetime
+from typing import Optional, Dict, Union, List, Any
+from collections.abc import MutableSequence
+
+from pytion.envs import NOTION_URL
+
+
+# I wanna use pydantic, but API provide variable names of property
+
+class RichText(object):
+    def __init__(self, **kwargs) -> None:
+        self.plain_text: str = kwargs.get("plain_text")
+        self.href: Optional[str] = kwargs.get("href")
+        self.annotations: Dict[str, Union[bool, str]] = kwargs.get("annotations")
+        # if not self.annotations:
+        #     self._create_default_annotations()
+        self.type: str = kwargs.get("type")
+        self.simple = ""
+        if self.type == "mention":
+            subtype = kwargs[self.type].get("type")
+            if subtype == "user":
+                self.data = User(**kwargs[self.type].get(subtype))
+                self.plain_text = str(self.data)
+                self.simple = LinkTo(from_object=self.data).link
+            elif subtype == "page":
+                sub_id = kwargs[self.type][subtype].get("id") if kwargs[self.type].get(subtype) else ""
+                self.data = LinkTo.create(page=sub_id)
+                if self.plain_text == "Untitled":
+                    self.plain_text = repr(self.data)
+                else:
+                    self.plain_text = "LinkTo(" + self.plain_text + ")"
+                self.simple = self.data.link
+            elif subtype == "database":
+                sub_id = kwargs[self.type][subtype].get("id") if kwargs[self.type].get(subtype) else ""
+                self.data = LinkTo.create(database_id=sub_id)
+                if self.plain_text == "Untitled":
+                    self.plain_text = repr(self.data)
+                else:
+                    self.plain_text = "LinkTo(" + self.plain_text + ")"
+                self.simple = self.data.link
+            elif subtype == "date":
+                self.data = {
+                    "start": Model.format_iso_time(kwargs[self.type][subtype].get("start")),
+                    "end": Model.format_iso_time(kwargs[self.type][subtype].get("end"))
+                }
+                self.simple = str(self.plain_text)
+            elif subtype == "link_preview":
+                self.simple = str(self.plain_text)
+                self.plain_text = f"<{self.plain_text}>"
+                self.data: Dict = kwargs[self.type]
+        else:
+            self.data: Dict = kwargs[self.type]
+            self.simple = str(self.plain_text)
+
+    def __str__(self):
+        return str(self.plain_text)
+
+    def __repr__(self):
+        return f"RichText({self.plain_text})"
+
+    def __bool__(self):
+        return bool(self.plain_text)
+
+    def _create_default_annotations(self):
+        self.annotations = {
+            "bold": False, "italic": False, "strikethrough": False,
+            "underline": False, "code": False, "color": "default"
+        }
+
+    # def __len__(self):
+    #     return len(self.plain_text)
+
+    def get(self) -> Dict[str, Any]:
+        """
+        Text type supported only
+        """
+        return {
+            "type": "text",
+            "text": {"content": self.plain_text, "link": None},
+            # "annotations": self.annotations,
+            # "plain_text": self.plain_text,
+        }
+
+
+class RichTextArray(MutableSequence):
+    def __init__(self, array: List[Dict]) -> None:
+        self.array = [RichText(**rt) for rt in array]
+
+    def __getitem__(self, item):
+        return self.array[item]
+
+    def __setitem__(self, key, value):
+        self.array[key] = value
+
+    def __delitem__(self, key):
+        del self.array[key]
+
+    def __len__(self):
+        return len(self.array)
+
+    def insert(self, index: int, value) -> None:
+        self.array.insert(index, value)
+
+    def __str__(self):
+        return "".join(str(rt) for rt in self)
+
+    def __repr__(self):
+        return f"RichTextArray({str(self)})"
+
+    def __bool__(self):
+        return any(map(bool, self.array))
+
+    def __add__(self, another: Union[RichTextArray, str]):
+        if isinstance(another, str):
+            another = RichTextArray.create(another)
+        self.array.extend(another)
+        return self
+
+    def get(self) -> List[Dict[str, Any]]:
+        return [item.get() for item in self]
+
+    @classmethod
+    def create(cls, text: str):
+        return cls([{"type": "text", "plain_text": text, "text": {}}])
+
+    @property
+    def simple(self) -> str:
+        return "".join(rt.simple for rt in self)
+
+
+class User(object):
+    """
+    The User object represents a user in a Notion workspace.
+    """
+    path = "users"
+
+    def __init__(self, **kwargs) -> None:
+        """
+        Create an User object by providing dict from API.
+
+        API attrs (from API docs):
+        Mandatory:
+        :param id: str
+        :param object: str
+
+        Optional:
+        :param type: str
+        :param name: str
+        :param avatar_url: str
+
+        Also Local attrs:
+        :param raw: dict from API
+        :param email: str if user is person
+        """
+        self.id = kwargs.get("id", "").replace("-", "")
+        self.object = kwargs.get("object")  # user
+        self.type = kwargs.get("type")
+        self.name = kwargs.get("name")
+        self.avatar_url = kwargs.get("avatar_url")
+        if self.type == "person" and kwargs.get(self.type):
+            self.email = kwargs[self.type].get("email")
+            self.workspace_name = None
+        elif self.type == "bot":
+            self.email = None
+            self.workspace_name = kwargs[self.type].get("workspace_name")
+        else:
+            self.email = None
+            self.workspace_name = None
+        self.raw = kwargs
+
+    def __str__(self):
+        if self.name and self.email:
+            name = f"{self.name}({self.email})"
+        else:
+            name = self.name
+        return name if name else self.id
+
+    def __repr__(self):
+        return f"User({self})"
+
+    def get(self) -> Dict[str, str]:
+        return {
+            "object": self.object,
+            "id": self.id
+        }
+
+    @classmethod
+    def create(cls, id: str):
+        return cls(object="user", id=id)
+
+
+class Model(object):
+    """
+    :param id:
+    :param object:
+    :param created_time:
+    :param last_edited_time:
+    :param created_by:
+    :param last_edited_by:
+    :param raw:
+    """
+
+    def __init__(self, **kwargs) -> None:
+        self.id = kwargs.get("id", "").replace("-", "")
+        self.object = kwargs.get("object")
+        self.created_time = self.format_iso_time(kwargs.get("created_time"))
+        self.last_edited_time = self.format_iso_time(kwargs.get("last_edited_time"))
+        self.created_by = User(**kwargs["created_by"]) if kwargs.get("created_by") else None
+        self.last_edited_by = User(**kwargs["last_edited_by"]) if kwargs.get("last_edited_by") else None
+        self.raw = kwargs
+
+    @classmethod
+    def format_iso_time(cls, time: str) -> Optional[datetime]:
+        if not time:
+            return None
+        return datetime.fromisoformat(time.replace("Z", "+00:00"))
+
+
+class Property(object):
+    def __init__(self, data: Dict[str, Any]):
+        self.to_delete = True if data.get("type", False) is None else False
+        self.id: str = data.get("id")
+        self.type: str = data.get("type", "")
+        self.name: str = data.get("name")
+        self.raw = data
+        self.subtype = None
+
+        if self.type == "relation":
+            if isinstance(data[self.type], dict):
+                self.subtype = data[self.type].get("type")
+                self.relation = LinkTo.create(database_id=data[self.type].get("database_id"))
+                if self.subtype == "single_property":
+                    pass
+                elif self.subtype == "dual_property":
+                    self.relation_property_id = data[self.type][self.subtype].get("synced_property_id")
+                    self.relation_property_name = data[self.type][self.subtype].get("synced_property_name")
+
+        elif self.type == "status":
+            if isinstance(data[self.type], dict):
+                self.options = data[self.type].get("options", [])
+                self.groups = data[self.type].get("groups", [])
+
+        elif self.type == "rollup":
+            if isinstance(data[self.type], dict):
+                self.function = data[self.type].get("function")
+                self.relation_property_id = data[self.type].get("relation_property_id")
+                self.relation_property_name = data[self.type].get("relation_property_name")
+                self.rollup_property_id = data[self.type].get("rollup_property_id")
+                self.rollup_property_name = data[self.type].get("rollup_property_name")
+
+    def __str__(self):
+        return self.name if self.name else self.type
+
+    def __repr__(self):
+        return f"Property({self})"
+
+    def get(self) -> Optional[Dict[str, Dict]]:
+        # property removing while patch
+        if self.to_delete:
+            return None
+        # property renaming while patch
+        data = {}
+        if self.name:
+            data["name"] = self.name
+        # property retyping while patch
+        if self.type:
+            # create relation type property with configuration
+            if self.type == "relation":
+                data[self.type] = {self.subtype: {}, "database_id": self.relation.id}
+            elif self.type == "status":
+                data[self.type] = {}
+                # not configurable by API
+                # if self.options:
+                #     data[self.type]["options"] = self.options
+                # if self.groups:
+                #     data[self.type]["groups"] = self.groups
+            elif self.type == "rollup":
+                data[self.type] = {"function": self.function}
+                if self.relation_property_id:
+                    data[self.type]["relation_property_id"] = self.relation_property_id
+                if self.relation_property_name:
+                    data[self.type]["relation_property_name"] = self.relation_property_name
+                if self.rollup_property_id:
+                    data[self.type]["rollup_property_id"] = self.rollup_property_id
+                if self.rollup_property_name:
+                    data[self.type]["rollup_property_name"] = self.rollup_property_name
+            else:
+                data[self.type] = {}
+        return data
+
+    @classmethod
+    def create(cls, type_: Optional[str] = "", **kwargs):
+        """
+        Property Schema Object (watch docs)
+        :param type_: see "create (DB)" column in "Supported Property types" matrix of README
+
+        + addons:
+        set type_ = `None` to delete this Property
+        set param `name` to rename this Property
+
+        + relation type:
+        set param `single_property` with `database_id` value OR
+        set param `dual_property` with `database_id` value
+        Property.create(type_="relation", dual_property="v111c132c12c1242341c41c")
+
+        + rollup type:
+        set param `function` from Nation API Rollup reference (BE AWARE ABOUT THE VALUE TYPE AND CHECK FUNCTION)
+        set param `relation_property_id` with Property ID with Relation type OR \
+        set param `relation_property_name` with Property NAME with Relation type
+        set param `rollup_property_id` with Property ID of related database OR \
+        set param `rollup_property_name` with Property NAME of related database
+        Property.create("rollup", function="average", relation_property_id="GHpm", rollup_property_id="mvpx")
+        """
+        if type_ == "relation":
+            subtype = next(kwarg for kwarg in kwargs if kwarg in ("single_property", "dual_property"))
+            kwargs["relation"] = {"type": subtype, subtype: {}, "database_id": kwargs[subtype]}
+        elif type_ == "status":
+            kwargs["status"] = {}
+        elif type_ == "rollup":
+            kwargs["rollup"] = kwargs
+        return cls({"type": type_, **kwargs})
+
+
+class PropertyValue(Property):
+    def __init__(self, data: Dict, name: str, **kwargs):
+        super().__init__(data)
+        # getting Paginated Properties (for retrieving property item)
+        # *Pagination
+        if data.get("object") and data["object"] == "list":
+            if data.get("results"):
+                self.type = data["results"][0].get("type")
+                data[self.type] = [sub_dict.get(sub_dict.get("type")) for sub_dict in data["results"]]
+
+        self.name = name
+        self.value = None
+
+        if self.type in ["title", "rich_text"]:
+            if isinstance(data[self.type], list):
+                self.value = RichTextArray(data[self.type])
+            elif isinstance(data[self.type], RichTextArray):
+                self.value = data[self.type]
+            else:
+                self.value = RichTextArray.create(data[self.type])
+
+        if self.type == "number":
+            self.value: Union[int, float, None] = data["number"]
+
+        if self.type == "select":
+            if data["select"] and isinstance(data["select"], dict):
+                self.value: Optional[str] = data["select"].get("name")
+            elif data["select"] and isinstance(data["select"], str):
+                self.value = data["select"]
+            else:
+                self.value = None
+
+        if self.type == "multi_select":
+            self.value: List[str] = [(v.get("name") if isinstance(v, dict) else v) for v in data["multi_select"]]
+
+        if self.type == "checkbox":
+            self.value: bool = data["checkbox"]
+
+        if self.type == "date":
+            if isinstance(data["date"], datetime):
+                self.value = data["date"].isoformat()
+                self.start = data["date"]
+                self.end = None
+            elif data["date"]:
+                self.value: Optional[str] = data["date"].get("start")
+                self.start: Optional[datetime] = Model.format_iso_time(data["date"].get("start"))
+                self.end: Optional[datetime] = Model.format_iso_time(data["date"].get("end"))
+            else:
+                self.value = None
+                self.start = None
+                self.end = None
+
+        if "time" in self.type:
+            self.value: Optional[datetime] = Model.format_iso_time(data.get(self.type))
+
+        if self.type == "formula":
+            formula_type = data["formula"]["type"]
+            if formula_type == "date":
+                if data["formula"]["date"]:
+                    self.value: str = data["formula"]["date"].get("start")
+                    self.start: Optional[datetime] = Model.format_iso_time(data["formula"]["date"].get("start"))
+                    self.end: Optional[datetime] = Model.format_iso_time(data["formula"]["date"].get("end"))
+                else:
+                    self.value = None
+                    self.start = None
+                    self.end = None
+            else:
+                self.value: Union[str, int, float, bool] = data["formula"][formula_type]
+
+        if self.type == "created_by":
+            self.value = User(**data.get(self.type))
+
+        if self.type == "last_edited_by":
+            self.value = User(**data.get(self.type))
+
+        if self.type == "people":
+            self.value = [user if isinstance(user, User) else User(**user) for user in data[self.type]]
+
+        if self.type == "relation":
+            self.value: List[LinkTo] = [
+                LinkTo.create(page_id=item.get("id")) if not isinstance(item, LinkTo) else item
+                for item in data[self.type]
+            ]
+            self.has_more = data["has_more"] if "has_more" in data else False
+
+        if self.type == "status":
+            self.value = data[self.type].get("name") if isinstance(data[self.type], dict) else data[self.type]
+
+        if self.type == "rollup":
+            rollup_type = data["rollup"]["type"]
+            if rollup_type == "array":
+                if len(data["rollup"]["array"]) == 0:
+                    self.value = None
+                elif len(data["rollup"]["array"]) == 1:
+                    self.value = PropertyValue(data["rollup"]["array"][0], rollup_type)
+                else:
+                    self.value = [PropertyValue(element, rollup_type).value for element in data["rollup"]["array"]]
+
+            elif rollup_type == "number":
+                self.value: Union[int, float, None] = data["rollup"]["number"]
+
+            elif rollup_type == "date":
+                if data["rollup"]["date"]:
+                    self.value: Optional[str] = data["rollup"]["date"].get("start")
+                    self.start: Optional[datetime] = Model.format_iso_time(data["rollup"]["date"].get("start"))
+                    self.end: Optional[datetime] = Model.format_iso_time(data["rollup"]["date"].get("end"))
+                else:
+                    self.value = None
+                    self.start = None
+                    self.end = None
+            else:
+                self.value = "unsupported rollup type"
+
+        if self.type == "files":
+            self.value = "unsupported"
+
+        if self.type == "url":
+            self.value: Optional[str] = data.get("url")
+
+        if self.type == "email":
+            self.value: Optional[str] = data.get("email")
+
+        if self.type == "phone_number":
+            self.value: Optional[str] = data.get("phone_number")
+
+    def __str__(self):
+        return str(self.value)
+
+    def __repr__(self):
+        return f"{self.name}({self})"
+
+    def get(self):
+        # checkbox can not be `None`
+        if self.type in ["checkbox"]:
+            return {self.type: self.value}
+
+        # empty values
+        elif not self.value:
+            if self.type in ["multi_select", "relation", "rich_text", "people", "files"]:
+                return {self.type: []}
+            return {self.type: None}
+
+        # RichTextArray
+        elif self.type in ["title", "rich_text"] and hasattr(self.value, "get"):
+            return {self.type: self.value.get()}
+
+        # simple values
+        elif self.type in ["number", "url", "email", "phone_number"]:
+            return {self.type: self.value}
+
+        # select type
+        elif self.type == "select":
+            return {self.type: {"name": self.value}}
+
+        # multi-select type
+        elif self.type == "multi_select":
+            return {self.type: [{"name": tag} for tag in self.value]}
+
+        # date type
+        elif self.type == "date" and hasattr(self, "start") and hasattr(self, "end"):
+            with_time = True if self.start.hour or self.start.minute else False
+            if self.start:
+                start = self.start.astimezone().isoformat() if with_time else str(self.start.date())
+            else:
+                start = None
+            if self.end:
+                end = self.end.astimezone().isoformat() if with_time else str(self.end.date())
+            else:
+                end = None
+            return {self.type: {"start": start, "end": end}}
+
+        # people type
+        elif self.type == "people":
+            return {self.type: [user.get() for user in self.value]}
+
+        # relation type
+        elif self.type == "relation":
+            return {self.type: [{"id": lt.id} for lt in self.value]}
+
+        # status type
+        elif self.type == "status":
+            return {self.type: {"name": self.value}}
+
+        # unsupported types:
+        elif self.type in ["files"]:
+            return {self.type: []}
+        elif self.type in ["created_time", "last_edited_by", "last_edited_time", "created_by"]:
+            return None
+        elif self.type in ["formula", "rollup"]:
+            return {self.type: {}}
+        return None
+
+    @classmethod
+    def create(cls, type_: str = "", value: Any = None, **kwargs):
+        """
+        PropertyValue Schema Object (watch docs)
+        :param type_: see "create value (Page)" column in "Supported Property types" matrix of README
+        :param value: see "value type" column in "Supported Property types" matrix of README
+
+        ~ examples:
+        + relation type:
+        pv = PropertyValue.create("relation", value=[LinkTo.create(page_id="04262843082a478d97f741948a32613b")])
+        + people type:
+        pv = PropertyValue.create(type_="people", value=[User.create('1d393ffb5efd4d09adfc2cb6738e4812')])
+        + date type:
+        pv = PropertyValue.create(type_="date", value=datetime.now())
+        pv = PropertyValue.create(type_="date", date={"start": str(datetime(2022, 2, 1, 5)), "end": str(datetime.now())})
+        """
+        return cls({"type": type_, type_: value, **kwargs}, name="")
+
+
+class Database(Model):
+    object = "database"
+    path = "databases"
+
+    def __init__(self, **kwargs) -> None:
+        """
+        params from Model +
+        :param cover:
+        :param icon:
+        :param title:
+        :param properties:
+        :param parent:
+        :param url:
+        :param is_inline:
+        """
+        super().__init__(**kwargs)
+        self.cover: Optional[Dict] = kwargs.get("cover")
+        self.icon: Optional[Dict] = kwargs.get("icon")
+        self.title = (kwargs.get("title")
+                      if isinstance(kwargs["title"], RichTextArray) or not kwargs.get("title")
+                      else RichTextArray(kwargs["title"])
+                      )
+        self.properties = {
+            name: (value if isinstance(value, Property) else Property(value))
+            for name, value in kwargs["properties"].items()
+        }
+        self.parent = kwargs["parent"] if isinstance(kwargs.get("parent"), LinkTo) else LinkTo(**kwargs["parent"])
+        self.url: str = kwargs.get("url")
+        self.description = None
+        if "description" in kwargs and kwargs["description"]:
+            if isinstance(kwargs["description"], RichTextArray):
+                self.description = kwargs["description"]
+            elif isinstance(kwargs["description"], str):
+                self.description = RichTextArray.create(kwargs["description"])
+            else:
+                self.description = RichTextArray(kwargs["description"])
+        self.is_inline: bool = kwargs.get("is_inline")
+
+    def __str__(self):
+        return str(self.title)
+
+    def __repr__(self):
+        return f"Database({self.title})"
+
+    def get(self) -> Dict[str, Dict]:
+        new_dict = {
+            "parent": self.parent.get(),
+            "properties": {name: value.get() for name, value in self.properties.items()}
+        }
+        if isinstance(self.title, RichTextArray):
+            new_dict["title"] = self.title.get()
+        if self.description:
+            new_dict["description"] = self.description.get()
+        return new_dict
+
+    @classmethod
+    def create(cls, parent: LinkTo, properties: Dict[str, Property], title: Optional[RichTextArray] = None, **kwargs):
+        return cls(parent=parent, properties=properties, title=title, **kwargs)
+
+
+class Page(Model):
+    object = "page"
+    path = "pages"
+
+    def __init__(self, **kwargs) -> None:
+        """
+        params from Model +
+        :param cover:
+        :param icon:
+        :param parent:
+        :param archived:
+        :param properties:
+        :param url:
+        """
+        super().__init__(**kwargs)
+        self.cover: Optional[Dict] = kwargs.get("cover")
+        self.icon: Optional[Dict] = kwargs.get("icon")
+        self.parent = kwargs["parent"] if isinstance(kwargs.get("parent"), LinkTo) else LinkTo(**kwargs["parent"])
+        self.archived: bool = kwargs.get("archived")
+        self.url: str = kwargs.get("url")
+        self.children = kwargs["children"] if "children" in kwargs else LinkTo(block=self)
+        self.properties = {
+            name: (PropertyValue(data, name) if not isinstance(data, PropertyValue) else data)
+            for name, data in kwargs["properties"].items()
+        }
+        for p in self.properties.values():
+            if "title" in p.type:
+                self.title = p.value
+                break
+        else:
+            self.title = None
+
+    def __str__(self):
+        return str(self.title)
+
+    def __repr__(self):
+        return f"Page({self.title})"
+
+    def get(self):
+        new_dict = {
+            "parent": self.parent.get(without_type=True),
+            "icon": self.icon,  # optional
+            "cover": self.cover,  # optional
+            "properties": {name: p.get() for name, p in self.properties.items()},
+        }
+        if getattr(self, "children", None):
+            new_dict["children"] = self.children.get()  # can not be None
+        return new_dict
+
+    @classmethod
+    def create(
+            cls, parent: LinkTo, properties: Optional[Dict[str, PropertyValue]] = None,
+            title: Union[RichTextArray, str, None] = None, children: Optional[BlockArray] = None, **kwargs
+    ):
+        if not properties:
+            properties = {}
+        if title:
+            properties["title"] = PropertyValue.create("title", title)
+        return cls(parent=parent, properties=properties, children=children, **kwargs)
+
+
+class Block(Model):
+    object = "block"
+    path = "blocks"
+
+    def __init__(self, **kwargs):
+        """
+        params from Model +
+        :param has_children:
+        :param type:
+        :param archived:
+        :param create_mode:
+        """
+        super().__init__(**kwargs)
+        self.type: str = kwargs.get("type")
+        self.has_children: bool = kwargs.get("has_children")
+        self.archived: bool = kwargs.get("archived")
+        self.children = LinkTo(block=self)
+        self._level = kwargs["level"] if kwargs.get("level") else 0
+        self.create_mode: bool = kwargs["create_mode"] if "create_mode" in kwargs else False
+        self.parent = None
+        self._plain_text = ""
+
+        if self.create_mode:
+            self.text = kwargs[self.type]
+            if "checked" in kwargs:
+                self.checked = kwargs["checked"]
+            if "language" in kwargs:
+                self.language = kwargs["language"]
+            if "caption" in kwargs:
+                self.caption = kwargs["caption"]
+                if isinstance(self.caption, str):
+                    self.caption = RichTextArray.create(self.caption)
+            if "is_toggleable" in kwargs:
+                self.is_toggleable = kwargs["is_toggleable"]
+            return
+        self.parent = kwargs["parent"] if isinstance(kwargs.get("parent"), LinkTo) else LinkTo(**kwargs["parent"])
+
+        if self.type == "paragraph":
+            self.text = RichTextArray(kwargs[self.type].get("rich_text"))
+            self._plain_text = self.text.simple
+
+        elif "heading" in self.type:
+            indent = self.type.split("_")[-1]
+            indent_num = int(indent) if indent.isdigit() else 0
+            prefix = "#" * indent_num + " "
+            r_text = RichTextArray(kwargs[self.type].get("rich_text"))
+            self.text = RichTextArray.create(prefix) + r_text
+            self._plain_text = r_text.simple
+            self.is_toggleable: bool = kwargs[self.type].get("is_toggleable")
+
+        elif self.type == "callout":
+            self.text = RichTextArray(kwargs[self.type].get("rich_text"))
+            self._plain_text = self.text.simple
+            self.icon: Dict = kwargs[self.type].get("icon")
+
+        elif self.type == "quote":
+            r_text = RichTextArray(kwargs[self.type].get("rich_text"))
+            self.text = RichTextArray.create("| ") + r_text
+            self._plain_text = r_text.simple
+
+        elif "list_item" in self.type:
+            r_text = RichTextArray(kwargs[self.type].get("rich_text"))
+            self.text = RichTextArray.create("- ") + r_text
+            self._plain_text = r_text.simple
+            # Numbers does not support cause of lack of relativity
+
+        elif self.type == "to_do":
+            self.checked: bool = kwargs[self.type].get("checked")
+            prefix = "[x] " if self.checked else "[ ] "
+            r_text = RichTextArray(kwargs[self.type].get("rich_text"))
+            self.text = RichTextArray.create(prefix) + r_text
+            self._plain_text = r_text.simple
+
+        elif self.type == "toggle":
+            r_text = RichTextArray(kwargs[self.type].get("rich_text"))
+            self.text = RichTextArray.create("> ") + r_text
+            self._plain_text = r_text.simple
+
+        elif self.type == "code":
+            r_text = RichTextArray(kwargs[self.type].get("rich_text"))
+            self.language: str = kwargs[self.type].get("language")
+            prefix = RichTextArray.create(f"```{self.language}\n") if self.language else RichTextArray.create("```\n")
+            self.text = prefix + r_text + "\n```"
+            self._plain_text = r_text.simple
+            self.caption = RichTextArray(kwargs[self.type].get("caption"))
+
+        # when the block is child_page, parent will be the page object
+        # when the block is child_database, parent AND children will be the database object
+        elif "child" in self.type:
+            self.text: str = kwargs[self.type].get("title")
+            self._plain_text = str(self.text)
+            if self.type == "child_page":
+                # self.children is already set
+                self.parent = LinkTo(type="page", page=self.id)
+                self._plain_text = str(self.parent.link)
+            elif self.type == "child_database":
+                # well yes. parent and children are the same. parent of this database will be the page of this block
+                # and the database is children of this block
+                self.parent = LinkTo.create(database_id=self.id)
+                self.children = LinkTo.create(database_id=self.id)
+                self._plain_text = str(self.parent.link)
+                if not self.text:
+                    self.text = repr(self.children)
+            # page self.has_children is correct. checked.
+            # database self.has_children is false.
+            # database with custom source had no title!
+
+        # hello, markdown
+        elif self.type == "embed":
+            self.caption = RichTextArray(kwargs[self.type].get("caption"))
+            text = kwargs[self.type].get("url")
+            self._plain_text = str(text)
+            if self.caption:
+                self.text = f'[{self.caption}]({text})'
+            else:
+                self.text = f'<{text}>' if text else "*Empty embed*"
+
+        elif self.type == "image":
+            self.caption = RichTextArray(kwargs[self.type].get("caption"))
+            subtype = kwargs[self.type].get("type")
+            if subtype == "file":
+                # The file S3 URL will be valid for 1 hour
+                self.expiry_time = Model.format_iso_time(kwargs[self.type][subtype].get("expiry_time"))
+            else:
+                self.expiry_time = None
+            if subtype in ("file", "external"):
+                text = kwargs[self.type][subtype].get("url")
+                self._plain_text = str(text)
+                if self.caption:
+                    self.text = f'[{self.caption}]({text})'
+                else:
+                    self.text = f'<{text}>'
+            else:
+                self.text = "*Unknown image type*"
+                self._plain_text = "None"
+
+        elif self.type == "video":
+            self.caption = RichTextArray(kwargs[self.type].get("caption"))
+            subtype = kwargs[self.type].get("type")
+            if subtype == "file":
+                self.expiry_time = Model.format_iso_time(kwargs[self.type][subtype].get("expiry_time"))
+            else:
+                self.expiry_time = None
+            if subtype in ("file", "external"):
+                text = kwargs[self.type][subtype].get("url")
+                self._plain_text = str(text)
+                if self.caption:
+                    self.text = f'[{self.caption}]({text})'
+                else:
+                    self.text = f'<{text}>'
+            else:
+                self.text = "*Unknown video type*"
+                self._plain_text = "None"
+
+        elif self.type == "file":
+            self.caption = RichTextArray(kwargs[self.type].get("caption"))
+            subtype = kwargs[self.type].get("type")
+            if subtype == "file":
+                self.expiry_time = Model.format_iso_time(kwargs[self.type][subtype].get("expiry_time"))
+            else:
+                self.expiry_time = None
+            if subtype in ("file", "external"):
+                text = kwargs[self.type][subtype].get("url")
+                self._plain_text = str(text)
+                if self.caption:
+                    self.text = f'[{self.caption}]({text})'
+                else:
+                    self.text = f'<{text}>'
+            else:
+                self.text = "*Unknown file type*"
+                self._plain_text = "None"
+
+        elif self.type == "pdf":
+            self.caption = RichTextArray(kwargs[self.type].get("caption"))
+            subtype = kwargs[self.type].get("type")
+            if subtype == "file":
+                self.expiry_time = Model.format_iso_time(kwargs[self.type][subtype].get("expiry_time"))
+            else:
+                self.expiry_time = None
+            if subtype in ("file", "external"):
+                text = kwargs[self.type][subtype].get("url")
+                self._plain_text = str(text)
+                if self.caption:
+                    self.text = f'[{self.caption}]({text})'
+                else:
+                    self.text = f'<{text}>'
+            else:
+                self.text = "*Unknown pdf type*"
+                self._plain_text = "None"
+
+        elif self.type == "breadcrumb":
+            self.text = "*breadcrumb block*"
+            self._plain_text = "None"
+
+        elif self.type == "bookmark":
+            self.caption = RichTextArray(kwargs[self.type].get("caption"))
+            text = kwargs[self.type].get("url")
+            self._plain_text = str(text)
+            if self.caption:
+                self.text = f'[{self.caption}]({text})'
+            else:
+                self.text = f'<{text}>' if text else "*Empty bookmark*"
+
+        elif self.type == "link_preview":
+            text = kwargs[self.type].get("url")
+            self._plain_text = str(text)
+            self.text = f'<{text}>'
+
+        elif self.type == "link_to_page":
+            self.link = LinkTo(**kwargs[self.type])
+            self.text = repr(self.link)
+            self._plain_text = str(self.link.link)
+
+        elif self.type == "equation":
+            self.text: str = kwargs[self.type].get("expression")
+            self._plain_text = str(self.text)
+
+        elif self.type == "divider":
+            self.text = "---"
+            self._plain_text = "None"
+
+        elif self.type == "table_of_contents":
+            self.text = "*Table of contents*"
+            self._plain_text = "None"
+
+        elif self.type == "template":
+            r_text = RichTextArray(kwargs[self.type].get("rich_text"))
+            self.text = RichTextArray.create("Template: ") + r_text
+            self._plain_text = r_text.simple
+
+        elif self.type == "synced_block":
+            synced_from = kwargs[self.type].get("synced_from")
+            self.text = "*SYNCED BLOCK:*"
+            self._plain_text = "None"
+            self.synced_from = LinkTo(**synced_from) if synced_from else None
+
+        elif self.type == "table":
+            self.table_width: int = kwargs[self.type].get("table_width")
+            self.text = f"*Table {self.table_width}xN:*"
+            self._plain_text = "None"
+
+        elif self.type == "table_row":
+            cells = kwargs[self.type].get("cells")
+            self.text = RichTextArray.create("| ")
+            for cell in cells:
+                text_cell = RichTextArray(cell)
+                self._plain_text += f"\"{text_cell}\","
+                self.text += text_cell + " | "
+            self._plain_text = self._plain_text.strip(",")
+
+        elif self.type == "unsupported":
+            self.text = "*****"
+            self._plain_text = "None"
+
+        else:
+            self.text = "*UNKNOWN_BLOCK_TYPE*"
+            self._plain_text = "None"
+
+    def __str__(self):
+        return str(self.text)
+
+    def __repr__(self):
+        return f"Block({str(self.text)[:30]})"
+
+    def get(self, with_object_type: bool = False):
+        if self.type in [
+            "paragraph", "quote", "heading_1", "heading_2", "heading_3", "to_do",
+            "bulleted_list_item", "numbered_list_item", "toggle", "callout", "code", "child_database"
+        ]:
+
+            text = RichTextArray.create(self.text) if isinstance(self.text, str) else self.text
+
+            # base content
+            new_dict = {self.type: {"rich_text": text.get()}}
+
+            # to_do type attrs
+            if self.type == "to_do" and hasattr(self, "checked"):
+                new_dict[self.type]["checked"] = self.checked
+
+            # code type attrs
+            elif self.type == "code":
+                new_dict[self.type]["language"] = getattr(self, "language", "plain text")
+                if hasattr(self, "caption"):
+                    new_dict[self.type]["caption"] = self.caption.get()
+
+            # child_database type struct
+            elif self.type == "child_database":
+                new_dict = {self.type: {"title": str(text)}}
+
+            # heading_X types attrs
+            elif "heading" in self.type:
+                if hasattr(self, "is_toggleable") and isinstance(self.is_toggleable, bool):
+                    new_dict[self.type]["is_toggleable"] = self.is_toggleable
+                else:
+                    new_dict[self.type]["is_toggleable"] = False
+
+            if with_object_type:
+                new_dict["object"] = "block"
+                new_dict["type"] = self.type
+            return new_dict
+        return None
+
+    @property
+    def simple(self) -> str:
+        if self._plain_text:
+            return self._plain_text if self._plain_text != "None" else ""
+        if getattr(self, "text", None):
+            return str(self.text)
+        return self._plain_text
+
+    @classmethod
+    def create(cls, text: str, type_: str = "paragraph", **kwargs):
+        """
+        :param text:   Block content
+        :param type_:  Block types (API)
+        :param kwargs:
+            :kwargs param checked:          bool for to_do
+            :kwargs param language:         str for code
+            :kwargs param caption:          str or RichTextArray for code
+            :kwargs param is_toggleable:    bool for heading_1, heading_2, heading_3
+        :return:
+        """
+        new_dict = {
+            "type": type_,
+            type_: text,
+        }
+        return cls(**new_dict, create_mode=True, **kwargs)
+
+
+class ElementArray(MutableSequence):
+    class_map = {"page": Page, "database": Database, "block": Block}
+
+    def __init__(self, array, create: bool = False):
+        if create:
+            self.array = array
+            return
+
+        self.array = []
+        for ele in array:
+            if ele.get("object") and ele["object"] in self.class_map:
+                self.array.append(self.class_map[ele["object"]](**ele))
+
+    def __getitem__(self, item):
+        return self.array[item]
+
+    def __setitem__(self, key, value):
+        self.array[key] = value
+
+    def __delitem__(self, key):
+        del self.array[key]
+
+    def __len__(self):
+        return len(self.array)
+
+    def insert(self, index: int, value) -> None:
+        self.array.insert(index, value)
+
+    def __str__(self):
+        return "\n".join(str(b) for b in self)
+
+    def __repr__(self):
+        r = str(self)[:30].replace("\n", " ")
+        return f"ElementArray({r})"
+
+
+class BlockArray(ElementArray):
+    def __str__(self):
+        return "\n".join(b._level * "\t" + str(b) for b in self)
+
+    def __repr__(self):
+        r = str(self)[:30].replace("\n", " ")
+        return f"BlockArray({r})"
+
+    def get(self):
+        return [b.get() for b in self]
+
+    @property
+    def simple(self) -> str:
+        return "\n".join(b._level * "\t" + b.simple for b in self)
+
+
+class PageArray(ElementArray):
+    def __repr__(self):
+        r = str(self)[:30].replace("\n", " ")
+        return f"PageArray({r})"
+
+
+class LinkTo(object):
+    """
+    schema
+    .type = `element_type`
+    .id = `elementID`
+
+    .get() - return API like style
+    .create() - create in format `(page_id="123412341234")` or (database_id="13412341234")`
+    """
+
+    def __init__(
+            self, block: Optional[Model] = None, from_object: Union[Block, Page, Database, None] = None, **kwargs
+    ):
+        """
+        Creates LinkTo object from API dict
+
+        :param block: Block object can be provided instead other attrs. Internal usage.
+        :param from_object: Any model object can be provided to create LinkTo to it.
+        :param kwargs: API attrs. Internal usage.
+        """
+        if block:
+            self.type = block.object
+            self.id = block.id
+            self.after_path = "children"
+            self.uri = "blocks"
+        # You can provide the object to create the LinkTo to it
+        elif from_object:
+            self.uri = from_object.path
+            self.id = from_object.id
+            if isinstance(from_object, Page):
+                self.type = "page_id"
+            elif isinstance(from_object, Database):
+                self.type = "database_id"
+            elif isinstance(from_object, Block):
+                self.type = "block_id"
+            elif isinstance(from_object, User):
+                self.type = "user_id"
+        else:
+            self.type: str = kwargs.get("type")
+            self.id: str = kwargs.get(self.type) if kwargs.get(self.type) else kwargs.get("id")
+            if self.type == "workspace":
+                self.id = ""
+            self.after_path = ""
+            if self.type == "page_id":
+                self.uri = "pages"
+            elif self.type == "database_id":
+                self.uri = "databases"
+            # when type is set manually
+            elif self.type == "page":  # deprecated.
+                self.uri = "pages"
+            elif self.type == "block_id":
+                self.uri = "blocks"
+            elif self.type == "user_id":
+                self.uri = "users"
+            else:
+                self.uri = None
+
+        if isinstance(self.id, str):
+            self.id = self.id.replace("-", "")
+
+    def __str__(self):
+        prefix = self.uri if self.uri else self.type
+        if getattr(self, "after_path", ""):
+            return f"{prefix}/{self.id}/{self.after_path}"
+        return f"{prefix}/{self.id}"
+
+    def __repr__(self):
+        return f"LinkTo({self})"
+
+    @property
+    def link(self) -> str:
+        return NOTION_URL + str(self)
+
+    def get(self, without_type: bool = False):
+        if self.type == "workspace":
+            return {"type": "workspace", "workspace": True}
+        if without_type:
+            return {self.type: self.id}
+        return {"type": self.type, self.type: self.id}
+
+    @classmethod
+    def create(cls, **kwargs):
+        """
+        `.create(page_id="123412341234")`
+        `.create(database_id="13412341234")`
+        `.create(workspace=True)`
+        """
+        for key, value in kwargs.items():
+            return cls(type=key, id=value)
```

### Comparing `pytion-1.3.3/pytion/query.py` & `pytion-1.3.4/pytion/query.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,259 +1,259 @@
-# -*- coding: utf-8 -*-
-
-import logging
-from urllib.parse import urlencode
-from typing import Dict, Optional, Any, Union
-from datetime import datetime
-
-import requests
-
-import pytion.envs as envs
-from pytion.models import Property, PropertyValue, User
-from pytion.exceptions import find_response_error
-
-
-logger = logging.getLogger(__name__)
-
-
-class Filter(object):
-    _filter_condition_types = [
-        "rich_text", "number", "checkbox", "select", "multi_select", "date", "phone_number", "people", "title",
-        "created_time", "last_edited_time", "phone_number", "status"
-    ]
-
-    def __init__(
-            self,
-            property_name: Optional[str] = None,
-            value: Optional[Any] = None,
-            property_type: Optional[str] = None,
-            condition: Optional[str] = None,
-            raw: Optional[Dict] = None,
-            property_obj: Optional[Union[Property, PropertyValue]] = None,
-            **kwargs,
-    ):
-        if raw:
-            self.filter = raw
-            return
-        if property_obj:
-            if property_obj.id:
-                self.property_name = property_obj.id
-            else:
-                self.property_name = property_obj.name
-            if property_obj.type in ["title", "rich_text", "url", "email"]:
-                self.property_type = "rich_text"
-            elif "time" in property_obj.type:
-                self.property_type = "date"
-            else:
-                self.property_type = property_obj.type
-        else:
-            self.property_type = property_type
-            self.property_name = property_name
-
-        if self.property_type not in self._filter_condition_types:
-            raise ValueError(f"Allowed types {self.allowed_condition_types} ({property_type} is provided)")
-
-        if self.property_type == "rich_text":
-            self.condition = "contains" if not condition else condition
-            self.value = str(value)
-        elif self.property_type == "number":
-            self.condition = "equals" if not condition else condition
-            if "." in value:
-                self.value = float(value)
-            else:
-                self.value = int(value)
-        elif self.property_type == "checkbox":
-            self.condition = "equals" if not condition else condition
-            self.value = bool(value) if value else True
-        elif self.property_type == "select":
-            self.condition = "equals" if not condition else condition
-            self.value = str(value)
-        elif self.property_type == "multi_select":
-            self.condition = "contains" if not condition else condition
-            self.value = value[0] if isinstance(value, list) else str(value)
-        elif self.property_type == "phone_number":
-            self.condition = "contains" if not condition else condition
-            self.value = str(value)
-        elif self.property_type == "people":
-            self.condition = "contains" if not condition else condition
-            if isinstance(value, User):
-                self.value = value.id
-            else:
-                self.value = str(value)
-        elif self.property_type == "title":
-            self.condition = "contains" if not condition else condition
-            self.value = str(value)
-        elif self.property_type == "date" or "_time" in self.property_type:
-            self.condition = "equals" if not condition else condition
-            if isinstance(value, datetime):
-                if not value.hour and not value.minute:
-                    self.value = str(value.date())
-                else:
-                    self.value = value.isoformat()
-            else:
-                self.value = str(value)
-        elif self.property_type == "status":
-            self.condition = "equals" if not condition else condition
-            self.value = str(value)
-
-        if property_obj and not value:
-            self.value = getattr(property_obj, "value", None)
-            if isinstance(self.value, list):
-                self.value = self.value[0]
-        if self.condition in ["is_empty", "is_not_empty"]:
-            self.value = True
-        elif self.condition in [
-            "past_week", "past_month", "past_year", "next_week", "next_month", "next_year", "this_week"
-        ]:
-            self.value = {}
-        self.filter = {
-            "property": self.property_name,
-            self.property_type: {self.condition: self.value}
-        }
-
-    @property
-    def allowed_condition_types(self):
-        return ", ".join(self._filter_condition_types)
-
-    def __repr__(self):
-        if not getattr(self, "property_type"):
-            return f"Filter({str(self.filter)})"
-        return f"Filter({self.property_name} {self.condition} {self.value})"
-
-
-class Sort(object):
-    directions = ["ascending", "descending"]
-
-    def __init__(self, property_name: str, direction: str = "ascending"):
-        """
-        Sort object is used while querying database or search query:
-        - self.sort object is used in search query (only single item supported by API)
-        - self.sorts can contain multiple criteria and is used in database query
-        """
-        if direction not in self.directions:
-            raise ValueError(f"Allowed types {self.directions} ({direction} is provided)")
-        if property_name in ("created_time", "last_edited_time"):
-            self.sort = {"timestamp": property_name, "direction": direction}
-            self.sorts = [self.sort]
-        else:
-            self.sort = {"property": property_name, "direction": direction}
-            self.sorts = [self.sort]
-
-    def add(self, property_name: str, direction: str):
-        if direction not in self.directions:
-            raise ValueError(f"Allowed types {self.directions} ({direction} is provided)")
-        self.sort = {"property": property_name, "direction": direction}
-        self.sorts.append(self.sort)
-
-    def __repr__(self):
-        r = [e.values() for e in self.sorts]
-        return f"Sorts({r})"
-
-
-class Request(object):
-    def __init__(
-            self,
-            api: object,  # Notion object
-            method: Optional[str] = None,
-            path: Optional[str] = None,
-            id_: str = "",
-            data: Optional[Dict] = None,
-            base: Optional[str] = None,
-            token: Optional[str] = None,
-            after_path: Optional[str] = None,
-            limit: int = 0,
-            filter_: Optional[Filter] = None,
-            sorts: Optional[Sort] = None,
-    ):
-        self.session = requests.Session()
-        self.session.headers["accept"] = "application/json"
-        self.base = base if base else envs.NOTION_URL
-        self._token = token if token else envs.NOTION_SECRET
-        if not self._token:
-            logger.error("Token is not provided or file `token` is not found!")
-        self.version = getattr(api, "version")
-        self.auth = {"Authorization": "Bearer " + self._token}
-        self.session.headers.update({"Notion-Version": self.version, **self.auth})
-        self.result = None
-
-        if method:
-            self.result = self.method(method, path, id_, data, after_path, limit, filter_, sorts)
-
-    def method(
-            self, method: str, path: str, id_: str = "", data: Optional[Dict] = None,
-            after_path: Optional[str] = None, limit: int = 0, filter_: Optional[Filter] = None,
-            sorts: Optional[Sort] = None, pagination_loop: bool = False, sort: Optional[Sort] = None,
-    ):
-        if filter_:
-            if data:
-                data["filter"] = filter_.filter
-            else:
-                data = {"filter": filter_.filter}
-        if sorts:
-            if data:
-                data["sorts"] = sorts.sorts
-            else:
-                data = {"sorts": sorts.sorts}
-        if sort:  # specific attr in 'search' query. strange
-            if data:
-                data["sort"] = sort.sort
-            else:
-                data = {"sort": sort.sort}
-        url = self.base + path + "/" + id_
-        if limit and method == "get":
-            if after_path:
-                after_path += "?" + urlencode({"page_size": limit})
-            else:
-                path += "?" + urlencode({"page_size": limit})
-        if limit and method == "post":
-            if not data:
-                data = {}
-            data.update({"page_size": limit})
-        if after_path:
-            url += "/" + after_path
-        logger.info(f"Request {method} {url}")
-        logger.debug(f"METHOD: {method.upper()}")
-        logger.debug(f"URL: {url}")
-        logger.debug(f"DATA: {data}")
-        result = self.session.request(method=method, url=url, json=data)
-        logger.debug(f"STATUS CODE: {result.status_code}")
-        logger.debug(f"CONTENT: {result.content}")
-        logger.info(f"{result.status_code} Received")
-
-        r = find_response_error(result)
-
-        # pagination section
-        if not limit and not pagination_loop:
-            self.paginate(r, method, path, id_, data, after_path)
-
-        return r
-
-    def paginate(self, result, method, path, id_, data, after_path):
-        if (result.get("has_more", False) is True) and (result.get("object", "") == "list"):
-            next_start = result.get("next_cursor")
-            logger.info(f"Paginated answer. Repeat with offset {next_start}")
-
-            super_after_path = after_path
-            super_path = path
-
-            while next_start:
-                # if GET method then parameters are in request string
-                # if POST method then parameters are in body
-                if method == "get":
-                    if after_path:
-                        super_after_path = after_path + "?" + urlencode({"start_cursor": next_start})
-                    else:
-                        super_path = path + "?" + urlencode({"start_cursor": next_start})
-                elif method == "post":
-                    if not data:
-                        data = {}
-                    data.update({"start_cursor": next_start})
-
-                r = self.method(method, super_path, id_, data, super_after_path, pagination_loop=True)
-                if r.get("object", "") == "list" and r.get("results"):
-                    result["results"].extend(r["results"])
-                if r.get("has_more"):
-                    next_start = r.get("next_cursor")
-                else:
-                    next_start = None
-                result["has_more"] = r.get("has_more")
-                result["next_cursor"] = r.get("next_cursor")
+# -*- coding: utf-8 -*-
+
+import logging
+from urllib.parse import urlencode
+from typing import Dict, Optional, Any, Union
+from datetime import datetime
+
+import requests
+
+import pytion.envs as envs
+from pytion.models import Property, PropertyValue, User
+from pytion.exceptions import find_response_error
+
+
+logger = logging.getLogger(__name__)
+
+
+class Filter(object):
+    _filter_condition_types = [
+        "rich_text", "number", "checkbox", "select", "multi_select", "date", "phone_number", "people", "title",
+        "created_time", "last_edited_time", "phone_number", "status"
+    ]
+
+    def __init__(
+            self,
+            property_name: Optional[str] = None,
+            value: Optional[Any] = None,
+            property_type: Optional[str] = None,
+            condition: Optional[str] = None,
+            raw: Optional[Dict] = None,
+            property_obj: Optional[Union[Property, PropertyValue]] = None,
+            **kwargs,
+    ):
+        if raw:
+            self.filter = raw
+            return
+        if property_obj:
+            if property_obj.id:
+                self.property_name = property_obj.id
+            else:
+                self.property_name = property_obj.name
+            if property_obj.type in ["title", "rich_text", "url", "email"]:
+                self.property_type = "rich_text"
+            elif "time" in property_obj.type:
+                self.property_type = "date"
+            else:
+                self.property_type = property_obj.type
+        else:
+            self.property_type = property_type
+            self.property_name = property_name
+
+        if self.property_type not in self._filter_condition_types:
+            raise ValueError(f"Allowed types {self.allowed_condition_types} ({property_type} is provided)")
+
+        if self.property_type == "rich_text":
+            self.condition = "contains" if not condition else condition
+            self.value = str(value)
+        elif self.property_type == "number":
+            self.condition = "equals" if not condition else condition
+            if "." in value:
+                self.value = float(value)
+            else:
+                self.value = int(value)
+        elif self.property_type == "checkbox":
+            self.condition = "equals" if not condition else condition
+            self.value = bool(value) if value else True
+        elif self.property_type == "select":
+            self.condition = "equals" if not condition else condition
+            self.value = str(value)
+        elif self.property_type == "multi_select":
+            self.condition = "contains" if not condition else condition
+            self.value = value[0] if isinstance(value, list) else str(value)
+        elif self.property_type == "phone_number":
+            self.condition = "contains" if not condition else condition
+            self.value = str(value)
+        elif self.property_type == "people":
+            self.condition = "contains" if not condition else condition
+            if isinstance(value, User):
+                self.value = value.id
+            else:
+                self.value = str(value)
+        elif self.property_type == "title":
+            self.condition = "contains" if not condition else condition
+            self.value = str(value)
+        elif self.property_type == "date" or "_time" in self.property_type:
+            self.condition = "equals" if not condition else condition
+            if isinstance(value, datetime):
+                if not value.hour and not value.minute:
+                    self.value = str(value.date())
+                else:
+                    self.value = value.isoformat()
+            else:
+                self.value = str(value)
+        elif self.property_type == "status":
+            self.condition = "equals" if not condition else condition
+            self.value = str(value)
+
+        if property_obj and not value:
+            self.value = getattr(property_obj, "value", None)
+            if isinstance(self.value, list):
+                self.value = self.value[0]
+        if self.condition in ["is_empty", "is_not_empty"]:
+            self.value = True
+        elif self.condition in [
+            "past_week", "past_month", "past_year", "next_week", "next_month", "next_year", "this_week"
+        ]:
+            self.value = {}
+        self.filter = {
+            "property": self.property_name,
+            self.property_type: {self.condition: self.value}
+        }
+
+    @property
+    def allowed_condition_types(self):
+        return ", ".join(self._filter_condition_types)
+
+    def __repr__(self):
+        if not getattr(self, "property_type"):
+            return f"Filter({str(self.filter)})"
+        return f"Filter({self.property_name} {self.condition} {self.value})"
+
+
+class Sort(object):
+    directions = ["ascending", "descending"]
+
+    def __init__(self, property_name: str, direction: str = "ascending"):
+        """
+        Sort object is used while querying database or search query:
+        - self.sort object is used in search query (only single item supported by API)
+        - self.sorts can contain multiple criteria and is used in database query
+        """
+        if direction not in self.directions:
+            raise ValueError(f"Allowed types {self.directions} ({direction} is provided)")
+        if property_name in ("created_time", "last_edited_time"):
+            self.sort = {"timestamp": property_name, "direction": direction}
+            self.sorts = [self.sort]
+        else:
+            self.sort = {"property": property_name, "direction": direction}
+            self.sorts = [self.sort]
+
+    def add(self, property_name: str, direction: str):
+        if direction not in self.directions:
+            raise ValueError(f"Allowed types {self.directions} ({direction} is provided)")
+        self.sort = {"property": property_name, "direction": direction}
+        self.sorts.append(self.sort)
+
+    def __repr__(self):
+        r = [e.values() for e in self.sorts]
+        return f"Sorts({r})"
+
+
+class Request(object):
+    def __init__(
+            self,
+            api: object,  # Notion object
+            method: Optional[str] = None,
+            path: Optional[str] = None,
+            id_: str = "",
+            data: Optional[Dict] = None,
+            base: Optional[str] = None,
+            token: Optional[str] = None,
+            after_path: Optional[str] = None,
+            limit: int = 0,
+            filter_: Optional[Filter] = None,
+            sorts: Optional[Sort] = None,
+    ):
+        self.session = requests.Session()
+        self.session.headers["accept"] = "application/json"
+        self.base = base if base else envs.NOTION_URL
+        self._token = token if token else envs.NOTION_SECRET
+        if not self._token:
+            logger.error("Token is not provided or file `token` is not found!")
+        self.version = getattr(api, "version")
+        self.auth = {"Authorization": "Bearer " + self._token}
+        self.session.headers.update({"Notion-Version": self.version, **self.auth})
+        self.result = None
+
+        if method:
+            self.result = self.method(method, path, id_, data, after_path, limit, filter_, sorts)
+
+    def method(
+            self, method: str, path: str, id_: str = "", data: Optional[Dict] = None,
+            after_path: Optional[str] = None, limit: int = 0, filter_: Optional[Filter] = None,
+            sorts: Optional[Sort] = None, pagination_loop: bool = False, sort: Optional[Sort] = None,
+    ):
+        if filter_:
+            if data:
+                data["filter"] = filter_.filter
+            else:
+                data = {"filter": filter_.filter}
+        if sorts:
+            if data:
+                data["sorts"] = sorts.sorts
+            else:
+                data = {"sorts": sorts.sorts}
+        if sort:  # specific attr in 'search' query. strange
+            if data:
+                data["sort"] = sort.sort
+            else:
+                data = {"sort": sort.sort}
+        url = self.base + path + "/" + id_
+        if limit and method == "get":
+            if after_path:
+                after_path += "?" + urlencode({"page_size": limit})
+            else:
+                path += "?" + urlencode({"page_size": limit})
+        if limit and method == "post":
+            if not data:
+                data = {}
+            data.update({"page_size": limit})
+        if after_path:
+            url += "/" + after_path
+        logger.info(f"Request {method} {url}")
+        logger.debug(f"METHOD: {method.upper()}")
+        logger.debug(f"URL: {url}")
+        logger.debug(f"DATA: {data}")
+        result = self.session.request(method=method, url=url, json=data)
+        logger.debug(f"STATUS CODE: {result.status_code}")
+        logger.debug(f"CONTENT: {result.content}")
+        logger.info(f"{result.status_code} Received")
+
+        r = find_response_error(result)
+
+        # pagination section
+        if not limit and not pagination_loop:
+            self.paginate(r, method, path, id_, data, after_path)
+
+        return r
+
+    def paginate(self, result, method, path, id_, data, after_path):
+        if (result.get("has_more", False) is True) and (result.get("object", "") == "list"):
+            next_start = result.get("next_cursor")
+            logger.info(f"Paginated answer. Repeat with offset {next_start}")
+
+            super_after_path = after_path
+            super_path = path
+
+            while next_start:
+                # if GET method then parameters are in request string
+                # if POST method then parameters are in body
+                if method == "get":
+                    if after_path:
+                        super_after_path = after_path + "?" + urlencode({"start_cursor": next_start})
+                    else:
+                        super_path = path + "?" + urlencode({"start_cursor": next_start})
+                elif method == "post":
+                    if not data:
+                        data = {}
+                    data.update({"start_cursor": next_start})
+
+                r = self.method(method, super_path, id_, data, super_after_path, pagination_loop=True)
+                if r.get("object", "") == "list" and r.get("results"):
+                    result["results"].extend(r["results"])
+                if r.get("has_more"):
+                    next_start = r.get("next_cursor")
+                else:
+                    next_start = None
+                result["has_more"] = r.get("has_more")
+                result["next_cursor"] = r.get("next_cursor")
```

### Comparing `pytion-1.3.3/pytion.egg-info/PKG-INFO` & `pytion-1.3.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,482 +1,560 @@
-Metadata-Version: 2.1
-Name: pytion
-Version: 1.3.3
-Summary: Unofficial Python client for official Notion API
-Home-page: https://github.com/lastorel/pytion
-Author: Yegor Gomzin
-Author-email: slezycmex@mail.ru
-Project-URL: Bug Tracker, https://github.com/lastorel/pytion/issues
-Project-URL: Changelog, https://github.com/lastorel/pytion/blob/main/CHANGELOG.md
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pytion
-
-[![PyPI](https://img.shields.io/pypi/v/pytion.svg)](https://pypi.org/project/pytion)
-![PyVersion](https://img.shields.io/pypi/pyversions/pytion)
-![CodeSize](https://img.shields.io/github/languages/code-size/lastorel/pytion)
-[![LICENSE](https://img.shields.io/github/license/lastorel/pytion)](LICENSE)
-
-Independent unofficial **Python client** for the official **Notion API** (for internal integrations only)
-
-Client is built with its own object model based on API
-
-So if you are using **notion.so** and want to automate some stuff with the original API, you're welcome!  
-You can read any available data, create basic models, and even work with databases.
-
-Current Notion API version = **"2022-06-28"**
-
-_*does not use notion-sdk-py client_
-
-See [Change Log](./CHANGELOG.md)
-
-# Contents
-
-1. [Quick Start](#quick-start)
-2. [Pytion API](#pytion-api)
-   1. [Searching](#search)
-   2. [pytion.api.Element](#pytionapielement)
-3. [Models](#models)
-   1. [pytion.models](#pytionmodels)
-   2. [Supported Property types](#supported-property-types)
-   3. [Supported block types](#supported-block-types)
-      1. [Block creating examples](#block-creating-examples)
-      2. [Block deleting](#block-deleting)
-   4. [Database operations](#database-operations)
-      1. [Retrieving](#retrieving)
-4. [Logging](#logging)
-
-# Quick start
-
-```
-pip install pytion
-```
-
-Create new integration and get your Notion API Token at notion.so -> [here](https://www.notion.com/my-integrations).  
-Invite your new integration 'manager' to your pages or databases.
-
-```python
-from pytion import Notion; no = Notion(token=SOME_TOKEN)
-```
-
-Or put your token for Notion API into file `token` at script directory and use simple `no = Notion()`
-
-```python
-from pytion import Notion
-no = Notion(token=SOME_TOKEN)
-page = no.pages.get("PAGE ID")  # retrieve page data (not content) and create object
-blocks = page.get_block_children()  # retrieve page content and create list of objects
-database = no.databases.get("Database ID")  # retrieve database data (not content) and create object
-# retrieve database content by filtering with sorting
-pages = database.db_filter(property_name="Done", property_type="checkbox", value=False, descending="title")
-```
-
-```
-In [1]: from pytion import Notion
-
-In [2]: no = Notion(token=SOME_TOKEN)
-
-In [3]: page = no.pages.get("a458613160da45fa96367c8a594297c7")
-In [4]: print(page)
-Notion/pages/Page(Example page)
-
-In [5]: blocks = page.get_block_children_recursive()
-
-In [6]: print(blocks)
-Notion/blocks/BlockArray(## Migration planning [x] Rese)
-
-In [7]: print(blocks.obj)
-## Migration planning
-[x] Reset new switch 2022-05-12T00:00:00.000+03:00 → 2022-05-13T01:00:00.000+03:00 
-	- reboot
-	- hold reset button
-[x] Connect to console with baud rate 9600
-[ ] Skip default configuration dialog
-Use LinkTo(configs) 
-[Integration changes](https://developers.notion.com/changelog?page=2)
-
-In [8]: print(blocks.obj.simple)
-Migration planning
-Reset new switch 2022-05-12T00:00:00.000+03:00 → 2022-05-13T01:00:00.000+03:00 
-	reboot
-	hold reset button
-Connect to console with baud rate 9600
-Skip default configuration dialog
-Use https://api.notion.com/v1/pages/90ea1231865f4af28055b855c2fba267 
-https://developers.notion.com/changelog?page=2
-```
-
-# Pytion API
-
-Almost all operations are carried out through `Notion` or `Element` object:
-
-```python
-page = no.pages.get("a458613160da45fa96367c8a594297c7")
-
-# no -> Notion
-# pages -> URI in https://api.notion.com/v1/PAGES/a458613160da45fa96367c8a594297c7
-# get -> pytion API method
-# page -> Element
-# page.obj -> Page (main data structure)
-```
-
-so:
-
-- `isinstance(no, Notion) == True`
-- `isinstance(no.pages, Element) == True`
-- `isinstance(no.databases, Element) == True`
-- `isinstance(page, Element) == True`
-- `isinstance(page.obj, Page) == True`
-
-and if you want to retrieve a database - you must use _"databases"_ URI
-
-```python
-database = no.databases.get("123412341234")
-```
-
-and the same applies for _"blocks"_ and _"users"_. Valid URI-s are:
-
-- _pages_
-- _blocks_
-- _databases_
-- _users_
-
-When you work with existing `Element` object like `page` above, all [methods](#pytionapielement) below will be applied to this Page:
-
-```python
-new_page = page.page_update(title="new page name 2")
-
-# new_page is not a new page, it is updated page
-# new_page.obj is equal page.obj except title and last_edited properties
-```
-
-## Search
-
-There is a search example:
-```python
-no = Notion(token)
-
-r = no.search("updating", object_type="page")
-print(r.obj)
-# output:
-# Page for updating
-# Page to updating databases
-```
-
-
-## pytion.api.Element
-
-There is a list of available methods for communicate with **api.notion.com**. These methods are better structured in [next chapter](#pytionmodels).
-
-`.get(id_)` - Get Element by ID.
-
-`.get_parent(id_)` - Get parent object of current object if possible.
-
-`.get_block_children(id_, limit)` - Get children Block objects of current Block object (tabulated texts) if exist.
-
-`.get_block_children_recursive(id_, max_depth, limit, force)` - Get children Block objects of current Block object (tabulated texts) if exist recursive.
-
-`.get_page_property(property_id, id_, limit)` - Retrieve a page property item.
-
-`.get_page_properties(title_only, obj)` - Retrieve the title or all properties of current Page or Page `obj`
-*(deprecated, useful for v1.3.0 only)*
-
-`.db_query(id_, limit, filter_, sorts)` - Query Database.
-
-`.db_filter(...see desc...)` - Query Database.
-
-`.db_create(database_obj, parent, properties, title)` - Create Database.
-
-**_There is no way to delete a database object yet!_**
-
-`.db_update(id_, title, properties)` - Update Database.
-
-`.page_create(page_obj, parent, properties, title)` - Create Page.
-
-`.page_update(id_, properties, title, archived)` - Update Page.
-
-`.block_update(id_, block_obj, new_text, archived)` - Update text in Block.
-
-`.block_append(id_, block, blocks)` - Append block or blocks children.
-
-`.get_myself()` - Retrieve my bot User.
-
-`.from_linkto(linkto)` - Creates new Element object based on LinkTo information.
-
-`.from_object(model)` - Creates new Element object from Page, Block or Database object. Usable while Element object contains an Array.
-
-> More details and usage examples of these methods you can see into func descriptions.
-
-# Models
-
-### pytion.models
-
-There are classes **based on API** structures:
-
-- `RichText` based on [Rich text object](https://developers.notion.com/reference/rich-text)
-- `RichTextArray` is a list of RichText objects with useful methods
-  - You can create object by simple `RichTextArray.create("My title text")` and then use it in any methods
-  - Any Rich Text getting from API will be RichTextArray
-  - `str()` returns plain text of all "Rich Texts". ez
-  - `+` operator is available with `str` and `RichTextArray`
-  - `.simple` property returns stripped plain text without any markdown syntax. useful for URL
-- `Database` based on [Database object](https://developers.notion.com/reference/database)
-  - You can create object `Database.create(...)` and/or use `.db_create(...)` API method
-  - attrs represent API model. Complex structures like `created_by` are wrapped in internal objects
-  - use `.db_update()` API method for modify a real database (for ex. properties or title)
-  - use `.db_query()` to get all database content (it will be `PageArray`)
-  - use `.db_filter()` to get database content with filtering and/or sorting
-  - has `.description` attr
-  - has `.is_inline` attr with the value True if the database appears in the page as an inline block
-- `Page` based on [Page object](https://developers.notion.com/reference/page)
-  - You can create object `Page.create(...)` and/or use `.page_create(...)` API method
-  - use `.page_update()` method to modify attributes or delete the page
-  - use `.get_block_children()` to get page content (without nested blocks) (it will be `BlockArray`)
-  - use `.get_block_children_recursive()` to get page content with nested blocks
-  - use `.get_page_property()` to retrieve the specific `PropertyValue` of the page
-- `Block` based on [Block object](https://developers.notion.com/reference/block)
-  - You can create object `Block.create(...)` of specific type from [_support matrix_](#supported-block-types) below and then use it while creating pages or appending
-  - use `.block_update()` to replace content or change _extension attributes_ or delete the block
-  - use `.block_append()` to add a new block to a page or add a nested block to another block
-  - use `.get_block_children()` to get first level nested blocks
-  - use `.get_block_children_recursive()` to get all levels nested blocks
-- `User` based on [User object](https://developers.notion.com/reference/user)
-  - You can create object `User.create(...)` and use it in some properties like `people` type property
-  - You can retrieve more data about a User by his ID using `.get()`
-  - use `.get_myself()` to retrieve the current bot User
-  - has `.workspace_name` attr for `bot` type users
-- `Property` based on [Property object](https://developers.notion.com/reference/property-object)
-  - You can create object `Property.create(...)` while creating or editing database: `.db_create()` or `.db_update()`
-  - `formula`, `rollup` type properties configuration is not supported
-- `PropertyValue` based on [Property values](https://developers.notion.com/reference/property-value-object)
-  - You can create object `PropertyValue.create(...)` to set or edit page properties by `.page_create()` or `.page_update()`
-  - `files`, `formula`, `rollup` type properties are not editable
-
-There are also useful **internal** classes:
-
-- `BlockArray` is found when API returns page content in "list of blocks" format
-  - it is useful to represent all content by `str()`
-  - also it has `simple` property like `RichTextArray` object
-  - it automatically indents `str` output of nested blocks
-- `PageArray` is found when API returns the result of database query (list of pages)
-- `LinkTo` is basic internal model to link to any Notion object
-  - You can create object `LinkTo.create()` and use it in many places and methods
-  - use `LinkTo(from_object=my_page1)` to quickly create a link to any existing object of pytion.models
-  - `link` property of `LinkTo` returns expanded URL
-- `ElementArray` is found while using `.search()` endpoint. It's a parent of `PageArray`
-
-> And every model has a `.get()` method that returns API friendly JSON.
- 
-### Supported Property types
-
-| Property type            | value type          | read (DB) | read value (Page) | create (DB) | create value (Page) | Oper attrs                          | Config attrs                        |
-|--------------------------|---------------------|-----------|-------------------|-------------|---------------------|-------------------------------------|-------------------------------------|
-| `title`                  | `RichTextArray`     | +         | +                 | +           | +                   |                                     |                                     |
-| `rich_text`              | `RichTextArray`     | +         | +                 | +           | +                   |                                     |                                     |
-| `number`                 | `int`/`float`       | +         | +                 | +           | +                   |                                     | ~~format~~                          |
-| `select`                 | `str`               | +         | +                 | +           | +                   |                                     | ~~options~~                         |
-| `multi_select`           | `List[str]`         | +         | +                 | +           | +                   |                                     | ~~options~~                         |
-| `status`                 | `str`               | +         | +                 | +           | +\*\*\*\*           |                                     | `options`, `groups` (read-only)     |
-| `date`                   | `str`               | +         | +                 | +           | +                   | `start: datetime` `end: datetime`\* |                                     |
-| `people`                 | `List[User]`        | +         | +                 | +           | +\*\*               |                                     |                                     |
-| `files`                  |                     | +         | -                 | +           | -                   |                                     |                                     |
-| `checkbox`               | `bool`              | +         | +                 | +           | +                   |                                     |                                     |
-| `url`                    | `str`               | +         | +                 | +           | +                   |                                     |                                     |
-| `email`                  | `str`               | +         | +                 | +           | +                   |                                     |                                     |
-| `phone_number`           | `str`               | +         | +                 | +           | +                   |                                     |                                     |
-| `formula`                |                     | -         | +                 | -           | -                   |                                     |                                     |
-| `relation`               | `List[LinkTo]`      | +         | +                 | +           | +                   | `has_more: bool`                    | `single_property` / `dual_property` |
-| `rollup`                 | depends on relation | -         | +                 | -           | -                   |                                     |                                     |
-| `created_time`\*\*\*     | `datetime`          | +         | +                 | +           | -                   |                                     |                                     |
-| `created_by`\*\*\*       | `User`              | +         | +                 | +           | -                   |                                     |                                     |
-| `last_edited_time`\*\*\* | `datetime`          | +         | +                 | +           | -                   |                                     |                                     |
-| `last_edited_by`\*\*\*   | `User`              | +         | +                 | +           | -                   |                                     |                                     |
-
-> [\*] - Create examples:  
-> `pv = PropertyValue.create(type_="date", value=datetime.now())`  
-> `pv = PropertyValue.create(type_="date", date={"start": str(datetime(2022, 2, 1, 5)), "end": str(datetime.now())})`  
-> [\*\*] - Create example:  
-> `user = User.create('1d393ffb5efd4d09adfc2cb6738e4812')`  
-> `pv = PropertyValue.create(type_="people", value=[user])`  
-> [\*\*\*] - Every Base model like Page already has mandatory attributes created/last_edited returned by API  
-> [\*\*\*\*] - Status type is not configurable. API doesn't support NEW options added via Property modify or updating a Page
-
-
-## Supported block types
-
-At present the API only supports the block types which are listed in the reference below. Any unsupported block types will continue to appear in the structure, but only contain a `type` set to `"unsupported"`.
-Colors are not yet supported.
-
-Every Block has mandatory attributes and extension attributes. There are mandatory:
-
-- `id: str` - UUID-64 without hyphens
-- `object: str` - always `"block"` (from API)
-- `created_time: datetime` - from API
-- `created_by: User` - from API
-- `last_edited_time: datetime` - from API
-- `last_edited_by: User` - from API
-- `type: str` - the type of block (from API)
-- `has_children: bool` - does the block have children blocks (from API)
-- `archived: bool` - does the block marked as deleted (from API)
-- `text: Union[str, RichTextArray]` - **main content**
-- `simple: str` - only simple text string (url expanded)
-
-Extension attributes are listed below in support matrix:
-
-| Block Type           | Description                               | Read support | Create support | Can have children | Extension attributes                              |
-|----------------------|-------------------------------------------|--------------|----------------|-------------------|---------------------------------------------------|
-| `paragraph`          | Simple Block with text                    | +            | +              | +                 |                                                   |
-| `heading_1`          | Heading Block with text highest level     | +            | +              | -/+\*             | `is_toggleable: bool`                             |
-| `heading_2`          | Heading Block with text medium level      | +            | +              | -/+\*             | `is_toggleable: bool`                             |
-| `heading_3`          | Heading Block with text lowest level      | +            | +              | -/+\*             | `is_toggleable: bool`                             |
-| `bulleted_list_item` | Text Block with bullet                    | +            | -              | +                 |                                                   |
-| `numbered_list_item` | Text Block with number                    | +            | -              | +                 |                                                   |
-| `to_do`              | Text Block with checkbox                  | +            | +              | +                 | `checked: bool`                                   |
-| `toggle`             | Text Block with toggle to children blocks | +            | -              | +                 |                                                   |
-| `code`               | Text Block with code style                | +            | +              | +                 | `language: str`, `caption: RichTextArray`         |
-| `child_page`         | Page inside                               | +            | -              | +                 |                                                   |
-| `child_database`     | Database inside                           | +            | -              | +                 |                                                   |
-| `embed`              | Embed online content                      | +            | -              | -                 | `caption: RichTextArray`                          |
-| `image`              | Embed image content                       | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
-| `video`              | Embed video content                       | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
-| `file`               | Embed file content                        | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
-| `pdf`                | Embed pdf content                         | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
-| `bookmark`           | Block for URL Link                        | +            | -              | -                 | `caption: RichTextArray`                          |
-| `callout`            | Highlighted footnote text Block           | +            | -              | +                 | `icon: dict`                                      |
-| `quote`              | Text Block with quote style               | +            | -              | +                 |                                                   |
-| `equation`           | KaTeX compatible text Block               | +            | -              | -                 |                                                   |
-| `divider`            | Simple line to divide the page            | +            | -              | -                 |                                                   |
-| `table_of_contents`  | Block with content structure in the page  | +            | -              | -                 |                                                   |
-| `column`             |                                           | -            | -              | +                 |                                                   |
-| `column_list`        |                                           | -            | -              | -                 |                                                   |
-| `link_preview`       | Same as `bookmark`                        | +            | -              | -                 |                                                   |
-| `synced_block`       | Block for synced content aka parent       | +            | -              | +                 | `synced_from: LinkTo`                             |
-| `template`           | Template Block title                      | +            | -              | +                 |                                                   |
-| `link_to_page`       | Block with link to particular page `@...` | +            | -              | -                 | `link: LinkTo`                                    |
-| `table`              | Table Block with some attrs               | +            | -              | +                 | `table_width: int`                                |
-| `table_row`          | Children Blocks with table row content    | +            | -              | -                 |                                                   |
-| `breadcrumb`         | Empty Block actually                      | +            | -              | -                 |                                                   |
-| `unsupported`        | Blocks unsupported by API                 | +            | -              | -                 |                                                   |
-
-> [\*] - `heading_X` blocks can have children if `is_toggleable` is True 
-
-### Block creating examples
-
-Create `paragraph` block object and add it to Notion:
-
-```python
-from pytion.models import Block
-my_text_block = Block.create("Hello World!")
-my_text_block = Block.create(text="Hello World!", type_="paragraph")  # the same
-
-# indented append my block to other known block:
-no.blocks.block_append("5f60073a9dda4a9c93a212a74a107359", block=my_text_block)
-
-# append my block to a known page (in the end)
-no.blocks.block_append("9796f2525016128d9af4bf12b236b555", block=my_text_block)  # the same operation actually
-
-# another way to append:
-my_page = no.pages.get("9796f2525016128d9af4bf12b236b555")
-my_page.block_append(block=my_text_block)
-```
-
-Create `to_do` block object:
-
-```python
-from pytion.models import Block
-my_todo_block = Block.create("create readme documentation", type_="to_do")
-my_todo_block2 = Block.create("add 'create' method", type_="to_do", checked=True)
-```
-
-Create `code` block object:
-
-```python
-from pytion.models import Block
-my_code_block = Block.create("code example here", type_="code", language="javascript")
-my_code_block2 = Block.create("another code example", type_="code", caption="it will be plain text code block with caption")
-```
-
-Create `heading` block object:
-
-```python
-from pytion.models import Block
-my_code_block = Block.create("Title 1 example here", type_="heading_1")
-my_code_block2 = Block.create("Toggle Title 2", type_="heading_2", is_toggleable=True)
-```
-
-### Block deleting
-
-```python
-no.blocks.block_update("3d4af9f0f98641dea8c44e3864eed4d0", archived=True)
-# or if you have Element with Block object already
-block.block_update(archived=True)
-```
-
-## Database operations
-
-### Retrieving
-
-```python
-from pytion import Notion
-no = Notion(token=TOKEN)
-
-# get all pages from Database
-# example 1
-pages = no.databases.db_query("114f1ef1f1241e2f12f41fe2f")
-# example 2
-db = no.databases.get("114f1ef1f1241e2f12f41fe2f")
-pages = db.db_query()
-print(pages.obj)
-
-# get pages with "task" in title
-pages = db.db_filter("task")
-
-# get all pages with sorting by property name "Tags"
-pages = db.db_filter("", ascending="Tags")
-pages = db.db_filter("", descending="Tags")
-
-# get pages with Status property equals Done
-pages = db.db_filter(property_name="Status", property_type="status", value="Done")
-
-# get pages with Price property greater than 150
-pages = db.db_filter(property_name="Price", property_type="number", condition="greater_than", value=150)
-
-# complex query
-pages = db.db_filter(
-    property_name="WorkTime", property_type="date", condition="before",
-    value=datetime.now(), descending="Deadline", limit=25
-)
-```
-
-> Queries with multifiltering and multisorting are not supported  
-> But you can compose your custom filter dict from API reference and call `db.db_filter(raw={...})` 
-
-Filter conditions and types combination -> [Official API reference](https://developers.notion.com/reference/post-database-query-filter)
-
-After you got `pages` which is `Element` object, you can not call API methods directly on `pages`
-because there is `PageArray` object with List of Pages.
-If you need to change a Page or something else, you can follow these steps:
-
-```python
-# 1. create new Element object with non-list object type
-page = no.pages.from_object(pages.obj[14])  # choosed page from the PageArray
-# 2. call the desired API method on this page
-page.page_update(archived=True)  # delete Page example
-```
-
-# Logging
-
-Logging is muted by default. To enable to stdout and/or to file:
-
-```python
-from pytion import setup_logging
-
-setup_logging(level="debug", to_console=True, filename="pytion.log")
-```
+# pytion
+
+[![PyPI](https://img.shields.io/pypi/v/pytion.svg)](https://pypi.org/project/pytion)
+![PyVersion](https://img.shields.io/pypi/pyversions/pytion)
+![CodeSize](https://img.shields.io/github/languages/code-size/lastorel/pytion)
+[![LICENSE](https://img.shields.io/github/license/lastorel/pytion)](LICENSE)
+
+Independent unofficial **Python client** for the official **Notion API** (for internal integrations only)
+
+Client is built with its own object model based on API
+
+So if you are using **notion.so** and want to automate some stuff with the original API, you're welcome!  
+You can read any available data, create basic models, and even work with databases.
+
+Current Notion API version = **"2022-06-28"**
+
+_*does not use notion-sdk-py client_
+
+See [Change Log](./CHANGELOG.md)
+
+# Contents
+
+1. [Quick Start](#quick-start)
+2. [Pytion API](#pytion-api)
+   1. [Searching](#search)
+   2. [pytion.api.Element](#pytionapielement)
+3. [Models](#models)
+   1. [pytion.models](#pytionmodels)
+   2. [Supported Property types](#supported-property-types)
+   3. [Supported block types](#supported-block-types)
+      1. [Block creating examples](#block-creating-examples)
+      2. [Block deleting](#block-deleting)
+   4. [Database operations](#database-operations)
+      1. [Retrieving](#retrieving)
+      2. [Appending (creating a Page)](#appending-creating-a-page)
+      3. [Property Values](#property-values)
+4. [Logging](#logging)
+
+# Quick start
+
+```
+pip install pytion
+```
+
+Create new integration and get your Notion API Token at notion.so -> [here](https://www.notion.com/my-integrations).  
+Add your new integration 'manager' to your pages or databases by going to the page's menu (three dots), at the bottom of the menu clicking on Add connections and then searching for you new Integration.
+
+```python
+from pytion import Notion; no = Notion(token=SOME_TOKEN)
+```
+
+Or put your token for Notion API into file `token` at script directory and use simple `no = Notion()`
+
+```python
+from pytion import Notion
+no = Notion(token=SOME_TOKEN)
+page = no.pages.get("PAGE ID")  # retrieve page data (not content) and create object
+blocks = page.get_block_children()  # retrieve page content and create list of objects
+database = no.databases.get("Database ID")  # retrieve database data (not content) and create object
+# retrieve database content by filtering with sorting
+pages = database.db_filter(property_name="Done", property_type="checkbox", value=False, descending="title")
+```
+
+```
+In [1]: from pytion import Notion
+
+In [2]: no = Notion(token=SOME_TOKEN)
+
+In [3]: page = no.pages.get("a458613160da45fa96367c8a594297c7")
+In [4]: print(page)
+Notion/pages/Page(Example page)
+
+In [5]: blocks = page.get_block_children_recursive()
+
+In [6]: print(blocks)
+Notion/blocks/BlockArray(## Migration planning [x] Rese)
+
+In [7]: print(blocks.obj)
+## Migration planning
+[x] Reset new switch 2022-05-12T00:00:00.000+03:00 → 2022-05-13T01:00:00.000+03:00 
+	- reboot
+	- hold reset button
+[x] Connect to console with baud rate 9600
+[ ] Skip default configuration dialog
+Use LinkTo(configs) 
+[Integration changes](https://developers.notion.com/changelog?page=2)
+
+In [8]: print(blocks.obj.simple)
+Migration planning
+Reset new switch 2022-05-12T00:00:00.000+03:00 → 2022-05-13T01:00:00.000+03:00 
+	reboot
+	hold reset button
+Connect to console with baud rate 9600
+Skip default configuration dialog
+Use https://api.notion.com/v1/pages/90ea1231865f4af28055b855c2fba267 
+https://developers.notion.com/changelog?page=2
+```
+
+# Pytion API
+
+Almost all operations are carried out through `Notion` or `Element` object:
+
+```python
+page = no.pages.get("a458613160da45fa96367c8a594297c7")
+
+# no -> Notion
+# pages -> URI in https://api.notion.com/v1/PAGES/a458613160da45fa96367c8a594297c7
+# get -> pytion API method
+# page -> Element
+# page.obj -> Page (main data structure)
+```
+
+so:
+
+- `isinstance(no, Notion) == True`
+- `isinstance(no.pages, Element) == True`
+- `isinstance(no.databases, Element) == True`
+- `isinstance(page, Element) == True`
+- `isinstance(page.obj, Page) == True`
+
+and if you want to retrieve a database - you must use _"databases"_ URI
+
+```python
+database = no.databases.get("123412341234")
+```
+
+and the same applies for _"blocks"_ and _"users"_. Valid URI-s are:
+
+- _pages_
+- _blocks_
+- _databases_
+- _users_
+
+When you work with existing `Element` object like `page` above, all [methods](#pytionapielement) below will be applied to this Page:
+
+```python
+new_page = page.page_update(title="new page name 2")
+
+# new_page is not a new page, it is updated page
+# new_page.obj is equal page.obj except title and last_edited properties
+```
+
+## Search
+
+There is a search example:
+```python
+no = Notion(token)
+
+r = no.search("updating", object_type="page")
+print(r.obj)
+# output:
+# Page for updating
+# Page to updating databases
+```
+
+
+## pytion.api.Element
+
+There is a list of available methods for communicate with **api.notion.com**. These methods are better structured in [next chapter](#pytionmodels).
+
+`.get(id_)` - Get Element by ID.
+
+`.get_parent(id_)` - Get parent object of current object if possible.
+
+`.get_block_children(id_, limit)` - Get children Block objects of current Block object (tabulated texts) if exist.
+
+`.get_block_children_recursive(id_, max_depth, limit, force)` - Get children Block objects of current Block object (tabulated texts) if exist recursive.
+
+`.get_page_property(property_id, id_, limit)` - Retrieve a page property item.
+
+`.get_page_properties(title_only, obj)` - Retrieve the title or all properties of current Page or Page `obj`
+*(deprecated, useful for v1.3.0 only)*
+
+`.db_query(id_, limit, filter_, sorts)` - Query Database.
+
+`.db_filter(...see desc...)` - Query Database.
+
+`.db_create(database_obj, parent, properties, title)` - Create Database.
+
+**_There is no way to delete a database object yet!_**
+
+`.db_update(id_, title, properties)` - Update Database.
+
+`.page_create(page_obj, parent, properties, title)` - Create Page.
+
+`.page_update(id_, properties, title, archived)` - Update Page.
+
+`.block_update(id_, block_obj, new_text, archived)` - Update text in Block.
+
+`.block_append(id_, block, blocks)` - Append block or blocks children.
+
+`.get_myself()` - Retrieve my bot User.
+
+`.from_linkto(linkto)` - Creates new Element object based on LinkTo information.
+
+`.from_object(model)` - Creates new Element object from Page, Block or Database object. Usable while Element object contains an Array.
+
+> More details and usage examples of these methods you can see into func descriptions.
+
+# Models
+
+### pytion.models
+
+There are classes **based on API** structures:
+
+- `RichText` based on [Rich text object](https://developers.notion.com/reference/rich-text)
+- `RichTextArray` is a list of RichText objects with useful methods
+  - You can create object by simple `RichTextArray.create("My title text")` and then use it in any methods
+  - Any Rich Text getting from API will be RichTextArray
+  - `str()` returns plain text of all "Rich Texts". ez
+  - `+` operator is available with `str` and `RichTextArray`
+  - `.simple` property returns stripped plain text without any markdown syntax. useful for URL
+- `Database` based on [Database object](https://developers.notion.com/reference/database)
+  - You can create object `Database.create(...)` and/or use `.db_create(...)` API method
+  - attrs represent API model. Complex structures like `created_by` are wrapped in internal objects
+  - use `.db_update()` API method for modify a real database (for ex. properties or title)
+  - use `.db_query()` to get all database content (it will be `PageArray`)
+  - use `.db_filter()` to get database content with filtering and/or sorting
+  - has `.description` attr
+  - has `.is_inline` attr with the value True if the database appears in the page as an inline block
+- `Page` based on [Page object](https://developers.notion.com/reference/page)
+  - You can create object `Page.create(...)` and/or use `.page_create(...)` API method
+  - use `.page_update()` method to modify attributes or delete the page
+  - use `.get_block_children()` to get page content (without nested blocks) (it will be `BlockArray`)
+  - use `.get_block_children_recursive()` to get page content with nested blocks
+  - use `.get_page_property()` to retrieve the specific `PropertyValue` of the page
+- `Block` based on [Block object](https://developers.notion.com/reference/block)
+  - You can create object `Block.create(...)` of specific type from [_support matrix_](#supported-block-types) below and then use it while creating pages or appending
+  - use `.block_update()` to replace content or change _extension attributes_ or delete the block
+  - use `.block_append()` to add a new block to a page or add a nested block to another block
+  - use `.get_block_children()` to get first level nested blocks
+  - use `.get_block_children_recursive()` to get all levels nested blocks
+- `User` based on [User object](https://developers.notion.com/reference/user)
+  - You can create object `User.create(...)` and use it in some properties like `people` type property
+  - You can retrieve more data about a User by his ID using `.get()`
+  - use `.get_myself()` to retrieve the current bot User
+  - has `.workspace_name` attr for `bot` type users
+- `Property` based on [Property object](https://developers.notion.com/reference/property-object)
+  - You can create object `Property.create(...)` while creating or editing database: `.db_create()` or `.db_update()`
+  - `formula` type properties configuration is not supported
+- `PropertyValue` based on [Property values](https://developers.notion.com/reference/property-value-object)
+  - You can create object `PropertyValue.create(...)` to set or edit page properties by `.page_create()` or `.page_update()`
+  - `files`, `formula`, `rollup` type properties are not editable
+
+There are also useful **internal** classes:
+
+- `BlockArray` is found when API returns page content in "list of blocks" format
+  - it is useful to represent all content by `str()`
+  - also it has `simple` property like `RichTextArray` object
+  - it automatically indents `str` output of nested blocks
+- `PageArray` is found when API returns the result of database query (list of pages)
+- `LinkTo` is basic internal model to link to any Notion object
+  - You can create object `LinkTo.create()` and use it in many places and methods
+  - use `LinkTo(from_object=my_page1)` to quickly create a link to any existing object of pytion.models
+  - `link` property of `LinkTo` returns expanded URL
+- `ElementArray` is found while using `.search()` endpoint. It's a parent of `PageArray`
+
+> And every model has a `.get()` method that returns API friendly JSON.
+ 
+### Supported Property types
+
+| Property type            | value type                       | read (DB) | read value (Page) | create (DB) | create value (Page) | Oper attrs                          | Config attrs                                                                                                 |
+|--------------------------|----------------------------------|-----------|-------------------|-------------|---------------------|-------------------------------------|--------------------------------------------------------------------------------------------------------------|
+| `title`                  | `RichTextArray`                  | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `rich_text`              | `RichTextArray`                  | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `number`                 | `int`/`float`                    | +         | +                 | +           | +                   |                                     | ~~format~~                                                                                                   |
+| `select`                 | `str`                            | +         | +                 | +           | +                   |                                     | ~~options~~                                                                                                  |
+| `multi_select`           | `List[str]`                      | +         | +                 | +           | +                   |                                     | ~~options~~                                                                                                  |
+| `status`                 | `str`                            | +         | +                 | +           | +\*\*\*\*           |                                     | `options`, `groups` (read-only)                                                                              |
+| `date`                   | `str`                            | +         | +                 | +           | +                   | `start: datetime` `end: datetime`\* |                                                                                                              |
+| `people`                 | `List[User]`                     | +         | +                 | +           | +\*\*               |                                     |                                                                                                              |
+| `files`                  |                                  | +         | -                 | +           | -                   |                                     |                                                                                                              |
+| `checkbox`               | `bool`                           | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `url`                    | `str`                            | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `email`                  | `str`                            | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `phone_number`           | `str`                            | +         | +                 | +           | +                   |                                     |                                                                                                              |
+| `formula`                |                                  | -         | +                 | -           | n/a                 |                                     |                                                                                                              |
+| `relation`               | `List[LinkTo]`                   | +         | +                 | +           | +                   | `has_more: bool`                    | `single_property` / `dual_property`                                                                          |
+| `rollup`                 | depends on relation and function | +         | +                 | +           | n/a                 | ~~has_more~~\*\*\*\*\*              | `function`, `relation_property_id` / `relation_property_name`, `rollup_property_id` / `rollup_property_name` |
+| `created_time`\*\*\*     | `datetime`                       | +         | +                 | +           | n/a                 |                                     |                                                                                                              |
+| `created_by`\*\*\*       | `User`                           | +         | +                 | +           | n/a                 |                                     |                                                                                                              |
+| `last_edited_time`\*\*\* | `datetime`                       | +         | +                 | +           | n/a                 |                                     |                                                                                                              |
+| `last_edited_by`\*\*\*   | `User`                           | +         | +                 | +           | n/a                 |                                     |                                                                                                              |
+
+> [\*] - Create examples:  
+> `pv = PropertyValue.create(type_="date", value=datetime.now())`  
+> `pv = PropertyValue.create(type_="date", date={"start": str(datetime(2022, 2, 1, 5)), "end": str(datetime.now())})`  
+> [\*\*] - Create example:  
+> `user = User.create('1d393ffb5efd4d09adfc2cb6738e4812')`  
+> `pv = PropertyValue.create(type_="people", value=[user])`  
+> [\*\*\*] - Every Base model like Page already has mandatory attributes created/last_edited returned by API  
+> [\*\*\*\*] - Status type is not configurable. API doesn't support NEW options added via Property modify or updating a Page
+> [\*\*\*\*\*] - Notion API hasn't `has_more` attr. Only 25 references can be shown in the array
+
+More details and examples can be found in Database [section](#property-values)
+
+More details and examples can be found in Database [section](#property-values)
+
+
+## Supported block types
+
+At present the API only supports the block types which are listed in the reference below. Any unsupported block types will continue to appear in the structure, but only contain a `type` set to `"unsupported"`.
+Colors are not yet supported.
+
+Every Block has mandatory attributes and extension attributes. There are mandatory:
+
+- `id: str` - UUID-64 without hyphens
+- `object: str` - always `"block"` (from API)
+- `created_time: datetime` - from API
+- `created_by: User` - from API
+- `last_edited_time: datetime` - from API
+- `last_edited_by: User` - from API
+- `type: str` - the type of block (from API)
+- `has_children: bool` - does the block have children blocks (from API)
+- `archived: bool` - does the block marked as deleted (from API)
+- `text: Union[str, RichTextArray]` - **main content**
+- `simple: str` - only simple text string (url expanded)
+
+Extension attributes are listed below in support matrix:
+
+| Block Type           | Description                               | Read support | Create support | Can have children | Extension attributes                              |
+|----------------------|-------------------------------------------|--------------|----------------|-------------------|---------------------------------------------------|
+| `paragraph`          | Simple Block with text                    | +            | +              | +                 |                                                   |
+| `heading_1`          | Heading Block with text highest level     | +            | +              | -/+\*             | `is_toggleable: bool`                             |
+| `heading_2`          | Heading Block with text medium level      | +            | +              | -/+\*             | `is_toggleable: bool`                             |
+| `heading_3`          | Heading Block with text lowest level      | +            | +              | -/+\*             | `is_toggleable: bool`                             |
+| `bulleted_list_item` | Text Block with bullet                    | +            | -              | +                 |                                                   |
+| `numbered_list_item` | Text Block with number                    | +            | -              | +                 |                                                   |
+| `to_do`              | Text Block with checkbox                  | +            | +              | +                 | `checked: bool`                                   |
+| `toggle`             | Text Block with toggle to children blocks | +            | -              | +                 |                                                   |
+| `code`               | Text Block with code style                | +            | +              | +                 | `language: str`, `caption: RichTextArray`         |
+| `child_page`         | Page inside                               | +            | -              | +                 |                                                   |
+| `child_database`     | Database inside                           | +            | -              | +                 |                                                   |
+| `embed`              | Embed online content                      | +            | -              | -                 | `caption: RichTextArray`                          |
+| `image`              | Embed image content                       | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
+| `video`              | Embed video content                       | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
+| `file`               | Embed file content                        | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
+| `pdf`                | Embed pdf content                         | +            | -              | -                 | `caption: RichTextArray`, `expiry_time: datetime` |
+| `bookmark`           | Block for URL Link                        | +            | -              | -                 | `caption: RichTextArray`                          |
+| `callout`            | Highlighted footnote text Block           | +            | -              | +                 | `icon: dict`                                      |
+| `quote`              | Text Block with quote style               | +            | -              | +                 |                                                   |
+| `equation`           | KaTeX compatible text Block               | +            | -              | -                 |                                                   |
+| `divider`            | Simple line to divide the page            | +            | -              | -                 |                                                   |
+| `table_of_contents`  | Block with content structure in the page  | +            | -              | -                 |                                                   |
+| `column`             |                                           | -            | -              | +                 |                                                   |
+| `column_list`        |                                           | -            | -              | -                 |                                                   |
+| `link_preview`       | Same as `bookmark`                        | +            | -              | -                 |                                                   |
+| `synced_block`       | Block for synced content aka parent       | +            | -              | +                 | `synced_from: LinkTo`                             |
+| `template`           | Template Block title                      | +            | -              | +                 |                                                   |
+| `link_to_page`       | Block with link to particular page `@...` | +            | -              | -                 | `link: LinkTo`                                    |
+| `table`              | Table Block with some attrs               | +            | -              | +                 | `table_width: int`                                |
+| `table_row`          | Children Blocks with table row content    | +            | -              | -                 |                                                   |
+| `breadcrumb`         | Empty Block actually                      | +            | -              | -                 |                                                   |
+| `unsupported`        | Blocks unsupported by API                 | +            | -              | -                 |                                                   |
+
+> [\*] - `heading_X` blocks can have children if `is_toggleable` is True 
+
+### Block creating examples
+
+Create `paragraph` block object and add it to Notion:
+
+```python
+from pytion.models import Block
+my_text_block = Block.create("Hello World!")
+my_text_block = Block.create(text="Hello World!", type_="paragraph")  # the same
+
+# indented append my block to other known block:
+no.blocks.block_append("5f60073a9dda4a9c93a212a74a107359", block=my_text_block)
+
+# append my block to a known page (in the end)
+no.blocks.block_append("9796f2525016128d9af4bf12b236b555", block=my_text_block)  # the same operation actually
+
+# another way to append:
+my_page = no.pages.get("9796f2525016128d9af4bf12b236b555")
+my_page.block_append(block=my_text_block)
+```
+
+Create `to_do` block object:
+
+```python
+from pytion.models import Block
+my_todo_block = Block.create("create readme documentation", type_="to_do")
+my_todo_block2 = Block.create("add 'create' method", type_="to_do", checked=True)
+```
+
+Create `code` block object:
+
+```python
+from pytion.models import Block
+my_code_block = Block.create("code example here", type_="code", language="javascript")
+my_code_block2 = Block.create("another code example", type_="code", caption="it will be plain text code block with caption")
+```
+
+Create `heading` block object:
+
+```python
+from pytion.models import Block
+my_code_block = Block.create("Title 1 example here", type_="heading_1")
+my_code_block2 = Block.create("Toggle Title 2", type_="heading_2", is_toggleable=True)
+```
+
+### Block deleting
+
+```python
+no.blocks.block_update("3d4af9f0f98641dea8c44e3864eed4d0", archived=True)
+# or if you have Element with Block object already
+block.block_update(archived=True)
+```
+
+## Database operations
+
+### Retrieving
+
+```python
+from pytion import Notion
+no = Notion(token=TOKEN)
+
+# get all pages from Database
+# example 1
+pages = no.databases.db_query("114f1ef1f1241e2f12f41fe2f")
+# example 2
+db = no.databases.get("114f1ef1f1241e2f12f41fe2f")
+pages = db.db_query()
+print(pages.obj)
+
+# get pages with "task" in title
+pages = db.db_filter("task")
+
+# get all pages with sorting by property name "Tags"
+pages = db.db_filter("", ascending="Tags")
+pages = db.db_filter("", descending="Tags")
+
+# get pages with Status property equals Done
+pages = db.db_filter(property_name="Status", property_type="status", value="Done")
+
+# get pages with Price property greater than 150
+pages = db.db_filter(property_name="Price", property_type="number", condition="greater_than", value=150)
+
+# complex query
+pages = db.db_filter(
+    property_name="WorkTime", property_type="date", condition="before",
+    value=datetime.now(), descending="Deadline", limit=25
+)
+```
+
+> Queries with multifiltering and multisorting are not supported  
+> But you can compose your custom filter dict from API reference and call `db.db_filter(raw={...})` 
+
+Filter conditions and types combination -> [Official API reference](https://developers.notion.com/reference/post-database-query-filter)
+
+After you got `pages` which is `Element` object, you can not call API methods directly on `pages`
+because there is `PageArray` object with List of Pages.
+If you need to change a Page or something else, you can follow these steps:
+
+```python
+# 1. create new Element object with non-list object type
+page = no.pages.from_object(pages.obj[14])  # choosed page from the PageArray
+# 2. call the desired API method on this page
+page.page_update(archived=True)  # delete Page example
+```
+
+### Appending (creating a Page)
+
+There is a way to create a row into database. The same method is used to create any Page.
+The difference is in only in `parent` argument which can be the Page or the Database.
+
+```python
+from pytion.models import LinkTo
+
+# choose the parent target
+# it can be the database
+parent = LinkTo.create(database_id="043cb52491a44b80a5e5006237a4278f")
+# or the page
+parent2 = LinkTo.create(page_id="043cb52491a44b80a5e5006237a4278f")
+
+# if you need to set Properties
+from pytion.models import PropertyValue
+props = {
+            "Tags": PropertyValue.create(type_="multi_select", value=["tag1", "tag2"]),
+            "done": PropertyValue.create("checkbox", True),
+            "AnotherPropertyNAME": PropertyValue.create("date", datetime.now()),
+        }
+
+# create the Page
+page = no.pages.page_create(parent=parent, title="Page 2")  # without properties (will be empty)
+# or
+page2 = no.pages.page_create(parent=parent, properties=props, title="Page 2")  # with properties
+```
+
+### Property Values
+
+Pytion Properties support table is described [above](#supported-property-types)
+
+There are Properties that are used in Database operations and PropertyValues that are used in Page operations.
+
+It's necessary to choose the type (`type_` arg) and value (`value`) of property.
+The table shows the mapping between Property type and value (python) type.
+
+The `type_` must correspond to your database schema in Notion.
+
+```python
+from datetime import datetime
+from pytion.models import PropertyValue, LinkTo, RichTextArray, User
+
+# + relation type:
+pv = PropertyValue.create("relation", value=[LinkTo.create(page_id="04262843082a478d97f741948a32613b")])
+# + people type:
+pv = PropertyValue.create(type_="people", value=[User.create('1d393ffb5efd4d09adfc2cb6738e4812')])
+# + date type:
+pv = PropertyValue.create(type_="date", value=datetime.now())
+pv = PropertyValue.create(type_="date", date={"start": str(datetime(2022, 2, 1, 5)), "end": str(datetime.now())})
+# + rich_text (text or title field)
+pv = PropertyValue.create(type_="rich_text", value="Something Interesting")
+pv = PropertyValue.create("rich_text", value=RichTextArray.create("Something Interesting"))
+# + nubmer
+pv = PropertyValue.create(type_="number", value=156.2)
+# + status
+pv = PropertyValue.create("status", value="Done")
+
+# update needed property values
+new_props = {
+    "Tags": PropertyValue.create("multi_select", ["tag2"]),
+    "done": PropertyValue.create("checkbox", False),
+    "when": PropertyValue.create("date", datetime.now()),
+}
+page = page_for_updates.page_update(properties=new_props)
+page = no.pages.page_update(page_for_updates_id, properties=new_props)  # the same
+
+# rename (edit title property)
+page = page_for_updates.page_update(title=new_name)
+```
+
+Pytion also provides the ways to change database schema - create/update/rename/delete properties:
+
+```python
+from pytion.models import Property
+
+# rename property
+properties = {"Name": Property.create(type_="title", name="Subject")}
+database = database_for_updates.db_update(properties=properties)
+database = no.databases.db_update(database_for_updates_id, properties=properties)  # the same
+# change property type
+properties = {"Tags": Property.create("select")}
+database = database_for_updates.db_update(properties=properties)
+# delete property from database
+properties = {"Old property name": Property.create(None)}
+database = database_for_updates.db_update(properties=properties)
+# rename database
+database = database_for_updates.db_update(title="Refactoring")
+```
+
+# Logging
+
+Logging is muted by default. To enable to stdout and/or to file:
+
+```python
+from pytion import setup_logging
+
+setup_logging(level="debug", to_console=True, filename="pytion.log")
+```
```

### Comparing `pytion-1.3.3/setup.py` & `pytion-1.3.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-import setuptools
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="pytion",
-    version="1.3.3",
-    author="Yegor Gomzin",
-    author_email="slezycmex@mail.ru",
-    description="Unofficial Python client for official Notion API",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/lastorel/pytion",
-    project_urls={
-        "Bug Tracker": "https://github.com/lastorel/pytion/issues",
-        "Changelog": "https://github.com/lastorel/pytion/blob/main/CHANGELOG.md",
-    },
-    classifiers=[
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Operating System :: OS Independent",
-    ],
-    packages=setuptools.find_packages(),
-    python_requires=">=3.7",
-    install_requires=[
-        "requests>=2.26.0"
-    ]
-)
+import setuptools
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="pytion",
+    version="1.3.4",
+    author="Yegor Gomzin",
+    author_email="slezycmex@mail.ru",
+    description="Unofficial Python client for official Notion API",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/lastorel/pytion",
+    project_urls={
+        "Bug Tracker": "https://github.com/lastorel/pytion/issues",
+        "Changelog": "https://github.com/lastorel/pytion/blob/main/CHANGELOG.md",
+    },
+    classifiers=[
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Operating System :: OS Independent",
+    ],
+    packages=setuptools.find_packages(),
+    python_requires=">=3.7",
+    install_requires=[
+        "requests>=2.26.0"
+    ]
+)
```

### Comparing `pytion-1.3.3/tests/test_api.py` & `pytion-1.3.4/tests/test_api.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,671 +1,671 @@
-from datetime import datetime
-
-import pytest
-
-from pytion.models import Page, Block, Database, User, RichTextArray, ElementArray
-from pytion.models import BlockArray, PropertyValue, PageArray, LinkTo, Property
-from pytion import InvalidRequestURL, ObjectNotFound, ValidationError
-
-
-def test_notion(no):
-    assert no.version == "2022-06-28"
-    assert no.session.base == "https://api.notion.com/v1/"
-
-
-def test_search__empty(no):
-    r = no.search("123412341234")
-    assert isinstance(r.obj, ElementArray)
-    assert len(r.obj) == 0
-
-
-def test_search__type_and_limit(no):
-    r = no.search(object_type="database", limit=4)
-    assert isinstance(r.obj, ElementArray)
-    assert len(r.obj) == 4
-    assert all(isinstance(item, Database) for item in r.obj)
-
-
-def test_search__query(no):
-    r = no.search("tests")
-    assert isinstance(r.obj, ElementArray)
-    assert len(r.obj) >= 1
-    assert str(r.obj[0]) == "Pytion Tests"
-
-
-class TestElement:
-    def test_get__page(self, root_page):
-        page = root_page
-        assert isinstance(page.obj, Page), "get of .pages. must return Page object"
-        assert page.obj.id == "878d628488d94894ab14f9b872cd6870"
-        assert str(page.obj.title) == "Pytion Tests"
-
-    def test_get__block(self, no):
-        block = no.blocks.get("878d628488d94894ab14f9b872cd6870")  # root page
-        assert isinstance(block.obj, Block)
-        assert block.obj.id == "878d628488d94894ab14f9b872cd6870"
-        assert block.obj.text == "Pytion Tests"
-
-    def test_get__database(self, no):
-        database = no.databases.get("0e9539099cff456d89e44684d6b6c701")  # Little Database
-        assert isinstance(database.obj, Database)
-        assert database.obj.id == "0e9539099cff456d89e44684d6b6c701"
-        assert str(database.obj.title) == "Little Database"
-        assert str(database.obj.description) == "Database has a super description! Don’t touch it!"
-        assert database.obj.is_inline is False
-
-    def test_get__user(self, no):
-        user = no.users.get("01c67faf3aba45ffaa022407f87c86a5")
-        assert isinstance(user.obj, User)
-        assert user.obj.id == "01c67faf3aba45ffaa022407f87c86a5"
-        assert user.obj.name == "Yegor Gomzin"
-
-    def test_get__bad_url(self, no):
-        with pytest.raises(InvalidRequestURL):
-            no.page.get("878d628488d94894ab14f9b872cd6870")  # root page
-
-    def test_get__bad_id(self, no):
-        with pytest.raises(ObjectNotFound):
-            no.pages.get("878d628488d94894ab14f9b872cd6872")  # random id
-
-    def test_get__after_path_page(self, no):
-        blocks = no.blocks.get("82ee5677402f44819a5da3302273400a", _after_path="children")  # Page with some texts
-        assert isinstance(blocks.obj, BlockArray)
-        assert len(blocks.obj) == 3
-        assert isinstance(blocks.obj[0], Block)
-        blocks = no.blocks.get("82ee5677402f44819a5da3302273400a", _after_path="children", limit=2)  # Page with some te
-        assert len(blocks.obj) == 2
-
-    def test_get__after_path_block(self, no):
-        blocks = no.blocks.get("8a920ba7dc1d4961811e5c82b28028ed", _after_path="children")  # Hello! How are you?
-        assert isinstance(blocks.obj, BlockArray)
-        assert len(blocks.obj) == 3
-        assert isinstance(blocks.obj[0], Block)
-
-    def test_get_parent__block(self, no):
-        parent_block = no.blocks.get_parent("9b2026c3a0cb45fc8cee330142d60f3a")  # I'm fine!
-        assert isinstance(parent_block.obj, Block)
-        assert parent_block.obj.id == "8a920ba7dc1d4961811e5c82b28028ed"
-        assert str(parent_block.obj) == "Hello! How are you?"
-
-    def test_get_parent__block2(self, no):
-        parent_block = no.blocks.get_parent("8a920ba7dc1d4961811e5c82b28028ed")  # Hello! How are you?
-        assert isinstance(parent_block.obj, Page)
-        assert parent_block.obj.id == "82ee5677402f44819a5da3302273400a"
-        assert str(parent_block.obj) == "Page with some texts"
-
-    def test_get_parent__page(self, no):
-        parent_page_block = no.pages.get_parent("82ee5677402f44819a5da3302273400a")  # Page with some texts
-        assert isinstance(parent_page_block.obj, Block)
-        assert parent_page_block.obj.id == "6001eb5621f2428392d532bf08bc8ecd"
-        assert "Page with some texts" in str(parent_page_block.obj)
-
-    def test_get_parent__database(self, no, root_page):
-        parent_page_block = no.databases.get_parent("0e9539099cff456d89e44684d6b6c701")  # Little Database
-        assert isinstance(parent_page_block.obj, Page)
-        assert parent_page_block.obj.id == root_page.obj.id
-
-    def test_get_parent__user(self, no):
-        something = no.users.get_parent("01c67faf3aba45ffaa022407f87c86a5")
-        assert something is None, "User object has not any parent"
-
-    def test_get_parent__block_obj(self, no):
-        block = no.blocks.get("8a920ba7dc1d4961811e5c82b28028ed")  # Hello! How are you?
-        parent_block = block.get_parent()
-        assert isinstance(parent_block.obj, Page)
-        assert parent_block.obj.id == "82ee5677402f44819a5da3302273400a"
-        assert str(parent_block.obj) == "Page with some texts"
-
-    def test_get_parent__page_obj(self, no):  # Database is the parent of this page
-        page = no.pages.get("b85877eaf7bf4245a8c5218055eeb81f")  # Parent testing page
-        database = page.get_parent()
-        assert isinstance(database.obj, Database)
-        assert database.obj.id == "0e9539099cff456d89e44684d6b6c701"
-        assert str(database.obj.title) == "Little Database"
-
-    def test_get_parent__database_obj(self, little_database):
-        database = little_database  # Little Database
-        parent_page_block = database.get_parent()
-        assert isinstance(parent_page_block.obj, Page)
-        assert parent_page_block.obj.id == "878d628488d94894ab14f9b872cd6870"
-        assert str(parent_page_block.obj) == "Pytion Tests"
-
-    def test_get_parent__child_page(self, no):
-        child_page = no.blocks.get("878d628488d94894ab14f9b872cd6870")  # root page
-        page = child_page.get_parent()
-        assert isinstance(page.obj, Page)
-        assert page.obj.id == "878d628488d94894ab14f9b872cd6870"
-        assert str(page.obj.title) == "Pytion Tests"
-
-    def test_get_parent__child_database(self, no):
-        child_database = no.blocks.get("0e9539099cff456d89e44684d6b6c701")  # Little Database
-        database = child_database.get_parent()
-        assert isinstance(database.obj, Database)
-        assert database.obj.id == "0e9539099cff456d89e44684d6b6c701"
-        assert str(database.obj.title) == "Little Database"
-
-    def test_get_parent__workspace(self, root_page):
-        workspace = root_page.get_parent()
-        assert workspace is None
-
-    def test_get_block_children__page_id(self, no):
-        blocks = no.pages.get_block_children("82ee5677402f44819a5da3302273400a")  # Page with some texts
-        assert isinstance(blocks.obj, BlockArray)
-        assert len(blocks.obj) == 3
-        assert isinstance(blocks.obj[0], Block)
-
-    def test_get_block_children__page_obj(self, page_some_texts):
-        page = page_some_texts  # Page with some texts
-        blocks = page.get_block_children()
-        assert isinstance(blocks.obj, BlockArray)
-        assert len(blocks.obj) == 3
-        assert isinstance(blocks.obj[0], Block)
-
-    def test_get_block_children__block_id(self, no):
-        blocks = no.blocks.get_block_children("8a920ba7dc1d4961811e5c82b28028ed")  # Hello! How are you?
-        assert isinstance(blocks.obj, BlockArray)
-        assert len(blocks.obj) == 3
-        assert isinstance(blocks.obj[0], Block)
-
-    def test_get_block_children__block_obj(self, no):
-        block = no.blocks.get("8a920ba7dc1d4961811e5c82b28028ed")  # Hello! How are you?
-        blocks = block.get_block_children()
-        assert isinstance(blocks.obj, BlockArray)
-        assert len(blocks.obj) == 3
-        assert isinstance(blocks.obj[0], Block)
-
-    def test_get_block_children__database_id(self, no):
-        something = no.databases.get_block_children("0e9539099cff456d89e44684d6b6c701")  # Little Database
-        assert something is None, "Database has no children"
-
-    def test_get_block_children__database_obj(self, little_database):
-        database = little_database  # Little Database
-        something = database.get_block_children()
-        assert something is None, "Database has no children"
-
-    def test_get_block_children__child_database(self, no):
-        database_block = no.blocks.get("0e9539099cff456d89e44684d6b6c701")  # Little Database
-        database = database_block.get_block_children()
-        assert isinstance(database.obj, Database)
-        assert database.obj.id == "0e9539099cff456d89e44684d6b6c701"
-        assert str(database.obj.title) == "Little Database"
-
-    def test_get_block_children_recursive__page_id(self, no):
-        blocks = no.pages.get_block_children_recursive("82ee5677402f44819a5da3302273400a")  # Page with some texts
-        assert isinstance(blocks.obj, BlockArray)
-        assert len(blocks.obj) == 6
-        assert isinstance(blocks.obj[0], Block)
-
-    def test_get_block_children_recursive__page_obj(self, page_some_texts):
-        page = page_some_texts  # Page with some texts
-        blocks = page.get_block_children_recursive()
-        assert isinstance(blocks.obj, BlockArray)
-        assert len(blocks.obj) == 6
-        assert isinstance(blocks.obj[0], Block)
-
-    def test_get_block_children_recursive__block_id(self, no):
-        blocks = no.blocks.get_block_children_recursive("8a920ba7dc1d4961811e5c82b28028ed")  # Hello! How are you?
-        assert isinstance(blocks.obj, BlockArray)
-        assert len(blocks.obj) == 3
-        assert isinstance(blocks.obj[0], Block)
-
-    def test_get_block_children_recursive__block_obj(self, no):
-        block = no.blocks.get("8a920ba7dc1d4961811e5c82b28028ed")  # Hello! How are you?
-        blocks = block.get_block_children_recursive()
-        assert isinstance(blocks.obj, BlockArray)
-        assert len(blocks.obj) == 3
-        assert isinstance(blocks.obj[0], Block)
-
-    def test_get_block_children_recursive__database_id(self, no):
-        something = no.databases.get_block_children_recursive("0e9539099cff456d89e44684d6b6c701")  # Little Database
-        assert something is None, "Database has no children"
-
-    def test_get_block_children_recursive__database_obj(self, little_database):
-        database = little_database  # Little Database
-        something = database.get_block_children_recursive()
-        assert something is None, "Database has no children"
-
-    def test_get_block_children_recursive__child_database(self, no):
-        database_block = no.blocks.get("0e9539099cff456d89e44684d6b6c701")  # Little Database
-        database = database_block.get_block_children_recursive()
-        assert isinstance(database.obj, Database)
-        assert database.obj.id == "0e9539099cff456d89e44684d6b6c701"
-        assert str(database.obj.title) == "Little Database"
-
-    def test_get_block_children_recursive__force(self, no):
-        block = no.blocks.get("8a920ba7dc1d4961811e5c82b28028ed")  # Hello! How are you?
-        blocks = block.get_block_children_recursive(force=True)
-        assert isinstance(blocks.obj, BlockArray)
-        assert len(blocks.obj) == 5
-        assert isinstance(blocks.obj[0], Block)
-
-    def test_get_block_children_recursive__max_depth(self, page_some_texts):
-        page = page_some_texts  # Page with some texts
-        blocks = page.get_block_children_recursive(force=True, max_depth=2)
-        assert isinstance(blocks.obj, BlockArray)
-        assert len(blocks.obj) == 7
-        assert isinstance(blocks.obj[0], Block)
-
-    def test_get_page_property__page_id(self, no):
-        p = no.pages.get_page_property("%7Dma%3F", "b85877eaf7bf4245a8c5218055eeb81f")
-        assert isinstance(p.obj, PropertyValue)
-        assert len(p.obj.value) == 2
-        assert p.obj.type == "multi_select"
-
-    def test_get_page_property__page_obj(self, no):
-        page = no.pages.get("b85877eaf7bf4245a8c5218055eeb81f")
-        p = page.get_page_property("%7Dma%3F")
-        assert isinstance(p.obj, PropertyValue)
-        assert len(p.obj.value) == 2
-        assert p.obj.type == "multi_select"
-
-    def test_get_page_property__bad_id(self, no):
-        with pytest.raises(ValidationError):
-            no.pages.get_page_property("%7Dma%3A", "b85877eaf7bf4245a8c5218055eeb81f")
-
-    def test_get_page_property__bad_page(self, no):
-        with pytest.raises(ObjectNotFound):
-            no.pages.get_page_property("%7Dma%3F", "b85877eaf7bf4245a8c5218055eeb81a")
-
-    def test_get_page_properties(self, no):
-        page = no.pages.get("b85877eaf7bf4245a8c5218055eeb81f")  # Parent testing page
-        assert isinstance(page.obj, Page)
-        # assert str(page.obj) == "unknown"
-        # assert isinstance(page.obj.properties["Done"], Property)
-        page.get_page_properties()
-        assert isinstance(page.obj.properties["Done"], PropertyValue)
-        assert page.obj.properties["Digit"].value == 2
-        assert "tag1" in page.obj.properties["Tags"].value
-
-    def test_get_page_properties__title(self, no):
-        page = no.pages.get("b85877eaf7bf4245a8c5218055eeb81f")  # Parent testing page
-        assert isinstance(page.obj, Page)
-        # assert str(page.obj) == "unknown"
-        # assert isinstance(page.obj.properties["Done"], Property)
-        page.get_page_properties(title_only=True)
-        # assert hasattr(page.obj.properties["by"], "value") is False
-        # assert isinstance(page.obj.properties["Done"], Property)
-        assert str(page.obj.title) == "Parent testing page"
-
-    def test_db_query__id(self, no):
-        pages = no.databases.db_query("0e9539099cff456d89e44684d6b6c701")  # Little Database
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 4
-        assert str(pages.obj[0].title) == ""
-
-    def test_db_query__obj(self, little_database):
-        pages = little_database.db_query(limit=3)
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 3
-        assert str(pages.obj[0].title) == ""
-
-    def test_db_filter__title_ez(self, little_database):
-        pages = little_database.db_filter("testing page")
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 1
-        assert str(pages.obj[0].title) == "Parent testing page"
-
-    def test_db_filter__not_contain(self, little_database):
-        pages = little_database.db_filter("testing page", condition="does_not_contain")
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 3
-        assert str(pages.obj[0].title) == ""
-
-    def test_db_filter__ends_with(self, little_database):
-        pages = little_database.db_filter(
-            property_name="Name", property_type="title", value="what?", condition="ends_with"
-        )
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 1
-        assert str(pages.obj[0].title) == "wait, what?"
-
-    def test_db_filter__is_empty(self, little_database):
-        pages = little_database.db_filter(property_name="title", property_type="title", condition="is_empty")
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 1
-        assert str(pages.obj[0].title) == ""
-
-    def test_db_filter__greater_than(self, little_database):
-        pages = little_database.db_filter(
-            property_name="Digit", property_type="number", condition="greater_than", value="1"
-        )
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 2
-        assert str(pages.obj[0].title) == "We are best friends, body"
-
-    def test_db_filter__checkbox(self, little_database):
-        pages = little_database.db_filter(property_name="Done", property_type="checkbox")
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 1
-        assert str(pages.obj[0].title) == "We are best friends, body"
-
-    def test_db_filter__contains_tag(self, little_database):
-        pages = little_database.db_filter(
-            property_name="Tags", property_type="multi_select", value="tag1"
-        )
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 2
-        assert str(pages.obj[0].title) == ""
-
-    def test_db_filter__notcontains_tag(self, little_database):
-        pages = little_database.db_filter(
-            property_name="Tags", property_type="multi_select", value="tag2", condition="does_not_contain"
-        )
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 3
-        assert str(pages.obj[0].title) == ""
-
-    def test_db_filter__no_tags(self, little_database):
-        pages = little_database.db_filter(
-            property_name="Tags", property_type="multi_select", condition="is_empty"
-        )
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 1
-        assert str(pages.obj[0].title) == "wait, what?"
-
-    def test_db_filter__tag_property_obj(self, no, little_database):
-        page = no.pages.get("c2fc6b3dc3d244e9be2a3d28b26082bf")  # Untitled
-        my_prop = page.obj.properties["Tags"]
-        pages = little_database.db_filter(property_obj=my_prop)
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 2
-        assert str(pages.obj[0].title) == ""
-
-    def test_db_filter__without_filter(self, little_database):
-        pages = little_database.db_filter("")
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 4
-        assert str(pages.obj[0].title) == ""
-
-    def test_db_filter__date_after(self, little_database):
-        pages = little_database.db_filter(
-            property_name="created", property_type="date", condition="on_or_after", value="2022-04-22"
-        )
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 2
-        assert str(pages.obj[0].title) == ""
-
-    def test_db_filter__date_next_year(self, little_database):
-        pages = little_database.db_filter(
-            property_name="created", property_type="created_time", condition="next_year", value="2022-04-22"
-        )
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 0
-
-    def test_db_filter__date_this_week(self, little_database):
-        pages = little_database.db_filter(
-            property_name="created", property_type="created_time", condition="this_week"
-        )
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 0
-
-    def test_db_filter__status(self, little_database):
-        pages = little_database.db_filter(
-            property_name="Status", property_type="status", value="Done"
-        )
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 1
-        assert str(pages.obj[0].title) == "wait, what?"
-
-    def test_db_filter__sort_desc(self, little_database):
-        pages = little_database.db_filter("", descending="created")
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 4
-        assert str(pages.obj[0].title) == ""
-        assert str(pages.obj[2].title) == "We are best friends, body"
-
-    def test_db_filter__sort_asc(self, little_database):
-        pages = little_database.db_filter("", ascending="Digit")
-        assert isinstance(pages.obj, PageArray)
-        assert len(pages.obj) == 4
-        assert str(pages.obj[0].title) == "wait, what?"
-        assert str(pages.obj[2].title) == "We are best friends, body"
-
-    def test_db_create(self, no):
-        parent = LinkTo.create(page_id="2dff77eb43d44ce097ffb421499f82aa")  # Page for creating databases
-        properties = {
-            "Name": Property.create("title"),
-            "Digit": Property.create("number"),
-            "Status": Property.create("select"),
-        }
-        title = "DB 1"
-        description = "ABCDEF"
-        database = no.databases.db_create(parent=parent, properties=properties, title=title, description=description)
-        assert isinstance(database.obj, Database)
-        assert str(database.obj.title) == title
-        assert "Status" in database.obj.properties
-        assert str(database.obj.description) == description
-
-        # Delete database manually. There is no way to delete a database by API
-
-    def test_db_update__rename_title(self, database_for_updates):
-        old_title = str(database_for_updates.obj.title)
-        new_title = "1 BDU"
-        database = database_for_updates.db_update(title=new_title)
-        assert isinstance(database.obj, Database)
-        assert str(database.obj.title) == new_title
-
-        old_database = database_for_updates.db_update(title=old_title)
-        assert str(old_database.obj.title) == old_title
-
-    def test_db_update__rename_prop(self, database_for_updates):
-        properties = {"Name": Property.create(type_="title", name="Subject")}
-        database = database_for_updates.db_update(properties=properties)
-        assert "Subject" in database.obj.properties
-
-        title_property = database.obj.properties["Subject"]
-        title_property.name = "Name"
-        old_properties = {title_property.id: title_property}
-        old_database = database.db_update(properties=old_properties)
-        assert "Name" in old_database.obj.properties
-
-    def test_db_update__retype_prop(self, database_for_updates):
-        properties = {"Tags": Property.create("select")}
-        database = database_for_updates.db_update(properties=properties)
-        assert database.obj.properties["Tags"].type == "select"
-
-        old_properties = {"Tags": Property.create("multi_select")}
-        old_database = database_for_updates.db_update(properties=old_properties)
-        assert old_database.obj.properties["Tags"].type == "multi_select"
-
-    def test_db_update__create_delete_prop(self, database_for_updates):
-        properties = {"New property": Property.create("checkbox")}
-        database = database_for_updates.db_update(properties=properties)
-        assert "New property" in database.obj.properties
-        assert database.obj.properties["New property"].type == "checkbox"
-
-        properties["New property"] = Property.create(None)
-        database = database.db_update(properties=properties)
-        assert "New property" not in database.obj.properties
-
-    def test_page_create__into_page(self, no, page_for_pages):
-        parent = LinkTo(from_object=page_for_pages.obj)
-        page = no.pages.page_create(parent=parent, title="Page 1")
-        assert isinstance(page.obj, Page)
-        assert str(page.obj.title) == "Page 1"
-        # delete section
-        delete_page = page.page_update(archived=True)
-        assert delete_page.obj.archived is True
-
-    def test_page_create__into_database(self, no):
-        parent = LinkTo.create(database_id="35f50aa293964b0d93e09338bc980e2e")  # Database for creating pages
-        page = no.pages.page_create(parent=parent, title="Page 2")
-        assert isinstance(page.obj, Page)
-        assert str(page.obj.title) == "Page 2"
-        # delete section
-        delete_page = page.page_update(archived=True)
-        assert delete_page.obj.archived is True
-
-    def test_page_create__into_database_props(self, no):
-        parent = LinkTo.create(database_id="35f50aa293964b0d93e09338bc980e2e")  # Database for creating pages
-        props = {
-            "Tags": PropertyValue.create(type_="multi_select", value=["tag1", "tag2"]),
-            "done": PropertyValue.create("checkbox", True),
-            "when": PropertyValue.create("date", datetime.now()),
-        }
-        page = no.pages.page_create(parent=parent, properties=props, title="Page 3")
-        assert isinstance(page.obj, Page)
-        assert str(page.obj.title) == "Page 3"
-        # delete section
-        delete_page = page.page_update(archived=True)
-        assert delete_page.obj.archived is True
-
-    def test_page_create__with_children(self, no, page_for_pages):
-        parent = LinkTo(from_object=page_for_pages.obj)
-        child = Block.create("Hello, World!")
-        page = no.pages.page_create(parent=parent, title="Page 4", children=[child])
-        assert isinstance(page.obj, Page)
-        assert str(page.obj.title) == "Page 4"
-        blocks = page.get_block_children()
-        assert isinstance(blocks.obj, BlockArray)
-        assert len(blocks.obj) == 1
-        assert isinstance(blocks.obj[0], Block)
-        assert str(blocks.obj[0].text) == "Hello, World!"
-        # delete section
-        delete_page = page.page_update(archived=True)
-        assert delete_page.obj.archived is True
-
-    def test_page_create__from_obj(self, no, page_for_pages):
-        parent = LinkTo(from_object=page_for_pages.obj)
-        page_obj = Page.create(parent=parent, title="Page 5")
-        page = no.pages.page_create(page_obj=page_obj)
-        assert isinstance(page.obj, Page)
-        assert str(page.obj.title) == "Page 5"
-        # delete section
-        delete_page = page.page_update(archived=True)
-        assert delete_page.obj.archived is True
-
-    def test_page_update__rename(self, page_for_updates):
-        old_name = str(page_for_updates.obj.title)
-        new_name = "Updating for page"
-        page = page_for_updates.page_update(title=new_name)
-        assert isinstance(page.obj, Page)
-        assert str(page.obj.title) == new_name
-
-        old_page = page.page_update(title=RichTextArray.create(old_name))
-        assert str(old_page.obj.title) == old_name
-
-    def test_page_update__change_props(self, page_for_updates):
-        old_props = page_for_updates.obj.properties
-        new_props = {
-            "Tags": PropertyValue.create("multi_select", ["tag2"]),
-            "done": PropertyValue.create("checkbox", False),
-            "when": PropertyValue.create("date", datetime.now()),
-        }
-        page = page_for_updates.page_update(properties=new_props)
-        assert isinstance(page.obj, Page)
-        assert "tag2" in page.obj.properties["Tags"].value
-        assert page.obj.properties["done"].value is False
-
-        old_page = page.page_update(properties=old_props)
-        assert "tag1" in old_page.obj.properties["Tags"].value
-        assert old_page.obj.properties["done"].value is True
-
-    def test_page_update__delete(self, page_for_updates):
-        page = page_for_updates.page_update(archived=True)
-        assert isinstance(page.obj, Page)
-        assert page.obj.archived is True
-
-        old_page = page.page_update(archived=False)
-        assert old_page.obj.archived is False
-
-    def test_block_update__rename(self, no):
-        block = no.blocks.get("08326405c2924ccc929bd78ceb70a2f3")  # Paragraph block to update.
-        old_name = str(block.obj.text)
-        new_name = old_name + old_name
-        new_block = no.blocks.block_update(id_="08326405c2924ccc929bd78ceb70a2f3", new_text=new_name)
-        assert isinstance(new_block.obj, Block)
-        assert str(new_block.obj.text) == new_name
-
-        old_block = new_block.block_update(new_text=old_name)
-        assert str(old_block.obj.text) == old_name
-
-    def test_block_update__delete(self, no):
-        block = no.blocks.get("08326405c2924ccc929bd78ceb70a2f3")  # Paragraph block to update.
-        new_block = block.block_update(archived=True)
-        assert isinstance(new_block.obj, Block)
-        assert new_block.obj.archived is True
-
-        old_block = new_block.block_update(archived=False)
-        assert old_block.obj.archived is False
-
-    def test_block_update__obj_retype(self, no):
-        block_obj = Block.create("To do block", type_="to_do")
-        with pytest.raises(ValidationError):
-            no.blocks.block_update(id_="08326405c2924ccc929bd78ceb70a2f3", block_obj=block_obj)
-
-    def test_block_update__obj(self, no):
-        block = no.blocks.get("08326405c2924ccc929bd78ceb70a2f3")  # Paragraph block to update.
-        old_block_obj = block.obj
-        new_name = "Updated paragraph block"
-        block_obj = Block.create(new_name)
-        new_block = block.block_update(block_obj=block_obj)
-        assert isinstance(new_block.obj, Block)
-        assert new_block.obj.simple == new_name
-
-        old_block = new_block.block_update(block_obj=old_block_obj)
-        assert str(old_block.obj) == old_block_obj.simple
-
-    def test_block_append__single(self, no):
-        page = no.pages.get("365985ab349149d7826035fd46858b3f")  # Page for creating blocks
-        my_block = Block.create("Such wow!")
-        blocks = page.block_append(block=my_block)
-        assert isinstance(blocks.obj, BlockArray)
-
-        blocks = page.get_block_children()
-        assert len(blocks.obj) == 1
-        assert str(blocks.obj[0].text) == "Such wow!"
-        remove_block = blocks.from_object(blocks.obj[0])
-        removed_block = remove_block.block_update(archived=True)
-        assert removed_block.obj.archived is True
-
-    def test_block_append__many(self, no):
-        my_block1 = Block.create("Do simple tests", type_="to_do", checked=True)
-        my_block2 = Block.create(
-            "multiline:\n  code: text", type_="code", caption="is it YAML?", language="yaml"
-        )
-        blocks = no.blocks.block_append("365985ab349149d7826035fd46858b3f", blocks=[my_block1, my_block2])
-        assert isinstance(blocks.obj, BlockArray)
-
-        blocks = no.pages.get_block_children("365985ab349149d7826035fd46858b3f")
-        assert len(blocks.obj) == 2
-        assert str(blocks.obj[0].text) == "[x] Do simple tests"
-        assert str(blocks.obj[1].caption) == "is it YAML?"
-        assert blocks.obj[1].language == "yaml"
-
-        for block in blocks.obj:
-            removed_block = no.blocks.block_update(block.id, archived=True)
-            assert removed_block.obj.archived is True
-
-    def test_get_myself(self, no):
-        bot = no.users.get_myself()
-        assert isinstance(bot.obj, User)
-        assert bot.obj.type == "bot"
-        assert bot.obj.name == "Pytion tests"
-        assert bot.obj.workspace_name == "Yegor's Workspace"
-
-    def test_get_myself__from_obj(self, root_page):
-        bot = root_page.get_myself()
-        assert isinstance(bot.obj, User)
-        assert bot.obj.type == "bot"
-        assert bot.obj.name == "Pytion tests"
-        assert bot.obj.workspace_name == "Yegor's Workspace"
-
-    def test_from_linkto__base(self, no):
-        link = LinkTo.create(page_id="878d628488d94894ab14f9b872cd6870")
-        page = no.pages.from_linkto(link)
-        assert isinstance(page.obj, Page)
-        assert page.obj.id == "878d628488d94894ab14f9b872cd6870"
-        assert str(page.obj) == "Pytion Tests"
-
-    def test_from_linkto__child(self, page_some_texts):
-        child = page_some_texts.from_linkto(page_some_texts.obj.children)
-        assert isinstance(child.obj, BlockArray)
-        assert len(child.obj) == 3
-        assert isinstance(child.obj[0], Block)
-
-    def test_from_linkto__parent(self, no, little_database):
-        page = no.pages.get("b85877eaf7bf4245a8c5218055eeb81f")  # Parent testing page
-        parent = page.from_linkto(page.obj.parent)
-        assert isinstance(parent.obj, Database)
-        assert parent.obj.id == little_database.obj.id
-        assert str(parent.obj.title) == str(little_database.obj.title)
+from datetime import datetime
+
+import pytest
+
+from pytion.models import Page, Block, Database, User, RichTextArray, ElementArray
+from pytion.models import BlockArray, PropertyValue, PageArray, LinkTo, Property
+from pytion import InvalidRequestURL, ObjectNotFound, ValidationError
+
+
+def test_notion(no):
+    assert no.version == "2022-06-28"
+    assert no.session.base == "https://api.notion.com/v1/"
+
+
+def test_search__empty(no):
+    r = no.search("123412341234")
+    assert isinstance(r.obj, ElementArray)
+    assert len(r.obj) == 0
+
+
+def test_search__type_and_limit(no):
+    r = no.search(object_type="database", limit=4)
+    assert isinstance(r.obj, ElementArray)
+    assert len(r.obj) == 4
+    assert all(isinstance(item, Database) for item in r.obj)
+
+
+def test_search__query(no):
+    r = no.search("tests")
+    assert isinstance(r.obj, ElementArray)
+    assert len(r.obj) >= 1
+    assert str(r.obj[0]) == "Pytion Tests"
+
+
+class TestElement:
+    def test_get__page(self, root_page):
+        page = root_page
+        assert isinstance(page.obj, Page), "get of .pages. must return Page object"
+        assert page.obj.id == "878d628488d94894ab14f9b872cd6870"
+        assert str(page.obj.title) == "Pytion Tests"
+
+    def test_get__block(self, no):
+        block = no.blocks.get("878d628488d94894ab14f9b872cd6870")  # root page
+        assert isinstance(block.obj, Block)
+        assert block.obj.id == "878d628488d94894ab14f9b872cd6870"
+        assert block.obj.text == "Pytion Tests"
+
+    def test_get__database(self, no):
+        database = no.databases.get("0e9539099cff456d89e44684d6b6c701")  # Little Database
+        assert isinstance(database.obj, Database)
+        assert database.obj.id == "0e9539099cff456d89e44684d6b6c701"
+        assert str(database.obj.title) == "Little Database"
+        assert str(database.obj.description) == "Database has a super description! Don’t touch it!"
+        assert database.obj.is_inline is False
+
+    def test_get__user(self, no):
+        user = no.users.get("01c67faf3aba45ffaa022407f87c86a5")
+        assert isinstance(user.obj, User)
+        assert user.obj.id == "01c67faf3aba45ffaa022407f87c86a5"
+        assert user.obj.name == "Yegor Gomzin"
+
+    def test_get__bad_url(self, no):
+        with pytest.raises(InvalidRequestURL):
+            no.page.get("878d628488d94894ab14f9b872cd6870")  # root page
+
+    def test_get__bad_id(self, no):
+        with pytest.raises(ObjectNotFound):
+            no.pages.get("878d628488d94894ab14f9b872cd6872")  # random id
+
+    def test_get__after_path_page(self, no):
+        blocks = no.blocks.get("82ee5677402f44819a5da3302273400a", _after_path="children")  # Page with some texts
+        assert isinstance(blocks.obj, BlockArray)
+        assert len(blocks.obj) == 3
+        assert isinstance(blocks.obj[0], Block)
+        blocks = no.blocks.get("82ee5677402f44819a5da3302273400a", _after_path="children", limit=2)  # Page with some te
+        assert len(blocks.obj) == 2
+
+    def test_get__after_path_block(self, no):
+        blocks = no.blocks.get("8a920ba7dc1d4961811e5c82b28028ed", _after_path="children")  # Hello! How are you?
+        assert isinstance(blocks.obj, BlockArray)
+        assert len(blocks.obj) == 3
+        assert isinstance(blocks.obj[0], Block)
+
+    def test_get_parent__block(self, no):
+        parent_block = no.blocks.get_parent("9b2026c3a0cb45fc8cee330142d60f3a")  # I'm fine!
+        assert isinstance(parent_block.obj, Block)
+        assert parent_block.obj.id == "8a920ba7dc1d4961811e5c82b28028ed"
+        assert str(parent_block.obj) == "Hello! How are you?"
+
+    def test_get_parent__block2(self, no):
+        parent_block = no.blocks.get_parent("8a920ba7dc1d4961811e5c82b28028ed")  # Hello! How are you?
+        assert isinstance(parent_block.obj, Page)
+        assert parent_block.obj.id == "82ee5677402f44819a5da3302273400a"
+        assert str(parent_block.obj) == "Page with some texts"
+
+    def test_get_parent__page(self, no):
+        parent_page_block = no.pages.get_parent("82ee5677402f44819a5da3302273400a")  # Page with some texts
+        assert isinstance(parent_page_block.obj, Block)
+        assert parent_page_block.obj.id == "6001eb5621f2428392d532bf08bc8ecd"
+        assert "Page with some texts" in str(parent_page_block.obj)
+
+    def test_get_parent__database(self, no, root_page):
+        parent_page_block = no.databases.get_parent("0e9539099cff456d89e44684d6b6c701")  # Little Database
+        assert isinstance(parent_page_block.obj, Page)
+        assert parent_page_block.obj.id == root_page.obj.id
+
+    def test_get_parent__user(self, no):
+        something = no.users.get_parent("01c67faf3aba45ffaa022407f87c86a5")
+        assert something is None, "User object has not any parent"
+
+    def test_get_parent__block_obj(self, no):
+        block = no.blocks.get("8a920ba7dc1d4961811e5c82b28028ed")  # Hello! How are you?
+        parent_block = block.get_parent()
+        assert isinstance(parent_block.obj, Page)
+        assert parent_block.obj.id == "82ee5677402f44819a5da3302273400a"
+        assert str(parent_block.obj) == "Page with some texts"
+
+    def test_get_parent__page_obj(self, no):  # Database is the parent of this page
+        page = no.pages.get("b85877eaf7bf4245a8c5218055eeb81f")  # Parent testing page
+        database = page.get_parent()
+        assert isinstance(database.obj, Database)
+        assert database.obj.id == "0e9539099cff456d89e44684d6b6c701"
+        assert str(database.obj.title) == "Little Database"
+
+    def test_get_parent__database_obj(self, little_database):
+        database = little_database  # Little Database
+        parent_page_block = database.get_parent()
+        assert isinstance(parent_page_block.obj, Page)
+        assert parent_page_block.obj.id == "878d628488d94894ab14f9b872cd6870"
+        assert str(parent_page_block.obj) == "Pytion Tests"
+
+    def test_get_parent__child_page(self, no):
+        child_page = no.blocks.get("878d628488d94894ab14f9b872cd6870")  # root page
+        page = child_page.get_parent()
+        assert isinstance(page.obj, Page)
+        assert page.obj.id == "878d628488d94894ab14f9b872cd6870"
+        assert str(page.obj.title) == "Pytion Tests"
+
+    def test_get_parent__child_database(self, no):
+        child_database = no.blocks.get("0e9539099cff456d89e44684d6b6c701")  # Little Database
+        database = child_database.get_parent()
+        assert isinstance(database.obj, Database)
+        assert database.obj.id == "0e9539099cff456d89e44684d6b6c701"
+        assert str(database.obj.title) == "Little Database"
+
+    def test_get_parent__workspace(self, root_page):
+        workspace = root_page.get_parent()
+        assert workspace is None
+
+    def test_get_block_children__page_id(self, no):
+        blocks = no.pages.get_block_children("82ee5677402f44819a5da3302273400a")  # Page with some texts
+        assert isinstance(blocks.obj, BlockArray)
+        assert len(blocks.obj) == 3
+        assert isinstance(blocks.obj[0], Block)
+
+    def test_get_block_children__page_obj(self, page_some_texts):
+        page = page_some_texts  # Page with some texts
+        blocks = page.get_block_children()
+        assert isinstance(blocks.obj, BlockArray)
+        assert len(blocks.obj) == 3
+        assert isinstance(blocks.obj[0], Block)
+
+    def test_get_block_children__block_id(self, no):
+        blocks = no.blocks.get_block_children("8a920ba7dc1d4961811e5c82b28028ed")  # Hello! How are you?
+        assert isinstance(blocks.obj, BlockArray)
+        assert len(blocks.obj) == 3
+        assert isinstance(blocks.obj[0], Block)
+
+    def test_get_block_children__block_obj(self, no):
+        block = no.blocks.get("8a920ba7dc1d4961811e5c82b28028ed")  # Hello! How are you?
+        blocks = block.get_block_children()
+        assert isinstance(blocks.obj, BlockArray)
+        assert len(blocks.obj) == 3
+        assert isinstance(blocks.obj[0], Block)
+
+    def test_get_block_children__database_id(self, no):
+        something = no.databases.get_block_children("0e9539099cff456d89e44684d6b6c701")  # Little Database
+        assert something is None, "Database has no children"
+
+    def test_get_block_children__database_obj(self, little_database):
+        database = little_database  # Little Database
+        something = database.get_block_children()
+        assert something is None, "Database has no children"
+
+    def test_get_block_children__child_database(self, no):
+        database_block = no.blocks.get("0e9539099cff456d89e44684d6b6c701")  # Little Database
+        database = database_block.get_block_children()
+        assert isinstance(database.obj, Database)
+        assert database.obj.id == "0e9539099cff456d89e44684d6b6c701"
+        assert str(database.obj.title) == "Little Database"
+
+    def test_get_block_children_recursive__page_id(self, no):
+        blocks = no.pages.get_block_children_recursive("82ee5677402f44819a5da3302273400a")  # Page with some texts
+        assert isinstance(blocks.obj, BlockArray)
+        assert len(blocks.obj) == 6
+        assert isinstance(blocks.obj[0], Block)
+
+    def test_get_block_children_recursive__page_obj(self, page_some_texts):
+        page = page_some_texts  # Page with some texts
+        blocks = page.get_block_children_recursive()
+        assert isinstance(blocks.obj, BlockArray)
+        assert len(blocks.obj) == 6
+        assert isinstance(blocks.obj[0], Block)
+
+    def test_get_block_children_recursive__block_id(self, no):
+        blocks = no.blocks.get_block_children_recursive("8a920ba7dc1d4961811e5c82b28028ed")  # Hello! How are you?
+        assert isinstance(blocks.obj, BlockArray)
+        assert len(blocks.obj) == 3
+        assert isinstance(blocks.obj[0], Block)
+
+    def test_get_block_children_recursive__block_obj(self, no):
+        block = no.blocks.get("8a920ba7dc1d4961811e5c82b28028ed")  # Hello! How are you?
+        blocks = block.get_block_children_recursive()
+        assert isinstance(blocks.obj, BlockArray)
+        assert len(blocks.obj) == 3
+        assert isinstance(blocks.obj[0], Block)
+
+    def test_get_block_children_recursive__database_id(self, no):
+        something = no.databases.get_block_children_recursive("0e9539099cff456d89e44684d6b6c701")  # Little Database
+        assert something is None, "Database has no children"
+
+    def test_get_block_children_recursive__database_obj(self, little_database):
+        database = little_database  # Little Database
+        something = database.get_block_children_recursive()
+        assert something is None, "Database has no children"
+
+    def test_get_block_children_recursive__child_database(self, no):
+        database_block = no.blocks.get("0e9539099cff456d89e44684d6b6c701")  # Little Database
+        database = database_block.get_block_children_recursive()
+        assert isinstance(database.obj, Database)
+        assert database.obj.id == "0e9539099cff456d89e44684d6b6c701"
+        assert str(database.obj.title) == "Little Database"
+
+    def test_get_block_children_recursive__force(self, no):
+        block = no.blocks.get("8a920ba7dc1d4961811e5c82b28028ed")  # Hello! How are you?
+        blocks = block.get_block_children_recursive(force=True)
+        assert isinstance(blocks.obj, BlockArray)
+        assert len(blocks.obj) == 5
+        assert isinstance(blocks.obj[0], Block)
+
+    def test_get_block_children_recursive__max_depth(self, page_some_texts):
+        page = page_some_texts  # Page with some texts
+        blocks = page.get_block_children_recursive(force=True, max_depth=2)
+        assert isinstance(blocks.obj, BlockArray)
+        assert len(blocks.obj) == 7
+        assert isinstance(blocks.obj[0], Block)
+
+    def test_get_page_property__page_id(self, no):
+        p = no.pages.get_page_property("%7Dma%3F", "b85877eaf7bf4245a8c5218055eeb81f")
+        assert isinstance(p.obj, PropertyValue)
+        assert len(p.obj.value) == 2
+        assert p.obj.type == "multi_select"
+
+    def test_get_page_property__page_obj(self, no):
+        page = no.pages.get("b85877eaf7bf4245a8c5218055eeb81f")
+        p = page.get_page_property("%7Dma%3F")
+        assert isinstance(p.obj, PropertyValue)
+        assert len(p.obj.value) == 2
+        assert p.obj.type == "multi_select"
+
+    def test_get_page_property__bad_id(self, no):
+        with pytest.raises(ValidationError):
+            no.pages.get_page_property("%7Dma%3A", "b85877eaf7bf4245a8c5218055eeb81f")
+
+    def test_get_page_property__bad_page(self, no):
+        with pytest.raises(ObjectNotFound):
+            no.pages.get_page_property("%7Dma%3F", "b85877eaf7bf4245a8c5218055eeb81a")
+
+    def test_get_page_properties(self, no):
+        page = no.pages.get("b85877eaf7bf4245a8c5218055eeb81f")  # Parent testing page
+        assert isinstance(page.obj, Page)
+        # assert str(page.obj) == "unknown"
+        # assert isinstance(page.obj.properties["Done"], Property)
+        page.get_page_properties()
+        assert isinstance(page.obj.properties["Done"], PropertyValue)
+        assert page.obj.properties["Digit"].value == 2
+        assert "tag1" in page.obj.properties["Tags"].value
+
+    def test_get_page_properties__title(self, no):
+        page = no.pages.get("b85877eaf7bf4245a8c5218055eeb81f")  # Parent testing page
+        assert isinstance(page.obj, Page)
+        # assert str(page.obj) == "unknown"
+        # assert isinstance(page.obj.properties["Done"], Property)
+        page.get_page_properties(title_only=True)
+        # assert hasattr(page.obj.properties["by"], "value") is False
+        # assert isinstance(page.obj.properties["Done"], Property)
+        assert str(page.obj.title) == "Parent testing page"
+
+    def test_db_query__id(self, no):
+        pages = no.databases.db_query("0e9539099cff456d89e44684d6b6c701")  # Little Database
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 4
+        assert str(pages.obj[0].title) == ""
+
+    def test_db_query__obj(self, little_database):
+        pages = little_database.db_query(limit=3)
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 3
+        assert str(pages.obj[0].title) == ""
+
+    def test_db_filter__title_ez(self, little_database):
+        pages = little_database.db_filter("testing page")
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 1
+        assert str(pages.obj[0].title) == "Parent testing page"
+
+    def test_db_filter__not_contain(self, little_database):
+        pages = little_database.db_filter("testing page", condition="does_not_contain")
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 3
+        assert str(pages.obj[0].title) == ""
+
+    def test_db_filter__ends_with(self, little_database):
+        pages = little_database.db_filter(
+            property_name="Name", property_type="title", value="what?", condition="ends_with"
+        )
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 1
+        assert str(pages.obj[0].title) == "wait, what?"
+
+    def test_db_filter__is_empty(self, little_database):
+        pages = little_database.db_filter(property_name="title", property_type="title", condition="is_empty")
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 1
+        assert str(pages.obj[0].title) == ""
+
+    def test_db_filter__greater_than(self, little_database):
+        pages = little_database.db_filter(
+            property_name="Digit", property_type="number", condition="greater_than", value="1"
+        )
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 2
+        assert str(pages.obj[0].title) == "We are best friends, body"
+
+    def test_db_filter__checkbox(self, little_database):
+        pages = little_database.db_filter(property_name="Done", property_type="checkbox")
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 1
+        assert str(pages.obj[0].title) == "We are best friends, body"
+
+    def test_db_filter__contains_tag(self, little_database):
+        pages = little_database.db_filter(
+            property_name="Tags", property_type="multi_select", value="tag1"
+        )
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 2
+        assert str(pages.obj[0].title) == ""
+
+    def test_db_filter__notcontains_tag(self, little_database):
+        pages = little_database.db_filter(
+            property_name="Tags", property_type="multi_select", value="tag2", condition="does_not_contain"
+        )
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 3
+        assert str(pages.obj[0].title) == ""
+
+    def test_db_filter__no_tags(self, little_database):
+        pages = little_database.db_filter(
+            property_name="Tags", property_type="multi_select", condition="is_empty"
+        )
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 1
+        assert str(pages.obj[0].title) == "wait, what?"
+
+    def test_db_filter__tag_property_obj(self, no, little_database):
+        page = no.pages.get("c2fc6b3dc3d244e9be2a3d28b26082bf")  # Untitled
+        my_prop = page.obj.properties["Tags"]
+        pages = little_database.db_filter(property_obj=my_prop)
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 2
+        assert str(pages.obj[0].title) == ""
+
+    def test_db_filter__without_filter(self, little_database):
+        pages = little_database.db_filter("")
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 4
+        assert str(pages.obj[0].title) == ""
+
+    def test_db_filter__date_after(self, little_database):
+        pages = little_database.db_filter(
+            property_name="created", property_type="date", condition="on_or_after", value="2022-04-22"
+        )
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 2
+        assert str(pages.obj[0].title) == ""
+
+    def test_db_filter__date_next_year(self, little_database):
+        pages = little_database.db_filter(
+            property_name="created", property_type="created_time", condition="next_year", value="2022-04-22"
+        )
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 0
+
+    def test_db_filter__date_this_week(self, little_database):
+        pages = little_database.db_filter(
+            property_name="created", property_type="created_time", condition="this_week"
+        )
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 0
+
+    def test_db_filter__status(self, little_database):
+        pages = little_database.db_filter(
+            property_name="Status", property_type="status", value="Done"
+        )
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 1
+        assert str(pages.obj[0].title) == "wait, what?"
+
+    def test_db_filter__sort_desc(self, little_database):
+        pages = little_database.db_filter("", descending="created")
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 4
+        assert str(pages.obj[0].title) == ""
+        assert str(pages.obj[2].title) == "We are best friends, body"
+
+    def test_db_filter__sort_asc(self, little_database):
+        pages = little_database.db_filter("", ascending="Digit")
+        assert isinstance(pages.obj, PageArray)
+        assert len(pages.obj) == 4
+        assert str(pages.obj[0].title) == "wait, what?"
+        assert str(pages.obj[2].title) == "We are best friends, body"
+
+    def test_db_create(self, no):
+        parent = LinkTo.create(page_id="2dff77eb43d44ce097ffb421499f82aa")  # Page for creating databases
+        properties = {
+            "Name": Property.create("title"),
+            "Digit": Property.create("number"),
+            "Status": Property.create("select"),
+        }
+        title = "DB 1"
+        description = "ABCDEF"
+        database = no.databases.db_create(parent=parent, properties=properties, title=title, description=description)
+        assert isinstance(database.obj, Database)
+        assert str(database.obj.title) == title
+        assert "Status" in database.obj.properties
+        assert str(database.obj.description) == description
+
+        # Delete database manually. There is no way to delete a database by API
+
+    def test_db_update__rename_title(self, database_for_updates):
+        old_title = str(database_for_updates.obj.title)
+        new_title = "1 BDU"
+        database = database_for_updates.db_update(title=new_title)
+        assert isinstance(database.obj, Database)
+        assert str(database.obj.title) == new_title
+
+        old_database = database_for_updates.db_update(title=old_title)
+        assert str(old_database.obj.title) == old_title
+
+    def test_db_update__rename_prop(self, database_for_updates):
+        properties = {"Name": Property.create(type_="title", name="Subject")}
+        database = database_for_updates.db_update(properties=properties)
+        assert "Subject" in database.obj.properties
+
+        title_property = database.obj.properties["Subject"]
+        title_property.name = "Name"
+        old_properties = {title_property.id: title_property}
+        old_database = database.db_update(properties=old_properties)
+        assert "Name" in old_database.obj.properties
+
+    def test_db_update__retype_prop(self, database_for_updates):
+        properties = {"Tags": Property.create("select")}
+        database = database_for_updates.db_update(properties=properties)
+        assert database.obj.properties["Tags"].type == "select"
+
+        old_properties = {"Tags": Property.create("multi_select")}
+        old_database = database_for_updates.db_update(properties=old_properties)
+        assert old_database.obj.properties["Tags"].type == "multi_select"
+
+    def test_db_update__create_delete_prop(self, database_for_updates):
+        properties = {"New property": Property.create("checkbox")}
+        database = database_for_updates.db_update(properties=properties)
+        assert "New property" in database.obj.properties
+        assert database.obj.properties["New property"].type == "checkbox"
+
+        properties["New property"] = Property.create(None)
+        database = database.db_update(properties=properties)
+        assert "New property" not in database.obj.properties
+
+    def test_page_create__into_page(self, no, page_for_pages):
+        parent = LinkTo(from_object=page_for_pages.obj)
+        page = no.pages.page_create(parent=parent, title="Page 1")
+        assert isinstance(page.obj, Page)
+        assert str(page.obj.title) == "Page 1"
+        # delete section
+        delete_page = page.page_update(archived=True)
+        assert delete_page.obj.archived is True
+
+    def test_page_create__into_database(self, no):
+        parent = LinkTo.create(database_id="35f50aa293964b0d93e09338bc980e2e")  # Database for creating pages
+        page = no.pages.page_create(parent=parent, title="Page 2")
+        assert isinstance(page.obj, Page)
+        assert str(page.obj.title) == "Page 2"
+        # delete section
+        delete_page = page.page_update(archived=True)
+        assert delete_page.obj.archived is True
+
+    def test_page_create__into_database_props(self, no):
+        parent = LinkTo.create(database_id="35f50aa293964b0d93e09338bc980e2e")  # Database for creating pages
+        props = {
+            "Tags": PropertyValue.create(type_="multi_select", value=["tag1", "tag2"]),
+            "done": PropertyValue.create("checkbox", True),
+            "when": PropertyValue.create("date", datetime.now()),
+        }
+        page = no.pages.page_create(parent=parent, properties=props, title="Page 3")
+        assert isinstance(page.obj, Page)
+        assert str(page.obj.title) == "Page 3"
+        # delete section
+        delete_page = page.page_update(archived=True)
+        assert delete_page.obj.archived is True
+
+    def test_page_create__with_children(self, no, page_for_pages):
+        parent = LinkTo(from_object=page_for_pages.obj)
+        child = Block.create("Hello, World!")
+        page = no.pages.page_create(parent=parent, title="Page 4", children=[child])
+        assert isinstance(page.obj, Page)
+        assert str(page.obj.title) == "Page 4"
+        blocks = page.get_block_children()
+        assert isinstance(blocks.obj, BlockArray)
+        assert len(blocks.obj) == 1
+        assert isinstance(blocks.obj[0], Block)
+        assert str(blocks.obj[0].text) == "Hello, World!"
+        # delete section
+        delete_page = page.page_update(archived=True)
+        assert delete_page.obj.archived is True
+
+    def test_page_create__from_obj(self, no, page_for_pages):
+        parent = LinkTo(from_object=page_for_pages.obj)
+        page_obj = Page.create(parent=parent, title="Page 5")
+        page = no.pages.page_create(page_obj=page_obj)
+        assert isinstance(page.obj, Page)
+        assert str(page.obj.title) == "Page 5"
+        # delete section
+        delete_page = page.page_update(archived=True)
+        assert delete_page.obj.archived is True
+
+    def test_page_update__rename(self, page_for_updates):
+        old_name = str(page_for_updates.obj.title)
+        new_name = "Updating for page"
+        page = page_for_updates.page_update(title=new_name)
+        assert isinstance(page.obj, Page)
+        assert str(page.obj.title) == new_name
+
+        old_page = page.page_update(title=RichTextArray.create(old_name))
+        assert str(old_page.obj.title) == old_name
+
+    def test_page_update__change_props(self, page_for_updates):
+        old_props = page_for_updates.obj.properties
+        new_props = {
+            "Tags": PropertyValue.create("multi_select", ["tag2"]),
+            "done": PropertyValue.create("checkbox", False),
+            "when": PropertyValue.create("date", datetime.now()),
+        }
+        page = page_for_updates.page_update(properties=new_props)
+        assert isinstance(page.obj, Page)
+        assert "tag2" in page.obj.properties["Tags"].value
+        assert page.obj.properties["done"].value is False
+
+        old_page = page.page_update(properties=old_props)
+        assert "tag1" in old_page.obj.properties["Tags"].value
+        assert old_page.obj.properties["done"].value is True
+
+    def test_page_update__delete(self, page_for_updates):
+        page = page_for_updates.page_update(archived=True)
+        assert isinstance(page.obj, Page)
+        assert page.obj.archived is True
+
+        old_page = page.page_update(archived=False)
+        assert old_page.obj.archived is False
+
+    def test_block_update__rename(self, no):
+        block = no.blocks.get("08326405c2924ccc929bd78ceb70a2f3")  # Paragraph block to update.
+        old_name = str(block.obj.text)
+        new_name = old_name + old_name
+        new_block = no.blocks.block_update(id_="08326405c2924ccc929bd78ceb70a2f3", new_text=new_name)
+        assert isinstance(new_block.obj, Block)
+        assert str(new_block.obj.text) == new_name
+
+        old_block = new_block.block_update(new_text=old_name)
+        assert str(old_block.obj.text) == old_name
+
+    def test_block_update__delete(self, no):
+        block = no.blocks.get("08326405c2924ccc929bd78ceb70a2f3")  # Paragraph block to update.
+        new_block = block.block_update(archived=True)
+        assert isinstance(new_block.obj, Block)
+        assert new_block.obj.archived is True
+
+        old_block = new_block.block_update(archived=False)
+        assert old_block.obj.archived is False
+
+    def test_block_update__obj_retype(self, no):
+        block_obj = Block.create("To do block", type_="to_do")
+        with pytest.raises(ValidationError):
+            no.blocks.block_update(id_="08326405c2924ccc929bd78ceb70a2f3", block_obj=block_obj)
+
+    def test_block_update__obj(self, no):
+        block = no.blocks.get("08326405c2924ccc929bd78ceb70a2f3")  # Paragraph block to update.
+        old_block_obj = block.obj
+        new_name = "Updated paragraph block"
+        block_obj = Block.create(new_name)
+        new_block = block.block_update(block_obj=block_obj)
+        assert isinstance(new_block.obj, Block)
+        assert new_block.obj.simple == new_name
+
+        old_block = new_block.block_update(block_obj=old_block_obj)
+        assert str(old_block.obj) == old_block_obj.simple
+
+    def test_block_append__single(self, no):
+        page = no.pages.get("365985ab349149d7826035fd46858b3f")  # Page for creating blocks
+        my_block = Block.create("Such wow!")
+        blocks = page.block_append(block=my_block)
+        assert isinstance(blocks.obj, BlockArray)
+
+        blocks = page.get_block_children()
+        assert len(blocks.obj) == 1
+        assert str(blocks.obj[0].text) == "Such wow!"
+        remove_block = blocks.from_object(blocks.obj[0])
+        removed_block = remove_block.block_update(archived=True)
+        assert removed_block.obj.archived is True
+
+    def test_block_append__many(self, no):
+        my_block1 = Block.create("Do simple tests", type_="to_do", checked=True)
+        my_block2 = Block.create(
+            "multiline:\n  code: text", type_="code", caption="is it YAML?", language="yaml"
+        )
+        blocks = no.blocks.block_append("365985ab349149d7826035fd46858b3f", blocks=[my_block1, my_block2])
+        assert isinstance(blocks.obj, BlockArray)
+
+        blocks = no.pages.get_block_children("365985ab349149d7826035fd46858b3f")
+        assert len(blocks.obj) == 2
+        assert str(blocks.obj[0].text) == "[x] Do simple tests"
+        assert str(blocks.obj[1].caption) == "is it YAML?"
+        assert blocks.obj[1].language == "yaml"
+
+        for block in blocks.obj:
+            removed_block = no.blocks.block_update(block.id, archived=True)
+            assert removed_block.obj.archived is True
+
+    def test_get_myself(self, no):
+        bot = no.users.get_myself()
+        assert isinstance(bot.obj, User)
+        assert bot.obj.type == "bot"
+        assert bot.obj.name == "Pytion tests"
+        assert bot.obj.workspace_name == "Yegor's Workspace"
+
+    def test_get_myself__from_obj(self, root_page):
+        bot = root_page.get_myself()
+        assert isinstance(bot.obj, User)
+        assert bot.obj.type == "bot"
+        assert bot.obj.name == "Pytion tests"
+        assert bot.obj.workspace_name == "Yegor's Workspace"
+
+    def test_from_linkto__base(self, no):
+        link = LinkTo.create(page_id="878d628488d94894ab14f9b872cd6870")
+        page = no.pages.from_linkto(link)
+        assert isinstance(page.obj, Page)
+        assert page.obj.id == "878d628488d94894ab14f9b872cd6870"
+        assert str(page.obj) == "Pytion Tests"
+
+    def test_from_linkto__child(self, page_some_texts):
+        child = page_some_texts.from_linkto(page_some_texts.obj.children)
+        assert isinstance(child.obj, BlockArray)
+        assert len(child.obj) == 3
+        assert isinstance(child.obj[0], Block)
+
+    def test_from_linkto__parent(self, no, little_database):
+        page = no.pages.get("b85877eaf7bf4245a8c5218055eeb81f")  # Parent testing page
+        parent = page.from_linkto(page.obj.parent)
+        assert isinstance(parent.obj, Database)
+        assert parent.obj.id == little_database.obj.id
+        assert str(parent.obj.title) == str(little_database.obj.title)
```

