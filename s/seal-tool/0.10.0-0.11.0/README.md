# Comparing `tmp/seal-tool-0.10.0.tar.gz` & `tmp/seal_tool-0.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seal-tool-0.10.0.tar", last modified: Wed Feb  7 22:36:27 2024, max compression
+gzip compressed data, was "seal_tool-0.11.0.tar", last modified: Fri Apr 26 20:55:00 2024, max compression
```

## Comparing `seal-tool-0.10.0.tar` & `seal_tool-0.11.0.tar`

### file list

```diff
@@ -1,28 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-02-07 22:36:27.418416 seal-tool-0.10.0/
--rw-rw-rw-   0        0        0    32472 2024-02-07 22:32:18.000000 seal-tool-0.10.0/LICENSE
--rw-rw-rw-   0        0        0    45611 2024-02-07 22:36:27.417416 seal-tool-0.10.0/PKG-INFO
--rw-rw-rw-   0        0        0     5925 2024-02-07 22:32:18.000000 seal-tool-0.10.0/README.md
--rw-rw-rw-   0        0        0     2212 2024-02-07 22:32:18.000000 seal-tool-0.10.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-07 22:36:27.419418 seal-tool-0.10.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-07 22:36:27.242583 seal-tool-0.10.0/src/
-drwxrwxrwx   0        0        0        0 2024-02-07 22:36:27.330666 seal-tool-0.10.0/src/seal/
--rw-rw-rw-   0        0        0        0 2024-02-07 22:32:18.000000 seal-tool-0.10.0/src/seal/__init__.py
--rw-rw-rw-   0        0        0     5789 2024-02-07 22:32:18.000000 seal-tool-0.10.0/src/seal/__main__.py
--rw-rw-rw-   0        0        0    67022 2024-02-07 22:32:18.000000 seal-tool-0.10.0/src/seal/analyze.py
--rw-rw-rw-   0        0        0      914 2024-02-07 22:32:18.000000 seal-tool-0.10.0/src/seal/common.py
--rw-rw-rw-   0        0        0     3148 2024-02-07 22:32:18.000000 seal-tool-0.10.0/src/seal/config.py
--rw-rw-rw-   0        0        0     8941 2024-02-07 22:32:18.000000 seal-tool-0.10.0/src/seal/misc.py
--rw-rw-rw-   0        0        0    16873 2024-02-07 22:32:18.000000 seal-tool-0.10.0/src/seal/plot.py
--rw-rw-rw-   0        0        0    11645 2024-02-07 22:32:18.000000 seal-tool-0.10.0/src/seal/preprocess.py
-drwxrwxrwx   0        0        0        0 2024-02-07 22:36:27.415415 seal-tool-0.10.0/src/seal_tool.egg-info/
--rw-rw-rw-   0        0        0    45611 2024-02-07 22:36:27.000000 seal-tool-0.10.0/src/seal_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2024-02-07 22:36:27.000000 seal-tool-0.10.0/src/seal_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-07 22:36:27.000000 seal-tool-0.10.0/src/seal_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-02-07 22:36:27.000000 seal-tool-0.10.0/src/seal_tool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      186 2024-02-07 22:36:27.000000 seal-tool-0.10.0/src/seal_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-02-07 22:36:27.000000 seal-tool-0.10.0/src/seal_tool.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-07 22:36:27.414415 seal-tool-0.10.0/tests/
--rw-rw-rw-   0        0        0     2916 2024-02-07 22:32:19.000000 seal-tool-0.10.0/tests/test-analyze.py
--rw-rw-rw-   0        0        0      597 2024-02-07 22:32:19.000000 seal-tool-0.10.0/tests/test-misc.py
--rw-rw-rw-   0        0        0      201 2024-02-07 22:32:19.000000 seal-tool-0.10.0/tests/test-plot.py
--rw-rw-rw-   0        0        0      690 2024-02-07 22:32:19.000000 seal-tool-0.10.0/tests/test-preprocess.py
+drwxr-xr-x   0 mmatous   (1000) mmatous   (1000)        0 2024-04-26 20:55:00.178980 seal_tool-0.11.0/
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)    32472 2024-04-26 18:05:35.000000 seal_tool-0.11.0/LICENSE
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)    45015 2024-04-26 20:55:00.178980 seal_tool-0.11.0/PKG-INFO
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)     6158 2024-04-26 18:05:57.000000 seal_tool-0.11.0/README.md
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)     3150 2024-04-26 20:54:52.000000 seal_tool-0.11.0/pyproject.toml
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)       38 2024-04-26 20:55:00.178980 seal_tool-0.11.0/setup.cfg
+drwxr-xr-x   0 mmatous   (1000) mmatous   (1000)        0 2024-04-26 20:55:00.175980 seal_tool-0.11.0/src/
+drwxr-xr-x   0 mmatous   (1000) mmatous   (1000)        0 2024-04-26 20:55:00.176980 seal_tool-0.11.0/src/seal/
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)        0 2024-04-26 18:05:35.000000 seal_tool-0.11.0/src/seal/__init__.py
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)     5762 2024-04-26 18:05:57.000000 seal_tool-0.11.0/src/seal/__main__.py
+-rwxr-xr-x   0 mmatous   (1000) mmatous   (1000)    74146 2024-04-26 18:48:20.000000 seal_tool-0.11.0/src/seal/analyze.py
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)     1722 2024-04-26 18:29:22.000000 seal_tool-0.11.0/src/seal/common.py
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)     4905 2024-04-26 18:32:51.000000 seal_tool-0.11.0/src/seal/config.py
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)     2157 2024-04-26 18:05:57.000000 seal_tool-0.11.0/src/seal/exceptions.py
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)     8299 2024-04-26 18:05:57.000000 seal_tool-0.11.0/src/seal/misc.py
+-rwxr-xr-x   0 mmatous   (1000) mmatous   (1000)    17088 2024-04-26 18:30:47.000000 seal_tool-0.11.0/src/seal/plot.py
+-rwxr-xr-x   0 mmatous   (1000) mmatous   (1000)    12429 2024-04-26 18:05:57.000000 seal_tool-0.11.0/src/seal/preprocess.py
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)        0 2024-04-26 18:05:55.000000 seal_tool-0.11.0/src/seal/py.typed
+drwxr-xr-x   0 mmatous   (1000) mmatous   (1000)        0 2024-04-26 20:55:00.177980 seal_tool-0.11.0/src/seal_tool.egg-info/
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)    45015 2024-04-26 20:55:00.000000 seal_tool-0.11.0/src/seal_tool.egg-info/PKG-INFO
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)      454 2024-04-26 20:55:00.000000 seal_tool-0.11.0/src/seal_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)        1 2024-04-26 20:55:00.000000 seal_tool-0.11.0/src/seal_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)       44 2024-04-26 20:55:00.000000 seal_tool-0.11.0/src/seal_tool.egg-info/entry_points.txt
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)      193 2024-04-26 20:55:00.000000 seal_tool-0.11.0/src/seal_tool.egg-info/requires.txt
+-rw-r--r--   0 mmatous   (1000) mmatous   (1000)        5 2024-04-26 20:55:00.000000 seal_tool-0.11.0/src/seal_tool.egg-info/top_level.txt
```

### Comparing `seal-tool-0.10.0/LICENSE` & `seal_tool-0.11.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seal-tool-0.10.0/PKG-INFO` & `seal_tool-0.11.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,851 +1,863 @@
-Metadata-Version: 2.1
-Name: seal-tool
-Version: 0.10.0
-Summary: A tool to perform richness-extent-grain analyses
-Author-email: Martin Matouš <m@matous.dev>, Barbora Winterová <winterova@mail.muni.cz>
-License:                     GNU GENERAL PUBLIC LICENSE
-                               Version 3, 29 June 2007
-        
-         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
-         Everyone is permitted to copy and distribute verbatim copies
-         of this license document, but changing it is not allowed.
-        
-                                    Preamble
-        
-          The GNU General Public License is a free, copyleft license for
-        software and other kinds of works.
-        
-          The licenses for most software and other practical works are designed
-        to take away your freedom to share and change the works.  By contrast,
-        the GNU General Public License is intended to guarantee your freedom to
-        share and change all versions of a program--to make sure it remains free
-        software for all its users.  We, the Free Software Foundation, use the
-        GNU General Public License for most of our software; it applies also to
-        any other work released this way by its authors.  You can apply it to
-        your programs, too.
-        
-          When we speak of free software, we are referring to freedom, not
-        price.  Our General Public Licenses are designed to make sure that you
-        have the freedom to distribute copies of free software (and charge for
-        them if you wish), that you receive source code or can get it if you
-        want it, that you can change the software or use pieces of it in new
-        free programs, and that you know you can do these things.
-        
-          To protect your rights, we need to prevent others from denying you
-        these rights or asking you to surrender the rights.  Therefore, you have
-        certain responsibilities if you distribute copies of the software, or if
-        you modify it: responsibilities to respect the freedom of others.
-        
-          For example, if you distribute copies of such a program, whether
-        gratis or for a fee, you must pass on to the recipients the same
-        freedoms that you received.  You must make sure that they, too, receive
-        or can get the source code.  And you must show them these terms so they
-        know their rights.
-        
-          Developers that use the GNU GPL protect your rights with two steps:
-        (1) assert copyright on the software, and (2) offer you this License
-        giving you legal permission to copy, distribute and/or modify it.
-        
-          For the developers' and authors' protection, the GPL clearly explains
-        that there is no warranty for this free software.  For both users' and
-        authors' sake, the GPL requires that modified versions be marked as
-        changed, so that their problems will not be attributed erroneously to
-        authors of previous versions.
-        
-          Some devices are designed to deny users access to install or run
-        modified versions of the software inside them, although the manufacturer
-        can do so.  This is fundamentally incompatible with the aim of
-        protecting users' freedom to change the software.  The systematic
-        pattern of such abuse occurs in the area of products for individuals to
-        use, which is precisely where it is most unacceptable.  Therefore, we
-        have designed this version of the GPL to prohibit the practice for those
-        products.  If such problems arise substantially in other domains, we
-        stand ready to extend this provision to those domains in future versions
-        of the GPL, as needed to protect the freedom of users.
-        
-          Finally, every program is threatened constantly by software patents.
-        States should not allow patents to restrict development and use of
-        software on general-purpose computers, but in those that do, we wish to
-        avoid the special danger that patents applied to a free program could
-        make it effectively proprietary.  To prevent this, the GPL assures that
-        patents cannot be used to render the program non-free.
-        
-          The precise terms and conditions for copying, distribution and
-        modification follow.
-        
-                               TERMS AND CONDITIONS
-        
-          0. Definitions.
-        
-          "This License" refers to version 3 of the GNU General Public License.
-        
-          "Copyright" also means copyright-like laws that apply to other kinds of
-        works, such as semiconductor masks.
-        
-          "The Program" refers to any copyrightable work licensed under this
-        License.  Each licensee is addressed as "you".  "Licensees" and
-        "recipients" may be individuals or organizations.
-        
-          To "modify" a work means to copy from or adapt all or part of the work
-        in a fashion requiring copyright permission, other than the making of an
-        exact copy.  The resulting work is called a "modified version" of the
-        earlier work or a work "based on" the earlier work.
-        
-          A "covered work" means either the unmodified Program or a work based
-        on the Program.
-        
-          To "propagate" a work means to do anything with it that, without
-        permission, would make you directly or secondarily liable for
-        infringement under applicable copyright law, except executing it on a
-        computer or modifying a private copy.  Propagation includes copying,
-        distribution (with or without modification), making available to the
-        public, and in some countries other activities as well.
-        
-          To "convey" a work means any kind of propagation that enables other
-        parties to make or receive copies.  Mere interaction with a user through
-        a computer network, with no transfer of a copy, is not conveying.
-        
-          An interactive user interface displays "Appropriate Legal Notices"
-        to the extent that it includes a convenient and prominently visible
-        feature that (1) displays an appropriate copyright notice, and (2)
-        tells the user that there is no warranty for the work (except to the
-        extent that warranties are provided), that licensees may convey the
-        work under this License, and how to view a copy of this License.  If
-        the interface presents a list of user commands or options, such as a
-        menu, a prominent item in the list meets this criterion.
-        
-          1. Source Code.
-        
-          The "source code" for a work means the preferred form of the work
-        for making modifications to it.  "Object code" means any non-source
-        form of a work.
-        
-          A "Standard Interface" means an interface that either is an official
-        standard defined by a recognized standards body, or, in the case of
-        interfaces specified for a particular programming language, one that
-        is widely used among developers working in that language.
-        
-          The "System Libraries" of an executable work include anything, other
-        than the work as a whole, that (a) is included in the normal form of
-        packaging a Major Component, but which is not part of that Major
-        Component, and (b) serves only to enable use of the work with that
-        Major Component, or to implement a Standard Interface for which an
-        implementation is available to the public in source code form.  A
-        "Major Component", in this context, means a major essential component
-        (kernel, window system, and so on) of the specific operating system
-        (if any) on which the executable work runs, or a compiler used to
-        produce the work, or an object code interpreter used to run it.
-        
-          The "Corresponding Source" for a work in object code form means all
-        the source code needed to generate, install, and (for an executable
-        work) run the object code and to modify the work, including scripts to
-        control those activities.  However, it does not include the work's
-        System Libraries, or general-purpose tools or generally available free
-        programs which are used unmodified in performing those activities but
-        which are not part of the work.  For example, Corresponding Source
-        includes interface definition files associated with source files for
-        the work, and the source code for shared libraries and dynamically
-        linked subprograms that the work is specifically designed to require,
-        such as by intimate data communication or control flow between those
-        subprograms and other parts of the work.
-        
-          The Corresponding Source need not include anything that users
-        can regenerate automatically from other parts of the Corresponding
-        Source.
-        
-          The Corresponding Source for a work in source code form is that
-        same work.
-        
-          2. Basic Permissions.
-        
-          All rights granted under this License are granted for the term of
-        copyright on the Program, and are irrevocable provided the stated
-        conditions are met.  This License explicitly affirms your unlimited
-        permission to run the unmodified Program.  The output from running a
-        covered work is covered by this License only if the output, given its
-        content, constitutes a covered work.  This License acknowledges your
-        rights of fair use or other equivalent, as provided by copyright law.
-        
-          You may make, run and propagate covered works that you do not
-        convey, without conditions so long as your license otherwise remains
-        in force.  You may convey covered works to others for the sole purpose
-        of having them make modifications exclusively for you, or provide you
-        with facilities for running those works, provided that you comply with
-        the terms of this License in conveying all material for which you do
-        not control copyright.  Those thus making or running the covered works
-        for you must do so exclusively on your behalf, under your direction
-        and control, on terms that prohibit them from making any copies of
-        your copyrighted material outside their relationship with you.
-        
-          Conveying under any other circumstances is permitted solely under
-        the conditions stated below.  Sublicensing is not allowed; section 10
-        makes it unnecessary.
-        
-          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-        
-          No covered work shall be deemed part of an effective technological
-        measure under any applicable law fulfilling obligations under article
-        11 of the WIPO copyright treaty adopted on 20 December 1996, or
-        similar laws prohibiting or restricting circumvention of such
-        measures.
-        
-          When you convey a covered work, you waive any legal power to forbid
-        circumvention of technological measures to the extent such circumvention
-        is effected by exercising rights under this License with respect to
-        the covered work, and you disclaim any intention to limit operation or
-        modification of the work as a means of enforcing, against the work's
-        users, your or third parties' legal rights to forbid circumvention of
-        technological measures.
-        
-          4. Conveying Verbatim Copies.
-        
-          You may convey verbatim copies of the Program's source code as you
-        receive it, in any medium, provided that you conspicuously and
-        appropriately publish on each copy an appropriate copyright notice;
-        keep intact all notices stating that this License and any
-        non-permissive terms added in accord with section 7 apply to the code;
-        keep intact all notices of the absence of any warranty; and give all
-        recipients a copy of this License along with the Program.
-        
-          You may charge any price or no price for each copy that you convey,
-        and you may offer support or warranty protection for a fee.
-        
-          5. Conveying Modified Source Versions.
-        
-          You may convey a work based on the Program, or the modifications to
-        produce it from the Program, in the form of source code under the
-        terms of section 4, provided that you also meet all of these conditions:
-        
-            a) The work must carry prominent notices stating that you modified
-            it, and giving a relevant date.
-        
-            b) The work must carry prominent notices stating that it is
-            released under this License and any conditions added under section
-            7.  This requirement modifies the requirement in section 4 to
-            "keep intact all notices".
-        
-            c) You must license the entire work, as a whole, under this
-            License to anyone who comes into possession of a copy.  This
-            License will therefore apply, along with any applicable section 7
-            additional terms, to the whole of the work, and all its parts,
-            regardless of how they are packaged.  This License gives no
-            permission to license the work in any other way, but it does not
-            invalidate such permission if you have separately received it.
-        
-            d) If the work has interactive user interfaces, each must display
-            Appropriate Legal Notices; however, if the Program has interactive
-            interfaces that do not display Appropriate Legal Notices, your
-            work need not make them do so.
-        
-          A compilation of a covered work with other separate and independent
-        works, which are not by their nature extensions of the covered work,
-        and which are not combined with it such as to form a larger program,
-        in or on a volume of a storage or distribution medium, is called an
-        "aggregate" if the compilation and its resulting copyright are not
-        used to limit the access or legal rights of the compilation's users
-        beyond what the individual works permit.  Inclusion of a covered work
-        in an aggregate does not cause this License to apply to the other
-        parts of the aggregate.
-        
-          6. Conveying Non-Source Forms.
-        
-          You may convey a covered work in object code form under the terms
-        of sections 4 and 5, provided that you also convey the
-        machine-readable Corresponding Source under the terms of this License,
-        in one of these ways:
-        
-            a) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by the
-            Corresponding Source fixed on a durable physical medium
-            customarily used for software interchange.
-        
-            b) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by a
-            written offer, valid for at least three years and valid for as
-            long as you offer spare parts or customer support for that product
-            model, to give anyone who possesses the object code either (1) a
-            copy of the Corresponding Source for all the software in the
-            product that is covered by this License, on a durable physical
-            medium customarily used for software interchange, for a price no
-            more than your reasonable cost of physically performing this
-            conveying of source, or (2) access to copy the
-            Corresponding Source from a network server at no charge.
-        
-            c) Convey individual copies of the object code with a copy of the
-            written offer to provide the Corresponding Source.  This
-            alternative is allowed only occasionally and noncommercially, and
-            only if you received the object code with such an offer, in accord
-            with subsection 6b.
-        
-            d) Convey the object code by offering access from a designated
-            place (gratis or for a charge), and offer equivalent access to the
-            Corresponding Source in the same way through the same place at no
-            further charge.  You need not require recipients to copy the
-            Corresponding Source along with the object code.  If the place to
-            copy the object code is a network server, the Corresponding Source
-            may be on a different server (operated by you or a third party)
-            that supports equivalent copying facilities, provided you maintain
-            clear directions next to the object code saying where to find the
-            Corresponding Source.  Regardless of what server hosts the
-            Corresponding Source, you remain obligated to ensure that it is
-            available for as long as needed to satisfy these requirements.
-        
-            e) Convey the object code using peer-to-peer transmission, provided
-            you inform other peers where the object code and Corresponding
-            Source of the work are being offered to the general public at no
-            charge under subsection 6d.
-        
-          A separable portion of the object code, whose source code is excluded
-        from the Corresponding Source as a System Library, need not be
-        included in conveying the object code work.
-        
-          A "User Product" is either (1) a "consumer product", which means any
-        tangible personal property which is normally used for personal, family,
-        or household purposes, or (2) anything designed or sold for incorporation
-        into a dwelling.  In determining whether a product is a consumer product,
-        doubtful cases shall be resolved in favor of coverage.  For a particular
-        product received by a particular user, "normally used" refers to a
-        typical or common use of that class of product, regardless of the status
-        of the particular user or of the way in which the particular user
-        actually uses, or expects or is expected to use, the product.  A product
-        is a consumer product regardless of whether the product has substantial
-        commercial, industrial or non-consumer uses, unless such uses represent
-        the only significant mode of use of the product.
-        
-          "Installation Information" for a User Product means any methods,
-        procedures, authorization keys, or other information required to install
-        and execute modified versions of a covered work in that User Product from
-        a modified version of its Corresponding Source.  The information must
-        suffice to ensure that the continued functioning of the modified object
-        code is in no case prevented or interfered with solely because
-        modification has been made.
-        
-          If you convey an object code work under this section in, or with, or
-        specifically for use in, a User Product, and the conveying occurs as
-        part of a transaction in which the right of possession and use of the
-        User Product is transferred to the recipient in perpetuity or for a
-        fixed term (regardless of how the transaction is characterized), the
-        Corresponding Source conveyed under this section must be accompanied
-        by the Installation Information.  But this requirement does not apply
-        if neither you nor any third party retains the ability to install
-        modified object code on the User Product (for example, the work has
-        been installed in ROM).
-        
-          The requirement to provide Installation Information does not include a
-        requirement to continue to provide support service, warranty, or updates
-        for a work that has been modified or installed by the recipient, or for
-        the User Product in which it has been modified or installed.  Access to a
-        network may be denied when the modification itself materially and
-        adversely affects the operation of the network or violates the rules and
-        protocols for communication across the network.
-        
-          Corresponding Source conveyed, and Installation Information provided,
-        in accord with this section must be in a format that is publicly
-        documented (and with an implementation available to the public in
-        source code form), and must require no special password or key for
-        unpacking, reading or copying.
-        
-          7. Additional Terms.
-        
-          "Additional permissions" are terms that supplement the terms of this
-        License by making exceptions from one or more of its conditions.
-        Additional permissions that are applicable to the entire Program shall
-        be treated as though they were included in this License, to the extent
-        that they are valid under applicable law.  If additional permissions
-        apply only to part of the Program, that part may be used separately
-        under those permissions, but the entire Program remains governed by
-        this License without regard to the additional permissions.
-        
-          When you convey a copy of a covered work, you may at your option
-        remove any additional permissions from that copy, or from any part of
-        it.  (Additional permissions may be written to require their own
-        removal in certain cases when you modify the work.)  You may place
-        additional permissions on material, added by you to a covered work,
-        for which you have or can give appropriate copyright permission.
-        
-          Notwithstanding any other provision of this License, for material you
-        add to a covered work, you may (if authorized by the copyright holders of
-        that material) supplement the terms of this License with terms:
-        
-            a) Disclaiming warranty or limiting liability differently from the
-            terms of sections 15 and 16 of this License; or
-        
-            b) Requiring preservation of specified reasonable legal notices or
-            author attributions in that material or in the Appropriate Legal
-            Notices displayed by works containing it; or
-        
-            c) Prohibiting misrepresentation of the origin of that material, or
-            requiring that modified versions of such material be marked in
-            reasonable ways as different from the original version; or
-        
-            d) Limiting the use for publicity purposes of names of licensors or
-            authors of the material; or
-        
-            e) Declining to grant rights under trademark law for use of some
-            trade names, trademarks, or service marks; or
-        
-            f) Requiring indemnification of licensors and authors of that
-            material by anyone who conveys the material (or modified versions of
-            it) with contractual assumptions of liability to the recipient, for
-            any liability that these contractual assumptions directly impose on
-            those licensors and authors.
-        
-          All other non-permissive additional terms are considered "further
-        restrictions" within the meaning of section 10.  If the Program as you
-        received it, or any part of it, contains a notice stating that it is
-        governed by this License along with a term that is a further
-        restriction, you may remove that term.  If a license document contains
-        a further restriction but permits relicensing or conveying under this
-        License, you may add to a covered work material governed by the terms
-        of that license document, provided that the further restriction does
-        not survive such relicensing or conveying.
-        
-          If you add terms to a covered work in accord with this section, you
-        must place, in the relevant source files, a statement of the
-        additional terms that apply to those files, or a notice indicating
-        where to find the applicable terms.
-        
-          Additional terms, permissive or non-permissive, may be stated in the
-        form of a separately written license, or stated as exceptions;
-        the above requirements apply either way.
-        
-          8. Termination.
-        
-          You may not propagate or modify a covered work except as expressly
-        provided under this License.  Any attempt otherwise to propagate or
-        modify it is void, and will automatically terminate your rights under
-        this License (including any patent licenses granted under the third
-        paragraph of section 11).
-        
-          However, if you cease all violation of this License, then your
-        license from a particular copyright holder is reinstated (a)
-        provisionally, unless and until the copyright holder explicitly and
-        finally terminates your license, and (b) permanently, if the copyright
-        holder fails to notify you of the violation by some reasonable means
-        prior to 60 days after the cessation.
-        
-          Moreover, your license from a particular copyright holder is
-        reinstated permanently if the copyright holder notifies you of the
-        violation by some reasonable means, this is the first time you have
-        received notice of violation of this License (for any work) from that
-        copyright holder, and you cure the violation prior to 30 days after
-        your receipt of the notice.
-        
-          Termination of your rights under this section does not terminate the
-        licenses of parties who have received copies or rights from you under
-        this License.  If your rights have been terminated and not permanently
-        reinstated, you do not qualify to receive new licenses for the same
-        material under section 10.
-        
-          9. Acceptance Not Required for Having Copies.
-        
-          You are not required to accept this License in order to receive or
-        run a copy of the Program.  Ancillary propagation of a covered work
-        occurring solely as a consequence of using peer-to-peer transmission
-        to receive a copy likewise does not require acceptance.  However,
-        nothing other than this License grants you permission to propagate or
-        modify any covered work.  These actions infringe copyright if you do
-        not accept this License.  Therefore, by modifying or propagating a
-        covered work, you indicate your acceptance of this License to do so.
-        
-          10. Automatic Licensing of Downstream Recipients.
-        
-          Each time you convey a covered work, the recipient automatically
-        receives a license from the original licensors, to run, modify and
-        propagate that work, subject to this License.  You are not responsible
-        for enforcing compliance by third parties with this License.
-        
-          An "entity transaction" is a transaction transferring control of an
-        organization, or substantially all assets of one, or subdividing an
-        organization, or merging organizations.  If propagation of a covered
-        work results from an entity transaction, each party to that
-        transaction who receives a copy of the work also receives whatever
-        licenses to the work the party's predecessor in interest had or could
-        give under the previous paragraph, plus a right to possession of the
-        Corresponding Source of the work from the predecessor in interest, if
-        the predecessor has it or can get it with reasonable efforts.
-        
-          You may not impose any further restrictions on the exercise of the
-        rights granted or affirmed under this License.  For example, you may
-        not impose a license fee, royalty, or other charge for exercise of
-        rights granted under this License, and you may not initiate litigation
-        (including a cross-claim or counterclaim in a lawsuit) alleging that
-        any patent claim is infringed by making, using, selling, offering for
-        sale, or importing the Program or any portion of it.
-        
-          11. Patents.
-        
-          A "contributor" is a copyright holder who authorizes use under this
-        License of the Program or a work on which the Program is based.  The
-        work thus licensed is called the contributor's "contributor version".
-        
-          A contributor's "essential patent claims" are all patent claims
-        owned or controlled by the contributor, whether already acquired or
-        hereafter acquired, that would be infringed by some manner, permitted
-        by this License, of making, using, or selling its contributor version,
-        but do not include claims that would be infringed only as a
-        consequence of further modification of the contributor version.  For
-        purposes of this definition, "control" includes the right to grant
-        patent sublicenses in a manner consistent with the requirements of
-        this License.
-        
-          Each contributor grants you a non-exclusive, worldwide, royalty-free
-        patent license under the contributor's essential patent claims, to
-        make, use, sell, offer for sale, import and otherwise run, modify and
-        propagate the contents of its contributor version.
-        
-          In the following three paragraphs, a "patent license" is any express
-        agreement or commitment, however denominated, not to enforce a patent
-        (such as an express permission to practice a patent or covenant not to
-        sue for patent infringement).  To "grant" such a patent license to a
-        party means to make such an agreement or commitment not to enforce a
-        patent against the party.
-        
-          If you convey a covered work, knowingly relying on a patent license,
-        and the Corresponding Source of the work is not available for anyone
-        to copy, free of charge and under the terms of this License, through a
-        publicly available network server or other readily accessible means,
-        then you must either (1) cause the Corresponding Source to be so
-        available, or (2) arrange to deprive yourself of the benefit of the
-        patent license for this particular work, or (3) arrange, in a manner
-        consistent with the requirements of this License, to extend the patent
-        license to downstream recipients.  "Knowingly relying" means you have
-        actual knowledge that, but for the patent license, your conveying the
-        covered work in a country, or your recipient's use of the covered work
-        in a country, would infringe one or more identifiable patents in that
-        country that you have reason to believe are valid.
-        
-          If, pursuant to or in connection with a single transaction or
-        arrangement, you convey, or propagate by procuring conveyance of, a
-        covered work, and grant a patent license to some of the parties
-        receiving the covered work authorizing them to use, propagate, modify
-        or convey a specific copy of the covered work, then the patent license
-        you grant is automatically extended to all recipients of the covered
-        work and works based on it.
-        
-          A patent license is "discriminatory" if it does not include within
-        the scope of its coverage, prohibits the exercise of, or is
-        conditioned on the non-exercise of one or more of the rights that are
-        specifically granted under this License.  You may not convey a covered
-        work if you are a party to an arrangement with a third party that is
-        in the business of distributing software, under which you make payment
-        to the third party based on the extent of your activity of conveying
-        the work, and under which the third party grants, to any of the
-        parties who would receive the covered work from you, a discriminatory
-        patent license (a) in connection with copies of the covered work
-        conveyed by you (or copies made from those copies), or (b) primarily
-        for and in connection with specific products or compilations that
-        contain the covered work, unless you entered into that arrangement,
-        or that patent license was granted, prior to 28 March 2007.
-        
-          Nothing in this License shall be construed as excluding or limiting
-        any implied license or other defenses to infringement that may
-        otherwise be available to you under applicable patent law.
-        
-          12. No Surrender of Others' Freedom.
-        
-          If conditions are imposed on you (whether by court order, agreement or
-        otherwise) that contradict the conditions of this License, they do not
-        excuse you from the conditions of this License.  If you cannot convey a
-        covered work so as to satisfy simultaneously your obligations under this
-        License and any other pertinent obligations, then as a consequence you may
-        not convey it at all.  For example, if you agree to terms that obligate you
-        to collect a royalty for further conveying from those to whom you convey
-        the Program, the only way you could satisfy both those terms and this
-        License would be to refrain entirely from conveying the Program.
-        
-          13. Use with the GNU Affero General Public License.
-        
-          Notwithstanding any other provision of this License, you have
-        permission to link or combine any covered work with a work licensed
-        under version 3 of the GNU Affero General Public License into a single
-        combined work, and to convey the resulting work.  The terms of this
-        License will continue to apply to the part which is the covered work,
-        but the special requirements of the GNU Affero General Public License,
-        section 13, concerning interaction through a network will apply to the
-        combination as such.
-        
-          14. Revised Versions of this License.
-        
-          The Free Software Foundation may publish revised and/or new versions of
-        the GNU General Public License from time to time.  Such new versions will
-        be similar in spirit to the present version, but may differ in detail to
-        address new problems or concerns.
-        
-          Each version is given a distinguishing version number.  If the
-        Program specifies that a certain numbered version of the GNU General
-        Public License "or any later version" applies to it, you have the
-        option of following the terms and conditions either of that numbered
-        version or of any later version published by the Free Software
-        Foundation.  If the Program does not specify a version number of the
-        GNU General Public License, you may choose any version ever published
-        by the Free Software Foundation.
-        
-          If the Program specifies that a proxy can decide which future
-        versions of the GNU General Public License can be used, that proxy's
-        public statement of acceptance of a version permanently authorizes you
-        to choose that version for the Program.
-        
-          Later license versions may give you additional or different
-        permissions.  However, no additional obligations are imposed on any
-        author or copyright holder as a result of your choosing to follow a
-        later version.
-        
-          15. Disclaimer of Warranty.
-        
-          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-        
-          16. Limitation of Liability.
-        
-          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-        SUCH DAMAGES.
-        
-          17. Interpretation of Sections 15 and 16.
-        
-          If the disclaimer of warranty and limitation of liability provided
-        above cannot be given local legal effect according to their terms,
-        reviewing courts shall apply local law that most closely approximates
-        an absolute waiver of all civil liability in connection with the
-        Program, unless a warranty or assumption of liability accompanies a
-        copy of the Program in return for a fee.
-        
-                             END OF TERMS AND CONDITIONS
-Project-URL: Homepage, https://codeberg.org/mmatous/seal
-Project-URL: Bug Tracker, https://codeberg.org/mmatous/seal/issues
-Keywords: area,distance decay,ecology,extent,grain,richness,SAR,scale,species,species-area
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: alive-progress~=3.1
-Requires-Dist: numba~=0.59
-Requires-Dist: numexpr~=2.9
-Requires-Dist: pandas[plot]~=2.2
-Requires-Dist: pyhocon~=0.3
-Requires-Dist: seaborn~=0.13.2
-Provides-Extra: dev
-Requires-Dist: mypy~=1.6; extra == "dev"
-Requires-Dist: pandas-stubs~=2.0; extra == "dev"
-Requires-Dist: pytest~=7.4; extra == "dev"
-Requires-Dist: pytest-cov~=4.1; extra == "dev"
-Requires-Dist: ruff~=0.2.0; extra == "dev"
-Provides-Extra: alt-plot
-Requires-Dist: plotly; extra == "alt-plot"
-
-# seal
-
-Perform richness-extent-grain analyses inspired by Palmer & White
-([doi:10.1086/285704](https://doi.org/10.1086/285704), [doi:10.17615/n84a-pd17](https://doi.org/10.17615/n84a-pd17))
-
-## Setup
-
-### Installation
-
-Simply download `seal` from Codeberg [releases](https://codeberg.org/mmatous/seal)
-or clone the repository using git.
-
-### First run
-
-Done only when installing and running the tool for the first time.
-
-Open the project directory in your
-command-line interface.
-
-#### Linux
-
-In POSIX-compatible shell run:
-```bash
-source ./src/firstrun.sh
-```
-
-#### Windows
-
-In PowerShell Run:
-```
-./src/firstrun.ps1
-```
-
-If you encounter an error such as `./src/firstrun.ps1 cannot be loaded because running scripts is disabled on this system`
-on Windows, it means the script was blocked by your
-security settings. In that case either unblock
-the script e.g. using the [`Unblock-File` or `Set-ExecutionPolicy` cmdlets](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.security/set-executionpolicy?view=powershell-7.4#example-7-unblock-a-script-to-run-it-without-changing-the-execution-policy) or run the
-necessary commands manually.
-
-```
-python -m venv ./venv
-./venv/Scripts/Activate.ps1
-pip install .[dev]
-```
-
-
-You should see `(venv)` before your shell prompt now and `seal --help`
-should run the tool without errors. Continue with [Usage](#Usage).
-
-### Subsequent runs
-
-Done when running the tool any time after the first initial installation.
-
-Linux:
-```
-source ./venv/bin/activate
-seal <subcommand>
-```
-
-Windows PowerShell:
-```
-./venv/Scripts/activate.ps1
-seal <subcommand>
-```
-
-## Usage
-
-One would generally want to use `preprocess`, `analyse` and `plot` subcommands in this order.
-`misc` subcommand contains several scripts that
-may be useful while converting or modifying either datasets or quadrat
-lists for analysis.
-
-More detailed help can be accesed by `seal --help`
-or `seal <subcommand> --help`.
-
-### Preprocess
-
-Preprocess will ensure given dataset is fit to be processed
-by the `analyse` command by e.g. sanitizing strings,
-warning for missing values or
-checking whether species column remains consistent with
-name, morph and phase.
-
-Example:
-```
-seal preprocess --dataset ./datasets/raw.csv --output ./datasets/clean.csv
-```
-
-
-### Analysis
-
-`analyse` subcommand ingests [taskfile](./tasks/example-task.conf)
-to perform analyses requested therein.
-
-Example:
-```
-seal analyse --taskfile ./tasks/example-task.conf
-```
-
-Currently supported analyses are:
-
-#### a1 - Overview
-
-This analysis calculates per-quadrat species number
-and number of encountered individuals for each level.
-
-The additional data contain general description of given dataset and various smaller statistics for each level.
-Such statistics include, for example, the most common value, mean, median, min and such for each data column.
-
-This helps familiarize oneself with the data and serves as a basic check of the levels-creating strategy.
-
-#### a2 - Species-area relationship
-
-This analysis shows relationship between species richness and area sampled.
-
-Species-area curve is calculated for each level by accumulating quadrats
-and tallying the number of species. Since this method is sensitive to order of the
-quadrats, number of permutations must be specified and their arithmetic mean is plotted.
-
-The additional data contain statistics of the calculated results.
-
-#### a3 - Distance-dependent species difference
-
-This analysis creates pairwise difference of sets of encountered species
-in two quadrats.
-
-Result is the difference as a function of distance of the quadrats.
-
-#### a4 - Radius richness
-
-This analysis calculates the number of species within various distance intervals (interval's width is set by
-the `interval-step` parameter)
-from each quadrat. The radius forms a belt of sorts with a specified width.
-
-We recommend using the size of the smallest quadrat as the smallest possible step.
-
-#### a5 - Ratio of observed and expected species
-
-This analysis calculates the ratio of observed and expected number of species for each
-quadrat. The expected value is calculated as $$\sum_{}P_i * (1 - P_i)$$  where P<sub>i</sub> is the proportion
-of quadrats occupied by species _i_ and the summation is over all the species in the study grid.
-
-#### a6 - Ratio of shared and unique species
-
-This analysis calculates several ratios for pairs of quadrats based on their distance.
-1) Ratio of shared species among the quadrats and exclusive species among the quadrats.
-2) Ratio of shared species among the quadrats and all
-the species in the dataset.
-3) Ratio of shared species among the quadrats and
-all the species in the study grid.
-
-
-#### a7 - Jaccard dissimilarity
-
-This analysis calculates Jaccard dissimilarity with regards to species between
-all possible pairs of quadrats.
-
-Result is plotted as dissimilarity against the distance
-of the quadrats.
-
-Jaccard dissimilarity between quadrats _a_ and _b_ is calculated as:
-$$J(a, b) = 1 - \frac{intersect_{ab}}{intersect_{ab} + exclusive_a + exclusive_b}$$
-
-
-
-### Ploting
-
-`plot` subcommand ingests [taskfile](./tasks/example-task.conf) to detect results of previous analyses
-and present them as graphs.
-
-Generated graphs will be saved to the same directory as
-analysis results.
-
-Example:
-```
-seal plot --taskfile ./tasks/example-task.conf
-```
-
-### Misc
-
-`misc` subcommand is a kitchen sink of opinionated
-convenience tools.
-
-## Development
-
-For unit tests run `python -m doctest ./src/seal/<file>`.
-
-For functional tests run `pytest`.
-
-### License
-The source code—including the tests and documentation—is licensed under [GPLv3](./LICENSE)
-
-`./datasets/data-bmd-sl.csv` is licensed under [CC-BY-SA-4.0](./datasets/LICENSE)
-
-[aopk-fish.csv](./datasets/aopk-fish.csv) was provided under [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/)
-by AOPK ČR, Nálezová databáze ochrany přírody, on-line database portal.nature.cz. Downloaded 2024-02-05.
+Metadata-Version: 2.1
+Name: seal-tool
+Version: 0.11.0
+Summary: A tool to perform richness-extent-grain analyses
+Author-email: Martin Matouš <m@matous.dev>, Barbora Winterová <winterova@mail.muni.cz>
+License:                     GNU GENERAL PUBLIC LICENSE
+                               Version 3, 29 June 2007
+        
+         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+         Everyone is permitted to copy and distribute verbatim copies
+         of this license document, but changing it is not allowed.
+        
+                                    Preamble
+        
+          The GNU General Public License is a free, copyleft license for
+        software and other kinds of works.
+        
+          The licenses for most software and other practical works are designed
+        to take away your freedom to share and change the works.  By contrast,
+        the GNU General Public License is intended to guarantee your freedom to
+        share and change all versions of a program--to make sure it remains free
+        software for all its users.  We, the Free Software Foundation, use the
+        GNU General Public License for most of our software; it applies also to
+        any other work released this way by its authors.  You can apply it to
+        your programs, too.
+        
+          When we speak of free software, we are referring to freedom, not
+        price.  Our General Public Licenses are designed to make sure that you
+        have the freedom to distribute copies of free software (and charge for
+        them if you wish), that you receive source code or can get it if you
+        want it, that you can change the software or use pieces of it in new
+        free programs, and that you know you can do these things.
+        
+          To protect your rights, we need to prevent others from denying you
+        these rights or asking you to surrender the rights.  Therefore, you have
+        certain responsibilities if you distribute copies of the software, or if
+        you modify it: responsibilities to respect the freedom of others.
+        
+          For example, if you distribute copies of such a program, whether
+        gratis or for a fee, you must pass on to the recipients the same
+        freedoms that you received.  You must make sure that they, too, receive
+        or can get the source code.  And you must show them these terms so they
+        know their rights.
+        
+          Developers that use the GNU GPL protect your rights with two steps:
+        (1) assert copyright on the software, and (2) offer you this License
+        giving you legal permission to copy, distribute and/or modify it.
+        
+          For the developers' and authors' protection, the GPL clearly explains
+        that there is no warranty for this free software.  For both users' and
+        authors' sake, the GPL requires that modified versions be marked as
+        changed, so that their problems will not be attributed erroneously to
+        authors of previous versions.
+        
+          Some devices are designed to deny users access to install or run
+        modified versions of the software inside them, although the manufacturer
+        can do so.  This is fundamentally incompatible with the aim of
+        protecting users' freedom to change the software.  The systematic
+        pattern of such abuse occurs in the area of products for individuals to
+        use, which is precisely where it is most unacceptable.  Therefore, we
+        have designed this version of the GPL to prohibit the practice for those
+        products.  If such problems arise substantially in other domains, we
+        stand ready to extend this provision to those domains in future versions
+        of the GPL, as needed to protect the freedom of users.
+        
+          Finally, every program is threatened constantly by software patents.
+        States should not allow patents to restrict development and use of
+        software on general-purpose computers, but in those that do, we wish to
+        avoid the special danger that patents applied to a free program could
+        make it effectively proprietary.  To prevent this, the GPL assures that
+        patents cannot be used to render the program non-free.
+        
+          The precise terms and conditions for copying, distribution and
+        modification follow.
+        
+                               TERMS AND CONDITIONS
+        
+          0. Definitions.
+        
+          "This License" refers to version 3 of the GNU General Public License.
+        
+          "Copyright" also means copyright-like laws that apply to other kinds of
+        works, such as semiconductor masks.
+        
+          "The Program" refers to any copyrightable work licensed under this
+        License.  Each licensee is addressed as "you".  "Licensees" and
+        "recipients" may be individuals or organizations.
+        
+          To "modify" a work means to copy from or adapt all or part of the work
+        in a fashion requiring copyright permission, other than the making of an
+        exact copy.  The resulting work is called a "modified version" of the
+        earlier work or a work "based on" the earlier work.
+        
+          A "covered work" means either the unmodified Program or a work based
+        on the Program.
+        
+          To "propagate" a work means to do anything with it that, without
+        permission, would make you directly or secondarily liable for
+        infringement under applicable copyright law, except executing it on a
+        computer or modifying a private copy.  Propagation includes copying,
+        distribution (with or without modification), making available to the
+        public, and in some countries other activities as well.
+        
+          To "convey" a work means any kind of propagation that enables other
+        parties to make or receive copies.  Mere interaction with a user through
+        a computer network, with no transfer of a copy, is not conveying.
+        
+          An interactive user interface displays "Appropriate Legal Notices"
+        to the extent that it includes a convenient and prominently visible
+        feature that (1) displays an appropriate copyright notice, and (2)
+        tells the user that there is no warranty for the work (except to the
+        extent that warranties are provided), that licensees may convey the
+        work under this License, and how to view a copy of this License.  If
+        the interface presents a list of user commands or options, such as a
+        menu, a prominent item in the list meets this criterion.
+        
+          1. Source Code.
+        
+          The "source code" for a work means the preferred form of the work
+        for making modifications to it.  "Object code" means any non-source
+        form of a work.
+        
+          A "Standard Interface" means an interface that either is an official
+        standard defined by a recognized standards body, or, in the case of
+        interfaces specified for a particular programming language, one that
+        is widely used among developers working in that language.
+        
+          The "System Libraries" of an executable work include anything, other
+        than the work as a whole, that (a) is included in the normal form of
+        packaging a Major Component, but which is not part of that Major
+        Component, and (b) serves only to enable use of the work with that
+        Major Component, or to implement a Standard Interface for which an
+        implementation is available to the public in source code form.  A
+        "Major Component", in this context, means a major essential component
+        (kernel, window system, and so on) of the specific operating system
+        (if any) on which the executable work runs, or a compiler used to
+        produce the work, or an object code interpreter used to run it.
+        
+          The "Corresponding Source" for a work in object code form means all
+        the source code needed to generate, install, and (for an executable
+        work) run the object code and to modify the work, including scripts to
+        control those activities.  However, it does not include the work's
+        System Libraries, or general-purpose tools or generally available free
+        programs which are used unmodified in performing those activities but
+        which are not part of the work.  For example, Corresponding Source
+        includes interface definition files associated with source files for
+        the work, and the source code for shared libraries and dynamically
+        linked subprograms that the work is specifically designed to require,
+        such as by intimate data communication or control flow between those
+        subprograms and other parts of the work.
+        
+          The Corresponding Source need not include anything that users
+        can regenerate automatically from other parts of the Corresponding
+        Source.
+        
+          The Corresponding Source for a work in source code form is that
+        same work.
+        
+          2. Basic Permissions.
+        
+          All rights granted under this License are granted for the term of
+        copyright on the Program, and are irrevocable provided the stated
+        conditions are met.  This License explicitly affirms your unlimited
+        permission to run the unmodified Program.  The output from running a
+        covered work is covered by this License only if the output, given its
+        content, constitutes a covered work.  This License acknowledges your
+        rights of fair use or other equivalent, as provided by copyright law.
+        
+          You may make, run and propagate covered works that you do not
+        convey, without conditions so long as your license otherwise remains
+        in force.  You may convey covered works to others for the sole purpose
+        of having them make modifications exclusively for you, or provide you
+        with facilities for running those works, provided that you comply with
+        the terms of this License in conveying all material for which you do
+        not control copyright.  Those thus making or running the covered works
+        for you must do so exclusively on your behalf, under your direction
+        and control, on terms that prohibit them from making any copies of
+        your copyrighted material outside their relationship with you.
+        
+          Conveying under any other circumstances is permitted solely under
+        the conditions stated below.  Sublicensing is not allowed; section 10
+        makes it unnecessary.
+        
+          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+        
+          No covered work shall be deemed part of an effective technological
+        measure under any applicable law fulfilling obligations under article
+        11 of the WIPO copyright treaty adopted on 20 December 1996, or
+        similar laws prohibiting or restricting circumvention of such
+        measures.
+        
+          When you convey a covered work, you waive any legal power to forbid
+        circumvention of technological measures to the extent such circumvention
+        is effected by exercising rights under this License with respect to
+        the covered work, and you disclaim any intention to limit operation or
+        modification of the work as a means of enforcing, against the work's
+        users, your or third parties' legal rights to forbid circumvention of
+        technological measures.
+        
+          4. Conveying Verbatim Copies.
+        
+          You may convey verbatim copies of the Program's source code as you
+        receive it, in any medium, provided that you conspicuously and
+        appropriately publish on each copy an appropriate copyright notice;
+        keep intact all notices stating that this License and any
+        non-permissive terms added in accord with section 7 apply to the code;
+        keep intact all notices of the absence of any warranty; and give all
+        recipients a copy of this License along with the Program.
+        
+          You may charge any price or no price for each copy that you convey,
+        and you may offer support or warranty protection for a fee.
+        
+          5. Conveying Modified Source Versions.
+        
+          You may convey a work based on the Program, or the modifications to
+        produce it from the Program, in the form of source code under the
+        terms of section 4, provided that you also meet all of these conditions:
+        
+            a) The work must carry prominent notices stating that you modified
+            it, and giving a relevant date.
+        
+            b) The work must carry prominent notices stating that it is
+            released under this License and any conditions added under section
+            7.  This requirement modifies the requirement in section 4 to
+            "keep intact all notices".
+        
+            c) You must license the entire work, as a whole, under this
+            License to anyone who comes into possession of a copy.  This
+            License will therefore apply, along with any applicable section 7
+            additional terms, to the whole of the work, and all its parts,
+            regardless of how they are packaged.  This License gives no
+            permission to license the work in any other way, but it does not
+            invalidate such permission if you have separately received it.
+        
+            d) If the work has interactive user interfaces, each must display
+            Appropriate Legal Notices; however, if the Program has interactive
+            interfaces that do not display Appropriate Legal Notices, your
+            work need not make them do so.
+        
+          A compilation of a covered work with other separate and independent
+        works, which are not by their nature extensions of the covered work,
+        and which are not combined with it such as to form a larger program,
+        in or on a volume of a storage or distribution medium, is called an
+        "aggregate" if the compilation and its resulting copyright are not
+        used to limit the access or legal rights of the compilation's users
+        beyond what the individual works permit.  Inclusion of a covered work
+        in an aggregate does not cause this License to apply to the other
+        parts of the aggregate.
+        
+          6. Conveying Non-Source Forms.
+        
+          You may convey a covered work in object code form under the terms
+        of sections 4 and 5, provided that you also convey the
+        machine-readable Corresponding Source under the terms of this License,
+        in one of these ways:
+        
+            a) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by the
+            Corresponding Source fixed on a durable physical medium
+            customarily used for software interchange.
+        
+            b) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by a
+            written offer, valid for at least three years and valid for as
+            long as you offer spare parts or customer support for that product
+            model, to give anyone who possesses the object code either (1) a
+            copy of the Corresponding Source for all the software in the
+            product that is covered by this License, on a durable physical
+            medium customarily used for software interchange, for a price no
+            more than your reasonable cost of physically performing this
+            conveying of source, or (2) access to copy the
+            Corresponding Source from a network server at no charge.
+        
+            c) Convey individual copies of the object code with a copy of the
+            written offer to provide the Corresponding Source.  This
+            alternative is allowed only occasionally and noncommercially, and
+            only if you received the object code with such an offer, in accord
+            with subsection 6b.
+        
+            d) Convey the object code by offering access from a designated
+            place (gratis or for a charge), and offer equivalent access to the
+            Corresponding Source in the same way through the same place at no
+            further charge.  You need not require recipients to copy the
+            Corresponding Source along with the object code.  If the place to
+            copy the object code is a network server, the Corresponding Source
+            may be on a different server (operated by you or a third party)
+            that supports equivalent copying facilities, provided you maintain
+            clear directions next to the object code saying where to find the
+            Corresponding Source.  Regardless of what server hosts the
+            Corresponding Source, you remain obligated to ensure that it is
+            available for as long as needed to satisfy these requirements.
+        
+            e) Convey the object code using peer-to-peer transmission, provided
+            you inform other peers where the object code and Corresponding
+            Source of the work are being offered to the general public at no
+            charge under subsection 6d.
+        
+          A separable portion of the object code, whose source code is excluded
+        from the Corresponding Source as a System Library, need not be
+        included in conveying the object code work.
+        
+          A "User Product" is either (1) a "consumer product", which means any
+        tangible personal property which is normally used for personal, family,
+        or household purposes, or (2) anything designed or sold for incorporation
+        into a dwelling.  In determining whether a product is a consumer product,
+        doubtful cases shall be resolved in favor of coverage.  For a particular
+        product received by a particular user, "normally used" refers to a
+        typical or common use of that class of product, regardless of the status
+        of the particular user or of the way in which the particular user
+        actually uses, or expects or is expected to use, the product.  A product
+        is a consumer product regardless of whether the product has substantial
+        commercial, industrial or non-consumer uses, unless such uses represent
+        the only significant mode of use of the product.
+        
+          "Installation Information" for a User Product means any methods,
+        procedures, authorization keys, or other information required to install
+        and execute modified versions of a covered work in that User Product from
+        a modified version of its Corresponding Source.  The information must
+        suffice to ensure that the continued functioning of the modified object
+        code is in no case prevented or interfered with solely because
+        modification has been made.
+        
+          If you convey an object code work under this section in, or with, or
+        specifically for use in, a User Product, and the conveying occurs as
+        part of a transaction in which the right of possession and use of the
+        User Product is transferred to the recipient in perpetuity or for a
+        fixed term (regardless of how the transaction is characterized), the
+        Corresponding Source conveyed under this section must be accompanied
+        by the Installation Information.  But this requirement does not apply
+        if neither you nor any third party retains the ability to install
+        modified object code on the User Product (for example, the work has
+        been installed in ROM).
+        
+          The requirement to provide Installation Information does not include a
+        requirement to continue to provide support service, warranty, or updates
+        for a work that has been modified or installed by the recipient, or for
+        the User Product in which it has been modified or installed.  Access to a
+        network may be denied when the modification itself materially and
+        adversely affects the operation of the network or violates the rules and
+        protocols for communication across the network.
+        
+          Corresponding Source conveyed, and Installation Information provided,
+        in accord with this section must be in a format that is publicly
+        documented (and with an implementation available to the public in
+        source code form), and must require no special password or key for
+        unpacking, reading or copying.
+        
+          7. Additional Terms.
+        
+          "Additional permissions" are terms that supplement the terms of this
+        License by making exceptions from one or more of its conditions.
+        Additional permissions that are applicable to the entire Program shall
+        be treated as though they were included in this License, to the extent
+        that they are valid under applicable law.  If additional permissions
+        apply only to part of the Program, that part may be used separately
+        under those permissions, but the entire Program remains governed by
+        this License without regard to the additional permissions.
+        
+          When you convey a copy of a covered work, you may at your option
+        remove any additional permissions from that copy, or from any part of
+        it.  (Additional permissions may be written to require their own
+        removal in certain cases when you modify the work.)  You may place
+        additional permissions on material, added by you to a covered work,
+        for which you have or can give appropriate copyright permission.
+        
+          Notwithstanding any other provision of this License, for material you
+        add to a covered work, you may (if authorized by the copyright holders of
+        that material) supplement the terms of this License with terms:
+        
+            a) Disclaiming warranty or limiting liability differently from the
+            terms of sections 15 and 16 of this License; or
+        
+            b) Requiring preservation of specified reasonable legal notices or
+            author attributions in that material or in the Appropriate Legal
+            Notices displayed by works containing it; or
+        
+            c) Prohibiting misrepresentation of the origin of that material, or
+            requiring that modified versions of such material be marked in
+            reasonable ways as different from the original version; or
+        
+            d) Limiting the use for publicity purposes of names of licensors or
+            authors of the material; or
+        
+            e) Declining to grant rights under trademark law for use of some
+            trade names, trademarks, or service marks; or
+        
+            f) Requiring indemnification of licensors and authors of that
+            material by anyone who conveys the material (or modified versions of
+            it) with contractual assumptions of liability to the recipient, for
+            any liability that these contractual assumptions directly impose on
+            those licensors and authors.
+        
+          All other non-permissive additional terms are considered "further
+        restrictions" within the meaning of section 10.  If the Program as you
+        received it, or any part of it, contains a notice stating that it is
+        governed by this License along with a term that is a further
+        restriction, you may remove that term.  If a license document contains
+        a further restriction but permits relicensing or conveying under this
+        License, you may add to a covered work material governed by the terms
+        of that license document, provided that the further restriction does
+        not survive such relicensing or conveying.
+        
+          If you add terms to a covered work in accord with this section, you
+        must place, in the relevant source files, a statement of the
+        additional terms that apply to those files, or a notice indicating
+        where to find the applicable terms.
+        
+          Additional terms, permissive or non-permissive, may be stated in the
+        form of a separately written license, or stated as exceptions;
+        the above requirements apply either way.
+        
+          8. Termination.
+        
+          You may not propagate or modify a covered work except as expressly
+        provided under this License.  Any attempt otherwise to propagate or
+        modify it is void, and will automatically terminate your rights under
+        this License (including any patent licenses granted under the third
+        paragraph of section 11).
+        
+          However, if you cease all violation of this License, then your
+        license from a particular copyright holder is reinstated (a)
+        provisionally, unless and until the copyright holder explicitly and
+        finally terminates your license, and (b) permanently, if the copyright
+        holder fails to notify you of the violation by some reasonable means
+        prior to 60 days after the cessation.
+        
+          Moreover, your license from a particular copyright holder is
+        reinstated permanently if the copyright holder notifies you of the
+        violation by some reasonable means, this is the first time you have
+        received notice of violation of this License (for any work) from that
+        copyright holder, and you cure the violation prior to 30 days after
+        your receipt of the notice.
+        
+          Termination of your rights under this section does not terminate the
+        licenses of parties who have received copies or rights from you under
+        this License.  If your rights have been terminated and not permanently
+        reinstated, you do not qualify to receive new licenses for the same
+        material under section 10.
+        
+          9. Acceptance Not Required for Having Copies.
+        
+          You are not required to accept this License in order to receive or
+        run a copy of the Program.  Ancillary propagation of a covered work
+        occurring solely as a consequence of using peer-to-peer transmission
+        to receive a copy likewise does not require acceptance.  However,
+        nothing other than this License grants you permission to propagate or
+        modify any covered work.  These actions infringe copyright if you do
+        not accept this License.  Therefore, by modifying or propagating a
+        covered work, you indicate your acceptance of this License to do so.
+        
+          10. Automatic Licensing of Downstream Recipients.
+        
+          Each time you convey a covered work, the recipient automatically
+        receives a license from the original licensors, to run, modify and
+        propagate that work, subject to this License.  You are not responsible
+        for enforcing compliance by third parties with this License.
+        
+          An "entity transaction" is a transaction transferring control of an
+        organization, or substantially all assets of one, or subdividing an
+        organization, or merging organizations.  If propagation of a covered
+        work results from an entity transaction, each party to that
+        transaction who receives a copy of the work also receives whatever
+        licenses to the work the party's predecessor in interest had or could
+        give under the previous paragraph, plus a right to possession of the
+        Corresponding Source of the work from the predecessor in interest, if
+        the predecessor has it or can get it with reasonable efforts.
+        
+          You may not impose any further restrictions on the exercise of the
+        rights granted or affirmed under this License.  For example, you may
+        not impose a license fee, royalty, or other charge for exercise of
+        rights granted under this License, and you may not initiate litigation
+        (including a cross-claim or counterclaim in a lawsuit) alleging that
+        any patent claim is infringed by making, using, selling, offering for
+        sale, or importing the Program or any portion of it.
+        
+          11. Patents.
+        
+          A "contributor" is a copyright holder who authorizes use under this
+        License of the Program or a work on which the Program is based.  The
+        work thus licensed is called the contributor's "contributor version".
+        
+          A contributor's "essential patent claims" are all patent claims
+        owned or controlled by the contributor, whether already acquired or
+        hereafter acquired, that would be infringed by some manner, permitted
+        by this License, of making, using, or selling its contributor version,
+        but do not include claims that would be infringed only as a
+        consequence of further modification of the contributor version.  For
+        purposes of this definition, "control" includes the right to grant
+        patent sublicenses in a manner consistent with the requirements of
+        this License.
+        
+          Each contributor grants you a non-exclusive, worldwide, royalty-free
+        patent license under the contributor's essential patent claims, to
+        make, use, sell, offer for sale, import and otherwise run, modify and
+        propagate the contents of its contributor version.
+        
+          In the following three paragraphs, a "patent license" is any express
+        agreement or commitment, however denominated, not to enforce a patent
+        (such as an express permission to practice a patent or covenant not to
+        sue for patent infringement).  To "grant" such a patent license to a
+        party means to make such an agreement or commitment not to enforce a
+        patent against the party.
+        
+          If you convey a covered work, knowingly relying on a patent license,
+        and the Corresponding Source of the work is not available for anyone
+        to copy, free of charge and under the terms of this License, through a
+        publicly available network server or other readily accessible means,
+        then you must either (1) cause the Corresponding Source to be so
+        available, or (2) arrange to deprive yourself of the benefit of the
+        patent license for this particular work, or (3) arrange, in a manner
+        consistent with the requirements of this License, to extend the patent
+        license to downstream recipients.  "Knowingly relying" means you have
+        actual knowledge that, but for the patent license, your conveying the
+        covered work in a country, or your recipient's use of the covered work
+        in a country, would infringe one or more identifiable patents in that
+        country that you have reason to believe are valid.
+        
+          If, pursuant to or in connection with a single transaction or
+        arrangement, you convey, or propagate by procuring conveyance of, a
+        covered work, and grant a patent license to some of the parties
+        receiving the covered work authorizing them to use, propagate, modify
+        or convey a specific copy of the covered work, then the patent license
+        you grant is automatically extended to all recipients of the covered
+        work and works based on it.
+        
+          A patent license is "discriminatory" if it does not include within
+        the scope of its coverage, prohibits the exercise of, or is
+        conditioned on the non-exercise of one or more of the rights that are
+        specifically granted under this License.  You may not convey a covered
+        work if you are a party to an arrangement with a third party that is
+        in the business of distributing software, under which you make payment
+        to the third party based on the extent of your activity of conveying
+        the work, and under which the third party grants, to any of the
+        parties who would receive the covered work from you, a discriminatory
+        patent license (a) in connection with copies of the covered work
+        conveyed by you (or copies made from those copies), or (b) primarily
+        for and in connection with specific products or compilations that
+        contain the covered work, unless you entered into that arrangement,
+        or that patent license was granted, prior to 28 March 2007.
+        
+          Nothing in this License shall be construed as excluding or limiting
+        any implied license or other defenses to infringement that may
+        otherwise be available to you under applicable patent law.
+        
+          12. No Surrender of Others' Freedom.
+        
+          If conditions are imposed on you (whether by court order, agreement or
+        otherwise) that contradict the conditions of this License, they do not
+        excuse you from the conditions of this License.  If you cannot convey a
+        covered work so as to satisfy simultaneously your obligations under this
+        License and any other pertinent obligations, then as a consequence you may
+        not convey it at all.  For example, if you agree to terms that obligate you
+        to collect a royalty for further conveying from those to whom you convey
+        the Program, the only way you could satisfy both those terms and this
+        License would be to refrain entirely from conveying the Program.
+        
+          13. Use with the GNU Affero General Public License.
+        
+          Notwithstanding any other provision of this License, you have
+        permission to link or combine any covered work with a work licensed
+        under version 3 of the GNU Affero General Public License into a single
+        combined work, and to convey the resulting work.  The terms of this
+        License will continue to apply to the part which is the covered work,
+        but the special requirements of the GNU Affero General Public License,
+        section 13, concerning interaction through a network will apply to the
+        combination as such.
+        
+          14. Revised Versions of this License.
+        
+          The Free Software Foundation may publish revised and/or new versions of
+        the GNU General Public License from time to time.  Such new versions will
+        be similar in spirit to the present version, but may differ in detail to
+        address new problems or concerns.
+        
+          Each version is given a distinguishing version number.  If the
+        Program specifies that a certain numbered version of the GNU General
+        Public License "or any later version" applies to it, you have the
+        option of following the terms and conditions either of that numbered
+        version or of any later version published by the Free Software
+        Foundation.  If the Program does not specify a version number of the
+        GNU General Public License, you may choose any version ever published
+        by the Free Software Foundation.
+        
+          If the Program specifies that a proxy can decide which future
+        versions of the GNU General Public License can be used, that proxy's
+        public statement of acceptance of a version permanently authorizes you
+        to choose that version for the Program.
+        
+          Later license versions may give you additional or different
+        permissions.  However, no additional obligations are imposed on any
+        author or copyright holder as a result of your choosing to follow a
+        later version.
+        
+          15. Disclaimer of Warranty.
+        
+          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+        
+          16. Limitation of Liability.
+        
+          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+        SUCH DAMAGES.
+        
+          17. Interpretation of Sections 15 and 16.
+        
+          If the disclaimer of warranty and limitation of liability provided
+        above cannot be given local legal effect according to their terms,
+        reviewing courts shall apply local law that most closely approximates
+        an absolute waiver of all civil liability in connection with the
+        Program, unless a warranty or assumption of liability accompanies a
+        copy of the Program in return for a fee.
+        
+                             END OF TERMS AND CONDITIONS
+Project-URL: Homepage, https://codeberg.org/mmatous/seal
+Project-URL: Bug Tracker, https://codeberg.org/mmatous/seal/issues
+Keywords: area,distance decay,ecology,extent,grain,richness,SAR,scale,species,species-area
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: alive-progress~=3.1
+Requires-Dist: numba~=0.59
+Requires-Dist: numexpr~=2.9
+Requires-Dist: pandas~=2.2
+Requires-Dist: pydantic~=2.6
+Requires-Dist: scipy~=1.12
+Requires-Dist: seaborn~=0.13.2
+Provides-Extra: dev
+Requires-Dist: mypy==1.9; extra == "dev"
+Requires-Dist: pandas-stubs~=2.2; extra == "dev"
+Requires-Dist: pytest~=8.1; extra == "dev"
+Requires-Dist: pytest-cov~=5.0; extra == "dev"
+Requires-Dist: ruff==0.3.4; extra == "dev"
+Provides-Extra: alt-plot
+Requires-Dist: plotly; extra == "alt-plot"
+
+# seal
+
+Perform richness-extent-grain analyses inspired by Palmer & White
+([doi:10.1086/285704](https://doi.org/10.1086/285704), [doi:10.17615/n84a-pd17](https://doi.org/10.17615/n84a-pd17))
+
+## Setup
+
+### Installation
+
+From PyPI via `pip`:
+```
+pip install seal-tool
+```
+
+
+Or simply download `seal` from Codeberg [releases](https://codeberg.org/mmatous/seal)
+or clone the repository using git.
+
+
+### First run
+
+Done only when installing and running the tool for the first time
+and necessary only for non-PyPI installations.
+
+Open the project directory in your
+command-line interface.
+
+#### Linux
+
+In POSIX-compatible shell run:
+```bash
+source ./src/firstrun.sh
+```
+
+#### Windows
+
+In PowerShell Run:
+```
+./src/firstrun.ps1
+```
+
+If you encounter an error such as `./src/firstrun.ps1 cannot be loaded because running scripts is disabled on this system`
+on Windows, it means the script was blocked by your
+security settings. In that case either unblock
+the script e.g. using the [`Unblock-File` or `Set-ExecutionPolicy` cmdlets](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.security/set-executionpolicy?view=powershell-7.4#example-7-unblock-a-script-to-run-it-without-changing-the-execution-policy) or run the
+necessary commands manually.
+
+```
+python -m venv ./venv
+./venv/Scripts/Activate.ps1
+pip install .[dev]
+```
+
+
+You should see `(venv)` before your shell prompt now and `seal --help`
+should run the tool without errors. Continue with [Usage](#Usage).
+
+### Subsequent runs
+
+Done when running the tool any time after the first initial installation.
+
+Linux:
+```
+source ./venv/bin/activate
+seal <subcommand>
+```
+
+Windows PowerShell:
+```
+./venv/Scripts/activate.ps1
+seal <subcommand>
+```
+
+## Usage
+
+One would generally want to use `preprocess`, `analyse` and `plot` subcommands in this order.
+`misc` subcommand contains several scripts that
+may be useful while converting or modifying either datasets or quadrat
+lists for analysis.
+
+More detailed help can be accessed by `seal --help`
+or `seal <subcommand> --help`.
+
+### Preprocess
+
+Preprocess will ensure given dataset is fit to be processed
+by the `analyse` command by e.g. sanitizing strings,
+warning for missing values or
+checking whether species column remains consistent with
+name, morph and phase.
+
+Example:
+```
+seal preprocess --dataset ./datasets/raw.csv --output ./datasets/clean.csv
+```
+
+
+### Analysis
+
+`analyse` subcommand ingests a [taskfile](./tasks/0-example-task.toml)
+to perform analyses requested therein.
+
+Example:
+```
+seal analyse --taskfile ./tasks/0-example-task.toml
+```
+
+More example taskfiles are available at our [Codeberg repository](./tasks/)
+along with some [datasets](./datasets/).
+
+Currently supported analyses are:
+
+#### a1 - Overview
+
+This analysis calculates per-quadrat species number
+and number of encountered individuals for each level.
+
+The additional data contain general description of given dataset and various smaller statistics for each level.
+Such statistics include, for example, the most common value, mean, median, min and such for each data column.
+
+This helps familiarize oneself with the data and serves as a basic check of the levels-creating strategy.
+
+#### a2 - Species-area relationship
+
+This analysis shows relationship between species richness and area sampled.
+
+Species-area curve is calculated for each level by accumulating quadrats
+and tallying the number of species. Since this method is sensitive to order of the
+quadrats, number of permutations must be specified and their arithmetic mean is plotted.
+
+The additional data contain statistics of the calculated results.
+
+#### a3 - Distance-dependent species difference
+
+This analysis creates pairwise difference of sets of encountered species
+in two quadrats.
+
+Result is the difference as a function of distance of the quadrats.
+
+#### a4 - Radius richness
+
+This analysis calculates the number of species within various distance intervals (interval's width is set by
+the `interval-step` parameter)
+from each quadrat. The radius forms a belt of sorts with a specified width.
+
+We recommend using the size of the smallest quadrat as the smallest possible step.
+
+#### a5 - Ratio of observed and expected species
+
+This analysis calculates the ratio of observed and expected number of species for each
+quadrat. The expected value is calculated as $$\sum_{}P_i * (1 - P_i)$$  where P<sub>i</sub> is the proportion
+of quadrats occupied by species _i_ and the summation is over all the species in the study grid.
+
+#### a6 - Ratio of shared and unique species
+
+This analysis calculates several ratios for pairs of quadrats based on their distance.
+1) Ratio of shared species among the quadrats and exclusive species among the quadrats.
+2) Ratio of shared species among the quadrats and all
+the species in the dataset.
+3) Ratio of shared species among the quadrats and
+all the species in the study grid.
+
+
+#### a7 - Jaccard dissimilarity
+
+This analysis calculates Jaccard dissimilarity with regards to species between
+all possible pairs of quadrats.
+
+Result is plotted as dissimilarity against the distance
+of the quadrats.
+
+Jaccard dissimilarity between quadrats _a_ and _b_ is calculated as:
+$$J(a, b) = 1 - \frac{intersect_{ab}}{intersect_{ab} + exclusive_a + exclusive_b}$$
+
+
+
+### Plotting
+
+`plot` subcommand ingests [taskfile](./tasks/0-example-task.toml) to detect results of previous analyses
+and present them as graphs.
+
+Generated graphs will be saved to the same directory as
+analysis results.
+
+Example:
+```
+seal plot --taskfile ./tasks/0-example-task.toml
+```
+
+### Misc
+
+`misc` subcommand is a kitchen sink of opinionated
+convenience tools.
+
+## Development
+
+For unit tests run `python -m doctest ./src/seal/<file>`.
+
+For functional tests run `pytest`.
+
+### License
+The source code—including the tests and documentation—is licensed under [GPLv3](./LICENSE)
+
+`./datasets/data-bmd-sl.csv` is licensed under [CC-BY-SA-4.0](./datasets/LICENSE)
+
+[aopk-fish.csv](./datasets/aopk-fish.csv) was provided under [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/)
+by AOPK ČR, Nálezová databáze ochrany přírody, on-line database portal.nature.cz. Downloaded 2024-02-05.
```

### Comparing `seal-tool-0.10.0/README.md` & `seal_tool-0.11.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,28 @@
 Perform richness-extent-grain analyses inspired by Palmer & White
 ([doi:10.1086/285704](https://doi.org/10.1086/285704), [doi:10.17615/n84a-pd17](https://doi.org/10.17615/n84a-pd17))
 
 ## Setup
 
 ### Installation
 
-Simply download `seal` from Codeberg [releases](https://codeberg.org/mmatous/seal)
+From PyPI via `pip`:
+```
+pip install seal-tool
+```
+
+
+Or simply download `seal` from Codeberg [releases](https://codeberg.org/mmatous/seal)
 or clone the repository using git.
 
+
 ### First run
 
-Done only when installing and running the tool for the first time.
+Done only when installing and running the tool for the first time
+and necessary only for non-PyPI installations.
 
 Open the project directory in your
 command-line interface.
 
 #### Linux
 
 In POSIX-compatible shell run:
@@ -66,15 +74,15 @@
 ## Usage
 
 One would generally want to use `preprocess`, `analyse` and `plot` subcommands in this order.
 `misc` subcommand contains several scripts that
 may be useful while converting or modifying either datasets or quadrat
 lists for analysis.
 
-More detailed help can be accesed by `seal --help`
+More detailed help can be accessed by `seal --help`
 or `seal <subcommand> --help`.
 
 ### Preprocess
 
 Preprocess will ensure given dataset is fit to be processed
 by the `analyse` command by e.g. sanitizing strings,
 warning for missing values or
@@ -85,22 +93,25 @@
 ```
 seal preprocess --dataset ./datasets/raw.csv --output ./datasets/clean.csv
 ```
 
 
 ### Analysis
 
-`analyse` subcommand ingests [taskfile](./tasks/example-task.conf)
+`analyse` subcommand ingests a [taskfile](./tasks/0-example-task.toml)
 to perform analyses requested therein.
 
 Example:
 ```
-seal analyse --taskfile ./tasks/example-task.conf
+seal analyse --taskfile ./tasks/0-example-task.toml
 ```
 
+More example taskfiles are available at our [Codeberg repository](./tasks/)
+along with some [datasets](./datasets/).
+
 Currently supported analyses are:
 
 #### a1 - Overview
 
 This analysis calculates per-quadrat species number
 and number of encountered individuals for each level.
 
@@ -159,25 +170,25 @@
 of the quadrats.
 
 Jaccard dissimilarity between quadrats _a_ and _b_ is calculated as:
 $$J(a, b) = 1 - \frac{intersect_{ab}}{intersect_{ab} + exclusive_a + exclusive_b}$$
 
 
 
-### Ploting
+### Plotting
 
-`plot` subcommand ingests [taskfile](./tasks/example-task.conf) to detect results of previous analyses
+`plot` subcommand ingests [taskfile](./tasks/0-example-task.toml) to detect results of previous analyses
 and present them as graphs.
 
 Generated graphs will be saved to the same directory as
 analysis results.
 
 Example:
 ```
-seal plot --taskfile ./tasks/example-task.conf
+seal plot --taskfile ./tasks/0-example-task.toml
 ```
 
 ### Misc
 
 `misc` subcommand is a kitchen sink of opinionated
 convenience tools.
```

### Comparing `seal-tool-0.10.0/pyproject.toml` & `seal_tool-0.11.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [project]
 name = "seal-tool"
-version = "0.10.0"
+version = "0.11.0"
 authors = [
   { name = "Martin Matouš", email = "m@matous.dev" },
   { name = "Barbora Winterová", email = "winterova@mail.muni.cz" },
   ]
 description = "A tool to perform richness-extent-grain analyses"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">= 3.12"
 dependencies = [
   "alive-progress ~= 3.1",
   "numba ~= 0.59",
   "numexpr ~= 2.9", # leave out bottleneck from pandas[performance], requires compiler
-  "pandas[plot] ~= 2.2",
-  "pyhocon ~= 0.3",
+  "pandas ~= 2.2",
+  "pydantic ~= 2.6",
+  "scipy ~= 1.12",
   "seaborn ~= 0.13.2",
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -28,19 +29,19 @@
   "Topic :: Scientific/Engineering",
 ]
 keywords = ["area", "distance decay", "ecology", "extent", "grain", "richness", "SAR", "scale", "species", "species-area"]
 
 
 [project.optional-dependencies]
 dev = [
-  "mypy ~= 1.6",
-  "pandas-stubs ~= 2.0",
-  "pytest ~= 7.4",
-  "pytest-cov ~= 4.1",
-  "ruff ~= 0.2.0",
+  "mypy == 1.9",
+  "pandas-stubs ~= 2.2",
+  "pytest ~= 8.1",
+  "pytest-cov ~= 5.0",
+  "ruff == 0.3.4",
 ]
 alt_plot = [
   "plotly",
 ]
 
 [project.scripts]
 seal = "seal.__main__:main"
@@ -51,31 +52,99 @@
 # "Original Study" = "https://doi.org/10.1086/285704"
 # "Original Study, alt." = "https://doi.org/10.17615/n84a-pd17"
 
 [tool.ruff]
 line-length = 120
 target-version = "py312"
 
+[tool.ruff.lint]
+select = [
+  "A",
+  "ANN",
+  "ARG",
+  "ASYNC",
+  "B",
+  "C4",
+  "D",
+  "DTZ",
+  "E",
+  "F",
+  "FBT",
+  "I",
+  "LOG",
+  "N",
+  "PD",
+  "PL",
+  "PERF",
+  "PIE",
+  "PGH",
+  "PT",
+  "PTH",
+  "RET",
+  "RUF",
+  "S",
+  "SIM",
+  "TCH",
+  "TID",
+  "TRY",
+  "UP",
+  "W",
+]
+ignore = [
+  "ANN101",
+  "ANN102", # both deprecated as of ruff 0.3.3 anyway
+  "D10",
+  "E111",
+  "E114",
+  "E117",
+  "E501", # these Es are left up to ruff format
+  "PD008",
+  "PD009",
+  "PD901",
+  "RET504",
+  "N999",
+]
+
+[tool.ruff.lint.flake8-bandit]
+check-typed-exception = true
+
+[tool.ruff.lint.flake8-tidy-imports]
+ban-relative-imports = "all"
+
+[tool.ruff.lint.per-file-ignores]
+"tests/*" = ["D", "S101"]
+
+[tool.ruff.lint.pydocstyle]
+convention = "pep257"
+
 [tool.ruff.format]
 docstring-code-format = true
 line-ending = "lf"
 quote-style = "single"
 
-[tool.ruff.lint.flake8-quotes]
-inline-quotes = "single"
-multiline-quotes = "single"
-
 [tool.mypy]
 allow_redefinition = true
-disable_error_code = "valid-type"
+disable_error_code = [
+  "valid-type",
+]
 enable_error_code = [
   "ignore-without-code",
+  "possibly-undefined",
+  "redundant-expr",
+  "redundant-self",
+  "truthy-bool",
+  "truthy-iterable",
+  "unreachable",
+  # unused for now but nobody would remember to add these should related features be used later
+  "explicit-override",
+  "mutable-override",
+  "unused-awaitable",
 ]
-warn_unused_ignores = true
-warn_redundant_casts = true
+exclude = "build/"
+strict = true
 
 [tool.pytest.ini_options]
 addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 95"
 doctest_optionflags = "NORMALIZE_WHITESPACE"
 python_files = "test-*.py"
 
 [tool.coverage.run]
```

### Comparing `seal-tool-0.10.0/src/seal/__main__.py` & `seal_tool-0.11.0/src/seal/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import argparse
 import sys
-
 from pathlib import Path
+from typing import Any
 
 from seal.analyze import main as analyze_main
 from seal.misc import add_coord_cols, add_date_col, check_quadrat_list, convert_aopk, convert_biolib, join_analyses
 from seal.plot import main as plot_main
 from seal.preprocess import main as preprocess_main
 
 
-def main(argv=sys.argv):
+def main(argv: list[str] = sys.argv) -> Any:  # noqa: ANN401
     parser = argparse.ArgumentParser(
         prog='seal',
         description='Process and visualize influence of grain and extent on perceived species richness and species-area relationships',
     )
     subparsers = parser.add_subparsers(title='Subcommands', required=True)
 
     analyze = subparsers.add_parser(
         'analyze',
-        description='Calculate data necessary to plot various curves from an encounters dataset. \
-        May output additional potentially relevant data.',
+        description=(
+            'Calculate data necessary to plot various curves from an encounters dataset.'
+            'May output additional potentially relevant data.'
+        ),
     )
     analyze.add_argument('-t', '--taskfile', required=True, type=Path, help='path to taskfile')
     analyze.set_defaults(func=analyze_main)
 
     plot = subparsers.add_parser('plot', description='Plot data generated by seal-analyze.')
     plot.add_argument('-t', '--taskfile', type=Path, required=True, help='path to taskfile')
-    plot.add_argument('-j', '--joined', nargs=2, help='type of joined analysis and path to its data')
-    plot.add_argument('--png', action='store_true', help='save resulting graphs as .png instead of .svg')
     plot.set_defaults(func=plot_main)
 
     prepr = subparsers.add_parser(
         'preprocess',
-        description='''Checks and cleans datasets intended for analysis of influence of grain and extent on perceived species richness.
-            Data that satisfy all specified conditions will be written to [OUTPUT].''',
+        description=(
+            'Checks and cleans datasets intended for analysis of influence of grain and extent on perceived species richness.'
+            'Data that satisfy all specified conditions will be written to [OUTPUT].'
+        ),
     )
     full_checklist = [
         'dups',
         'coords',
         'family',
         'morph-species',
         'nas',
@@ -50,25 +52,26 @@
     default_checklist = ['dups', 'nas', 'strs']
     prepr.add_argument(
         '-c',
         '--checks',
         choices=full_checklist,
         default=default_checklist,
         nargs='+',
-        help='''Checks to perform:
-        \tdups: Check for potential duplicates (does not filter them automatically)
-        \tcoords: Check that coordinates correspond to quadrat_id
-        \tfamily: Labridae and Scaridae families should not exist in "ad" phase, ("term" phase is acceptable)
-        \tmorph-species: Morph attributes not starting with "M " should be equal to species
-        \tnas: Warn for missing values in dataset
-        \tspecies-name: species and name should only ever exist in one combination
-        \tspecies-phase-morph: species and phase combination should only ever belong to a sigle morph
-        \trefs: Ref should be arithmetic progression with a1=1 and d=1
-        \tstrs: Only permitted whitespace are simple nonconsecutive spaces
-        ''',
+        help=(
+            'Checks to perform:'
+            '\tdups: Check for potential duplicates (does not filter them automatically)'
+            '\tcoords: Check that coordinates correspond to quadrat_id'
+            '\tfamily: Labridae and Scaridae families should not exist in "ad" phase, ("term" phase is acceptable)'
+            '\tmorph-species: Morph attributes not starting with "M " should be equal to species'
+            '\tnas: Warn for missing values in dataset'
+            '\tspecies-name: species and name should only ever exist in one combination'
+            '\tspecies-phase-morph: species and phase combination should only ever belong to a single morph'
+            '\trefs: Ref should be arithmetic progression with a1=1 and d=1'
+            '\tstrs: Only permitted whitespace are simple nonconsecutive spaces'
+        ),
     )
     prepr.add_argument(
         '--drop-nas',
         action=argparse.BooleanOptionalAction,
         help='Set automatic action for dealing with missing values without prompting for user input.',
     )
     prepr.add_argument('--dataset', type=Path, help='Path to encounters dataset.')
@@ -118,12 +121,12 @@
 
     aopk = misc_subparsers.add_parser('convert-aopk', description='Convert AOPK data for preprocessing and analysis.')
     aopk.add_argument('input', type=Path, help='Paths dataset obtained from AOPK.')
     aopk.add_argument('output', type=Path, help='Output filename.')
     aopk.set_defaults(func=convert_aopk)
 
     args = parser.parse_args(argv[1:])
-    args.func(args)
+    return args.func(args)
 
 
 if __name__ == '__main__':
     sys.exit(main(sys.argv))
```

### Comparing `seal-tool-0.10.0/src/seal/analyze.py` & `seal_tool-0.11.0/src/seal/analyze.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,287 +1,237 @@
 import argparse
+import copy
 import math
-import numpy as np
-import pandas as pd
 import random
-import sys
-
-from alive_progress import alive_bar
-from alive_progress.animations.spinners import bouncing_spinner_factory
-from collections import defaultdict
-from collections.abc import Mapping, Sequence
-from dataclasses import dataclass
-from datetime import date
+import warnings
+from collections.abc import Callable, Iterator, Mapping, Sequence
+from dataclasses import astuple, dataclass
 from pathlib import Path
-from typing import cast, Callable, Literal, TypeGuard
+from typing import Literal, cast
+
+import numpy as np
+import pandas as pd
+from alive_progress import alive_bar  # type: ignore[import-untyped]
+from scipy import optimize  # type: ignore[import-untyped] # https://github.com/scipy/scipy/issues/17158
 
 import seal.config as conf
-from seal.common import analysis_results_name, enc_dtypes, Encounters, data_dir, Sides, QList
+from seal.common import analysis_results_filename, enc_dtypes, geom_r2, get_spinner, qlist_dtypes
+from seal.config import Analysis, Analysis2, Analysis3, Analysis4, Distance, LevelStrategy, QuadratType, Sides
+from seal.exceptions import InputType, InvalidFilterError, InvalidLiteralError, InvalidQuadratsError, MissingValuesError
 
-type Coord = tuple[int, int]  # type: ignore[valid-type]
-type CoordCol = Literal['coord_x', 'coord_y']
-type DistFunction = Callable[[pd.DataFrame, pd.DataFrame], pd.Series]
+type Caps = dict[Literal['centroid', 'diagonal', 'max1dx', 'max1dy', 'total_area'], float]
+type DistFunction = Callable[[pd.DataFrame, pd.DataFrame], 'pd.Series[float]']
 type Edge = Literal['left', 'right', 'top', 'bottom']
-type LvlType = Literal[
-    'nested-quadrats',
-    'overlaid-subgrids',
-    'repeated-transect-merging',
-    'striped-transect-merging',
-    'transect-additive',
-    'transect-merging',
-    'zone-additive',
-    'zone-merging',
-]
+type Encounters = pd.DataFrame
+type QList = pd.DataFrame
 type SppMatrix = pd.DataFrame
 
 
 @dataclass
-class Position:
-    """Represents coordinates of quadrat on a grid"""
-
-    x_g: int
-    y_g: int
-
-
-@dataclass
-class Point:
-    """Represents point on a grid with coordinates in meters"""
+class GridInfo:
+    """Contains information about spp. encounters and layout of the study grid."""
 
-    x_m: float
-    y_m: float
+    enc: Encounters
+    qlist: QList
 
+    def __iter__(self) -> Iterator[Encounters | QList]:
+        return iter(astuple(self))
 
-def main(args: argparse.Namespace) -> int:
-    """Load taskfile configuration, datasets, perform and save
-    requested analyses. Create output directory if necessary.
-    """
 
-    cfg = conf.Config.from_file(args.taskfile)
-    enc_path = Path(cfg.get_string('encounters'))
-    enc = load_encounters(enc_path)
+@dataclass
+class LevelInfo:
+    """Contains level- (and strategy-) dependent information about the study grid."""
 
+    subgrids: list[GridInfo]
+    dmats: list[pd.DataFrame]
+    sides: Sides
 
-    dist_fn_type = cfg.get_string('distance-type', 'diagonal')
-    quadrat_types = cfg.get_list('quadrat-types', ['normal'])
-    quadrat_types = [str(val) for val in quadrat_types]
-    locality = cfg.get_subconf('locality')
-    qlist_path = Path(locality.get_string('quadrat-list'))
-    quadrats = load_quadrats(qlist_path, quadrat_types)
+    def __iter__(self) -> Iterator[list[GridInfo] | list[pd.DataFrame] | Sides]:
+        return iter(astuple(self))
 
-    enc = filter_encounters(enc, cfg)
-    qids_enc = set(enc.quadrat_id)
-    qids_qlist = set(quadrats.quadrat_id)
-    qids_diff = qids_enc - qids_qlist
-    if len(qids_diff) > 0:
-        print(
-            f"""Filtered dataset contains encounters in quadrats not found in quadrat list.
-            Possible causes may be using quadrat list for unintended locality, incorrectly set-up filters, e.g. *from* and *to* dates in taskfile\'s locality section or simply mistakes/typos in provided quadrat list or dataset.
-            Extraneous IDs:
-            {qids_diff}
-            """
-        )
-        sys.exit(1)
 
-    discard_transect = cfg.get_bool('discard-transect-info', False)
-    discard_zone = cfg.get_bool('discard-zone-info', False)
-    sides_orig = Sides(**locality.get('sides'))  # type: ignore[arg-type] # is a mapping (or should be)
-    quadrats = add_quadrat_centroids(quadrats, sides_orig)
-    enc, quadrats, sides_adj = adjust_grid(enc, quadrats, sides_orig, discard_transect, discard_zone)
-    locality.put( # technically, they are adjusted, but for the purposes of other computations they replace original values completely
-        'sides', {'x': sides_adj.x, 'y': sides_adj.y}
-    )
-    caps = compute_caps(quadrats, sides_orig)
+def main(args: argparse.Namespace) -> int:
+    """Load taskfile configuration, datasets, perform and save requested analyses.
 
-    completed: dict[str, pd.DataFrame] = {}
-    additional: dict[str, list[str | pd.DataFrame]] = defaultdict(list)
+    Create output directory if necessary.
+    """
+    cfg = conf.Config.from_taskfile(args.taskfile)
+    enc = load_encounters(cfg.encounters)
 
-    levels = cfg.get_list('levels')
-    analyses = cfg.get_list('analyses')
-    n_tasks = len(levels) * len(analyses)
-    if not is_int_list(levels):
-        raise conf.InvalidTaskError('level values should be integers')
-    seed = cfg.get_int_unchecked('seed', None)
-
-    emoji = ['🐧', '🐡', '🐟', '🦑', '🦦', '🐠', '🦐', '🐙']
-    random.shuffle(emoji)
-    emoji = ''.join(emoji)
-    spinner = bouncing_spinner_factory(('🌊', emoji), 6, block=(1, 1), hide=True)
+    try:
+        enc = filter_encounters(enc, cfg)
+    except AttributeError as e:
+        raise InvalidFilterError(e.name, InputType.ENCOUNTERS) from e
+
+    if cfg.locality.quadrat_list:
+        try:
+            quadrats = load_quadrats(cfg.locality.quadrat_list, cfg.quadrat_types)
+        except AttributeError as e:
+            raise InvalidFilterError(e.name, InputType.QLIST) from e
+    else:
+        print('Quadrat list not passed separately, please ensure you understand the implications of doing this.')
+        quadrats = generate_quadrat_list(enc)
 
+    grinfo = GridInfo(enc, quadrats)
+    check_grid_consistency(grinfo)
+    (grinfo, sides_adj, caps) = adjust_grid(grinfo, cfg)
+
+    n_tasks = len(set(cfg.levels)) * len(cfg.analyses)
+    spinner = get_spinner()
+    lvl_infos = get_lvl_infos(grinfo, sides_adj, caps, cfg)
+    analysis_idx = {analysis.type_: 0 for analysis in cfg.analyses}
+    cfg.out_dir.mkdir(parents=True, exist_ok=True)
     with alive_bar(n_tasks, title='Analysis', spinner=spinner) as bar:
-        for level in levels:
-            lvl_strat = cfg.get_string('level-strategy', 'striped-transect-merging')
-            enc_subgrids, q_subgrids, sides_adj = adjust_for_lvl(
-                enc,
-                quadrats,
-                locality,
-                level,
-                max(levels),
-                lvl_strat,  # type: ignore[arg-type] # method rejects invalid strats, no need for TypeGuard
-                sides_orig,
-            )
-            capped_dist_fn = get_distance_function(dist_fn_type, sides_adj, caps)
-            dmats = [distance_matrix(qs, capped_dist_fn) for qs in q_subgrids]
-            for analysis in analyses:
-                analysis = conf.Config.from_string(f'type = {analysis}') if isinstance(analysis, str) else analysis
-                analysis = cast(conf.Config, analysis)
-                a_type = analysis.get_string('type')
-                bar.text(f'{a_type}, level {level}')
-                res, additional_data = do_analysis(enc_subgrids, q_subgrids, dmats, analysis, sides_adj, seed, caps)
+        for analysis in cfg.analyses:
+            completed = []
+            additional = []
+            for level, lvl_info in lvl_infos.items():
+                bar.text(f'{analysis.type_}, level {level}')
+                res, additional_data = do_analysis(lvl_info, analysis, cfg.seed, caps)
                 res['level'] = level
-
-                if additional_data is not None:
-                    additional[a_type].append(additional_data)
-                prev = completed.get(a_type, pd.DataFrame())
-                completed[a_type] = pd.concat([prev, res])  # todo: build list, concat just once
+                completed.append(res)
+                additional.append(additional_data)
                 bar()
-    out_dir = data_dir(cfg)
-    out_dir.mkdir(parents=True, exist_ok=True)
-    save_results(args, out_dir, completed, additional)
+            a_info = (analysis.type_, analysis_idx[analysis.type_])
+            save_results(args, cfg.out_dir, completed, additional, a_info)
+            analysis_idx[analysis.type_] += 1
     return 0
 
 
-def do_analysis(
-    enc_subgrid: list[Encounters],
-    q_subgrid: list[QList],
-    dmats: list[pd.DataFrame],
-    analysis: conf.Config,
-    sides_adj: Sides,
+def do_analysis(  # noqa: PLR0911
+    lvl_info: LevelInfo,
+    analysis: Analysis,
     seed: int | None,
-    caps: dict[str, float],
+    caps: Caps,
 ) -> tuple[pd.DataFrame, str | pd.DataFrame | None]:
-    """Pick appropriate analysis to perform on passed subgrids
-    with given config settings and return its results.
-    """
-
+    """Return results of `analysis` on passed subgrids with given config settings."""
     if seed:
         random.seed(seed)
         np.random.seed(seed)
 
-
-    spp_matrices = []
-    for enc, qlist in zip(enc_subgrid, q_subgrid, strict=True):
-        spp_matrices.append(get_spp_matrix(enc, qlist))
-    match analysis.get_string('type'):
+    subgrids = lvl_info.subgrids
+    spp_matrices = [get_spp_matrix(subgrid) for subgrid in subgrids]
+    match analysis.type_:
         case 'a1' | 'overview':
-            return a1_overview(enc_subgrid, q_subgrid)
+            return a1_overview(subgrids)
         case 'a2' | 'sar':
-            return a2_sar(enc_subgrid, q_subgrid, spp_matrices, analysis, sides_adj, caps)
+            return a2_sar(spp_matrices, cast(Analysis2, analysis), lvl_info.sides, caps)
         case 'a3' | 'spdiff':
-            return a3_species_delta(enc_subgrid, q_subgrid, spp_matrices, dmats, analysis)
+            return a3_species_delta(spp_matrices, lvl_info.dmats, cast(Analysis3, analysis))
         case 'a4' | 'rrich':
-            return a4_avg_radius_richness(enc_subgrid, q_subgrid, spp_matrices, dmats, analysis)
+            return a4_avg_radius_richness(spp_matrices, lvl_info.dmats, cast(Analysis4, analysis))
         case 'a5' | 'oerich':
-            return a5_observed_expected(enc_subgrid, q_subgrid, spp_matrices)
+            return a5_observed_expected(spp_matrices)
         case 'a6' | 'sratios':
-            return a6_shared_ratios(enc_subgrid, q_subgrid, spp_matrices, dmats)
+            return a6_shared_ratios(spp_matrices, lvl_info.dmats)
         case 'a7' | 'jaccard':
-            return a7_jaccard_diss(enc_subgrid, q_subgrid, spp_matrices, dmats)
+            return a7_jaccard_diss(spp_matrices, lvl_info.dmats)
+        case 'a8' | 'abundance':
+            return a8_abundance(subgrids)
         case _:
-            raise conf.InvalidTaskError(analysis.get_string('type'))
+            raise InvalidLiteralError(f'{analysis.type_=}')
 
 
 class TilingError(Exception):
     """Exception raised when request quadrat level doesn't fit the study grid.
 
     Attributes:
         level -- level being analyzed
         sides -- dimensions of the entire locality
     """
 
-    def __init__(self, level: int, sides: Sides):
+    def __init__(self, level: int, sides: Sides) -> None:
         super().__init__(f'Requested level {level} incompatible with locality dimensions: {sides.x} x {sides.y}')
 
 
 def describe_full(df: pd.DataFrame) -> pd.DataFrame:
     stats = df.describe(percentiles=[0.025, 0.25, 0.5, 0.75, 0.975], include='all')
     stats.loc['median'] = df.median(numeric_only=True)
     stats.loc['sem'] = df.sem(numeric_only=True)
     stats.loc['skewness'] = df.skew(numeric_only=True)
     stats.loc['kurtosis'] = df.kurtosis(numeric_only=True)
     return stats
 
 
-def a1_overview(enc_subgrid: list[Encounters], q_subgrid: list[QList]) -> tuple[pd.DataFrame, str]:
-    """Return DataFrame containing number of unique species
-    as well as number of individuals encountered in respective quadrats.
+def a1_overview(subgrids: list[GridInfo]) -> tuple[pd.DataFrame, str]:
+    """Return DataFrame containing number of unique species as well as number of individuals encountered in respective quadrats.
+
     Additional data contains per-level (and per-subgrid if applicable)
     descriptive statistics about encounters being processed.
     """
-
     res = []
     uniques = []
     res += ['====LEVEL OVERVIEW START====']
-    for i, (enc, quadrats) in enumerate(zip(enc_subgrid, q_subgrid, strict=True)):
-        if len(enc_subgrid) > 1:
+    for i, (enc, quadrats) in enumerate(subgrids):
+        if len(subgrids) > 1:
             res += [f'===SUBGRID #{i} START===']
         desc = describe_full(enc)
         res += [desc.to_string()]
 
         by_qid = enc.groupby(['coord_x', 'coord_y'])
         unique = by_qid.species.nunique()
         # fill 0 for quadrats where nothing was encountered
         unique = unique.reindex(quadrats.index, fill_value=0).to_frame('n_species')
-        unique['n_individuals'] = by_qid.individuals.sum()
-        assert (unique['n_individuals'] >= unique['n_species']).all()
+        if 'individuals' in enc.columns:
+            unique['n_individuals'] = by_qid.individuals.sum()
+
         unique = unique.fillna(0)
         res += ['\n==Unique per quadrat==']
         res += [unique.to_string()]
 
         avg = unique / len(quadrats)
         res += [f'\n==Avg per quadrat==\n{avg.to_string()}']
 
         indist_mask = enc.species.str.endswith(' sp.', na=True)
         indist_enc = indist_mask.sum()
         res += ['\n==Indistinguishable encounters #==']
         res += [f'{indist_enc}']
         res += ['\n==Indistinguishable encounters %==']
         res += [f'{100 * indist_enc / (indist_enc + len(enc.index))}']
-        indist_individuals = enc[indist_mask].individuals.sum()
-        res += ['\n==Indistinguishable individuals #==']
-        res += [f'{indist_individuals}']
-        res += ['\n==Indistinguishable individuals %==']
-        res += [f'{100 * indist_individuals / enc.individuals.sum()}']
-
-        res += ['\n==Direction richness difference==']
-        dirdiff = direction_difference(enc).dropna()
-        dirdiff['diff_abs#'] = dirdiff['diff_#'].abs()
-        dirdiff = dirdiff.sort_values(by='diff_abs#', ascending=False)
-        res += [describe_full(dirdiff).to_string(), '\n']
-        res += [dirdiff.to_string()]
 
-        if len(enc_subgrid) > 1:
+        if 'individuals' in enc.columns:
+            indist_individuals = enc[indist_mask].individuals.sum()
+            res += ['\n==Indistinguishable individuals #==']
+            res += [f'{indist_individuals}']
+            res += ['\n==Indistinguishable individuals %==']
+            res += [f'{100 * indist_individuals / enc.individuals.sum()}']
+
+        if 'direction' in enc.columns:
+            res += ['\n==Direction richness difference==']
+            dirdiff = direction_difference(enc).dropna()
+            dirdiff['diff_abs#'] = dirdiff['diff_#'].abs()
+            dirdiff = dirdiff.sort_values(by='diff_abs#', ascending=False)
+            res += [describe_full(dirdiff).to_string(), '\n']
+            res += [dirdiff.to_string()]
+
+        if len(subgrids) > 1:
             res += [f'===SUBGRID #{i} END===\n']
 
         unique = unique.reset_index(drop=False)
         uniques.append(unique)
     res += ['====LEVEL OVERVIEW END====\n\n']
     unique_avg = pd.concat(uniques, ignore_index=True).groupby(['coord_x', 'coord_y']).mean().convert_dtypes()
     unique_avg = unique_avg.assign(
         coord_x=quadrats.index.get_level_values('coord_x'), coord_y=quadrats.index.get_level_values('coord_y')
     )
     return (unique_avg, '\n'.join(res))
 
 
 def a2_sar(
-    enc_subgrids: list[Encounters],
-    q_subgrids: list[QList],
-    spp_matrices: list[pd.DataFrame],
-    analysis: conf.Config,
-    sides_adj: Sides,
-    caps: dict[str, float],
+    spp_matrices: list[pd.DataFrame], analysis: Analysis2, sides_adj: Sides, caps: Caps
 ) -> tuple[pd.DataFrame, pd.DataFrame]:
-    """Return DataFrame containing quadrat richness accumulation
-    in random order with separate columns for slowest and fastest
-    growing series and total accumulated area.
-    """
+    """Return DataFrame containing quadrat richness accumulations.
 
+    The accumulations are performed in random order and
+    separate columns are added for slowest and fastest growing series
+    and total accumulated area.
+    """
     accumulated = []
-    permutations = analysis.get_int('permutations')
     for spp_matrix in spp_matrices:
-        for _ in range(permutations):
+        for _ in range(analysis.permutations):
             shuff = acc_richness_shuffled(spp_matrix)
             accumulated.append(shuff)
     sar = pd.DataFrame(accumulated).transpose()
     sar_add = agg_results(sar, 'n_species', 'area')
 
     min_acc = sar[0].to_list()
     max_acc = sar[0].to_list()
@@ -297,121 +247,109 @@
     surface_area = sides_adj.x * sides_adj.y
     sar['area'] = np.minimum((sar.index + 1) * surface_area, caps['total_area'])
     sar_add['area'] = sar['area']
     return sar, sar_add
 
 
 def a3_species_delta(
-    enc_subgrids: list[Encounters],
-    q_subgrids: list[QList],
-    spp_matrices: list[SppMatrix],
-    dmats: list[pd.DataFrame],
-    analysis: conf.Config,
+    spp_matrices: list[SppMatrix], dmats: list[pd.DataFrame], analysis: Analysis3
 ) -> tuple[pd.DataFrame, pd.DataFrame]:
     """Return DataFrame containing distance-dependent species difference.
-    Absolute and relative differences between species lists are calculated
+
+    Absolute difference between species lists is calculated
     for each pair of quadrats of given distance. This is done with all possible
     pairs of quadrats of given level.
-    """
 
+    For relative comparison see `a7_jaccard_diss`.
+    """
     deltas_list = []
-    for enc, quadrats, richness, dmat in zip(enc_subgrids, q_subgrids, spp_matrices, dmats, strict=True):
+    for richness, dmat in zip(spp_matrices, dmats, strict=True):
         sub_deltas = species_delta(richness, dmat)
         deltas_list.append(sub_deltas)
     deltas = pd.concat(deltas_list)
     deltas = deltas[deltas.distance > 0]
 
     deltas_stats = deltas.reset_index(drop=True)
-    interval = analysis.get_float_unchecked('interval', None)
-    if interval and not deltas_stats.empty:
-        bins = pd.interval_range(0, deltas_stats.distance.max() + interval, freq=interval, closed='left') # type: ignore[call-overload] # should accept numeric, but rejects float; pandas 2.2.0 bug?
+    interval = analysis.interval
+    if interval and not deltas.empty:
+        bins = pd.interval_range(0, deltas.distance.max() + interval, freq=interval, closed='left')  # type: ignore[call-overload] # should accept numeric, but rejects float; pandas 2.2.0 bug?
+        deltas['distance_bin'] = pd.cut(deltas.distance, bins)
         deltas_stats['distance'] = pd.cut(deltas_stats.distance, bins)
     deltas_stats = deltas_stats.groupby('distance', observed=False).agg(AGG_STATS)
-    deltas_stats = flatten_multicolumns(deltas_stats)
+    deltas_stats = flatten_multicolumns(deltas_stats).reset_index()
     return (deltas, deltas_stats)
 
 
 def a4_avg_radius_richness(
-    enc_subgrids: list[Encounters],
-    q_subgrids: list[QList],
-    spp_matrices: list[pd.DataFrame],
-    dmats: list[pd.DataFrame],
-    cfg: conf.Config,
+    spp_matrices: list[pd.DataFrame], dmats: list[pd.DataFrame], analysis: Analysis4
 ) -> tuple[pd.DataFrame, pd.DataFrame]:
-    """Return DataFrame containing the sum of richness
-    of quadrats orbiting a select as a point of origin.
+    """Return DataFrame containing the sum of richness of quadrats orbiting a select as a point of origin.
+
     This is done for every quadrat in a grid for every distance bin.
     Additional data is returned as an aggregation of various statistics
     for said DataFrame.
     """
-
-    step = cfg.get_float('radius-step')
     radius_richness_lst = []
-    for enc, quadrats, spp_matrix, dmat in zip(enc_subgrids, q_subgrids, spp_matrices, dmats, strict=True):
-        radius_bins = pd.interval_range(0, dmat.distance.max() + step, freq=step, closed='left')  # type: ignore[call-overload]  # freq should accept float, pd or mypy err?
-        dmat = dmat.assign(distance=pd.cut(dmat.distance, radius_bins)).dropna()
+    step = analysis.radius_step
+    for spp_matrix, dmat_exact in zip(spp_matrices, dmats, strict=True):
+        radius_bins = pd.interval_range(0, dmat_exact.distance.max() + step, freq=step, closed='left')  # type: ignore[call-overload] # freq should accept float, pd or mypy err
+        dmat = dmat_exact.assign(distance=pd.cut(dmat_exact.distance, radius_bins)).dropna()
         dmat_groups = dmat.groupby(['coord_x', 'coord_y', 'distance'], observed=False)
 
         def rpd(df: pd.DataFrame) -> int:
-            return total_radius_richness(df, spp_matrix)
+            return total_radius_richness(df, spp_matrix)  # noqa: B023    # spp_matrix changing value is desirable
 
         radius_richness = dmat_groups.agg(rpd)
         radius_richness_lst.append(radius_richness)
     radius_richness = (
         pd.concat(radius_richness_lst).reset_index().rename({0: 'radius_richness'}, errors='raise', axis='columns')
     )
     stats = (
         radius_richness.drop(['coord_x', 'coord_y'], axis='columns', errors='raise')
         .groupby(by='distance', observed=False)
         .agg(AGG_STATS)
     )
-    stats = stats
-    stats = flatten_multicolumns(stats)
+    stats = flatten_multicolumns(stats).reset_index()
     return (radius_richness, stats)
 
 
-def a5_observed_expected(
-    enc_subgrids: list[pd.DataFrame], q_subgrids: list[pd.DataFrame], spp_matrices: list[SppMatrix]
-) -> tuple[pd.DataFrame, None]:
-    """Return DataFrame containing observed and expected
-    species occurences in a given list of subgrids.
-    """
-
+def a5_observed_expected(spp_matrices: list[SppMatrix]) -> tuple[pd.DataFrame, None]:
+    """Return DataFrame containing observed and expected species occurrences in a given list of subgrids."""
     oe_ratios = []
-    for enc, quadrats, spp_matrix in zip(enc_subgrids, q_subgrids, spp_matrices, strict=True):
-        species_in_n_quadrats = enc.groupby('species').quadrat_id.nunique()
-        observed_ratio = species_in_n_quadrats / len(quadrats)
+    for spp_matrix in spp_matrices:
+        species_in_n_quadrats = spp_matrix.sum(axis='index')
+        n_quadrats = len(spp_matrix)
+        observed_ratio = species_in_n_quadrats / n_quadrats
         expected_var = (observed_ratio * (1 - observed_ratio)).sum()
         q_richnesses = spp_matrix.sum(axis='columns')
         oe_ratio = q_richnesses / expected_var
         oe_ratios.append(pd.DataFrame({'oe_ratio': oe_ratio}))
     oe_ratios = pd.concat(oe_ratios, axis='columns')
     oe_ratios = pd.DataFrame(
         {'oe_ratio_mean': oe_ratios.mean(axis='columns'), 'oe_ratio_med': oe_ratios.median(axis='columns')}
     )
     return oe_ratios, None
 
 
-def a6_shared_ratios(
-    enc_subgrids: list[Encounters], q_subgrids: list[QList], spp_matrices: list[SppMatrix], dmats: list[pd.DataFrame]
-) -> tuple[pd.DataFrame, pd.DataFrame]:
-    """Return DataFrame containing ratios of species intersection vs
-    species total and union of species for respective distances
-    between quadrats in a given list of subgrids.
+def a6_shared_ratios(spp_matrices: list[SppMatrix], dmats: list[pd.DataFrame]) -> tuple[pd.DataFrame, pd.DataFrame]:
+    """Return DataFrame containing various ratios of quadrat spp. intersection with regards to distance.
+
+    Specifically spp. intersection vs
+    species total, vs. union of species and between total richness of quadrats in the entire subgrid.
+
     Additional data is returned as an aggregation of various statistics
     for said DataFrame.
     """
-
-    res: dict[str, list[pd.Series]] = {
+    res: dict[str, list['pd.Series[float]']] = {
         'common_diff': [],
         'common_total': [],
         'common_union': [],
         'distance': [],
     }
-    for enc, quadrats, spp_matrix, dmat in zip(enc_subgrids, q_subgrids, spp_matrices, dmats, strict=True):
+    for spp_matrix, dmat in zip(spp_matrices, dmats, strict=True):
         spp_grid_total = len(spp_matrix.columns)
         for idx, row in spp_matrix.iterrows():
             n_intersect = (spp_matrix & row).sum(axis='columns')
             n_xor = (spp_matrix ^ row).sum(axis='columns')
             n_union = (spp_matrix | row).sum(axis='columns')
 
             res['common_diff'].append(n_intersect / n_xor)
@@ -419,32 +357,71 @@
             res['common_union'].append(n_intersect / n_union)
             res['distance'].append(dmat.loc[idx, 'distance'])  # type: ignore[arg-type, index]   # is truly pd.Series, can be indexed by MultiIndex tuple just fine
     res = {k: pd.concat(v) for k, v in res.items()}
     ratios = pd.DataFrame(res)
     ratios = ratios[ratios.distance > 0]
     with np.errstate(invalid='ignore'):  # inf-inf may occur since values above may be inf
         ratios_stats = ratios.groupby('distance').agg(AGG_STATS)
-    ratios_stats = flatten_multicolumns(ratios_stats)
+    ratios_stats = flatten_multicolumns(ratios_stats).reset_index()
     return ratios, ratios_stats
 
 
-def a7_jaccard_diss(
-    enc_subgrids: list[Encounters], q_subgrids: list[QList], spp_matrices: list[pd.DataFrame], dmats: list[pd.DataFrame]
-) -> tuple[pd.DataFrame, None]:
-    """Return DataFrame containing Jaccard dissimilarity for
-    for respective distances between quadrats in a given list of subgrids.
-    """
-
+def a7_jaccard_diss(spp_matrices: list[pd.DataFrame], dmats: list[pd.DataFrame]) -> tuple[pd.DataFrame, None]:
+    """Return DataFrame containing Jaccard dissimilarity analysis for quadrats in respective distances."""
     jaccards_list = []
-    for enc, quadrats, spp_matrix, dmat in zip(enc_subgrids, q_subgrids, spp_matrices, dmats, strict=True):
+    for spp_matrix, dmat in zip(spp_matrices, dmats, strict=True):
         jaccards_list.append(jaccard_dissimilatity(spp_matrix, dmat))
     list_of_jaccard_lists = pd.concat(jaccards_list)
     return list_of_jaccard_lists, None
 
 
+def a8_abundance(subgrids: list[GridInfo]) -> tuple[pd.DataFrame, pd.DataFrame]:
+    """Return DataFrame containing equitability of abundance and species abundance distribution data.
+
+    Theoretical species richness as per Preston, F. W. (1948). "The Commonness, and Rarity, of Species",
+    doi:10.2307/1930989, p. 257 is returned as additional data.
+    """
+    enc = subgrids[0].enc  # disregard subgrids as they are most likely to be removed
+    spp_totals = enc[['individuals', 'species']].groupby('species', as_index=False).sum()
+
+    # formulas and curves explained in the paper in docs or at
+    # https://en.wikipedia.org/wiki/Relative_species_abundance#Calculating_theoretical_species_richness
+    bins_scalars = geom_r2(1, spp_totals.individuals.max())
+    spp_totals['individuals_bin'] = pd.cut(spp_totals.individuals, bins_scalars, right=False)
+    ns = spp_totals[['individuals_bin', 'species']].groupby('individuals_bin', observed=False).count()
+    ns['bin_position'] = range(len(ns))
+    n0_bin = ns['species'].idxmax()  # the modal bin
+    n0_position = ns.at[n0_bin, 'bin_position']
+    n0 = ns.at[n0_bin, 'species']  # number of spp in the modal bin
+    Rs = (ns['bin_position'] - n0_position).abs()  # noqa: N806 # consistency with literature, distances to modal bin
+
+    def gauss_curve(R: 'pd.Series[int]', a: int) -> 'pd.Series[float]':  # noqa: N803 # same as above
+        return cast('pd.Series[float]', n0 * np.exp(-((a * R) ** 2)))
+
+    try:
+        a = optimize.curve_fit(gauss_curve, Rs, ns['species'], nan_policy='raise')[0][0]
+    except RuntimeError:
+        a = math.nan
+    spp_theoretical = n0 * math.sqrt(math.pi) / a  # N in formulas above
+    spp_sampled = len(spp_totals)
+    add = pd.DataFrame(
+        {
+            'theoretical_richness': [spp_theoretical],
+            'sampled_richness': [spp_sampled],
+            'hidden_species': [spp_theoretical - spp_sampled],
+            'sampled_%': [100 * spp_sampled / spp_theoretical],
+        }
+    )
+
+    # prevent pandas.errors.IntCastingNaNError: Cannot convert non-finite values (NA or inf) to integer during pd.concat()
+    # pandas bug as of 2.2.1?
+    spp_totals['individuals_bin'] = spp_totals['individuals_bin'].astype(str)
+    return spp_totals, add
+
+
 def jaccard_dissimilatity(spp_matrix: pd.DataFrame, dmat: pd.DataFrame) -> pd.DataFrame:
     """Return Jaccard dissimilarity for respective distances in a DataFrame.
 
     >>> spp_idx = pd.MultiIndex.from_arrays([[0, 0, 1], [0, 1, 0]], names=('coord_x', 'coord_y'))
     >>> spp_matrix = pd.DataFrame(
     ...     index=spp_idx,
     ...     data={
@@ -474,15 +451,14 @@
     1                   0.75                  -0.124939         1
     2                   1.00                   0.000000         1
     3                   0.75                  -0.124939         1
     5                   1.00                   0.000000         2
     6                   1.00                   0.000000         1
     7                   1.00                   0.000000         2
     """
-
     jacc_diss = []
     dists = []
     for idx, row in spp_matrix.iterrows():
         n_intersect = (spp_matrix & row).sum(axis='columns')
         n_unique_a = (spp_matrix & ~row).sum(axis='columns')
         n_unique_b = (~spp_matrix & row).sum(axis='columns')
 
@@ -501,164 +477,470 @@
             'distance': pd.concat(dists, ignore_index=True),
         }
     )
     res = res[res.distance > 0]
     return res
 
 
+def adjust_grid(gri: GridInfo, cfg: conf.Config) -> tuple[GridInfo, Sides, Caps]:
+    sides = cfg.locality.sides
+    caps = compute_caps(gri.qlist, sides)
+    gri.qlist = add_quadrat_centroids(gri.qlist, sides)
+    gri_adj, sides_adj = discard_axes(
+        gri, sides, discard_transect=cfg.discard_transect_info, discard_zone=cfg.discard_zone_info
+    )
+    sides_adj = Sides(sides_adj.x, sides_adj.y)
+    return (gri_adj, sides_adj, caps)
+
+
 def adjust_for_lvl(
-    enc: Encounters, quadrats: QList, locality: conf.Config, lvl: int, max_lvl: int, lvl_strat: LvlType, sides: Sides
-) -> tuple[list[pd.DataFrame], list[pd.DataFrame], Sides]:
+    gri: GridInfo, lvl: int, max_lvl: int, lvl_strat: LevelStrategy, sides: Sides
+) -> tuple[list[GridInfo], Sides]:
     """Transform study grid according to current level and level strategy.
-    Returns list because 'overlaid-subgrids' level strategy averages multiple subgrids.
-    """
 
-    # todo: split into individual functions, docs + unit tests
-    new_x = sides.x
-    new_y = sides.y
-    # todo: use either .loc or standalone pd.Series
-    quadrats['coord_x'] = quadrats.index.get_level_values('coord_x')
-    quadrats['coord_y'] = quadrats.index.get_level_values('coord_y')
+    Returns `list[GridInfo]` because 'overlaid-subgrids' level strategy averages multiple subgrids.
+    """
+    enc, quadrats = gri
     if lvl_strat == 'transect-additive':
-        enc = enc[enc.coord_x < lvl]
-        quadrats = quadrats[quadrats.coord_x < lvl]
+        res = adjust_transect_additive(enc, quadrats, sides, lvl)
     elif lvl_strat == 'zone-additive':
-        enc = enc[enc.coord_y < lvl]
-        quadrats = quadrats[quadrats.coord_y < lvl]
+        res = adjust_zone_additive(enc, quadrats, sides, lvl)
     elif lvl_strat == 'overlaid-subgrids':
-        cutoffs = cutting_bounds(quadrats, lvl)
-        q_subgrids = create_subgrids(quadrats, cutoffs)
-        shift_tuples = get_shift_tuples(q_subgrids)
-        q_subgrids = shift_coords(q_subgrids, shift_tuples, lvl)
+        enc_subgrids, q_subgrids, sides_adj = adjust_overlaid_subgrids(enc, quadrats, sides, lvl)
+        subgrids = [GridInfo(e, q) for e, q in zip(enc_subgrids, q_subgrids, strict=True)]
+    elif lvl_strat == 'transect-merging':
+        res = adjust_transect_merging(enc, quadrats, sides, lvl)
+    elif lvl_strat == 'zone-merging':
+        res = adjust_zone_merging(enc, quadrats, sides, lvl)
+    elif lvl_strat == 'repeated-transect-merging':
+        res = adjust_repeated_transect_merging(enc, quadrats, sides, lvl)
+    elif lvl_strat == 'striped-transect-merging':
+        res = adjust_striped_transect_merging(enc, quadrats, sides, lvl, max_lvl)
+    elif lvl_strat == 'nested-quadrats':
+        res = adjust_nested_quadrats(enc, quadrats, sides, lvl, max_lvl)
+    else:
+        raise conf.InvalidTaskError(lvl_strat)
 
-        enc_subgrids = create_subgrids(enc, cutoffs)
-        enc_subgrids = shift_coords(enc_subgrids, shift_tuples, lvl)
+    if lvl_strat != 'overlaid-subgrids':
+        subgrids = [GridInfo(res[0], res[1])]  # type: ignore[possibly-undefined] # is defined for any other option
+        sides_adj = res[2]
 
-        quadrats['centroid_x'] = quadrats['centroid_x'] + ((sides.x / 2) * lvl)
-        quadrats['centroid_y'] = quadrats['centroid_y'] + ((sides.y / 2) * lvl)
+    for grid in subgrids:  # type: ignore[possibly-undefined] # guaranteed to be defined by two ifs above
+        check_grid_consistency(grid)
 
-        new_x *= lvl
-        new_y *= lvl
-    elif lvl_strat == 'transect-merging':
-        enc = enc[enc.coord_x < lvl]
-        enc = replace_coords(enc, {'coord_x': 0})
+    return (subgrids, sides_adj)  # type: ignore[possibly-undefined] # guaranteed to be defined by two ifs above
 
-        quadrats = quadrats[quadrats.coord_x < lvl]
-        quadrats = replace_coords(quadrats, {'coord_x': 0})
-        quadrats = quadrats.drop_duplicates(subset=['coord_x', 'coord_y'])
-        quadrats['centroid_x'] = quadrats['centroid_x'] + ((sides.x / 2) * lvl)
 
-        new_x *= lvl
-    elif lvl_strat == 'zone-merging':
-        enc = enc[enc.coord_y < lvl]
-        enc = replace_coords(enc, {'coord_y': 0})
+def check_grid_consistency(grinfo: GridInfo, *, post_adj: bool = False) -> None:
+    enc, quadrats = grinfo
+    enc.set_flags(allows_duplicate_labels=False)
+    quadrats.set_flags(allows_duplicate_labels=False)
+    qids_enc = set(zip(enc.coord_x, enc.coord_y, strict=False))
+    qids_qlist = set(
+        zip(quadrats.index.get_level_values('coord_x'), quadrats.index.get_level_values('coord_y'), strict=False)
+    )
+    qids_diff = qids_enc - qids_qlist
+    if len(qids_diff) > 0:
+        raise InvalidQuadratsError(qids_diff, post_adj=post_adj)
+    if quadrats.isna().any().any():
+        raise MissingValuesError(quadrats[quadrats.isna().any(axis='columns')], post_adj=post_adj)
+    enc_subset = enc[['species', 'coord_x', 'coord_y']]
+    if enc_subset.isna().any().any():
+        raise MissingValuesError(enc_subset[enc_subset.isna().any(axis='columns')], post_adj=post_adj)
 
-        quadrats = quadrats[quadrats.coord_y < lvl]
-        quadrats = replace_coords(quadrats, {'coord_y': 0})
-        quadrats = quadrats.drop_duplicates(subset=['coord_x', 'coord_y'])
-        quadrats['centroid_y'] = quadrats['centroid_y'] + ((sides.y / 2) * lvl)
 
-        new_y *= lvl
-    elif lvl_strat == 'repeated-transect-merging':
-        new_xs = enc.coord_x.floordiv(lvl)
-        enc = replace_coords(enc, {'coord_x': new_xs})
+def adjust_transect_additive(
+    enc: Encounters, qlist: QList, sides: Sides, level: int
+) -> tuple[Encounters, QList, Sides]:
+    """Adjust passed encounters, quadrat list and sides for transect-additive strategy at given `level`.
+
+    >>> enc = pd.DataFrame(
+    ...     {
+    ...         'coord_x': [0, 1, 1, 1, 3],
+    ...         'coord_y': [0, 0, 1, 0, 3],
+    ...         'species': ['B', 'A', 'A', 'C', 'B'],
+    ...     }
+    ... )
+    >>> qlist = pd.DataFrame(
+    ...     index=pd.MultiIndex.from_arrays([[0, 0, 1, 1, 2, 3], [0, 1, 0, 1, 0, 3]], names=('coord_x', 'coord_y')),
+    ...     data={'centroid_x': [2, 2, 6, 6, 10, 14], 'centroid_y': [2, 6, 2, 6, 2, 14]},
+    ... )
+    >>> sides = Sides(4, 4)
+    >>> res = adjust_transect_additive(enc, qlist, sides, level=2)
+    >>> res[0]
+       coord_x  coord_y species
+    0        0        0       B
+    1        1        0       A
+    2        1        1       A
+    3        1        0       C
+    >>> res[1]  # doctest: +NORMALIZE_WHITESPACE
+                     centroid_x  centroid_y
+    coord_x coord_y
+    0       0                 2           2
+            1                 2           6
+    1       0                 6           2
+            1                 6           6
+    >>> res[2]
+    Sides(x=4.0, y=4.0)
+    """
+    enc = enc[enc.coord_x < level]
+    idx = pd.IndexSlice
+    qlist = qlist.loc[idx[0 : level - 1, :], :]
+    return enc, qlist, sides
 
-        new_xs = quadrats.coord_x.floordiv(lvl)
-        quadrats = replace_coords(quadrats, {'coord_x': new_xs})
-        quadrats = quadrats.drop_duplicates(subset=['coord_x', 'coord_y'])
-        quadrats['centroid_x'] = quadrats['centroid_x'] + ((sides.x / 2) * lvl)
-        quadrats = quadrats.set_index(['coord_x', 'coord_y'], drop=False, verify_integrity=True)
 
-        new_x *= lvl
-    elif lvl_strat == 'striped-transect-merging':
-        enc = enc[(enc.coord_x % max_lvl) < lvl]
-        new_xs = enc.coord_x.floordiv(max_lvl)
-        enc = replace_coords(enc, {'coord_x': new_xs})
-
-        quadrats = quadrats[(quadrats.coord_x % max_lvl) < lvl]
-        new_xs = quadrats.coord_x.floordiv(max_lvl)
-        quadrats = replace_coords(quadrats, {'coord_x': new_xs})
-        quadrats = quadrats.drop_duplicates(subset=['coord_x', 'coord_y'])
-        quadrats = quadrats.set_index(['coord_x', 'coord_y'], drop=False, verify_integrity=True)
-        quadrats['centroid_x'] = quadrats['centroid_x'] + ((sides.x / 2) * lvl)
+def adjust_zone_additive(enc: Encounters, qlist: QList, sides: Sides, level: int) -> tuple[Encounters, QList, Sides]:
+    """Adjust passed encounters, quadrat list and sides for zone-additive strategy at given `level`.
 
-        new_x *= lvl
-    elif lvl_strat == 'nested-quadrats':
-        merges = [1, 2]
-        discards = [2, 1]
-        merge_n_quadrats = 2 ** (lvl - 1)
-        print('CURR LVL: ', lvl)
-        print(f'MERGING {merge_n_quadrats}x{merge_n_quadrats} orig quadrats\n')
-        assert merge_n_quadrats == merges[lvl - 1]
-        retain_every_nth = 2 ** (max_lvl - lvl)
-        print(f'WILL RETAIN EVERY {retain_every_nth}nd quadrat\n')
-        assert retain_every_nth == discards[lvl - 1]
-
-        new_xs = enc.coord_x.floordiv(merge_n_quadrats)
-        new_ys = enc.coord_y.floordiv(merge_n_quadrats)
-        enc = replace_coords(enc, {'coord_x': new_xs, 'coord_y': new_ys})
-        keep_x = (enc.coord_x % retain_every_nth) == 0
-        keep_y = (enc.coord_y % retain_every_nth) == 0
-        enc = enc[keep_x & keep_y]
-        # todo: do quadrats first, then simply drop those not in quadrats?
-
-        new_xs = quadrats.coord_x.floordiv(merge_n_quadrats)
-        new_ys = quadrats.coord_y.floordiv(merge_n_quadrats)
-        quadrats = replace_coords(quadrats, {'coord_x': new_xs, 'coord_y': new_ys})
-        quadrats = quadrats.drop_duplicates(subset=['coord_x', 'coord_y'])
-
-        keep_x = (quadrats.coord_x % retain_every_nth) == 0
-        keep_y = (quadrats.coord_y % retain_every_nth) == 0
-        quadrats = quadrats[keep_x & keep_y]
-
-        quadrats = quadrats.set_index(['coord_x', 'coord_y'], drop=False, verify_integrity=True)
-
-        quadrats['centroid_x'] = quadrats['centroid_x'] + ((sides.x / 2) * merge_n_quadrats)
-        quadrats['centroid_y'] = quadrats['centroid_y'] + ((sides.y / 2) * merge_n_quadrats)
-
-        new_x = sides.x * merge_n_quadrats
-        new_y = sides.y * merge_n_quadrats
-
-        qids_enc = set(enc.quadrat_id)
-        qids_qlist = set(quadrats.quadrat_id)
-        qids_diff = qids_enc - qids_qlist
-        if len(qids_diff) > 0:
-            print(
-                f'''Filtered dataset contains encounters in quadrats not found in quadrat list.
-                Possible causes may be using quadrat list for unintended locality, incorrectly set-up filters, e.g. *from* and *to* dates in taskfile\'s locality section or simply mistakes/typos in provided quadrat list or dataset.
-                Extraneous IDs:
-                {list(sorted(qids_diff))}
-                '''
-            )
-            sys.exit(1)
-    else:
-        raise conf.InvalidTaskError(lvl_strat)
+    >>> enc = pd.DataFrame(
+    ...     {
+    ...         'coord_x': [0, 1, 1, 1, 3],
+    ...         'coord_y': [0, 0, 1, 0, 3],
+    ...         'species': ['B', 'A', 'A', 'C', 'B'],
+    ...     }
+    ... )
+    >>> qlist = pd.DataFrame(
+    ...     index=pd.MultiIndex.from_arrays([[0, 0, 1, 1, 2, 3], [0, 1, 0, 1, 0, 3]], names=('coord_x', 'coord_y')),
+    ...     data={'centroid_x': [2, 2, 6, 6, 10, 14], 'centroid_y': [2, 6, 2, 6, 2, 14]},
+    ... )
+    >>> sides = Sides(4, 4)
+    >>> res = adjust_zone_additive(enc, qlist, sides, level=1)
+    >>> res[0]
+       coord_x  coord_y species
+    0        0        0       B
+    1        1        0       A
+    3        1        0       C
+    >>> res[1]  # doctest: +NORMALIZE_WHITESPACE
+                     centroid_x  centroid_y
+    coord_x coord_y
+    0       0                 2           2
+    1       0                 6           2
+    2       0                10           2
+    >>> res[2]
+    Sides(x=4.0, y=4.0)
+    """
+    enc = enc[enc.coord_y < level]
+    idx = pd.IndexSlice
+    qlist = qlist.loc[idx[:, 0 : level - 1], :]
+    return enc, qlist, sides
 
-    assert list(quadrats['coord_x']) == list(quadrats.index.get_level_values('coord_x'))
-    assert list(quadrats['coord_y']) == list(quadrats.index.get_level_values('coord_y'))
 
-    if lvl_strat != 'overlaid-subgrids':
-        enc_subgrids = [enc]
-        q_subgrids = [quadrats]
-    sides_adj = Sides(new_x, new_y)
+def adjust_transect_merging(enc: Encounters, qlist: QList, sides: Sides, level: int) -> tuple[Encounters, QList, Sides]:
+    """Adjust passed encounters, quadrat list and sides for transect-merging strategy at given `level`.
 
-    assert len(enc_subgrids) == len(q_subgrids)
-    for e, q in zip(enc_subgrids, q_subgrids, strict=True):
-        assert set(zip(e.coord_x, e.coord_y)).issubset(
-            set(zip(q.coord_x, q.coord_y))
-        )  # every encounter must be in a known quadrat
+    >>> enc = pd.DataFrame(
+    ...     {
+    ...         'coord_x': [0, 1, 1, 1, 3],
+    ...         'coord_y': [0, 0, 1, 2, 3],
+    ...         'species': ['B', 'A', 'A', 'C', 'B'],
+    ...     }
+    ... )
+    >>> qlist = pd.DataFrame(
+    ...     index=pd.MultiIndex.from_arrays([[0, 0, 1, 1, 1, 3], [0, 1, 0, 1, 2, 3]], names=('coord_x', 'coord_y')),
+    ...     data={'centroid_x': [2, 2, 6, 6, 10, 14], 'centroid_y': [2, 6, 2, 6, 10, 14]},
+    ... )
+    >>> sides = Sides(4, 4)
+    >>> res = adjust_transect_merging(enc, qlist, sides, level=3)
+    >>> res[0]
+       coord_x  coord_y species
+    0        0        0       B
+    1        0        0       A
+    2        0        1       A
+    3        0        2       C
+    >>> res[1]  # doctest: +NORMALIZE_WHITESPACE
+                     centroid_x  centroid_y
+    coord_x coord_y
+    0       0                 6           2
+            1                 6           6
+            2                 6          10
+    >>> res[2]
+    Sides(x=12.0, y=4.0)
+    """
+    enc = enc[enc.coord_x < level]
+    enc.loc[:, 'coord_x'] = 0
+
+    idx = pd.IndexSlice
+    qlist = qlist.loc[idx[0 : level - 1, :], :]
+    new_idx = pd.MultiIndex.from_arrays(
+        [[0] * len(qlist), qlist.index.get_level_values('coord_y')], names=['coord_x', 'coord_y']
+    )
+    qlist = qlist.set_index(new_idx)
+    qlist = qlist[~qlist.index.duplicated()]
+    qlist.loc[:, 'centroid_x'] = (sides.x * level) / 2
+    qlist = qlist.drop_duplicates()
 
-    return (enc_subgrids, q_subgrids, sides_adj)
+    return enc, qlist, Sides(sides.x * level, sides.y)
 
 
-def is_int_list(lst: Sequence[object]) -> TypeGuard[Sequence[int]]:
-    """Verify that all objects in *lst* are integers."""
-    # todo: test
+def adjust_zone_merging(enc: Encounters, qlist: QList, sides: Sides, level: int) -> tuple[Encounters, QList, Sides]:
+    """Adjust passed encounters, quadrat list and sides for zone-merging strategy at given `level`.
 
-    return all(isinstance(elem, int) for elem in lst)
+    >>> enc = pd.DataFrame(
+    ...     {
+    ...         'coord_x': [0, 1, 1, 1, 3],
+    ...         'coord_y': [0, 0, 1, 2, 3],
+    ...         'species': ['B', 'A', 'A', 'C', 'B'],
+    ...     }
+    ... )
+    >>> qlist = pd.DataFrame(
+    ...     index=pd.MultiIndex.from_arrays([[0, 0, 1, 1, 1, 3], [0, 1, 0, 1, 2, 3]], names=('coord_x', 'coord_y')),
+    ...     data={'centroid_x': [2, 2, 6, 6, 10, 14], 'centroid_y': [2, 6, 2, 6, 10, 14]},
+    ... )
+    >>> sides = Sides(4, 4)
+    >>> res = adjust_zone_merging(enc, qlist, sides, level=3)
+    >>> res[0]
+       coord_x  coord_y species
+    0        0        0       B
+    1        1        0       A
+    2        1        0       A
+    3        1        0       C
+    >>> res[1]  # doctest: +NORMALIZE_WHITESPACE
+                     centroid_x  centroid_y
+    coord_x coord_y
+    0       0                 2           6
+    1       0                 6           6
+    >>> res[2]
+    Sides(x=4.0, y=12.0)
+    """
+    enc = enc[enc.coord_y < level]
+    enc.loc[:, 'coord_y'] = 0
+
+    idx = pd.IndexSlice
+    qlist = qlist.loc[idx[:, 0 : level - 1], :]
+    new_idx = pd.MultiIndex.from_arrays(
+        [qlist.index.get_level_values('coord_x'), [0] * len(qlist)], names=['coord_x', 'coord_y']
+    )
+    qlist = qlist.set_index(new_idx)
+    qlist = qlist[~qlist.index.duplicated()]
+    qlist.loc[:, 'centroid_y'] = (sides.y * level) / 2
+
+    return enc, qlist, Sides(sides.x, sides.y * level)
+
+
+def adjust_overlaid_subgrids(
+    enc: Encounters, qlist: QList, sides: Sides, level: int
+) -> tuple[list[Encounters], list[QList], Sides]:
+    """Adjust passed encounters, quadrat list and sides for overlaid-subgrids strategy at given `level`.
+
+    >>> enc = pd.DataFrame(
+    ...     {
+    ...         'coord_x': [0, 1, 1, 1, 3],
+    ...         'coord_y': [0, 0, 1, 2, 3],
+    ...         'species': ['B', 'A', 'A', 'C', 'B'],
+    ...     }
+    ... )
+    >>> qlist = pd.DataFrame(
+    ...     index=pd.MultiIndex.from_arrays([[0, 0, 1, 1, 1, 3], [0, 1, 0, 1, 2, 3]], names=('coord_x', 'coord_y')),
+    ...     data={'centroid_x': [2, 2, 6, 6, 10, 14], 'centroid_y': [2, 6, 2, 6, 10, 14]},
+    ... )
+    >>> sides = Sides(4, 4)
+    >>> res = adjust_overlaid_subgrids(enc, qlist, sides, level=1)
+    >>> res[0]
+    [   coord_x  coord_y species
+    0        0        0       B
+    1        1        0       A
+    2        1        1       A
+    3        1        2       C
+    4        3        3       B]
+    >>> res[1]  # doctest: +NORMALIZE_WHITESPACE
+    [                 centroid_x  centroid_y
+    coord_x coord_y
+    0       0                 2           2
+            1                 2           6
+    1       0                 6           2
+            1                 6           6
+            2                10          10
+    3       3                14          14]
+    >>> res[2]
+    Sides(x=4.0, y=4.0)
+    >>> res = adjust_overlaid_subgrids(enc, qlist, sides, level=2)
+    >>> res[0]
+    [   coord_x  coord_y species
+    0        0        0       B
+    1        0        0       A
+    2        0        0       A
+    3        0        1       C
+    4        1        1       B]
+    >>> res[1]  # doctest: +NORMALIZE_WHITESPACE
+    [                 centroid_x  centroid_y
+    coord_x coord_y
+    0       0                 4           4
+            1                 4           8
+    1       1                 8           8]
+    >>> res[2]
+    Sides(x=8.0, y=8.0)
+    """
+    qlist['coord_x'] = qlist.index.get_level_values('coord_x')
+    qlist['coord_y'] = qlist.index.get_level_values('coord_y')
+    cutoffs = cutting_bounds(qlist, level)
+    q_subgrids = create_subgrids(qlist, cutoffs)
+    shift_tuples = get_shift_tuples(q_subgrids)
+    q_subgrids = shift_coords(q_subgrids, shift_tuples, level)
+
+    enc_subgrids = create_subgrids(enc, cutoffs)
+    enc_subgrids = shift_coords(enc_subgrids, shift_tuples, level)
+
+    for q_subgrid in q_subgrids:
+        q_subgrid.loc[:, 'centroid_x'] = qlist['centroid_x'] + ((sides.x / 2) * (level - 1))
+        q_subgrid.loc[:, 'centroid_y'] = qlist['centroid_y'] + ((sides.y / 2) * (level - 1))
+        q_subgrid.drop(columns=['coord_x', 'coord_y'], inplace=True)  # noqa: PD002
+
+    return enc_subgrids, q_subgrids, Sides(sides.x * level, sides.y * level)
+
+
+def adjust_repeated_transect_merging(
+    enc: Encounters, qlist: QList, sides: Sides, level: int
+) -> tuple[Encounters, QList, Sides]:
+    """Adjust passed encounters, quadrat list and sides for striped-transect-merging strategy at given `level`.
+
+    >>> enc = pd.DataFrame(
+    ...     {
+    ...         'coord_x': [0, 1, 1, 1, 3],
+    ...         'coord_y': [0, 0, 1, 2, 3],
+    ...         'species': ['B', 'A', 'A', 'C', 'B'],
+    ...     }
+    ... )
+    >>> qlist = pd.DataFrame(
+    ...     index=pd.MultiIndex.from_arrays([[0, 0, 1, 1, 1, 3], [0, 1, 0, 1, 2, 3]], names=('coord_x', 'coord_y')),
+    ...     data={'centroid_x': [2, 2, 6, 6, 10, 14], 'centroid_y': [2, 6, 2, 6, 10, 14]},
+    ... )
+    >>> sides = Sides(4, 4)
+    >>> res = adjust_repeated_transect_merging(enc, qlist, sides, level=2)
+    >>> res[0]
+       coord_x  coord_y species
+    0        0        0       B
+    1        0        0       A
+    2        0        1       A
+    3        0        2       C
+    4        1        3       B
+    >>> res[1]  # doctest: +NORMALIZE_WHITESPACE
+                     centroid_x  centroid_y
+    coord_x coord_y
+    0       0               6.0           2
+            1               6.0           6
+            2              14.0          10
+    1       3              18.0          14
+    >>> res[2]
+    Sides(x=8.0, y=4.0)
+    """
+    new_xs = enc.coord_x.floordiv(level)
+    enc.loc[:, 'coord_x'] = new_xs
+
+    new_xs = qlist.index.get_level_values('coord_x').to_series().floordiv(level)
+    new_idx = pd.MultiIndex.from_arrays([new_xs, qlist.index.get_level_values('coord_y')], names=('coord_x', 'coord_y'))
+    qlist = qlist.set_index(new_idx)
+    qlist = qlist[~qlist.index.duplicated()]
+    qlist['centroid_x'] = qlist['centroid_x'] + ((sides.x / 2) * level)
+
+    return enc, qlist, Sides(sides.x * level, sides.y)
+
+
+def adjust_striped_transect_merging(
+    enc: Encounters, qlist: QList, sides: Sides, level: int, max_level: int
+) -> tuple[Encounters, QList, Sides]:
+    """Adjust passed grid info list and sides for striped-transect-merging strategy at given `level` and `max_level`.
+
+    >>> enc = pd.DataFrame(
+    ...     {
+    ...         'coord_x': [0, 1, 1, 1, 3],
+    ...         'coord_y': [0, 0, 1, 2, 3],
+    ...         'species': ['B', 'A', 'A', 'C', 'B'],
+    ...     }
+    ... )
+    >>> qlist = pd.DataFrame(
+    ...     index=pd.MultiIndex.from_arrays([[0, 0, 1, 1, 1, 3], [0, 1, 0, 1, 2, 3]], names=('coord_x', 'coord_y')),
+    ...     data={'centroid_x': [2, 2, 6, 6, 10, 14], 'centroid_y': [2, 6, 2, 6, 10, 14]},
+    ... )
+    >>> sides = Sides(4, 4)
+    >>> res = adjust_striped_transect_merging(enc, qlist, sides, level=1, max_level=2)
+    >>> res[0]
+       coord_x  coord_y species
+    0        0        0       B
+    >>> res[1]  # doctest: +NORMALIZE_WHITESPACE
+                     centroid_x  centroid_y
+    coord_x coord_y
+    0       0               4.0           2
+            1               4.0           6
+    >>> res[2]
+    Sides(x=4.0, y=4.0)
+    """
+    enc = enc[(enc.coord_x % max_level) < level]
+    new_xs = enc.coord_x.floordiv(max_level)
+    enc.loc[:, 'coord_x'] = new_xs
+
+    q_xs = qlist.index.get_level_values('coord_x')
+    qlist = qlist[(q_xs % max_level) < level]
+    q_xs = qlist.index.get_level_values('coord_x')
+    new_xs = q_xs.to_series().floordiv(max_level)
+    new_idx = pd.MultiIndex.from_arrays([new_xs, qlist.index.get_level_values('coord_y')], names=('coord_x', 'coord_y'))
+    qlist = qlist.set_index(new_idx)
+
+    qlist = qlist[~qlist.index.duplicated()]
+
+    qlist['centroid_x'] = qlist['centroid_x'] + ((sides.x / 2) * level)
+
+    return enc, qlist, Sides(sides.x * level, sides.y)
+
+
+def adjust_nested_quadrats(
+    enc: Encounters, qlist: QList, sides: Sides, level: int, max_level: int
+) -> tuple[Encounters, QList, Sides]:
+    """Adjust passed grid information for striped-transect-merging strategy at given `level` and `max_level`.
+
+    >>> enc = pd.DataFrame(
+    ...     {
+    ...         'coord_x': [0, 1, 1, 1, 3],
+    ...         'coord_y': [0, 0, 1, 2, 3],
+    ...         'species': ['B', 'A', 'A', 'C', 'B'],
+    ...     }
+    ... )
+    >>> qlist = pd.DataFrame(
+    ...     index=pd.MultiIndex.from_arrays([[0, 0, 1, 1, 1, 3], [0, 1, 0, 1, 2, 3]], names=('coord_x', 'coord_y')),
+    ...     data={'centroid_x': [2, 2, 6, 6, 10, 14], 'centroid_y': [2, 6, 2, 6, 10, 14]},
+    ... )
+    >>> sides = Sides(4, 4)
+    >>> res = adjust_nested_quadrats(enc, qlist, sides, level=1, max_level=2)
+    >>> res[0]
+       coord_x  coord_y species
+    0        0        0       B
+    >>> res[1]  # doctest: +NORMALIZE_WHITESPACE
+                     centroid_x  centroid_y
+    coord_x coord_y
+    0       0               4.0         4.0
+    >>> res[2]
+    Sides(x=4.0, y=4.0)
+    """
+    merge_n_quadrats = 2 ** (level - 1)
+    retain_every_nth = 2 ** (max_level - level)
+
+    new_xs = enc.coord_x.floordiv(merge_n_quadrats)
+    new_ys = enc.coord_y.floordiv(merge_n_quadrats)
+    enc = enc.assign(coord_x=new_xs, coord_y=new_ys)
+    keep_x = (enc.coord_x % retain_every_nth) == 0
+    keep_y = (enc.coord_y % retain_every_nth) == 0
+    enc = enc[keep_x & keep_y]
+
+    qlist['coord_x'] = qlist.index.get_level_values('coord_x')
+    qlist['coord_y'] = qlist.index.get_level_values('coord_y')
+
+    new_xs = qlist.coord_x.floordiv(merge_n_quadrats)
+    new_ys = qlist.coord_y.floordiv(merge_n_quadrats)
+    qlist = qlist.assign(coord_x=new_xs, coord_y=new_ys)
+    qlist = qlist.drop_duplicates(subset=['coord_x', 'coord_y'])
+
+    keep_x = (qlist.coord_x % retain_every_nth) == 0
+    keep_y = (qlist.coord_y % retain_every_nth) == 0
+    qlist = qlist[keep_x & keep_y]
+
+    qlist = qlist.set_index(['coord_x', 'coord_y'], drop=True, verify_integrity=True)
+
+    qlist['centroid_x'] = qlist['centroid_x'] + ((sides.x / 2) * merge_n_quadrats)
+    qlist['centroid_y'] = qlist['centroid_y'] + ((sides.y / 2) * merge_n_quadrats)
+
+    return enc, qlist, Sides(sides.x * merge_n_quadrats, sides.y * merge_n_quadrats)
 
 
 def add_quadrat_centroids(quadrats: pd.DataFrame, sides: Sides) -> pd.DataFrame:
     """Add centroid_x and centroid_y columns to *quadrats* with coordinates of quadrats' centroids.
 
     >>> qlist = pd.DataFrame(
     ...     index=pd.MultiIndex.from_arrays([[0, 0, 1, 1, 2], [0, 1, 0, 1, 0]], names=('coord_x', 'coord_y'))
@@ -673,108 +955,91 @@
     2       0               2.5         1.0
     """
     quadrats['centroid_x'] = (quadrats.index.get_level_values('coord_x') * sides.x) + (sides.x / 2)
     quadrats['centroid_y'] = (quadrats.index.get_level_values('coord_y') * sides.y) + (sides.y / 2)
     return quadrats
 
 
-def compute_caps(quadrats: QList, sides: Sides) -> dict[str, float]:
-    """Compute and return maximum possible area distance in a study grid.
+def compute_caps(quadrats: QList, sides: Sides) -> Caps:
+    """Compute and return maximum possible area or distance in a study grid.
+
     This is necessary because some grid transformations, e.g. involving
     quadrat merging, could result in the grid seeming larger for a
     given level.
     Does not take grid irregularities, like nonsampled shallows, into account.
 
     >>> qlist = pd.DataFrame(
     ...     index=pd.MultiIndex.from_arrays([[0, 0, 1, 1, 2], [0, 1, 0, 1, 0]], names=('coord_x', 'coord_y'))
     ... )
     >>> compute_caps(qlist, Sides(1, 2))
-    {'total_area': 12, 'max1dx': 3, 'max1dy': 4, 'diagonal': 5.0, 'centroid': 2.8284271247461903}
+    {'total_area': 12.0, 'max1dx': 3.0, 'max1dy': 4.0, 'diagonal': 5.0, 'centroid': 2.8284271247461903}
     """
-
     x_max = quadrats.index.get_level_values('coord_x').max()
     y_max = quadrats.index.get_level_values('coord_y').max()
     max1dx = (1 + x_max) * sides.x
     max1dy = (1 + y_max) * sides.y
     total_area = max1dx * max1dy
     diagonal = math.sqrt(max1dx**2 + max1dy**2)
     centroid_diff = {'x': max1dx - sides.x, 'y': max1dy - sides.y}
     centroid = math.sqrt(centroid_diff['x'] ** 2 + centroid_diff['y'] ** 2)
     return {'total_area': total_area, 'max1dx': max1dx, 'max1dy': max1dy, 'diagonal': diagonal, 'centroid': centroid}
 
 
+def get_lvl_infos(grinfo: GridInfo, sides_adj: Sides, caps: Caps, cfg: conf.Config) -> dict[int, LevelInfo]:
+    infos = {}
+    for level in sorted(set(cfg.levels)):
+        subgrids, sides_adj_lvl = adjust_for_lvl(
+            grinfo,
+            level,
+            max(cfg.levels),
+            cfg.level_strategy,
+            sides_adj,
+        )
+        capped_dist_fn = get_distance_function(cfg.distance_type, sides_adj_lvl, caps)
+        dmats = [distance_matrix(gri.qlist, capped_dist_fn) for gri in subgrids]
+        infos[level] = copy.deepcopy(LevelInfo(subgrids, dmats, sides_adj_lvl))
+    return infos
+
+
 def save_results(
     args: argparse.Namespace,
     out_dir: Path,
-    completed: dict[str, pd.DataFrame],
-    additional: dict[str, list[str | pd.DataFrame]],
+    completed: list[pd.DataFrame],
+    additional: list[str | pd.DataFrame | None],
+    analysis_info: tuple[str, int],
 ) -> None:
-    """Save analysis results in *completed* and additional data in
-    *additional* to *out_dir*. *out_dir* must be created
-    beforehand.
-    """
-
-    for analysis, df in completed.items():
-        out_file = analysis_results_name(out_dir, args, analysis)
-        df.to_csv(out_file, index=False)
-        print(f'Result written to {out_file}')
-
-    for analysis, data_lst in additional.items():
-        out_file = out_dir / f'{args.taskfile.stem}-{analysis}-add'
-        if isinstance(data_lst[0], pd.DataFrame):
-            out_file = out_file.with_suffix('.csv')
-            for lvl, adf in enumerate(data_lst):
-                adf['level'] = lvl  # type: ignore[index]
-            pd.concat(data_lst).to_csv(out_file)  # type: ignore[arg-type]
-        else:
-            out_file = out_file.with_suffix('.txt')
-            with open(out_file, 'w') as out:
-                out.write('\n'.join(data_lst))  # type: ignore[arg-type]
-        print(f'Additional data written to {out_file}')
-
-
-def replace_coords(df: pd.DataFrame, coords: dict[CoordCol, int | pd.Series]) -> pd.DataFrame:
-    """Assigns coordinates to appropriate columns and changes quadrat_id to reflect said changes.
-    Erases dd/mm/yyyy part because it causes certain quadrats to be split over dates
+    """Save analysis results in `completed` and additional data in `additional` to `out_dir`.
 
-    >>> df = pd.DataFrame(
-    ...     {
-    ...         'coord_x': [0, 0, 1, 1, 2],
-    ...         'coord_y': [0, 1, 0, 1, 0],
-    ...         'quadrat_id': [
-    ...             'T_1_2/3/2022_1',
-    ...             'T_1_2/3/2022_2',
-    ...             'T_2_2/3/2022_1',
-    ...             'T_2_3/3/2022_2',
-    ...             'T_3_3/3/2022_1',
-    ...         ],
-    ...     }
-    ... )
-    >>> new_coords = {'coord_x': [3, 4, 5, 6, 7], 'coord_y': [8, 7, 6, 5, 4]}
-    >>> replace_coords(df, new_coords)
-       coord_x  coord_y quadrat_id
-    0        3        8      T_4_9
-    1        4        7      T_5_8
-    2        5        6      T_6_7
-    3        6        5      T_7_6
-    4        7        4      T_8_5
-    """
-
-    df = df.assign(**coords)  # type: ignore[misc]
-
-    id_split = df['quadrat_id'].str.split('_')
-    q_id_iter = zip(id_split, df['coord_x'], df['coord_y'], strict=True)
-    new_ids = [strs[0] + f'_{x+1}_{y+1}' for strs, x, y in q_id_iter]
-    id_split = pd.Series(data=new_ids, index=id_split.index)
-    df['quadrat_id'] = id_split
-    return df
+    `out_dir` must be created beforehand.
+    """
+    a_type, a_idx = analysis_info
+    out_file = analysis_results_filename(out_dir, args.taskfile, a_type, a_idx)
+    pd.concat(completed).to_csv(out_file, index=False)
+    print(f'Result written to {out_file}')
+
+    additional = list(filter(lambda x: x is not None, additional))
+    if not additional:
+        return
+    out_file = out_file.with_stem(f'{out_file.stem}-add')
+    if isinstance(additional[0], pd.DataFrame):
+        out_file = out_file.with_suffix('.csv')
+        for lvl, adf in enumerate(additional):
+            adf['level'] = lvl + 1  # type: ignore[index]
+        with warnings.catch_warnings():
+            warnings.simplefilter(action='ignore', category=FutureWarning)
+            pd.concat(additional, ignore_index=True).to_csv(out_file, index=False)  # type: ignore[arg-type]
+    else:
+        out_file = out_file.with_suffix('.txt')
+        out_file.write_text('\n'.join(additional))  # type: ignore[arg-type] # guaranteed list[str]
+    print(f'Additional data written to {out_file}')
 
 
 def total_radius_richness(dist_group: pd.DataFrame, spp_matrix: pd.DataFrame) -> int:
     """Return total richness in a given distance group.
+
     Assumes that distance group (radius) from a certain quadrat
     has already been created by previous grouping.
 
     >>> idx = pd.MultiIndex.from_arrays(
     ...     [[0, 0, 0, 0], [0, 0, 0, 0], [10, 10, 10, 10], [0, 0, 0, 0], [0, 1, 2, 3]],
     ...     names=('coord_x', 'coord_y', 'distance', 'coord_x_other', 'coord_y_other'),
     ... )
@@ -789,228 +1054,210 @@
     ...         'D': [False, False, False, False],
     ...         'E': [False, False, True, False],
     ...     },
     ... )
     >>> total_radius_richness(dist_group, spp_matrix)
     4
     """
-
     peri_idx = pd.MultiIndex.from_arrays(
         [dist_group.index.get_level_values('coord_x_other'), dist_group.index.get_level_values('coord_y_other')]
     )
     perimeter = spp_matrix.loc[peri_idx]
-    perimeter_richness = perimeter.cumsum().astype(bool).iloc[-1].sum()
+    perimeter_richness = cast(int, perimeter.cumsum().astype(bool).iloc[-1].sum())
     return perimeter_richness
 
 
 def flatten_multicolumns(df: pd.DataFrame) -> pd.DataFrame:
-    """Convenience function to flatten and rename multicolumns in a DataFrame
+    """Flatten and rename multicolumns in a DataFrame.
 
     >>> cols = pd.MultiIndex.from_tuples([('top', 'btm1'), ('top', 'btm2')])
     >>> multi = pd.DataFrame(data=[[0, 1], [2, 3]], columns=cols)
     >>> flatten_multicolumns(multi)
        top_btm1  top_btm2
     0         0         1
     1         2         3
     """
-    df.columns = df.columns.to_flat_index()
+    df.columns = df.columns.to_flat_index()  # type: ignore[no-untyped-call] # is typed, mypy 1.9.0 bug?
     name_map = {col: f'{col[0]}_{col[1]}' for col in df.columns}
     df = df.rename(name_map, axis='columns', errors='raise')
     return df
 
 
-def get_distance_function(dist_type: str, sides_adj: Sides, caps: dict[str, float]) -> DistFunction:
+def get_distance_function(dist_type: Distance, sides_adj: Sides, caps: Caps) -> DistFunction:
     """Return function to use for computing values in distance matrix.
 
-    >>> loc = conf.Config.from_string('sides_adj = { x = 1, y = 1}')
-    >>> get_distance_function('diagonal', loc, None)  # doctest: +ELLIPSIS
+    >>> sides = Sides(1, 1)
+    >>> get_distance_function('diagonal', sides, None)  # doctest: +ELLIPSIS
     <function get_distance_function.<locals>.<lambda> at ...>
-    >>> get_distance_function(':)', loc, None)  # doctest: +IGNORE_EXCEPTION_DETAIL
+    >>> get_distance_function(':)', sides, None)  # doctest: +IGNORE_EXCEPTION_DETAIL
     Traceback (most recent call last):
-    RuntimeError: Invalid distance ":)" specified in taskfile
+    seal.exceptions.InvalidLiteralError: argument dist_type=':)' is not a valid choice
     """
-
     if dist_type == 'centroid':
-        return lambda ps, qs: q_distance_centroid(ps, qs, sides_adj, caps)
-    elif dist_type == 'max1d':
+        return lambda ps, qs: q_distance_centroid(ps, qs, caps)
+    if dist_type == 'max1d':
         return lambda ps, qs: q_distance_collapsed(ps, qs, sides_adj, caps)
-    elif dist_type == 'diagonal':
+    if dist_type == 'diagonal':
         return lambda ps, qs: q_distance_diagonal(ps, qs, sides_adj, caps)
-    else:
-        raise RuntimeError(f'Invalid distance "{dist_type}" specified in taskfile')
+    raise InvalidLiteralError(f'{dist_type=}')
 
 
 def filter_encounters(enc: pd.DataFrame, cfg: conf.Config) -> pd.DataFrame:
-    """Return encounters filtered according to criteria specified in *cfg*
-    Supported criteria are documented in example-task.conf.
-    """
+    """Return encounters filtered according to criteria specified in `cfg`.
 
-    locality = cfg.get_subconf('locality')
-    l_from = date.fromisoformat(locality.get_string('from', f'{date.min}'))
-    l_to = date.fromisoformat(locality.get_string('to', f'{date.max}'))
-    l_name = locality.get_string('name')
-    enc = enc[(enc.locality == l_name) & (enc.date.dt.date >= l_from) & (enc.date.dt.date <= l_to)]
+    Supported criteria are documented in 0-example-task.toml.
+    """
+    if cfg.locality.name:
+        enc = enc[enc.locality == cfg.locality.name]
+    if cfg.locality.from_:
+        enc = enc[enc.date >= cfg.locality.from_]
+    if cfg.locality.to:
+        enc = enc[enc.date <= cfg.locality.to]
 
-    direction = cfg.get_string('direction', '-')
-    if direction[0] == 'r':
+    if cfg.direction == 'richer':
         dirdiff = direction_difference(enc)
         enc = enc.join(dirdiff, on=['coord_x', 'coord_y'], validate='m:1')
         # drop if (forward_has_more_species) and (direction_is_b)
         enc = enc[~((enc['diff_#'] >= 0) & (enc.direction == 'b'))]
         enc = enc[~((enc['diff_#'] < 0) & (enc.direction == 'f'))]
         enc = enc.drop(['f_species', 'b_species', 'diff_%', 'diff_#'], axis='columns', errors='raise')
-    elif direction[0] == 'b' or direction[0] == 'f':
-        enc = enc[enc.direction == direction[0]]
+    elif cfg.direction[0] in {'backward', 'forward'}:
+        enc = enc[enc.direction == cfg.direction[0]]
 
-    include_families = cfg.get_list('include-families', [])
-    if include_families:
-        enc = enc[enc.family.isin(include_families)]
-    else:
-        exclude_families = cfg.get_list('exclude-families', [])
-        enc = enc[~enc.family.isin(exclude_families)]
-    phases = cfg.get_list('exclude-phases', [])
-    enc = enc[~enc.phase.isin(phases)]
-    include_tiny = cfg.get_bool('include-tiny', False)
-    if not include_tiny:
+    if cfg.include_families:
+        enc = enc[enc.family.isin(cfg.include_families)]
+    elif cfg.exclude_families:
+        enc = enc[~enc.family.isin(cfg.exclude_families)]
+    if cfg.exclude_phases:
+        enc = enc[~enc.phase.isin(cfg.exclude_phases)]
+    if not cfg.include_tiny:
         enc = enc[enc.significant_size]
-    use_morph = cfg.get_bool('use-morph', False)
-    # backup for analyses where orig values are needed for indistinguishables
-    # currently only a1
-    enc['species_orig'] = enc['species']
-    if use_morph:
-        enc['species'] = enc['morph']
 
-    indist_mask = enc.species.str.endswith(' sp.', na=True)
-    discard_ind = cfg.get_bool('discard-indistinguishable', False)
-    if discard_ind:
+    if cfg.use_morph:
+        # backup for analyses where orig values are needed for indistinguishables
+        # currently only a1
+        enc['species_orig'] = enc['species']
+        enc['species'] = enc['morph']
+    if cfg.discard_indistinguishable:
+        indist_mask = enc.species.str.endswith(' sp.', na=True)
         enc = enc[~indist_mask]
-    assert pd.api.types.is_integer_dtype(enc.coord_x)
-    assert pd.api.types.is_integer_dtype(enc.coord_y)
     enc = enc.reset_index(drop=True)
     return enc
 
 
-def adjust_grid(
-    enc: Encounters, qlist: QList, sides: Sides, discard_transect: bool, discard_zone: bool
-) -> tuple[Encounters, QList, Sides]:
-    """Transform coordinates and quadrat_ids in DataFrames to reflect discarding transect
-    and/or zone information if requested.
+def discard_axes(gri: GridInfo, sides: Sides, *, discard_transect: bool, discard_zone: bool) -> tuple[GridInfo, Sides]:
+    """Transform coordinates in DataFrames to reflect discarding transect and/or zone information if requested.
 
     >>> enc = pd.DataFrame(
     ...     {
     ...         'coord_x': [0, 1, 1, 1, 1],
     ...         'coord_y': [0, 0, 1, 0, 1],
     ...         'species': ['B', 'A', 'A', 'C', 'B'],
-    ...         'quadrat_id': ['T_1_1', 'T_2_1', 'T_2_2', 'T_2_1', 'T_2_2'],
     ...     }
     ... )
     >>> idx = pd.MultiIndex.from_arrays([[0, 0, 1, 1, 2], [0, 1, 0, 1, 0]], names=('coord_x', 'coord_y'))
     >>> quadrats = pd.DataFrame(
     ...     index=idx,
     ...     data={
     ...         'centroid_x': [0.5, 0.5, 1.5, 1.5, 2.5],
     ...         'centroid_y': [0.5, 1.5, 0.5, 1.5, 0.5],
-    ...         'quadrat_id': ['T_1_1', 'T_1_2', 'T_2_1', 'T_2_2', 'T_3_1'],
     ...     },
     ... )
+    >>> gri = GridInfo(enc, quadrats)
     >>> sides = Sides(1, 1)
-    >>> res = adjust_grid(enc.copy(), quadrats.copy(), sides, discard_transect=True, discard_zone=False)
-    >>> res[0]
-       coord_x  coord_y species quadrat_id
-    0        0        0       B      T_1_1
-    1        0        0       A      T_1_1
-    2        0        1       A      T_1_2
-    3        0        0       C      T_1_1
-    4        0        1       B      T_1_2
-    >>> res[1]  # doctest: +NORMALIZE_WHITESPACE
-                     centroid_x  centroid_y quadrat_id
+    >>> res = discard_axes(gri, sides, discard_transect=True, discard_zone=False)
+    >>> res[0].enc
+       coord_x  coord_y species
+    0        0        0       B
+    1        0        0       A
+    2        0        1       A
+    3        0        0       C
+    4        0        1       B
+    >>> res[0].qlist  # doctest: +NORMALIZE_WHITESPACE
+                     centroid_x  centroid_y
     coord_x coord_y
-    0       0               0.5         0.5      T_1_1
-            1               0.5         1.5      T_1_2
-    >>> res[2]
-    Sides(x=3, y=1)
+    0       0               0.5         0.5
+            1               0.5         1.5
+    >>> res[1]
+    Sides(x=3.0, y=1.0)
 
-    >>> res = adjust_grid(enc.copy(), quadrats.copy(), sides, discard_transect=False, discard_zone=True)
-    >>> res[0]
-       coord_x  coord_y species quadrat_id
-    0        0        0       B      T_1_1
-    1        1        0       A      T_2_1
-    2        1        0       A      T_2_1
-    3        1        0       C      T_2_1
-    4        1        0       B      T_2_1
-    >>> res[1]  # doctest: +NORMALIZE_WHITESPACE
-                     centroid_x  centroid_y quadrat_id
+    >>> res = discard_axes(gri, sides, discard_transect=False, discard_zone=True)
+    >>> res[0].enc
+       coord_x  coord_y species
+    0        0        0       B
+    1        1        0       A
+    2        1        0       A
+    3        1        0       C
+    4        1        0       B
+    >>> res[0].qlist  # doctest: +NORMALIZE_WHITESPACE
+                     centroid_x  centroid_y
     coord_x coord_y
-    0       0               0.5         0.5      T_1_1
-    1       0               1.5         0.5      T_2_1
-    2       0               2.5         0.5      T_3_1
-    >>> res[2]
-    Sides(x=1, y=2)
+    0       0               0.5         0.5
+    1       0               1.5         0.5
+    2       0               2.5         0.5
+    >>> res[1]
+    Sides(x=1.0, y=2.0)
 
 
-    >>> res = adjust_grid(enc.copy(), quadrats.copy(), sides, discard_transect=True, discard_zone=True)
-    >>> res[0]
-       coord_x  coord_y species quadrat_id
-    0        0        0       B      T_1_1
-    1        0        0       A      T_1_1
-    2        0        0       A      T_1_1
-    3        0        0       C      T_1_1
-    4        0        0       B      T_1_1
-    >>> res[1]  # doctest: +NORMALIZE_WHITESPACE
-                     centroid_x  centroid_y quadrat_id
+    >>> res = discard_axes(gri, sides, discard_transect=True, discard_zone=True)
+    >>> res[0].enc
+       coord_x  coord_y species
+    0        0        0       B
+    1        0        0       A
+    2        0        0       A
+    3        0        0       C
+    4        0        0       B
+    >>> res[0].qlist  # doctest: +NORMALIZE_WHITESPACE
+                     centroid_x  centroid_y
     coord_x coord_y
-    0       0               0.5         0.5      T_1_1
-    >>> res[2]
-    Sides(x=3, y=2)
+    0       0               0.5         0.5
+    >>> res[1]
+    Sides(x=3.0, y=2.0)
 
 
-    >>> res = adjust_grid(enc.copy(), quadrats.copy(), sides, discard_transect=False, discard_zone=False)
-    >>> res[0]
-       coord_x  coord_y species quadrat_id
-    0        0        0       B      T_1_1
-    1        1        0       A      T_2_1
-    2        1        1       A      T_2_2
-    3        1        0       C      T_2_1
-    4        1        1       B      T_2_2
-    >>> res[1]  # doctest: +NORMALIZE_WHITESPACE
-                     centroid_x  centroid_y quadrat_id
+    >>> res = discard_axes(gri, sides, discard_transect=False, discard_zone=False)
+    >>> res[0].enc
+       coord_x  coord_y species
+    0        0        0       B
+    1        1        0       A
+    2        1        1       A
+    3        1        0       C
+    4        1        1       B
+    >>> res[0].qlist  # doctest: +NORMALIZE_WHITESPACE
+                     centroid_x  centroid_y
     coord_x coord_y
-    0       0               0.5         0.5      T_1_1
-            1               0.5         1.5      T_1_2
-    1       0               1.5         0.5      T_2_1
-            1               1.5         1.5      T_2_2
-    2       0               2.5         0.5      T_3_1
-    >>> res[2]
-    Sides(x=1, y=1)
+    0       0               0.5         0.5
+            1               0.5         1.5
+    1       0               1.5         0.5
+            1               1.5         1.5
+    2       0               2.5         0.5
+    >>> res[1]
+    Sides(x=1.0, y=1.0)
     """
-
+    enc, qlist = gri
     new_x = sides.x
     new_y = sides.y
     if discard_transect:
         enc['coord_x'] = 0
-        # replace group of digits after first underscore
-        enc['quadrat_id'] = enc['quadrat_id'].str.replace(r'(^[^_])_(\d+)', r'\1_1', regex=True)
-        qlist['quadrat_id'] = qlist['quadrat_id'].str.replace(r'(^[^_])_(\d+)', r'\1_1', regex=True)
         x_coords = qlist.index.get_level_values('coord_x')
         new_x = sides.x * (x_coords.max() + 1)
         qlist['centroid_x'] = sides.x / 2
     if discard_zone:
         enc['coord_y'] = 0
-        # replace group of digits at the end
-        enc['quadrat_id'] = enc['quadrat_id'].str.replace(r'_\d+$', '_1', regex=True)
-        qlist['quadrat_id'] = qlist['quadrat_id'].str.replace(r'_\d+$', '_1', regex=True)
         y_coords = qlist.index.get_level_values('coord_y')
         new_y = sides.y * (y_coords.max() + 1)
         qlist['centroid_y'] = sides.y / 2
     qlist = qlist.drop_duplicates()  # automatically adjusts index
-    return enc, qlist, Sides(new_x, new_y)
+    return GridInfo(enc, qlist), Sides(new_x, new_y)
 
 
 def direction_difference(enc: Encounters) -> pd.DataFrame:
-    """Return dataframe with (coord_x, coord_y) as index and columns 'f_species' and 'b_species'
+    """Return dataframe with absolute and relative differences in encountered species between sampling directions.
+
+    Resulting DataFrame has (coord_x, coord_y) as index and columns 'f_species' and 'b_species'
     describing how many species were sampled in a given direction, including absolute and
     relative differences between the two.
 
     >>> df = pd.DataFrame(
     ...     {
     ...         'coord_x': ['0', '0', '0', '1', '1'],
     ...         'coord_y': ['0', '0', '0', '1', '1'],
@@ -1038,78 +1285,95 @@
     )
     stats = f_lens.join(b_lens, how='outer')
     stats['diff_%'] = (stats['f_species'] - stats['b_species']) / stats['f_species']
     stats['diff_#'] = stats['f_species'] - stats['b_species']
     return stats
 
 
-def load_quadrats(qlist: Path, quadrat_types: Sequence[str]) -> QList:
-    """Load CSV dataset listing all quadrats in a grid from *qlist* filtered by *quadrat_types*"""
-
-    q_type = pd.CategoricalDtype(['normal', 'shallows', 'riptide'])
-    qs = pd.read_csv(qlist, dtype={'quadrat_type': q_type}, index_col=['coord_x', 'coord_y']).convert_dtypes()
-    assert pd.api.types.is_integer_dtype(qs.index.get_level_values(0))
-    assert pd.api.types.is_integer_dtype(qs.index.get_level_values(1))
-    qs.set_flags(allows_duplicate_labels=False)
-    qs = qs[qs.quadrat_type.isin(quadrat_types)].drop(columns='quadrat_type', errors='raise')
+def load_quadrats(qlist: Path, quadrat_types: Sequence[QuadratType] | None) -> QList:
+    """Load CSV dataset listing all quadrats in a grid from `qlist` filtered by `quadrat_types`."""
+    qs = pd.read_csv(qlist, dtype=qlist_dtypes(), index_col=['coord_x', 'coord_y']).convert_dtypes()
+    if quadrat_types:
+        qs = qs[qs.quadrat_type.isin(quadrat_types)]
+    qs = qs.drop(columns='quadrat_type', errors='ignore')
     qs = qs.sort_index()
     return qs
 
 
-def load_encounters(dataset: Path) -> Encounters:
-    """Load CSV dataset with encounters from *dataset*"""
+def generate_quadrat_list(enc: Encounters) -> QList:
+    idx = pd.MultiIndex.from_frame(enc[['coord_x', 'coord_y']].drop_duplicates())
+    return pd.DataFrame(index=idx)
+
 
+def load_encounters(dataset: Path) -> Encounters:
+    """Load CSV dataset with encounters from `dataset`."""
     dtype_dict = enc_dtypes()
-    enc = pd.read_csv(dataset, dtype=dtype_dict, parse_dates=['date']).convert_dtypes()
+    enc = pd.read_csv(dataset, dtype=dtype_dict).convert_dtypes()
+    if 'date' in enc.columns:
+        enc['date'] = pd.to_datetime(enc.date, format='ISO8601')
     enc.set_flags(allows_duplicate_labels=False)
     return enc
 
 
-def get_spp_matrix(enc: Encounters, quadrats: QList) -> SppMatrix:
-    """Return DataFrame with coordinate MultiIndex labels and species as columns
-    with bool denoting whether species COL was encountered in quadrat LABEL.
+def get_spp_matrix(grinfo: GridInfo) -> SppMatrix:
+    """Return DataFrame with species matrix for passed *grinfo*.
+
+    The species matrix has MultiIndex coord_x, coord_y labels with quadrat coordinates
+    and species as column names with bool values denoting whether species COL was encountered in quadrat LABEL.
 
     >>> enc = pd.DataFrame(
     ...     {'coord_x': [0, 1, 1, 1, 1], 'coord_y': [0, 0, 1, 0, 1], 'species': ['B', 'A', 'A', 'C', 'B']}
     ... )
     >>> idx = pd.MultiIndex.from_arrays([[0, 0, 1, 1, 2], [0, 1, 0, 1, 0]], names=('coord_x', 'coord_y'))
     >>> quadrats = pd.DataFrame(index=idx)
-    >>> get_spp_matrix(enc, quadrats)  # doctest: +NORMALIZE_WHITESPACE
+    >>> get_spp_matrix(GridInfo(enc, quadrats))  # doctest: +NORMALIZE_WHITESPACE
     species              A      B      C
     coord_x coord_y
     0       0        False   True  False
             1        False  False  False
     1       0         True  False   True
             1         True   True  False
     2       0        False  False  False
     """
-
+    enc, quadrats = grinfo
     enccoords = [enc.coord_x, enc.coord_y]
     spp_matrix = pd.crosstab(enccoords, columns=enc.species, dropna=False)
     spp_matrix = spp_matrix.reindex(quadrats.index).fillna(0).astype(bool)
     spp_matrix = spp_matrix.sort_index()
     return spp_matrix
 
 
-def p025(x: pd.Series) -> float:
-    """Return 0.25 quantile (25th percentile) of pandas Series"""
+def p025(x: 'pd.Series[float]') -> float:
+    """Return 0.25 quantile (25th percentile) of pandas Series."""
     return x.quantile(0.025)
 
 
-def p975(x: pd.Series) -> float:
-    """Return 0.975 quantile (97.5th percentile) of pandas Series"""
+def p975(x: 'pd.Series[float]') -> float:
+    """Return 0.975 quantile (97.5th percentile) of pandas Series."""
     return x.quantile(0.975)
 
 
-AGG_STATS: list[str | Callable] = ['mean', 'median', 'sem', 'std', 'count', 'min', 'max', 'skew', p025, p975]
-"""List with aggregation to be called at once for convenience"""
+AGG_STATS: list[str | Callable[['pd.Series[float]'], float]] = [
+    'mean',
+    'median',
+    'sem',
+    'std',
+    'count',
+    'min',
+    'max',
+    'skew',
+    p025,
+    p975,
+]
+"""List with aggregation to be called at once for convenience."""
 
 
-def acc_richness_shuffled(spp_matrix: pd.DataFrame) -> pd.Series:
+def acc_richness_shuffled(spp_matrix: pd.DataFrame) -> 'pd.Series[int]':
     """Return Series containing accumulated richness.
+
     Quadrats are accumulated in random order.
 
     >>> np.random.seed(0)
     >>> spp_matrix = pd.DataFrame(
     ...     {
     ...         'A': [True, False, True, False],
     ...         'B': [True, False, False, False],
@@ -1121,35 +1385,33 @@
     >>> acc_richness_shuffled(spp_matrix)
     0    2
     1    2
     2    3
     3    4
     dtype: int64
     """
-
     return (
         spp_matrix.sample(frac=1, ignore_index=True)  # reshuffle dataset
         .cumsum()
         .astype(bool)
         .sum(axis='columns')  # sum total species
     )
 
 
 def agg_results(df: pd.DataFrame, col_prefix: str, index_name: str) -> pd.DataFrame:
-    """Aggregate data from DataFrame in a wide format
+    """Aggregate data from DataFrame in a wide format.
 
     >>> pd.set_option('display.width', None)
     >>> df = pd.DataFrame({'col1': [1, 0], 'col2': [2, 1], 'col3': [2, 2], 'col4': [1, 3]})
     >>> agg_results(df, 'col', 'idx')  # doctest: +NORMALIZE_WHITESPACE
          col_mean  col_med   col_sem   col_std  col_count  col_p025  col_p975  col_min  col_max  col_skew  col_kurtosis
     idx
     0         1.5      1.5  0.288675  0.577350          4     1.000     2.000        1        2       0.0          -6.0
     1         1.5      1.5  0.645497  1.290994          4     0.075     2.925        0        3       0.0          -1.2
     """
-
     res = pd.DataFrame(index=df.index)
     res.index.name = index_name
     res[f'{col_prefix}_mean'] = df.mean(axis='columns')
     res[f'{col_prefix}_med'] = df.median(axis='columns')
     res[f'{col_prefix}_sem'] = df.sem(axis='columns')
     res[f'{col_prefix}_std'] = df.std(axis='columns')
     res[f'{col_prefix}_count'] = df.count(axis='columns')
@@ -1214,16 +1476,15 @@
     0 0         1         0
       1         0         0
     1 0         2         0
     0 0         1         0
       1         2         2
     1 0         0         0
     """
-
-    spp_diff: dict[str, list[pd.Series]] = {'distance': [], 'abs_diff': []}
+    spp_diff: dict[str, list['pd.Series[float]']] = {'distance': [], 'abs_diff': []}
     for idx, row in species.iterrows():
         abs_diffs = (species & ~row).sum(axis='columns')
         spp_diff['abs_diff'].append(abs_diffs)
         dists = dmat.loc[idx, 'distance']  # type: ignore[index]   # can be indexed by MultiIndex tuple just fine
         spp_diff['distance'].append(dists)  # type: ignore[arg-type]   # is Series, not DF, verified by assert
     res = pd.DataFrame(
         {
@@ -1235,15 +1496,14 @@
 
 
 def distance_matrix(quadrats: pd.DataFrame, distance: DistFunction) -> pd.DataFrame:
     """Convert quadrat's grid coordinates to quadrat's centroid coordinates on a meters-based plane.
 
     >>> df = pd.DataFrame(
     ...     {
-    ...         'quadrat_id': ['1_1', '1_2', '2_1', '2_2'],
     ...         'coord_x': [0, 0, 1, 1],
     ...         'coord_y': [0, 1, 0, 1],
     ...         'centroid_x': [0.5, 0.5, 1.5, 1.5],
     ...         'centroid_y': [0.5, 1.5, 0.5, 1.5],
     ...     }
     ... )
     >>> distance_matrix(
@@ -1264,51 +1524,46 @@
                     1             0              0.000000
                                   1              2.236068
             1       0             0              2.828427
                                   1              2.236068
                     1             0              2.236068
                                   1              0.000000
     """
-
-    quadrats = quadrats.reset_index(drop=True)
+    quadrats = quadrats.reset_index(drop=False)
     dmat = quadrats.join(quadrats, how='cross', rsuffix='_other')  # type: ignore[arg-type]     # pandas bug as of 2.0.3
-    dmat = dmat.set_index(['quadrat_id', 'quadrat_id_other'], verify_integrity=True)
     ps = dmat[['centroid_x', 'centroid_y']]
     qs = dmat[['centroid_x_other', 'centroid_y_other']]
-    qs = qs.rename(
-        columns={'centroid_x_other': 'centroid_x', 'centroid_y_other': 'centroid_y'}, errors='raise'
-    )  # 'coord_x_other': 'x_g', 'coord_y_other': 'y_g',
+    qs = qs.rename(columns={'centroid_x_other': 'centroid_x', 'centroid_y_other': 'centroid_y'}, errors='raise')
     dmat = dmat[['coord_x', 'coord_y', 'coord_x_other', 'coord_y_other']]
     dmat['distance'] = distance(ps, qs)
     dmat = dmat.set_index(['coord_x', 'coord_y', 'coord_x_other', 'coord_y_other'])
     dmat = dmat.sort_index()
     return dmat
 
 
-def q_distance_centroid(
-    c_coords1: pd.DataFrame, c_coords2: pd.DataFrame, sides: Sides, caps: dict[str, float]
-) -> pd.Series:
-    """Return series of euclidean distance between centroids of quadrats at *c_coords1* and *c_coords2*.
-    Distance is capped by *centroid* value from *caps*.
+def q_distance_centroid(q1: pd.DataFrame, q2: pd.DataFrame, caps: Caps) -> 'pd.Series[float]':
+    """Return series of euclidean distance between centroids of quadrats at `q1` and `q2`.
+
+    Distance is capped by `centroid` value from `caps`.
 
     Grid coords should be paired-up, e.g. using cross-join, beforehand.
 
-    >>> c_coords1 = pd.DataFrame(
+    >>> q1 = pd.DataFrame(
     ...     {
     ...         'centroid_x': [0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 1.5, 1.5, 1.5, 1.5, 1.5, 1.5, 1.5, 1.5],
     ...         'centroid_y': [0.5, 0.5, 0.5, 0.5, 1.5, 1.5, 1.5, 1.5, 0.5, 0.5, 0.5, 0.5, 1.5, 1.5, 1.5, 1.5],
     ...     }
     ... )
-    >>> c_coords2 = pd.DataFrame(
+    >>> q2 = pd.DataFrame(
     ...     {
     ...         'centroid_x': [0.5, 0.5, 1.5, 1.5, 0.5, 0.5, 1.5, 1.5, 0.5, 0.5, 1.5, 1.5, 0.5, 0.5, 1.5, 1.5],
     ...         'centroid_y': [0.5, 1.5, 0.5, 1.5, 0.5, 1.5, 0.5, 1.5, 0.5, 1.5, 0.5, 1.5, 0.5, 1.5, 0.5, 1.5],
     ...     }
     ... )
-    >>> q_distance_centroid(c_coords1, c_coords2, Sides(1, 1), {'centroid': 10})
+    >>> q_distance_centroid(q1, q2, {'centroid': 10})
     0     0.000000
     1     1.000000
     2     1.000000
     3     1.414214
     4     1.000000
     5     0.000000
     6     1.414214
@@ -1319,46 +1574,42 @@
     11    1.000000
     12    1.414214
     13    1.000000
     14    1.000000
     15    0.000000
     dtype: float64
     """
+    dists = pd.Series(np.sqrt((q1.centroid_x - q2.centroid_x) ** 2 + (q1.centroid_y - q2.centroid_y) ** 2))
+    dists = dists.where(dists <= caps['centroid'], caps['centroid'])
+    return cast('pd.Series[float]', dists)
 
-    dists = pd.Series(
-        np.sqrt((c_coords1.centroid_x - c_coords2.centroid_x) ** 2 + (c_coords1.centroid_y - c_coords2.centroid_y) ** 2)
-    )
-    return dists.where(dists <= caps['centroid'], caps['centroid'])
 
+def q_distance_collapsed(q1: pd.DataFrame, q2: pd.DataFrame, sides: Sides, caps: Caps) -> 'pd.Series[float]':
+    """Return series of farthest single direction side-to-side distances between dataframes of points at `q1` and `q2`.
 
-def q_distance_collapsed(
-    c_coords1: pd.DataFrame, c_coords2: pd.DataFrame, sides: Sides, caps: dict[str, float]
-) -> pd.Series:
-    """Return series of farthest single direction side-to-side distances between dataframes
-    of points at *c_coords1* and *c_coords2*.
     Extent as per P&W paper, longest distance on 1 axis, taking larger of x or y differences.
-    Distance is capped by *max1dx* value from *caps* in case x distance is taken and *max1dy* in case of y.
+    Distance is capped by `max1dx` value from `caps` in case x distance is taken and `max1dy` in case of y.
 
     Correction is applied to result to make distance of quadrat to itself 0.
 
     Grid coords should be paired-up, e.g. using cross-join, beforehand.
 
-    >>> c_coords1 = pd.DataFrame(
+    >>> q1 = pd.DataFrame(
     ...     {
     ...         'centroid_x': [0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 1.5, 1.5, 1.5, 1.5, 1.5, 1.5, 1.5, 1.5],
     ...         'centroid_y': [0.5, 0.5, 0.5, 0.5, 1.5, 1.5, 1.5, 1.5, 0.5, 0.5, 0.5, 0.5, 1.5, 1.5, 1.5, 1.5],
     ...     }
     ... )
-    >>> c_coords2 = pd.DataFrame(
+    >>> q2 = pd.DataFrame(
     ...     {
     ...         'centroid_x': [0.5, 0.5, 1.5, 1.5, 0.5, 0.5, 1.5, 1.5, 0.5, 0.5, 1.5, 1.5, 0.5, 0.5, 1.5, 1.5],
     ...         'centroid_y': [0.5, 1.5, 0.5, 1.5, 0.5, 1.5, 0.5, 1.5, 0.5, 1.5, 0.5, 1.5, 0.5, 1.5, 0.5, 1.5],
     ...     }
     ... )
-    >>> q_distance_collapsed(c_coords1, c_coords2, Sides(1, 1), {'max1dx': 10, 'max1dy': 10})
+    >>> q_distance_collapsed(q1, q2, Sides(1, 1), {'max1dx': 10, 'max1dy': 10})
     0     0.0
     1     2.0
     2     2.0
     3     2.0
     4     2.0
     5     0.0
     6     2.0
@@ -1369,46 +1620,45 @@
     11    2.0
     12    2.0
     13    2.0
     14    2.0
     15    0.0
     Name: centroid_x, dtype: float64
     """
-    x_diff = (c_coords1.centroid_x - c_coords2.centroid_x).abs()
-    y_diff = (c_coords1.centroid_y - c_coords2.centroid_y).abs()
+    x_diff = (q1.centroid_x - q2.centroid_x).abs()
+    y_diff = (q1.centroid_y - q2.centroid_y).abs()
     x_diff[x_diff > 0] += sides.x
     y_diff[y_diff > 0] += sides.y
     x_diff = x_diff.where(x_diff <= caps['max1dx'], caps['max1dx'])
     y_diff = y_diff.where(y_diff <= caps['max1dy'], caps['max1dy'])
     dist = x_diff.where(x_diff > y_diff, y_diff)
-    return dist
+    return cast('pd.Series[float]', dist)
+
 
+def q_distance_diagonal(q1: pd.DataFrame, q2: pd.DataFrame, sides: Sides, caps: Caps) -> 'pd.Series[float]':
+    """Return series of farthest corner-to-corner distances between quadrats in list `q1` and `q2`, row-wise.
 
-def q_distance_diagonal(
-    c_coords1: pd.DataFrame, c_coords2: pd.DataFrame, sides: Sides, caps: dict[str, float]
-) -> pd.Series:
-    """Return series of diagonal, farthest corner-to-corner, distances between dataframes of
-    points at *c_coords1* and *c_coords2*. Distance is capped by *diagonal* value
-    from *caps* to prevent overspilling from grid in case of merged quadrats.
+    Distance is capped by `diagonal` value from `caps` to prevent
+    overspilling from grid in case of merged quadrats.
 
-    Centroid coordinates should be paired-up beforehand, e.g. using cross join.
+    Quadrats should be paired-up beforehand, e.g. using cross join.
 
-    >>> c_coords1 = pd.DataFrame(
+    >>> q1 = pd.DataFrame(
     ...     {
     ...         'centroid_x': [0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 0.5, 1.5, 1.5, 1.5, 1.5, 1.5, 1.5, 1.5, 1.5],
     ...         'centroid_y': [0.5, 0.5, 0.5, 0.5, 1.5, 1.5, 1.5, 1.5, 0.5, 0.5, 0.5, 0.5, 1.5, 1.5, 1.5, 1.5],
     ...     }
     ... )
-    >>> c_coords2 = pd.DataFrame(
+    >>> q2 = pd.DataFrame(
     ...     {
     ...         'centroid_x': [0.5, 0.5, 1.5, 1.5, 0.5, 0.5, 1.5, 1.5, 0.5, 0.5, 1.5, 1.5, 0.5, 0.5, 1.5, 1.5],
     ...         'centroid_y': [0.5, 1.5, 0.5, 1.5, 0.5, 1.5, 0.5, 1.5, 0.5, 1.5, 0.5, 1.5, 0.5, 1.5, 0.5, 1.5],
     ...     }
     ... )
-    >>> q_distance_diagonal(c_coords1, c_coords2, Sides(1, 1), {'diagonal': 10})
+    >>> q_distance_diagonal(q1, q2, Sides(1, 1), {'diagonal': 10})
     0     0.000000
     1     2.236068
     2     2.236068
     3     2.828427
     4     2.236068
     5     0.000000
     6     2.828427
@@ -1418,15 +1668,15 @@
     10    0.000000
     11    2.236068
     12    2.828427
     13    2.236068
     14    2.236068
     15    0.000000
     dtype: float64
-    >>> q_distance_diagonal(c_coords1, c_coords2, Sides(1, 1), {'diagonal': 2.5})
+    >>> q_distance_diagonal(q1, q2, Sides(1, 1), {'diagonal': 2.5})
     0     0.000000
     1     2.236068
     2     2.236068
     3     2.500000
     4     2.236068
     5     0.000000
     6     2.500000
@@ -1437,28 +1687,28 @@
     11    2.236068
     12    2.500000
     13    2.236068
     14    2.236068
     15    0.000000
     dtype: float64
     """
-
-    # "push" centroids into oposite corners
-    x_dist = (c_coords1.centroid_x - c_coords2.centroid_x).abs() + sides.x
-    y_dist = (c_coords1.centroid_y - c_coords2.centroid_y).abs() + sides.y
-    dists_pre_sqrt = pd.Series(x_dist**2 + y_dist**2)
+    # "push" centroids into opposite corners
+    x_dist = (q1.centroid_x - q2.centroid_x).abs() + sides.x
+    y_dist = (q1.centroid_y - q2.centroid_y).abs() + sides.y
+    dists_pre_sqrt = cast('pd.Series[float]', pd.Series(x_dist**2 + y_dist**2))
     quadrat_diagonal_2 = sides.x**2 + sides.y**2
     dists_pre_sqrt[dists_pre_sqrt == quadrat_diagonal_2] = 0
-    dists = np.sqrt(dists_pre_sqrt)
-    return dists.where(dists <= caps['diagonal'], caps['diagonal'])
+    dists = cast('pd.Series[float]', np.sqrt(dists_pre_sqrt))
+    dists = dists.where(dists <= caps['diagonal'], caps['diagonal'])
+    return dists
 
 
 def cutting_bounds(quadrats: pd.DataFrame, level: int) -> dict[Edge, int]:
-    """Returns minimum and maximum coordinates to be retained when tiling subgrid with level x level tiles.
-    In other words
+    """Return minimum and maximum coordinates to be retained when tiling subgrid with level x level tiles.
+
     >>> idx = pd.MultiIndex.from_tuples(
     ...     [(0, 0), (0, 1), (0, 2), (1, 0), (1, 1), (1, 2), (2, 0), (2, 1), (2, 2), (3, 0), (3, 1), (3, 2)],
     ...     names=['coord_x', 'coord_y'],
     ... )
     >>> qs = pd.DataFrame(index=idx)
     >>> cutting_bounds(qs, 1)
     {'left': 0, 'bottom': 0, 'right': 3, 'top': 2}
@@ -1466,30 +1716,29 @@
     {'left': 0, 'bottom': 1, 'right': 3, 'top': 1}
     >>> cutting_bounds(qs, 3)
     {'left': 1, 'bottom': 0, 'right': 2, 'top': 2}
     >>> cutting_bounds(qs, 4)  # doctest: +IGNORE_EXCEPTION_DETAIL
     Traceback (most recent call last):
     TilingError: Requested level 4 incompatible with locality dimensions: 3 x 2
     """
-
     xmax = quadrats.index.get_level_values('coord_x').max()
     ymax = quadrats.index.get_level_values('coord_y').max()
     if (level > xmax + 1) or (level > ymax + 1):
         raise TilingError(level, Sides(xmax, ymax))
     xmin_cutoff = (xmax + 1) % level
     ymin_cutoff = (ymax + 1) % level
     xmax_cutoff = xmax - xmin_cutoff
     ymax_cutoff = ymax - ymin_cutoff
     return {'left': xmin_cutoff, 'bottom': ymin_cutoff, 'right': xmax_cutoff, 'top': ymax_cutoff}
 
 
 def get_shift_tuples(qlist_subgrid: list[QList]) -> list[tuple[int, int]]:
-    """Get a list containing tuples indicating by how many coordinates will
-    grids need to be shifted to start at (0, 0). In other words, tuples with
-    minimal coordinates on each axis.
+    """Get a list containing offsets for adjusting grid coordinates so that they start at (0, 0).
+
+    In other words, tuples with minimal coordinates on each axis.
 
     >>> df0 = pd.DataFrame(index=pd.MultiIndex.from_arrays([[0, 0, 1, 1], [0, 1, 0, 1]], names=('coord_x', 'coord_y')))
     >>> df1 = pd.DataFrame(index=pd.MultiIndex.from_arrays([[1, 1, 2, 2], [2, 3, 2, 3]], names=('coord_x', 'coord_y')))
     >>> get_shift_tuples([df0, df1])
     [(0, 0), (1, 2)]
     """
     shifts = []
@@ -1497,158 +1746,98 @@
         shift_x = subgrid.index.get_level_values('coord_x').min()
         shift_y = subgrid.index.get_level_values('coord_y').min()
         shifts.append((shift_x, shift_y))
     return shifts
 
 
 def shift_coords(df_subgrids: list[pd.DataFrame], shifts: list[tuple[int, int]], level: int) -> list[pd.DataFrame]:
-    """Shift (x, y) coordinates in cropped grids from *df_subgrids* to create proper subgrids of corresponding *level*.
-    The subgrids will start at (0, 0). Adjacent quadrats will be merged to create larger *level*x*level* quadrats.
+    """Shift (x, y) coordinates in cropped grids from `df_subgrids` to create proper subgrids of corresponding `level`.
+
+    The subgrids will start at (0, 0). Adjacent quadrats will be merged to create larger `level`x`level` quadrats.
 
     If quadrat list is passed (has coords as indices), duplicates will be dropped.
 
-    >>> df0 = pd.DataFrame(
-    ...     {
-    ...         'quadrat_id': ['P_1_date_1', 'P_1_date_2', 'P_2_date_1', 'P_2_date_2'],
-    ...         'coord_x': [0, 0, 1, 1],
-    ...         'coord_y': [0, 1, 0, 1],
-    ...     }
-    ... )
+    >>> df0 = pd.DataFrame({'coord_x': [0, 0, 1, 1], 'coord_y': [0, 1, 0, 1]})
     >>> res = shift_coords([df0], [(0, 0)], 1)
     >>> len(res)
     1
     >>> res[0]
-      quadrat_id  coord_x  coord_y
-    0      P_1_1        0        0
-    1      P_1_2        0        1
-    2      P_2_1        1        0
-    3      P_2_2        1        1
-    >>> df1 = pd.DataFrame(
-    ...     data={
-    ...         'quadrat_id': ['P_1_date_2', 'P_1_date_3', 'P_2_date_2', 'P_2_date_3'],
-    ...         'coord_x': [0, 0, 1, 1],
-    ...         'coord_y': [1, 2, 1, 2],
-    ...     }
-    ... )
+       coord_x  coord_y
+    0        0        0
+    1        0        1
+    2        1        0
+    3        1        1
+    >>> df1 = pd.DataFrame(data={'coord_x': [0, 0, 1, 1], 'coord_y': [1, 2, 1, 2]})
     >>> res = shift_coords([df0, df1], [(0, 0), (0, 1)], 2)
     >>> len(res)
     2
     >>> res[0]
-      quadrat_id  coord_x  coord_y
-    0      P_1_1        0        0
-    1      P_1_1        0        0
-    2      P_1_1        0        0
-    3      P_1_1        0        0
+       coord_x  coord_y
+    0        0        0
+    1        0        0
+    2        0        0
+    3        0        0
     >>> res[1]
-      quadrat_id  coord_x  coord_y
-    0      P_1_1        0        0
-    1      P_1_1        0        0
-    2      P_1_1        0        0
-    3      P_1_1        0        0
+       coord_x  coord_y
+    0        0        0
+    1        0        0
+    2        0        0
+    3        0        0
     >>> coords_idx = pd.MultiIndex.from_arrays([[0, 0, 1, 1], [1, 2, 1, 2]], names=('coord_x', 'coord_y'))
     >>> df2 = df1.copy().set_index(coords_idx, verify_integrity=True)
     >>> res = shift_coords([df2], [(0, 1)], 2)
     >>> res[0]  # doctest: +NORMALIZE_WHITESPACE
-                    quadrat_id  coord_x  coord_y
+                    coord_x  coord_y
     coord_x coord_y
-    0       0            P_1_1        0        0
+    0       0             0        0
     """
-
     res = []
     for subgrid, shift in zip(df_subgrids, shifts, strict=True):
         new_xs = subgrid.coord_x.sub(shift[0]).floordiv(level)
         new_ys = subgrid.coord_y.sub(shift[1]).floordiv(level)
-        subgrid = replace_coords(subgrid, {'coord_x': new_xs, 'coord_y': new_ys})
-        if 'coord_x' in subgrid.index.names:  # is qlist
-            subgrid = subgrid.drop_duplicates(subset=['coord_x', 'coord_y'])
+        shifted = subgrid.assign(coord_x=new_xs, coord_y=new_ys)
+        if 'coord_x' in shifted.index.names:  # is qlist
+            shifted = shifted.drop_duplicates(subset=['coord_x', 'coord_y'])
             # fix up out-of-sync coords after drop
-            subgrid = subgrid.set_index(['coord_x', 'coord_y'], drop=False, verify_integrity=True)
-        res.append(subgrid)
+            shifted = shifted.set_index(['coord_x', 'coord_y'], drop=False, verify_integrity=True)
+        res.append(shifted)
     return res
 
 
 def create_subgrids(df: pd.DataFrame, cutoffs: Mapping[Edge, int]) -> list[pd.DataFrame]:
     """Create up to 4 subgrids by cutting off transects/zones beyond cutoff from either side.
 
     >>> idx = pd.MultiIndex.from_tuples(
     ...     [(0, 0), (0, 1), (0, 2), (1, 0), (1, 1), (1, 2), (2, 0), (2, 1), (2, 2), (3, 0), (3, 1), (3, 2)],
     ...     names=['coord_x', 'coord_y'],
     ... )
-    >>> df = pd.DataFrame(
-    ...     index=idx,
-    ...     data={
-    ...         'quadrat_id': [
-    ...             'P_1_25/2/2022_1',
-    ...             'P_1_25/2/2022_2',
-    ...             'P_1_25/2/2022_3',
-    ...             'P_2_25/2/2022_1',
-    ...             'P_2_25/2/2022_2',
-    ...             'P_2_26/2/2022_3',
-    ...             'P_3_26/2/2022_1',
-    ...             'P_3_26/2/2022_2',
-    ...             'P_3_26/2/2022_3',
-    ...             'P_4_26/2/2022_1',
-    ...             'P_4_26/2/2022_2',
-    ...             'P_4_26/2/2022_3',
-    ...         ]
-    ...     },
-    ... )
+    >>> df = pd.DataFrame(index=idx)
     >>> res = create_subgrids(df, {'left': 0, 'bottom': 0, 'right': 3, 'top': 2})
     >>> len(res)
     1
-    >>> res[0]  # doctest: +NORMALIZE_WHITESPACE
-                          quadrat_id
-    coord_x coord_y
-    0       0        P_1_25/2/2022_1
-            1        P_1_25/2/2022_2
-            2        P_1_25/2/2022_3
-    1       0        P_2_25/2/2022_1
-            1        P_2_25/2/2022_2
-            2        P_2_26/2/2022_3
-    2       0        P_3_26/2/2022_1
-            1        P_3_26/2/2022_2
-            2        P_3_26/2/2022_3
-    3       0        P_4_26/2/2022_1
-            1        P_4_26/2/2022_2
-            2        P_4_26/2/2022_3
+    >>> res[0]
+    Empty DataFrame
+    Columns: []
+    Index: [(0, 0), (0, 1), (0, 2), (1, 0), (1, 1), (1, 2), (2, 0), (2, 1), (2, 2), (3, 0), (3, 1), (3, 2)]
     """
-
-    if not set(['coord_x', 'coord_y']).issubset(df.columns):
+    if not {'coord_x', 'coord_y'}.issubset(df.columns):
         coord_x = df.index.get_level_values('coord_x')
         coord_y = df.index.get_level_values('coord_y')
     else:
-        coord_x = df['coord_x'] # type: ignore[assignment]  # behaves the same for our purposes
-        coord_y = df['coord_y'] # type: ignore[assignment]  # behaves the same for our purposes
-    left_part = (coord_x <= cutoffs['right'])
-    bottom_part = (coord_y <= cutoffs['top'])
-    right_part = (coord_x >= cutoffs['left'])
-    top_part = (coord_y >= cutoffs['bottom'])
+        coord_x = df['coord_x']  # type: ignore[assignment]  # behaves the same for our purposes
+        coord_y = df['coord_y']  # type: ignore[assignment]  # behaves the same for our purposes
+    left_part = coord_x <= cutoffs['right']
+    bottom_part = coord_y <= cutoffs['top']
+    right_part = coord_x >= cutoffs['left']
+    top_part = coord_y >= cutoffs['bottom']
 
     df0 = df[bottom_part & left_part]
     df1 = df[bottom_part & right_part]
     df2 = df[top_part & left_part]
     df3 = df[top_part & right_part]
 
     res: list[pd.DataFrame] = []
-    for d in [df0, df1, df2, df3]:
-        df_is_in = is_in(res, d)
-        if not df_is_in:
-            res.append(d)
+    for maybe_dup in [df0, df1, df2, df3]:
+        df_added = any(maybe_dup.equals(res_df) for res_df in res)
+        if not df_added:
+            res.append(maybe_dup)
     return res
-
-
-def is_in(dfs: list[pd.DataFrame], maybe_duplicate: pd.DataFrame) -> bool:
-    """Checks whether *maybe_duplicate* DataFrame is already in *dfs* list
-
-    >>> dfs = [pd.DataFrame({'vals': [0, 1, 2, 3]}), pd.DataFrame({'vals': [1, 2, 3]})]
-    >>> is_in(dfs, pd.DataFrame({'vals': [1, 2, 3, 4]}))
-    False
-    >>> is_in(dfs, pd.DataFrame({'vals': [1, 2, 3]}))
-    True
-    >>> is_in(dfs, pd.DataFrame({'values': [0, 1, 2, 3]}))
-    False
-    """
-
-    for df in dfs:
-        if maybe_duplicate.equals(df):
-            return True
-    return False
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `seal-tool-0.10.0/src/seal/misc.py` & `seal_tool-0.11.0/src/seal/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,191 +1,184 @@
 #!/usr/bin/env python3
 
 import argparse
+import sys
+
 import numpy as np
 import pandas as pd
 
+from seal.common import qlist_dtypes
+
+CZ_KFME_X_MIN = 38
+CZ_KFME_Y_MIN = 49
+
 
 def add_date_col(args: argparse.Namespace) -> str | None:
-    """Add ISO 8601-formatted date column to input based on its
-    quadrat_id column.
+    """Add ISO 8601-formatted date column to input based on its quadrat_id column.
+
     Intended for datasets with encounters.
 
     >>> from io import StringIO
     >>> df = pd.DataFrame({'quadrat_id': ['A_0_1/1/1970', 'A_0_2/1/1970']}).to_csv(index=False)
     >>> args = argparse.Namespace()
     >>> args.dataset, args.output = StringIO(df), None
     >>> pd.read_csv(StringIO(add_date_col(args)))
          quadrat_id        date
     0  A_0_1/1/1970  1970-01-01
     1  A_0_2/1/1970  1970-01-02
     """
-
     inp = args.dataset
     df = pd.read_csv(inp)
     dates = df['quadrat_id'].str.split('_').str[2]
     dates = pd.to_datetime(dates, format='%d/%m/%Y')
     df['date'] = dates
-    return df.to_csv(args.output, index=False)
+    return df.to_csv(args.output, index=False)  # type: ignore[no-any-return] # has str type, mypy 1.9.0 bug?
 
 
 def check_quadrat_list(args: argparse.Namespace) -> None:
-    """Check quadrat lists for possibly erroneous values"""
-
+    """Check quadrat lists for possibly erroneous values."""
     qlist = args.quadrat_list
-    cols = pd.read_csv(qlist, index_col=False, nrows=0).columns.tolist()
-    if not ('quadrat_id' in cols and 'quadrat_type' in cols):
-        print(f'Missing header in {qlist}')
+    cols = set(pd.read_csv(qlist, index_col=False, nrows=0).columns.to_list())
+    mandatory_cols = {'coord_x', 'coord_y'}
+    if not mandatory_cols.issubset(cols):
+        print(f'Invalid header in {qlist}, missing {mandatory_cols - cols}')
         return
-    df = pd.read_csv(qlist, index_col='quadrat_id')
+    df = pd.read_csv(qlist, dtype=qlist_dtypes())
     min_x, min_y = df['coord_x'].min(), df['coord_y'].min()
     if min_x != 0:
         print(f'Unusual minimal x coordinate: {min_x}')
     if min_y != 0:
         print(f'Unusual minimal y coordinate: {min_y}')
     max_x, max_y = df['coord_x'].max(), df['coord_y'].max()
     quadrats_total = (max_x + 1) * (max_y + 1)
     if len(df) != quadrats_total:
         print(f'Unusual number of quadrats, {len(df)} != {quadrats_total}, ({max_x + 1} * {max_y + 1})')
     df.set_flags(allows_duplicate_labels=False)
     if df.columns[0] == 'Unnamed: 0':
         print('Possibly redundant column')
         df = df.drop(columns='Unnamed: 0')
-    if df.isnull().values.any():
-        print('Missing value(s)')
-    dates = df.index.str.split('_').str[2]
-    startdate = pd.to_datetime(dates, format='%d/%m/%Y').min()
-    startdate = startdate.isoformat().replace('-', '')[0:8]
+    if df.isna().to_numpy().any():
+        print('Missing or invalid value(s)')
     if not args.output:
-        qlist = qlist.parent / f'{qlist.stem}-{startdate}.csv'
-        qlist = str(qlist).lower().replace(' ', '-').replace("'", '')  # type: ignore[assignment]
+        qlist = qlist.parent / f'{qlist.stem}-clean.csv'
+        qlist = str(qlist).lower().replace(' ', '-').replace("'", '')
     else:
         qlist = args.output
     qlist.parent.mkdir(parents=True, exist_ok=True)
-    df.to_csv(qlist)
+    df.to_csv(qlist, index=False)
 
 
 def add_coord_cols(args: argparse.Namespace) -> None | str:
-    """Add coord_x and coord_y to quadrat list based on its quadrat_ids
+    """Add coord_x and coord_y to quadrat list based on its quadrat_ids.
 
     >>> from io import StringIO
     >>> df = pd.DataFrame({'quadrat_id': ['A_1_date_2', 'A_10_date_11']}).to_csv(index=False)
     >>> args = argparse.Namespace()
     >>> args.input, args.output = StringIO(df), None
     >>> pd.read_csv(StringIO(add_coord_cols(args)))
          quadrat_id  coord_x  coord_y
     0    A_1_date_2        0        1
     1  A_10_date_11        9       10
     """
-
     qlist = pd.read_csv(args.input, index_col='quadrat_id')
     qlist.set_flags(allows_duplicate_labels=False)
     xs = pd.to_numeric(qlist.index.str.split('_').str[1]) - 1  # type: ignore[call-overload]
     ys = pd.to_numeric(qlist.index.str.split('_').str[-1]) - 1  # type: ignore[call-overload]
     qlist['coord_x'] = xs
     qlist['coord_y'] = ys
-    return qlist.to_csv(args.output)
+    return qlist.to_csv(args.output)  # type: ignore[no-any-return] # has str type, mypy 1.9.0 bug?
 
 
 def join_analyses(args: argparse.Namespace) -> None | str:
-    """Concatenate analysis results for joint plotting
+    """Concatenate analysis results for joint plotting.
 
     >>> from io import StringIO
     >>> df0 = pd.DataFrame({'result1': ['0', '1'], 'result2': ['2', '3']}).to_csv(index=False)
     >>> df1 = pd.DataFrame({'result1': ['4', '5'], 'result2': ['6', '7']}).to_csv(index=False)
     >>> inputs = [StringIO(df0), StringIO(df1)]
     >>> args = argparse.Namespace()
     >>> args.inputs, args.output, args.discriminants = inputs, None, None
     >>> pd.read_csv(StringIO(join_analyses(args)))
        result1  result2  discriminant
     0        0        2             0
     1        1        3             0
     2        4        6             1
     3        5        7             1
     """
-
     df_list = []
     args.discriminants = args.discriminants if args.discriminants else range(len(args.inputs))
-    for df_path, discr in zip(args.inputs, args.discriminants):
+    for df_path, discr in zip(args.inputs, args.discriminants, strict=True):
         df = pd.read_csv(df_path)
         df['discriminant'] = discr
         df_list.append(df)
     joined = pd.concat(df_list)
-    return joined.to_csv(args.output, index=False)
+    return joined.to_csv(args.output, index=False)  # type: ignore[no-any-return] # has str type, mypy 1.9.0 bug?
 
 
 def convert_biolib(args: argparse.Namespace) -> None:
-    """Convert dataset from https://www.biolib.cz/cz/speciesmapping/id1/ for
-    preprocess and analysis.
+    """Convert dataset from https://www.biolib.cz/cz/speciesmappings for preprocessing and analysis.
 
     Expected columns: CREATED, DAY, LATIN, MONTH, SUBSQ, SQUARE, QUANTITY, YEAR
     """
-
-    biolib_dtypes = {'SQUARE': str, 'SUBSQ': pd.CategoricalDtype(categories=['a', 'b', 'c', 'd'])}
+    biolib_dtypes: dict[str, str | pd._typing.Dtype] = {
+        'SQUARE': str,
+        'SUBSQ': pd.CategoricalDtype(categories=['a', 'b', 'c', 'd']),
+    }
     biolib = (
         pd.read_csv(args.input, dtype=biolib_dtypes, parse_dates=['CREATED'], date_format='%d/%m/%Y')
         .rename(columns=str.lower)
         .convert_dtypes()
     )
-    assert not biolib.subsq.isna().any()
+    if biolib.subsq.isna().any():
+        print('ERR: SUBSQ column has value(s) other than one of {a, b, c, d}', file=sys.stderr)
+        sys.exit(1)
     biolib = biolib.rename(columns={'latin': 'species', 'quantity': 'individuals'}, errors='raise')
 
     biolib['individuals'] = pd.to_numeric(biolib['individuals'], errors='coerce').fillna(1)
 
     # workaround because some sighting dates are invalid (day 0 or month 0)
     biolib['month'] = np.where(biolib.month == 0, biolib.created.dt.month, biolib.month)
     biolib['day'] = np.where(biolib.day == 0, biolib.created.dt.day, biolib.day)
     dateframe = biolib[['year', 'month', 'day']]
     biolib['date'] = pd.to_datetime(dateframe)
 
     coord_x = biolib['square'].str[2:]
     biolib['coord_x'] = coord_x.astype('int64')
-    min_x = biolib['coord_x'].min()
-    biolib['coord_x'] = biolib['coord_x'] - min_x
+    biolib['coord_x'] = biolib['coord_x'] - CZ_KFME_X_MIN
 
     coord_y = biolib['square'].str[:2]
     biolib['coord_y'] = coord_y.astype('int64')
-    min_y = biolib['coord_y'].min()
-    biolib['coord_y'] = biolib['coord_y'] - min_y
+    biolib['coord_y'] = biolib['coord_y'] - CZ_KFME_Y_MIN
 
-    # adjust for subsquares to enable nested quadrats strategy
+    # adjust for subsquares for more fine-grained grid
+    # subsquare layout:
+    #       Y low
+    # X low  a b  X high
+    # X low  c d  X high
+    #       Y high
     biolib['coord_x'] *= 2
-    is_right_x = (biolib.subsq == 'b') | (biolib.subsq == 'd')
-    biolib['coord_x'] = biolib['coord_x'].where(is_right_x, biolib.coord_x + 1)
+    is_lower_x = (biolib.subsq == 'a') | (biolib.subsq == 'c')
+    biolib['coord_x'] = biolib['coord_x'].where(is_lower_x, biolib.coord_x + 1)
 
     biolib['coord_y'] *= 2
-    is_top_y = (biolib.subsq == 'a') | (biolib.subsq == 'b')
-    biolib['coord_y'] = biolib['coord_y'].where(is_top_y, biolib.coord_y + 1)
+    is_lower_y = (biolib.subsq == 'a') | (biolib.subsq == 'b')
+    biolib['coord_y'] = biolib['coord_y'].where(is_lower_y, biolib.coord_y + 1)
 
     biolib = biolib.sort_values(by=['coord_x', 'coord_y'])
-    biolib['quadrat_id'] = 'A_' + biolib.coord_x.astype(str) + '_A_' + biolib.coord_y.astype(str)
-    biolib['family'] = 'DUMMY'
-    biolib['phase'] = 'term'
-    biolib['direction'] = 'f'
-    biolib['significant_size'] = True
-    biolib['locality'] = 'CZ'
-
-    qlist = biolib[['quadrat_id', 'coord_x', 'coord_y']].drop_duplicates()
-    qlist = qlist.sort_values(by=['coord_x', 'coord_y'])
-    qlist['quadrat_type'] = 'normal'
-
-    qlist.to_csv(args.output.with_stem(f'{args.output.stem}-qlist'), index=False)
     biolib.to_csv(args.output, index=False)
 
 
 def convert_aopk(args: argparse.Namespace) -> None:
-    """Convert dataset from https://portal.nature.cz/nd/ for
-    preprocess and analysis.
+    """Convert dataset from https://portal.nature.cz/nd/ for preprocessing and analysis.
 
-    Expected columns: DRUH, CESKE_JMENO, DATI_INSERT, SITMAP, POCET
+    Expected columns: DRUH, DATI_INSERT, SITMAP, POCET
 
     Input is expected to use CP1250 encoding. This is the default
     after downloading from the source.
     """
-
     aopk_dtypes = {'SITMAP': str}
     try:
         aopk = pd.read_csv(
             args.input,
             dtype=aopk_dtypes,
             parse_dates=['DATI_INSERT'],
             date_format='%Y%m%d',
@@ -202,32 +195,18 @@
         columns={
             'dati_insert': 'date',
             'druh': 'species',
             'pocet': 'individuals',
         },
         errors='raise',
     )
-
     aopk['individuals'] = pd.to_numeric(aopk['individuals'], errors='coerce').fillna(1)
 
     coord_x = aopk['sitmap'].str[2:]
     aopk['coord_x'] = coord_x.astype('int64')
-    min_x = aopk['coord_x'].min()
-    aopk['coord_x'] = aopk['coord_x'] - min_x
+    aopk['coord_x'] = aopk['coord_x'] - CZ_KFME_X_MIN
 
     coord_y = aopk['sitmap'].str[:2]
     aopk['coord_y'] = coord_y.astype('int64')
-    min_y = aopk['coord_y'].min()
-    aopk['coord_y'] = aopk['coord_y'] - min_y
-
-    aopk['quadrat_id'] = 'A_' + aopk.coord_x.astype(str) + '_A_' + aopk.coord_y.astype(str)
-    aopk['family'] = 'DUMMY'
-    aopk['phase'] = 'term'
-    aopk['direction'] = 'f'
-    aopk['significant_size'] = True
-    aopk['locality'] = 'CZ'
-
-    qlist = aopk[['quadrat_id', 'coord_x', 'coord_y']].drop_duplicates()
-    qlist['quadrat_type'] = 'normal'
+    aopk['coord_y'] = aopk['coord_y'] - CZ_KFME_Y_MIN
 
-    qlist.to_csv(args.output.with_stem(f'{args.output.stem}-qlist'), index=False, encoding='utf8')
     aopk.to_csv(args.output, index=False, encoding='utf8')
```

### Comparing `seal-tool-0.10.0/src/seal/plot.py` & `seal_tool-0.11.0/src/seal/plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import argparse
 import datetime
-import matplotlib
-import matplotlib.pyplot as plt
-import pandas as pd
 import random
-import seaborn as sns
-
-from alive_progress import alive_bar
-from alive_progress.animations.spinners import bouncing_spinner_factory
-from matplotlib.ticker import ScalarFormatter
+from collections.abc import Generator
 from pathlib import Path
-from typing import Final, Generator, Literal, Optional
-
-import seal.config as conf
-from seal.common import analysis_results_name, data_dir, Sides
+from typing import Final, Literal
 
+import matplotlib
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+import seaborn as sns  # type: ignore[import-untyped] # wontfix'ed https://github.com/mwaskom/seaborn/issues/2212, partial https://github.com/mwaskom/seaborn/issues/3287
+from alive_progress import alive_bar  # type: ignore[import-untyped]
+from matplotlib.ticker import FixedLocator, ScalarFormatter
+
+from seal.common import analysis_results_filename, geom_r2, get_spinner
+from seal.config import Analysis, Config, Sides
+from seal.exceptions import InvalidLiteralError
 
 type Metadata = dict[str, str | list[str] | None]
+type PlotData = tuple[list[matplotlib.figure.Figure], Metadata]
 
 SVG_METADATA: Final[Metadata] = {
     'Description': (
         'Work was funded by project Influence of sample grain'
         ' and extent on coral reef fish richness, MUNI / IGA / 1076 / 2021.'
     ),
     'Contributor': ['Martin Matouš', 'Barbora Winterová'],
@@ -37,396 +39,394 @@
     'Copyright': 'CC BY-SA 4.0',
     'Creation Time': None,
     'Software': 'seal (https://pypi.org/project/seal-tool/)',
 }
 
 
 def main(args: argparse.Namespace) -> int:
-    sns.set_theme(palette='colorblind')
-    cfg = conf.Config.from_file(args.taskfile)
-    locality = cfg.get_subconf('locality')
-
-    if args.joined:
-        atype = args.joined[0]
-        joined_input = Path(args.joined[1])
-        analysis = config_analysis(atype, cfg)
-        df = pd.read_csv(joined_input)
-        fig, meta = plot_analysis(df, locality, analysis)
-        out_path = joined_input.with_stem(joined_input.stem + f'-{atype}').with_suffix('.svg')
-        fig.savefig(out_path, metadata=meta)
-        print(f'Graph plotted at {out_path}')
-        return 0
-
-    analyses = cfg.get_list('analyses')
-    csv_results_dir = data_dir(cfg)
-
-    emoji = ['🐧', '🐡', '🐟', '🦑', '🦦', '🐠', '🦐', '🐙']
-    random.shuffle(emoji)
-    emoji = ''.join(emoji)
-    spinner = bouncing_spinner_factory(('🌊', emoji), 6, block=(1, 1), hide=True)
-
-    with alive_bar(len(analyses), title='Plotting', spinner=spinner) as bar:
-        for pos, analysis in enumerate(analyses):
-            if not (isinstance(analysis, str) or isinstance(analysis, conf.Config)):
-                raise conf.InvalidTaskError(f'invalid analysis {analysis} on position {pos}')
-            analysis = config_analysis(analysis, cfg)
-            a_type = analysis.get_string('type')
-            analysis_file = analysis_results_name(csv_results_dir, args, a_type)
-            df = pd.read_csv(analysis_file)
-            figs, meta = plot_analysis(df, locality, analysis)
-            if args.png:
-                suffix = '.png'
-                meta = conv_png_metadata(meta)
-            else:
-                suffix = '.svg'
-            out_path = analysis_file.with_suffix(suffix)
-            for i, fig in enumerate(figs):
-                out_path = out_path.with_stem(f'{analysis_file.stem}-{i}')
-                fig.savefig(out_path, metadata=meta)
-                print(f'Graph plotted at {out_path}')
-            bar.text(f'{a_type}')
+    sns.set_theme(palette='colorblind', rc={'backend': 'svg'})
+    cfg = Config.from_taskfile(args.taskfile)
+    csv_results_dir = cfg.out_dir  # it's outdir from the perspective of analysis, not plot
+    spinner = get_spinner()
+    analysis_idx = {analysis.type_: 0 for analysis in cfg.analyses}
+    with alive_bar(len(cfg.analyses), title='Plotting', spinner=spinner) as bar:
+        for analysis in cfg.analyses:
+            analysis_file = analysis_results_filename(
+                csv_results_dir, args.taskfile, analysis.type_, analysis_idx[analysis.type_]
+            )
+            plot_analysis(analysis_file, cfg, analysis)
+            analysis_idx[analysis.type_] += 1
+            bar.text(f'{analysis.type_}')
             bar()
-
     return 0
 
 
-def plot_analysis(df, locality, analysis):
-    match analysis.get_string('type'):
+def plot_analysis(analysis_file: Path, cfg: Config, analysis: Analysis) -> None:
+    df = pd.read_csv(analysis_file)
+    # seaborn ignores palette for numeric hues
+    # https://github.com/mwaskom/seaborn/issues/2606
+    df['level'] = df['level'].astype(str)
+    random.seed(cfg.seed)
+    np.random.seed(cfg.seed)
+    figs, meta = plot_figures(df, cfg, analysis)
+    if cfg.plot.output_format == 'png':
+        meta = conv_png_metadata(meta)
+    out_path = analysis_file.with_suffix(f'.{cfg.plot.output_format}')
+    for i, fig in enumerate(figs):
+        out_path = out_path.with_stem(f'{analysis_file.stem}-{i}')
+        fig.savefig(out_path, metadata=meta)
+        print(f'Graph plotted at {out_path}')
+    matplotlib.pyplot.close('all')
+
+
+def plot_figures(df: pd.DataFrame, cfg: Config, analysis: Analysis) -> PlotData:  # noqa: PLR0911
+    match analysis.type_:
         case 'a1' | 'overview':
-            return a1(df, locality, analysis)
+            return a1(df, cfg)
         case 'a2' | 'sar':
-            return a2(df, locality, analysis)
+            return a2(df, cfg)
         case 'a3' | 'spdiff':
-            return a3(df, locality, analysis)
+            return a3(df, cfg)
         case 'a4' | 'rrich':
-            return a4(df, locality, analysis)
+            return a4(df, cfg)
         case 'a5' | 'oerich':
-            return a5(df, locality, analysis)
+            return a5(df, cfg)
         case 'a6' | 'sratios':
-            return a6(df, locality, analysis)
+            return a6(df, cfg)
         case 'a7' | 'jaccard':
-            return a7(df, locality, analysis)
+            return a7(df, cfg)
+        case 'a8' | 'abundance':
+            return a8(df, cfg)
         case _:
-            raise conf.InvalidTaskError(analysis.get_string('type'))
-
-
-def config_analysis(analysis: conf.Config | str, taskfile: conf.Config) -> conf.Config:
-    analysis = conf.Config.from_string(f'type = {analysis}') if isinstance(analysis, str) else analysis
-    analysis.put('plot', taskfile.get_subconf('plot'))
-    analysis.put('seed', taskfile.get_int_unchecked('seed', None))
-    analysis.put('level-strategy', taskfile.get_string('level-strategy'))
-    return analysis
+            raise InvalidLiteralError(f'{analysis.type_=}')
 
 
 def level_aspect(sides: Sides, level: int, lvl_strat: str) -> float:
-    if (
-        lvl_strat == 'transect-merging'
-        or lvl_strat == 'repeated-transect-merging'
-        or lvl_strat == 'striped-transect-merging'
-    ):
+    if lvl_strat in {'transect-merging', 'repeated-transect-merging', 'striped-transect-merging'}:
         return sides.y / (sides.x * level)
-    elif lvl_strat == 'zone-merging':
+    if lvl_strat == 'zone-merging':
         return sides.y * level / sides.x
-    elif (
-        lvl_strat == 'overlaid-subgrids'
-        or lvl_strat == 'transect-additive'
-        or lvl_strat == 'zone-additive'
-        or lvl_strat == 'nested-quadrats'
-    ):
+    if lvl_strat in {'overlaid-subgrids', 'transect-additive', 'zone-additive', 'nested-quadrats'}:
         return sides.y / sides.x
-    raise conf.InvalidTaskError(lvl_strat)
+    raise InvalidLiteralError(f'{lvl_strat=}')
 
 
-def a1(df: pd.DataFrame, locality: conf.Config, analysis: conf.Config) -> tuple[list[matplotlib.figure.Figure], Metadata]:
-    locname = locality.get_string('name')
+def a1(df: pd.DataFrame, cfg: Config) -> PlotData:
+    locname = cfg.locality.name
     meta = fill_metadata(locname, 'a1')
-    s = locality.get_subconf('sides')
-    sides = Sides(s.get_float('x'), s.get_float('y'))
-    lvl_strat = analysis.get_string('level-strategy')
+    bplot_cfg = [{'y': 'n_species', 'ylabel': 'species'}]
+    df = df.astype(int)
 
     figs = []
-    for ldf, level in df_levels(df):
-        ldf = ldf.astype(int)
-
+    level_dfs = list(df_levels(df))
+    for ldf, level in level_dfs:
         fig, ax = plt.subplots(figsize=(12, 12))
         fig.suptitle(f'{locname} species')
 
-        val_matrix = ldf.pivot(index='coord_y', columns='coord_x', values='n_species')
-        val_matrix.sort_index(ascending=False, inplace=True)
+        val_matrix = ldf.pivot_table(index='coord_y', columns='coord_x', values='n_species')
+        val_matrix = val_matrix.sort_index(ascending=False)
 
-        aspect = level_aspect(sides, level, lvl_strat)
-        sns.heatmap(val_matrix, annot=True, fmt='g', cmap='magma_r', linewidths=0.3, ax=ax)
-        ax.grid(False)
+        aspect = level_aspect(cfg.locality.sides, level, cfg.level_strategy)
+        sns.heatmap(val_matrix, annot=True, fmt='g', cmap='magma_r', linewidths=0.3, cbar_kws={'shrink': 0.5}, ax=ax)
+        ax.grid(visible=False)
         ax.set(xlabel='Transect', ylabel='Zone', aspect=aspect, title=f'Level {level}')
-        fig.text(x=0.7, y=0.05, s=f'Level strategy: {lvl_strat}')
+        fig.text(x=0.7, y=0.05, s=f'Level strategy: {cfg.level_strategy}')
         figs.append(fig)
 
-        fig, ax = plt.subplots(figsize=(12, 12))
-        fig.suptitle(f'{locname} individuals')
-
-        val_matrix = ldf.pivot(index='coord_y', columns='coord_x', values='n_individuals')
-        val_matrix.sort_index(ascending=False, inplace=True)
+    if 'n_individuals' in df.columns:
+        bplot_cfg.append({'y': 'n_individuals', 'ylabel': 'individuals'})
 
-        aspect = level_aspect(sides, level, lvl_strat)
-        sns.heatmap(val_matrix, annot=True, fmt='g', cmap='magma_r', linewidths=0.3, ax=ax)
-        ax.grid(False)
-        ax.set(xlabel='Transect', ylabel='Zone', aspect=aspect, title=f'Level {level}')
-        fig.text(x=0.7, y=0.05, s=f'Level strategy: {lvl_strat}')
+        for ldf, level in level_dfs:
+            fig, ax = plt.subplots(figsize=(12, 12))
+            fig.suptitle(f'{locname} individuals')
+            val_matrix = ldf.pivot_table(index='coord_y', columns='coord_x', values='n_individuals')
+            val_matrix = val_matrix.sort_index(ascending=False)
+            sns.heatmap(
+                val_matrix, annot=True, fmt='g', cmap='magma_r', linewidths=0.3, cbar_kws={'shrink': 0.5}, ax=ax
+            )
+            ax.grid(visible=False)
+            aspect = level_aspect(cfg.locality.sides, level, cfg.level_strategy)
+            ax.set(xlabel='Transect', ylabel='Zone', aspect=aspect, title=f'Level {level}')
+            fig.text(x=0.7, y=0.05, s=f'Level strategy: {cfg.level_strategy}')
+            figs.append(fig)
+
+    for bar_cfg in bplot_cfg:
+        fig, ax = plt.subplots(figsize=(48, 12))
+        fig.suptitle(f'{bar_cfg['ylabel'].title()} in quadrats')
+        ldf_s = ldf.sort_values(bar_cfg['y'], ascending=False)
+        sns.barplot(
+            x=map(str, zip(ldf_s.coord_x, ldf_s.coord_y, strict=False)),
+            y=ldf_s[bar_cfg['y']],
+            gap=0.2,
+            errorbar=cfg.plot.error_type,
+        )
+        ax.bar_label(ax.containers[0], fontsize=10)
+        ax.set(xlabel='Quadrat', ylabel=f'# of {bar_cfg['ylabel']}', title=f'{locname}, level {level}')
         figs.append(fig)
 
     return figs, meta
 
 
-def a2(df: pd.DataFrame, locality: conf.Config, analysis: conf.Config) -> tuple[list[matplotlib.figure.Figure], Metadata]:
-    locname = locality.get_string('name')
+def a2(df: pd.DataFrame, cfg: Config) -> PlotData:
+    locname = cfg.locality.name
     meta = fill_metadata(locname, 'a2')
-    ycol = 'species'
-    seed = analysis.get_int_unchecked('seed')
-    plotconf = analysis.get('plot')
-    err_style = plotconf.get_string('error-style', 'band')  # type: ignore[union-attr]   # todo: switch to loading params once in main
+    err_style = cfg.plot.error_style
 
     init_df = df.copy()
     df = df.drop(['min_acc', 'max_acc'], axis='columns', errors='raise')
     df['id'] = range(len(df))
-    df = pd.wide_to_long(df, stubnames='', i=['id'], j='area').rename({'': ycol}, axis='columns', errors='raise')
+    df = pd.wide_to_long(df, stubnames='', i=['id'], j='subid').rename({'': 'species'}, axis='columns', errors='raise')
 
     fig1, ax1 = plt.subplots()
 
     sns.lineplot(
         x='area',
-        y=ycol,
+        y='species',
         hue='level',
-        seed=seed,
+        seed=cfg.seed,
         estimator='mean',
         err_style=err_style,
         ax=ax1,
         data=df,
-        palette='colorblind',
+        errorbar=cfg.plot.error_type,
     )
     ax1.set(xlabel='Surface area ($m^2$)', ylabel='# of species', title='Species-area relationship')
 
     fig2, ax2 = plt.subplots()
     sns.lineplot(
         x='area',
         y='min_acc',
         hue='level',
-        seed=seed,
+        seed=cfg.seed,
         estimator='mean',
         err_style=None,
         data=init_df,
         ax=ax2,
         legend=False,
-        palette='colorblind',
     )
     sns.lineplot(
-        x='area',
-        y='max_acc',
-        hue='level',
-        seed=seed,
-        estimator='mean',
-        err_style=None,
-        data=init_df,
-        ax=ax2,
-        palette='colorblind',
+        x='area', y='max_acc', hue='level', seed=cfg.seed, estimator='mean', err_style=None, data=init_df, ax=ax2
     )
     ax2.set(xlabel='Surface area ($m^2$)', ylabel='# of species', title='Species-area relationship extremes')
 
-    if plotconf.get_bool('logscale-x'):   # type: ignore[union-attr]   # todo: switch to loading params once in main
+    if cfg.plot.logscale_x:
         for ax in [ax1, ax2]:
             ax.set_xscale('log')
+            min_area = init_df.area.min()
+            max_area = init_df.area.max()
+            ticks = geom_r2(min_area, max_area)
+            ax.xaxis.set_major_locator(FixedLocator(ticks))
             ax.xaxis.set_major_formatter(ScalarFormatter())
 
     return [fig1, fig2], meta
 
 
-def a3(df: pd.DataFrame, locality: conf.Config, analysis: conf.Config) -> tuple[list[matplotlib.figure.Figure], Metadata]:
-    locname = locality.get_string('name')
+def a3(df: pd.DataFrame, cfg: Config) -> PlotData:
+    locname = cfg.locality.name
     meta = fill_metadata(locname, 'a3')
-    seed = analysis.get_int_unchecked('seed')
-
-    interval = analysis.get_float_unchecked('interval', None)
-    if interval:
-        bins = pd.interval_range(0, df.distance.max() + interval, freq=interval, closed='left')  # type: ignore[call-overload]
-        df['distance_bin'] = pd.cut(df.distance, bins)
-
-    plotconf = analysis.get('plot')
-    err_style = plotconf.get_string('error-style', 'band')  # type: ignore[union-attr]   # todo: switch to loading params once in main
     figs = []
     axs = []
 
     fig1, ax1 = plt.subplots()
     fig1.suptitle('Pair-wise species difference')
     sns.lineplot(
         x='distance',
         y='abs_diff',
         hue='level',
-        seed=seed,
+        seed=cfg.seed,
         estimator='mean',
-        err_style=err_style,
+        err_style=cfg.plot.error_style,
+        errorbar=cfg.plot.error_type,
         ax=ax1,
         data=df,
-        palette='colorblind',
     )
     figs.append(fig1)
     axs.append(ax1)
 
     if 'distance_bin' in df.columns:
         fig2, ax2 = plt.subplots(figsize=(20, 20))
         fig2.suptitle('Pair-wise species difference')
-        sns.boxplot(x='distance_bin', y='abs_diff', hue='level', ax=ax2, data=df, palette='colorblind')
+        sns.boxplot(x='distance_bin', y='abs_diff', hue='level', ax=ax2, data=df)
         plt.setp(ax2.collections, alpha=0.3)
-        sns.rugplot(y='abs_diff', hue='level', ax=ax2, data=df, palette='colorblind')
+        sns.rugplot(y='abs_diff', hue='level', ax=ax2, data=df)
         ax2.tick_params(axis='x', labelrotation=45)
         figs.append(fig2)
         axs.append(ax2)
 
     for ax in axs:
         ax.set(xlabel='Distance ($m$)', ylabel='Difference', title=locname)
 
     return figs, meta
 
 
-def a4(df: pd.DataFrame, locality: conf.Config, analysis: conf.Config) -> tuple[list[matplotlib.figure.Figure], Metadata]:
-    locname = locality.get_string('name')
+def a4(df: pd.DataFrame, cfg: Config) -> PlotData:
+    locname = cfg.locality.name
     meta = fill_metadata(locname, 'a4')
-    seed = analysis.get_int_unchecked('seed')
 
     # intervals are simply strings to seaborn, can't be sorted automatically
-    df['distance'] = df['distance'].apply(to_interval)
+    df['distance'] = df['distance'].apply(to_interval)  # type: ignore[arg-type] # valid AggFuncTypeBase (basically Callable[Any]), mypy 1.9.0 bug?
     df = df.sort_values('distance')
     df['distance'] = df.distance.apply(str)
 
     fig1, ax1 = plt.subplots(figsize=(20, 20))
     fig1.suptitle('Richness of quadrats within distance')
-    sns.boxplot(x='distance', y='radius_richness', hue='level', ax=ax1, data=df, palette='colorblind')
+    sns.boxplot(x='distance', y='radius_richness', hue='level', ax=ax1, data=df)
 
     fig2, ax2 = plt.subplots(figsize=(20, 20))
     fig2.suptitle('Richness of quadrats within distance')
-    plotconf = analysis.get('plot')
-    err_style = plotconf.get_string('error-style', 'band')  # type: ignore[union-attr]   # todo: switch to loading params once in main
     sns.lineplot(
         x='distance',
         y='radius_richness',
-        seed=seed,
+        seed=cfg.seed,
         estimator='median',
-        err_style=err_style,
+        err_style=cfg.plot.error_style,
+        errorbar=cfg.plot.error_type,
         hue='level',
         ax=ax2,
         data=df,
-        palette='colorblind',
     )
 
     for ax in [ax1, ax2]:
         ax.set(title=locname, xlabel=r'Radius ($m$)', ylabel='# of species')
         ax.tick_params(axis='x', labelrotation=45)
 
     return [fig1, fig2], meta
 
 
-def a5(
-    df: pd.DataFrame, locality: conf.Config, analysis: conf.Config
-) -> tuple[list[matplotlib.figure.Figure], Metadata]:
+def a5(df: pd.DataFrame, cfg: Config) -> PlotData:
     ratios = []
+    medians = []
     for ldf, lvl in df_levels(df):
         ratios.append(pd.DataFrame({'oe_ratio': ldf['oe_ratio_mean'], 'level': lvl}))
+        m = ldf['oe_ratio_mean'].median()
+        medians.append({'value': m, 'vertical_offset': m * 0.05})
     df = pd.concat(ratios, ignore_index=True)
 
-    locname = locality.get_string('name')
+    locname = cfg.locality.name
     meta = fill_metadata(locname, 'a5')
 
     fig1, ax1 = plt.subplots()
     fig1.suptitle('Observed/expected ratio per level')
     sns.violinplot(x='level', y='oe_ratio', ax=ax1, data=df)
     plt.setp(ax1.collections, alpha=0.3)
     sns.rugplot(y='oe_ratio', ax=ax1, data=df)
     ax1.set(title=locname, xlabel='Level', ylabel='Observed/Expected')
 
     fig2, ax2 = plt.subplots()
     fig1.suptitle('Observed/expected ratio per level')
     sns.boxplot(x='level', y='oe_ratio', ax=ax2, data=df)
-    sns.stripplot(x='level', y='oe_ratio', ax=ax2, data=df)
+    sns.stripplot(x='level', y='oe_ratio', linewidth=0.7, ax=ax2, data=df)
     ax2.set(title=locname, xlabel='Level', ylabel='Observed/Expected')
+    for xtick, median in zip(ax2.get_xticks(), medians, strict=True):
+        ax2.text(
+            xtick,
+            median['value'] + median['vertical_offset'],
+            f'{median['value']:.2f}',
+            horizontalalignment='center',
+            size='x-small',
+            color='w',
+            weight='semibold',
+        )
 
     return [fig1, fig2], meta
 
 
-def a6(
-    df: pd.DataFrame, locality: conf.Config, analysis: conf.Config
-) -> tuple[list[matplotlib.figure.Figure], Metadata]:
-    locname = locality.get_string('name')
+def a6(df: pd.DataFrame, cfg: Config) -> PlotData:
+    locname = cfg.locality.name
     meta = fill_metadata(locname, 'a6')
-    seed = analysis.get_int_unchecked('seed')
 
-    cfgs = [
+    line_cfgs = [
         {'ycol': 'common_total', 'title': f'{locname}, common / total species ratio', 'ylabel': 'common / total'},
         {
             'ycol': 'common_diff',
             'title': f'{locname}, common / differing species ratio',
             'ylabel': 'common / differing',
         },
         {'ycol': 'common_union', 'title': f'{locname}, common / present species ratio', 'ylabel': 'common / present'},
     ]
 
-    plotconf = analysis.get('plot')
-    err_style = plotconf.get_string('error-style', 'band')  # type: ignore[union-attr]   # todo: switch to loading params once in main
+    err_style = cfg.plot.error_style
     figs = []
-    for cfg in cfgs:
+    for line_cfg in line_cfgs:
         fig, ax = plt.subplots()
         sns.lineplot(
             x='distance',
-            y=cfg['ycol'],
-            seed=seed,
+            y=line_cfg['ycol'],
+            seed=cfg.seed,
             estimator='mean',
             err_style=err_style,
+            errorbar=cfg.plot.error_type,
             hue='level',
             data=df,
-            palette='colorblind',
             ax=ax,
         )
-        ax.set(title=cfg['title'], xlabel=r'Quadrat distance ($m$)', ylabel=cfg['ylabel'])
+        ax.set(title=line_cfg['title'], xlabel=r'Quadrat distance ($m$)', ylabel=line_cfg['ylabel'])
         figs.append(fig)
 
     return figs, meta
 
 
-def a7(
-    df: pd.DataFrame, locality: conf.Config, analysis: conf.Config
-) -> tuple[list[matplotlib.figure.Figure], Metadata]:
-    locname = locality.get_string('name')
+def a7(df: pd.DataFrame, cfg: Config) -> PlotData:
+    locname = cfg.locality.name
     meta = fill_metadata(locname, 'a7')
-    seed = analysis.get_int_unchecked('seed')
 
-    plotconf = analysis.get('plot')
-    err_style = plotconf.get_string('error-style', 'band')  # type: ignore[union-attr]   # todo: switch to loading params once in main
+    err_style = cfg.plot.error_style
     fig, ax = plt.subplots()
     sns.lineplot(
         x='distance',
         y='jaccard_dissimilarity',
-        seed=seed,
+        seed=cfg.seed,
         estimator='mean',
         err_style=err_style,
+        errorbar=cfg.plot.error_type,
         hue='level',
         data=df,
-        palette='colorblind',
         ax=ax,
     )
     fig.suptitle('Jaccard dissimilarity / distance')
     ax.set(title=locname, xlabel=r'Quadrat distance ($m$)', ylabel='Jaccard dissimilarity')
 
     return [fig], meta
 
 
+def a8(df: pd.DataFrame, cfg: Config) -> PlotData:
+    locname = cfg.locality.name
+    meta = fill_metadata(locname, 'a8')
+    figs = []
+
+    fig, ax = plt.subplots(figsize=(12, 12))
+    df['individuals_bin'] = pd.cut(df.individuals, geom_r2(1, df.individuals.max()), right=False)
+    ab_dist_df = df.groupby(['level', 'individuals_bin'], as_index=False, observed=False).count()
+    sns.barplot(x='individuals_bin', y='species', hue='level', data=ab_dist_df, ax=ax, errorbar=cfg.plot.error_type)
+    fig.suptitle('Species abundance distribution')
+    ax.tick_params(axis='x', labelrotation=45)
+    ax.set(title=locname, xlabel='Abundance', ylabel='# of species')
+    figs.append(fig)
+
+    for ldf, lvl in df_levels(df):
+        fig, ax = plt.subplots(figsize=(20, 20))
+        ldf_sorted = ldf.sort_values('individuals', ascending=False)
+        sns.barplot(x='species', y='individuals', data=ldf_sorted, ax=ax)
+        ax.bar_label(ax.containers[0], fontsize=5)
+        fig.suptitle('Equitability of abundance')
+        ax.set(title=f'{locname}, level {lvl}', xlabel='Species', ylabel='Abundance')
+        ax.tick_params(axis='x', labelrotation=90)
+        figs.append(fig)
+
+    return figs, meta
+
+
 def df_levels(df: pd.DataFrame) -> Generator[tuple[pd.DataFrame, int], None, None]:
     levels = df['level'].unique()
     for level in sorted(levels):
         ldf = df[df.level == level]
-        yield (ldf, level)
+        yield (ldf, int(level))
 
 
-def to_interval(intr: str):
+def to_interval(intr: str) -> 'pd.Interval[float]':
     closed = (intr[0] == '[', intr[-1] == ']')
     cl_type: Literal['left', 'right', 'both', 'neither']
     match closed:
         case (True, False):
             cl_type = 'left'
         case (False, True):
             cl_type = 'right'
@@ -434,36 +434,38 @@
             cl_type = 'both'
         case (False, False):
             cl_type = 'neither'
     left, right = map(float, intr[1:-1].split(','))
     return pd.Interval(left, right, cl_type)
 
 
-def fill_metadata(title: str, analysis: str, locname: Optional[str] = None) -> Metadata:
-    if locname is None:
-        locname = title
+def fill_metadata(locname: str | None, analysis: str) -> Metadata:
     metadata = SVG_METADATA.copy()
-    metadata['Coverage'] = locname
-    per_analysis_kw = {
+    per_analysis_kw: dict[str, list[str]] = {
         'a1': ['overview', 'species', 'quadrat', 'transect', 'species richness'],
         'a2': ['species area relationship', 'species', 'area'],
         'a3': ['pairwise difference', 'distance', 'distance decay'],
         'a4': ['species', 'sum', 'radius'],
         'a5': ['expected species richness', 'observed/expected'],
         'a6': ['species', 'shared species', 'different specied', 'distance decay', 'common/total', 'common/differing'],
         'a7': ['jaccard dissimilarity', 'jaccard', 'distance decay'],
+        'a8': [],
     }
-    kws = ['marine', 'ecology', locname] + per_analysis_kw[analysis]
-    metadata['Keywords'] = list(sorted(kws))
-    metadata['Title'] = title
+    kws = ['marine', 'ecology'] + per_analysis_kw[analysis]
+    if locname:
+        metadata['Title'] = metadata['Coverage'] = locname
+        kws.append(locname)
+    else:
+        metadata['Title'] = metadata['Coverage'] = analysis
+    metadata['Keywords'] = sorted(kws)
     return metadata
 
 
 def conv_png_metadata(metadata: Metadata) -> Metadata:
     for key, val in ADD_PNG_METADATA.items():
         metadata[key] = val
     # vals must be latin1-encodable, convert lists to strs
     metadata['Keywords'] = ', '.join(metadata['Keywords'])  # type: ignore[arg-type]
-    metadata['Contributor'] = ', '.join(metadata['Contributor'])    # type: ignore[arg-type]
+    metadata['Contributor'] = ', '.join(metadata['Contributor'])  # type: ignore[arg-type]
     metadata['Creation Time'] = datetime.datetime.now().astimezone().isoformat()
     del metadata['Rights']  # PNG has "Copyright"
     return metadata
```

### Comparing `seal-tool-0.10.0/src/seal/preprocess.py` & `seal_tool-0.11.0/src/seal/preprocess.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,36 @@
 #!/usr/bin/env python3
 
 import argparse
+from typing import Any, cast
+
 import pandas as pd
 
 from seal.common import enc_dtypes
 
 
-def main(args: argparse.Namespace) -> int:
+def main(args: argparse.Namespace) -> int:  # noqa: PLR0912, PLR0915
     enc = pd.read_csv(args.dataset, dtype=enc_dtypes(), parse_dates=['date']).rename(columns=str.lower).convert_dtypes()
     pd.set_option('display.max_seq_items', None)
 
     if 'refs' in args.checks:
         diff = check_ref(enc)
         if not diff.empty:
             print(f'WARN: The following values of "ref" column are out of place:\n{diff}.\n')
 
     if 'nas' in args.checks:
         na_indices, checked_cols = check_nas(enc)
         if not na_indices.empty:
-            nas = enc.loc[na_indices, checked_cols]
-            print('WARN: The folowing rows are missing important values:')
-            for idx, row in nas.iterrows():
-                nas_columns = ', '.join(row[row.isna()].index.to_list())
-                print(f'Row {idx} NA columns: {nas_columns}')
-            if args.drop_nas:
-                enc = enc[~enc.index.isin(na_indices)]
-            elif args.drop_nas is None:
-                drop = input('[D]rop/[I]gnore?\n').lower()
-                if 'drop'.startswith(drop):
-                    enc = enc[~enc.index.isin(na_indices)]
-            print('\n')
+            enc = handle_nas(enc, na_indices, checked_cols, args)
 
     if 'strs' in args.checks:
         cleaned = check_clean_strs(enc)
         bad_only = cleaned.dropna(how='all')
         if not bad_only.empty:
-            print('WARN: The following strings were cleaned:')
-            for idx, row in bad_only.iterrows():
-                fixed_columns = ', '.join(row[~row.isna()].index.to_list())
-                print(f'Fixed string(s) in row {idx}, columns: {fixed_columns}')
-            print('\n')
-
-            for name in enc.columns:
-                if name not in cleaned.columns:
-                    cleaned[name] = pd.Series([pd.NA] * enc.shape[0])
-            cleaned = cleaned[enc.columns]
-            enc = enc.where(cleaned.isna() | (enc.equals(cleaned)), cleaned)
+            enc = handle_bad_strs(enc, bad_only, cleaned)
 
     if 'coords' in args.checks:
         x_diff, y_diff = check_coords(enc)
         if not x_diff.empty:
             print(f'WARN: Following x coordinates do not match corresponding quadrat ID:\n{x_diff}\n')
         if not y_diff.empty:
             print(f'WARN: Following y coordinates do not match corresponding quadrat ID:\n{y_diff}\n')
@@ -58,20 +39,15 @@
         diff = check_species_name(enc)
         if not diff.empty:
             print(f'WARN: The following species or name occurs in more than one pairing:\n{diff}\n')
 
     if 'species-phase-morph' in args.checks:
         diff = check_species_phase_morph(enc)
         if not diff.empty:
-            bad = enc.loc[diff, ['species', 'phase', 'name', 'morph']]
-            bad_groups = bad.groupby(['species', 'phase'], observed=True)
-            print(f'WARN: The following ((species, phase), morph) pairs occur in multiple combinations:\n{diff}')
-            for k, v in bad_groups:
-                print(f'\n{k} paired-up simultaneously with\n{v.T}')
-            print('\n')
+            handle_bad_combinations(enc, diff)
 
     if 'morph-species' in args.checks:
         diff = check_morph_species(enc)
         if not diff.empty:
             print(f'WARN: The following morphs do not match expected species:\n{diff}\n')
 
     if 'family' in args.checks:
@@ -81,27 +57,32 @@
             enc.loc[diff, 'phase'] = 'term'
             print(f'Converted "ad" these phases to "term"\n{diff}\n')
 
     if 'dups' in args.checks:
         sans_ref = enc.drop(columns='ref', errors='raise') if 'ref' in enc.columns else enc
         dups = enc[sans_ref.duplicated(keep=False)]
         if not dups.empty:
-            print(f'WARN: The folowing rows may be duplicates:\n{dups.index.tolist()}\n')
+            print(f'WARN: The following rows may be duplicates:\n{dups.index.tolist()}\n')
+
+    if 'individuals' in args.checks:
+        nonpositive = enc[enc['n_individuals'] > 0]
+        if not nonpositive.empty:
+            print(f'WARN: The following rows contain invalid number of individuals:\n{nonpositive.index.tolist()}\n')
 
     if enc.empty:
         print('Result is empty. No data will be written.')
         return 1
 
     args.output.parent.mkdir(parents=True, exist_ok=True)
     enc.to_csv(args.output, index=False)
     print(f'Done. {enc.shape[0]} rows written to {args.output}.')
     return 0
 
 
-def check_nas(enc: pd.DataFrame) -> tuple[pd.Index, list[str]]:
+def check_nas(enc: pd.DataFrame) -> tuple['pd.Index[Any]', list[str]]:
     """Return indices in *enc* where important values are NA.
 
     Note that "important value" does not mean it is necessarily used in analysis
     just that they should not be missing by consensus.
 
     >>> enc = pd.DataFrame(
     ...     {
@@ -123,15 +104,14 @@
     ... ).convert_dtypes()
     >>> res = check_nas(enc)
     >>> res[0]
     Index([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13], dtype='int64')
     >>> res[1]
     ['significant_size', 'coord_x', 'coord_y', 'family', 'individuals', 'locality', 'morph', 'name', 'phase', 'quadrat', 'quadrat_id', 'species', 'transect', 't']
     """
-
     checked_cols = [
         'significant_size',
         'coord_x',
         'coord_y',
         'family',
         'individuals',
         'locality',
@@ -146,63 +126,95 @@
     ]
     found_cols = [col for col in checked_cols if col in enc.columns]
 
     col_has_nas = enc[found_cols].isna().any(axis='columns')
     return enc[col_has_nas].index, found_cols
 
 
-def check_ref(enc: pd.DataFrame) -> pd.Index:
-    """Return indices of *enc* where they differ from the expected 1-inf
-    well behaved series
+def handle_nas(
+    enc: pd.DataFrame, na_indices: 'pd.Index[Any]', checked_cols: list[str], args: argparse.Namespace
+) -> pd.DataFrame:
+    nas = enc.loc[na_indices, checked_cols]
+    info = ['WARN: The following rows are missing important values:']
+    for idx, row in nas.iterrows():
+        nas_columns = ', '.join(row[row.isna()].index.to_list())
+        info.append(f'Row {idx} NA columns: {nas_columns}')
+    info.append('\n')
+    nas_info = '\n'.join(info)
+    print(nas_info)
+
+    if args.drop_nas:
+        enc = enc[~enc.index.isin(na_indices)]
+    elif args.drop_nas is None:
+        drop = input('[D]rop/[I]gnore?\n').lower()
+        if 'drop'.startswith(drop):
+            enc = enc[~enc.index.isin(na_indices)]
+    return enc
+
+
+def check_ref(enc: pd.DataFrame) -> 'pd.Index[Any]':
+    """Return indices of *enc* where they differ from the expected 1-inf well behaved series.
 
     >>> enc = pd.DataFrame({'ref': [1, 2, 3, 4, 5, 6]}).convert_dtypes()
     >>> check_ref(enc)
     Index([], dtype='int64')
 
     >>> enc = pd.DataFrame({'ref': [1, pd.NA, 3, 5, 4, 6]}).convert_dtypes()
     >>> check_ref(enc)
     Index([1, 3, 4], dtype='int64')
 
     >>> enc = pd.DataFrame({'ref': [1, 2, 4, 5, 6]}).convert_dtypes()
     >>> check_ref(enc)
     Index([2, 3, 4], dtype='int64')
     """
-
     good_ref = pd.Series(range(1, enc.shape[0] + 1), dtype=enc.ref.dtype)
     diffs = enc[(enc.ref != good_ref) | enc.ref.isna()].index
     return diffs
 
 
 def check_clean_strs(enc: pd.DataFrame) -> pd.DataFrame:
-    """Return new DataFrame containing values where any whitespace was not a simple
-    whitespace in the original DataFrame with the rest of values being <NA>
+    r"""Return new DataFrame containing values where any whitespace was not a simple whitespace in the original DataFrame with the rest of values being NA.
 
     >>> enc = pd.DataFrame(
     ...     {
-    ...         'locality': ['good1', 'go od 2', 'ba  d', 'ba\u00A0d', 'good3'],
+    ...         'locality': ['good1', 'go od 2', 'ba  d', 'ba\u00a0d', 'good3'],
     ...         'species': ['b\tad', 'good4', 'good5', 'bad  ', 'good7'],
     ...     }
     ... ).convert_dtypes()
     >>> check_clean_strs(enc)
       locality species
     0     <NA>    b ad
     1     <NA>    <NA>
     2     ba d    <NA>
     3     ba d     bad
     4     <NA>    <NA>
     """
     strs = enc.select_dtypes(['string'])
     cleaned_strs = strs.apply(lambda col: col.str.strip().replace(r'\s+', ' ', regex=True))
-    diff = cleaned_strs[strs != cleaned_strs]
+    diff = cast(pd.DataFrame, cleaned_strs[strs != cleaned_strs])
     return diff
 
 
-def check_coords(enc: pd.DataFrame) -> tuple[pd.Index, pd.Index]:
-    """Return tuple (idx_x, idx_y) of indices in *enc* where coord columns differ from the expected
-    value implied by the quadrat_id column.
+def handle_bad_strs(enc: pd.DataFrame, bad_only: pd.DataFrame, cleaned: pd.DataFrame) -> pd.DataFrame:
+    print('WARN: The following strings were cleaned:')
+    for idx, row in bad_only.iterrows():
+        fixed_columns = ', '.join(row[~row.isna()].index.to_list())
+        print(f'Fixed string(s) in row {idx}, columns: {fixed_columns}')
+    print('\n')
+
+    for name in enc.columns:
+        if name not in cleaned.columns:
+            cleaned[name] = pd.Series([pd.NA] * enc.shape[0])
+    cleaned = cleaned[enc.columns]
+    enc = enc.where(cleaned.isna() | (enc.equals(cleaned)), cleaned)
+    return enc
+
+
+def check_coords(enc: pd.DataFrame) -> tuple['pd.Index[Any]', 'pd.Index[Any]']:
+    """Return tuple (idx_x, idx_y) of indices in *enc* where coord columns differ from the expected value implied by the quadrat_id column.
 
     >>> enc = pd.DataFrame(
     ...     {
     ...         'quadrat_id': ['q_1_good_1', 'q_1_badx_2', 'q_2_bady_1', 'q_2_good_2'],
     ...         'coord_x': [0, 1, 1, 1],
     ...         'coord_y': [0, 1, -2, 1],
     ...     }
@@ -214,34 +226,32 @@
     x_from_qid = pd.to_numeric(splt[1], downcast='unsigned') - 1
     y_from_qid = pd.to_numeric(splt[3], downcast='unsigned') - 1
     x_diff = enc[(x_from_qid - enc.coord_x) != 0]
     y_diff = enc[(y_from_qid - enc.coord_y) != 0]
     return x_diff.index, y_diff.index
 
 
-def check_species_name(enc: pd.DataFrame) -> pd.Index:
-    """Return indices in *enc* where single species
-    has multiple values in name or vice versa.
+def check_species_name(enc: pd.DataFrame) -> 'pd.Index[Any]':
+    """Return indices in *enc* where single species has multiple values in name or vice versa.
 
     This should not happen has name is simply a translation of species.
 
     >>> enc = pd.DataFrame(
     ...     data={'species': ['spp1', 'spp2', 'spp2', 'spp3', 'spp4'], 'name': ['a', 'c', 'b', 'c', 'b']}
     ... ).convert_dtypes()
     >>> check_species_name(enc)
     Index([1, 2, 3, 4], dtype='int64')
     """
-
     spp_name = enc[['species', 'name']].drop_duplicates()
     spp_dups = spp_name.duplicated(subset='species', keep=False)
     name_dups = spp_name.duplicated(subset='name', keep=False)
     return spp_name[spp_dups | name_dups].index
 
 
-def check_species_phase_morph(enc: pd.DataFrame) -> pd.Index:
+def check_species_phase_morph(enc: pd.DataFrame) -> 'pd.Index[Any]':
     """Return indices in *enc* where a species in given phase occurs with more than one morph.
 
     This should not happen as species in given life phase are assigned only to one morphotaxon.
 
     >>> enc = pd.DataFrame(
     ...     data={
     ...         'species': ['spp1', 'spp2', 'spp2', 'spp1', 'spp1'],
@@ -253,16 +263,27 @@
     Index([0, 4], dtype='int64')
     """
     trio = enc[['species', 'phase', 'morph']].drop_duplicates()
     dups_bools = trio.duplicated(subset=['species', 'phase'], keep=False)
     return trio[dups_bools].index
 
 
-def check_morph_species(enc: pd.DataFrame) -> pd.Index:
-    """Return indices in *enc* where the morph is either not identical with the species
+def handle_bad_combinations(enc: pd.DataFrame, diff: 'pd.Index[Any]') -> None:
+    bad = enc.loc[diff, ['species', 'phase', 'name', 'morph']]
+    bad_groups = bad.groupby(['species', 'phase'], observed=True)
+    print(f'WARN: The following ((species, phase), morph) pairs occur in multiple combinations:\n{diff}')
+    for k, v in bad_groups:
+        print(f'\n{k} paired-up simultaneously with\n{v.T}')
+    print('\n')
+
+
+def check_morph_species(enc: pd.DataFrame) -> 'pd.Index[Any]':
+    """Return indices in `enc` with invalid morph values.
+
+    Morph is considered invalid where the it is either not identical with the species
     or does not start with 'M ', which indicates a morphotaxon.
 
     This should not happen as either the species itself should be known or the morphotaxon should be specified.
 
     >>> enc = pd.DataFrame(
     ...     data={
     ...         'morph': ['M morph0', 'M morph1', 'm morph0', 'Morph2', 'morph3'],
@@ -272,16 +293,17 @@
     >>> check_morph_species(enc)
     Index([3, 4], dtype='int64')
     """
     non_m = enc[~enc.morph.str.startswith('M ')]
     return non_m[non_m.morph != non_m.species].index
 
 
-def check_family(enc: pd.DataFrame) -> pd.Index:
+def check_family(enc: pd.DataFrame) -> 'pd.Index[Any]':
     """Return indices in *enc* where species is "Labridae" or "Scaridae" yet phase is "ad".
+
     This should not occur as while other families have only juvenile and adult phase in our datasets,
     Labridae and Scaridae have juvenile, initial and terminal phase.
 
     >>> enc = pd.DataFrame(
     ...     data={
     ...         'phase': ['ad', 'juv', 'init', 'term', 'ad'],
     ...         'family': ['Labridae', 'Labridae', 'Scaridae', 'Scaridae', 'Scaridae'],
```

### Comparing `seal-tool-0.10.0/src/seal_tool.egg-info/PKG-INFO` & `seal_tool-0.11.0/src/seal_tool.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,851 +1,863 @@
-Metadata-Version: 2.1
-Name: seal-tool
-Version: 0.10.0
-Summary: A tool to perform richness-extent-grain analyses
-Author-email: Martin Matouš <m@matous.dev>, Barbora Winterová <winterova@mail.muni.cz>
-License:                     GNU GENERAL PUBLIC LICENSE
-                               Version 3, 29 June 2007
-        
-         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
-         Everyone is permitted to copy and distribute verbatim copies
-         of this license document, but changing it is not allowed.
-        
-                                    Preamble
-        
-          The GNU General Public License is a free, copyleft license for
-        software and other kinds of works.
-        
-          The licenses for most software and other practical works are designed
-        to take away your freedom to share and change the works.  By contrast,
-        the GNU General Public License is intended to guarantee your freedom to
-        share and change all versions of a program--to make sure it remains free
-        software for all its users.  We, the Free Software Foundation, use the
-        GNU General Public License for most of our software; it applies also to
-        any other work released this way by its authors.  You can apply it to
-        your programs, too.
-        
-          When we speak of free software, we are referring to freedom, not
-        price.  Our General Public Licenses are designed to make sure that you
-        have the freedom to distribute copies of free software (and charge for
-        them if you wish), that you receive source code or can get it if you
-        want it, that you can change the software or use pieces of it in new
-        free programs, and that you know you can do these things.
-        
-          To protect your rights, we need to prevent others from denying you
-        these rights or asking you to surrender the rights.  Therefore, you have
-        certain responsibilities if you distribute copies of the software, or if
-        you modify it: responsibilities to respect the freedom of others.
-        
-          For example, if you distribute copies of such a program, whether
-        gratis or for a fee, you must pass on to the recipients the same
-        freedoms that you received.  You must make sure that they, too, receive
-        or can get the source code.  And you must show them these terms so they
-        know their rights.
-        
-          Developers that use the GNU GPL protect your rights with two steps:
-        (1) assert copyright on the software, and (2) offer you this License
-        giving you legal permission to copy, distribute and/or modify it.
-        
-          For the developers' and authors' protection, the GPL clearly explains
-        that there is no warranty for this free software.  For both users' and
-        authors' sake, the GPL requires that modified versions be marked as
-        changed, so that their problems will not be attributed erroneously to
-        authors of previous versions.
-        
-          Some devices are designed to deny users access to install or run
-        modified versions of the software inside them, although the manufacturer
-        can do so.  This is fundamentally incompatible with the aim of
-        protecting users' freedom to change the software.  The systematic
-        pattern of such abuse occurs in the area of products for individuals to
-        use, which is precisely where it is most unacceptable.  Therefore, we
-        have designed this version of the GPL to prohibit the practice for those
-        products.  If such problems arise substantially in other domains, we
-        stand ready to extend this provision to those domains in future versions
-        of the GPL, as needed to protect the freedom of users.
-        
-          Finally, every program is threatened constantly by software patents.
-        States should not allow patents to restrict development and use of
-        software on general-purpose computers, but in those that do, we wish to
-        avoid the special danger that patents applied to a free program could
-        make it effectively proprietary.  To prevent this, the GPL assures that
-        patents cannot be used to render the program non-free.
-        
-          The precise terms and conditions for copying, distribution and
-        modification follow.
-        
-                               TERMS AND CONDITIONS
-        
-          0. Definitions.
-        
-          "This License" refers to version 3 of the GNU General Public License.
-        
-          "Copyright" also means copyright-like laws that apply to other kinds of
-        works, such as semiconductor masks.
-        
-          "The Program" refers to any copyrightable work licensed under this
-        License.  Each licensee is addressed as "you".  "Licensees" and
-        "recipients" may be individuals or organizations.
-        
-          To "modify" a work means to copy from or adapt all or part of the work
-        in a fashion requiring copyright permission, other than the making of an
-        exact copy.  The resulting work is called a "modified version" of the
-        earlier work or a work "based on" the earlier work.
-        
-          A "covered work" means either the unmodified Program or a work based
-        on the Program.
-        
-          To "propagate" a work means to do anything with it that, without
-        permission, would make you directly or secondarily liable for
-        infringement under applicable copyright law, except executing it on a
-        computer or modifying a private copy.  Propagation includes copying,
-        distribution (with or without modification), making available to the
-        public, and in some countries other activities as well.
-        
-          To "convey" a work means any kind of propagation that enables other
-        parties to make or receive copies.  Mere interaction with a user through
-        a computer network, with no transfer of a copy, is not conveying.
-        
-          An interactive user interface displays "Appropriate Legal Notices"
-        to the extent that it includes a convenient and prominently visible
-        feature that (1) displays an appropriate copyright notice, and (2)
-        tells the user that there is no warranty for the work (except to the
-        extent that warranties are provided), that licensees may convey the
-        work under this License, and how to view a copy of this License.  If
-        the interface presents a list of user commands or options, such as a
-        menu, a prominent item in the list meets this criterion.
-        
-          1. Source Code.
-        
-          The "source code" for a work means the preferred form of the work
-        for making modifications to it.  "Object code" means any non-source
-        form of a work.
-        
-          A "Standard Interface" means an interface that either is an official
-        standard defined by a recognized standards body, or, in the case of
-        interfaces specified for a particular programming language, one that
-        is widely used among developers working in that language.
-        
-          The "System Libraries" of an executable work include anything, other
-        than the work as a whole, that (a) is included in the normal form of
-        packaging a Major Component, but which is not part of that Major
-        Component, and (b) serves only to enable use of the work with that
-        Major Component, or to implement a Standard Interface for which an
-        implementation is available to the public in source code form.  A
-        "Major Component", in this context, means a major essential component
-        (kernel, window system, and so on) of the specific operating system
-        (if any) on which the executable work runs, or a compiler used to
-        produce the work, or an object code interpreter used to run it.
-        
-          The "Corresponding Source" for a work in object code form means all
-        the source code needed to generate, install, and (for an executable
-        work) run the object code and to modify the work, including scripts to
-        control those activities.  However, it does not include the work's
-        System Libraries, or general-purpose tools or generally available free
-        programs which are used unmodified in performing those activities but
-        which are not part of the work.  For example, Corresponding Source
-        includes interface definition files associated with source files for
-        the work, and the source code for shared libraries and dynamically
-        linked subprograms that the work is specifically designed to require,
-        such as by intimate data communication or control flow between those
-        subprograms and other parts of the work.
-        
-          The Corresponding Source need not include anything that users
-        can regenerate automatically from other parts of the Corresponding
-        Source.
-        
-          The Corresponding Source for a work in source code form is that
-        same work.
-        
-          2. Basic Permissions.
-        
-          All rights granted under this License are granted for the term of
-        copyright on the Program, and are irrevocable provided the stated
-        conditions are met.  This License explicitly affirms your unlimited
-        permission to run the unmodified Program.  The output from running a
-        covered work is covered by this License only if the output, given its
-        content, constitutes a covered work.  This License acknowledges your
-        rights of fair use or other equivalent, as provided by copyright law.
-        
-          You may make, run and propagate covered works that you do not
-        convey, without conditions so long as your license otherwise remains
-        in force.  You may convey covered works to others for the sole purpose
-        of having them make modifications exclusively for you, or provide you
-        with facilities for running those works, provided that you comply with
-        the terms of this License in conveying all material for which you do
-        not control copyright.  Those thus making or running the covered works
-        for you must do so exclusively on your behalf, under your direction
-        and control, on terms that prohibit them from making any copies of
-        your copyrighted material outside their relationship with you.
-        
-          Conveying under any other circumstances is permitted solely under
-        the conditions stated below.  Sublicensing is not allowed; section 10
-        makes it unnecessary.
-        
-          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-        
-          No covered work shall be deemed part of an effective technological
-        measure under any applicable law fulfilling obligations under article
-        11 of the WIPO copyright treaty adopted on 20 December 1996, or
-        similar laws prohibiting or restricting circumvention of such
-        measures.
-        
-          When you convey a covered work, you waive any legal power to forbid
-        circumvention of technological measures to the extent such circumvention
-        is effected by exercising rights under this License with respect to
-        the covered work, and you disclaim any intention to limit operation or
-        modification of the work as a means of enforcing, against the work's
-        users, your or third parties' legal rights to forbid circumvention of
-        technological measures.
-        
-          4. Conveying Verbatim Copies.
-        
-          You may convey verbatim copies of the Program's source code as you
-        receive it, in any medium, provided that you conspicuously and
-        appropriately publish on each copy an appropriate copyright notice;
-        keep intact all notices stating that this License and any
-        non-permissive terms added in accord with section 7 apply to the code;
-        keep intact all notices of the absence of any warranty; and give all
-        recipients a copy of this License along with the Program.
-        
-          You may charge any price or no price for each copy that you convey,
-        and you may offer support or warranty protection for a fee.
-        
-          5. Conveying Modified Source Versions.
-        
-          You may convey a work based on the Program, or the modifications to
-        produce it from the Program, in the form of source code under the
-        terms of section 4, provided that you also meet all of these conditions:
-        
-            a) The work must carry prominent notices stating that you modified
-            it, and giving a relevant date.
-        
-            b) The work must carry prominent notices stating that it is
-            released under this License and any conditions added under section
-            7.  This requirement modifies the requirement in section 4 to
-            "keep intact all notices".
-        
-            c) You must license the entire work, as a whole, under this
-            License to anyone who comes into possession of a copy.  This
-            License will therefore apply, along with any applicable section 7
-            additional terms, to the whole of the work, and all its parts,
-            regardless of how they are packaged.  This License gives no
-            permission to license the work in any other way, but it does not
-            invalidate such permission if you have separately received it.
-        
-            d) If the work has interactive user interfaces, each must display
-            Appropriate Legal Notices; however, if the Program has interactive
-            interfaces that do not display Appropriate Legal Notices, your
-            work need not make them do so.
-        
-          A compilation of a covered work with other separate and independent
-        works, which are not by their nature extensions of the covered work,
-        and which are not combined with it such as to form a larger program,
-        in or on a volume of a storage or distribution medium, is called an
-        "aggregate" if the compilation and its resulting copyright are not
-        used to limit the access or legal rights of the compilation's users
-        beyond what the individual works permit.  Inclusion of a covered work
-        in an aggregate does not cause this License to apply to the other
-        parts of the aggregate.
-        
-          6. Conveying Non-Source Forms.
-        
-          You may convey a covered work in object code form under the terms
-        of sections 4 and 5, provided that you also convey the
-        machine-readable Corresponding Source under the terms of this License,
-        in one of these ways:
-        
-            a) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by the
-            Corresponding Source fixed on a durable physical medium
-            customarily used for software interchange.
-        
-            b) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by a
-            written offer, valid for at least three years and valid for as
-            long as you offer spare parts or customer support for that product
-            model, to give anyone who possesses the object code either (1) a
-            copy of the Corresponding Source for all the software in the
-            product that is covered by this License, on a durable physical
-            medium customarily used for software interchange, for a price no
-            more than your reasonable cost of physically performing this
-            conveying of source, or (2) access to copy the
-            Corresponding Source from a network server at no charge.
-        
-            c) Convey individual copies of the object code with a copy of the
-            written offer to provide the Corresponding Source.  This
-            alternative is allowed only occasionally and noncommercially, and
-            only if you received the object code with such an offer, in accord
-            with subsection 6b.
-        
-            d) Convey the object code by offering access from a designated
-            place (gratis or for a charge), and offer equivalent access to the
-            Corresponding Source in the same way through the same place at no
-            further charge.  You need not require recipients to copy the
-            Corresponding Source along with the object code.  If the place to
-            copy the object code is a network server, the Corresponding Source
-            may be on a different server (operated by you or a third party)
-            that supports equivalent copying facilities, provided you maintain
-            clear directions next to the object code saying where to find the
-            Corresponding Source.  Regardless of what server hosts the
-            Corresponding Source, you remain obligated to ensure that it is
-            available for as long as needed to satisfy these requirements.
-        
-            e) Convey the object code using peer-to-peer transmission, provided
-            you inform other peers where the object code and Corresponding
-            Source of the work are being offered to the general public at no
-            charge under subsection 6d.
-        
-          A separable portion of the object code, whose source code is excluded
-        from the Corresponding Source as a System Library, need not be
-        included in conveying the object code work.
-        
-          A "User Product" is either (1) a "consumer product", which means any
-        tangible personal property which is normally used for personal, family,
-        or household purposes, or (2) anything designed or sold for incorporation
-        into a dwelling.  In determining whether a product is a consumer product,
-        doubtful cases shall be resolved in favor of coverage.  For a particular
-        product received by a particular user, "normally used" refers to a
-        typical or common use of that class of product, regardless of the status
-        of the particular user or of the way in which the particular user
-        actually uses, or expects or is expected to use, the product.  A product
-        is a consumer product regardless of whether the product has substantial
-        commercial, industrial or non-consumer uses, unless such uses represent
-        the only significant mode of use of the product.
-        
-          "Installation Information" for a User Product means any methods,
-        procedures, authorization keys, or other information required to install
-        and execute modified versions of a covered work in that User Product from
-        a modified version of its Corresponding Source.  The information must
-        suffice to ensure that the continued functioning of the modified object
-        code is in no case prevented or interfered with solely because
-        modification has been made.
-        
-          If you convey an object code work under this section in, or with, or
-        specifically for use in, a User Product, and the conveying occurs as
-        part of a transaction in which the right of possession and use of the
-        User Product is transferred to the recipient in perpetuity or for a
-        fixed term (regardless of how the transaction is characterized), the
-        Corresponding Source conveyed under this section must be accompanied
-        by the Installation Information.  But this requirement does not apply
-        if neither you nor any third party retains the ability to install
-        modified object code on the User Product (for example, the work has
-        been installed in ROM).
-        
-          The requirement to provide Installation Information does not include a
-        requirement to continue to provide support service, warranty, or updates
-        for a work that has been modified or installed by the recipient, or for
-        the User Product in which it has been modified or installed.  Access to a
-        network may be denied when the modification itself materially and
-        adversely affects the operation of the network or violates the rules and
-        protocols for communication across the network.
-        
-          Corresponding Source conveyed, and Installation Information provided,
-        in accord with this section must be in a format that is publicly
-        documented (and with an implementation available to the public in
-        source code form), and must require no special password or key for
-        unpacking, reading or copying.
-        
-          7. Additional Terms.
-        
-          "Additional permissions" are terms that supplement the terms of this
-        License by making exceptions from one or more of its conditions.
-        Additional permissions that are applicable to the entire Program shall
-        be treated as though they were included in this License, to the extent
-        that they are valid under applicable law.  If additional permissions
-        apply only to part of the Program, that part may be used separately
-        under those permissions, but the entire Program remains governed by
-        this License without regard to the additional permissions.
-        
-          When you convey a copy of a covered work, you may at your option
-        remove any additional permissions from that copy, or from any part of
-        it.  (Additional permissions may be written to require their own
-        removal in certain cases when you modify the work.)  You may place
-        additional permissions on material, added by you to a covered work,
-        for which you have or can give appropriate copyright permission.
-        
-          Notwithstanding any other provision of this License, for material you
-        add to a covered work, you may (if authorized by the copyright holders of
-        that material) supplement the terms of this License with terms:
-        
-            a) Disclaiming warranty or limiting liability differently from the
-            terms of sections 15 and 16 of this License; or
-        
-            b) Requiring preservation of specified reasonable legal notices or
-            author attributions in that material or in the Appropriate Legal
-            Notices displayed by works containing it; or
-        
-            c) Prohibiting misrepresentation of the origin of that material, or
-            requiring that modified versions of such material be marked in
-            reasonable ways as different from the original version; or
-        
-            d) Limiting the use for publicity purposes of names of licensors or
-            authors of the material; or
-        
-            e) Declining to grant rights under trademark law for use of some
-            trade names, trademarks, or service marks; or
-        
-            f) Requiring indemnification of licensors and authors of that
-            material by anyone who conveys the material (or modified versions of
-            it) with contractual assumptions of liability to the recipient, for
-            any liability that these contractual assumptions directly impose on
-            those licensors and authors.
-        
-          All other non-permissive additional terms are considered "further
-        restrictions" within the meaning of section 10.  If the Program as you
-        received it, or any part of it, contains a notice stating that it is
-        governed by this License along with a term that is a further
-        restriction, you may remove that term.  If a license document contains
-        a further restriction but permits relicensing or conveying under this
-        License, you may add to a covered work material governed by the terms
-        of that license document, provided that the further restriction does
-        not survive such relicensing or conveying.
-        
-          If you add terms to a covered work in accord with this section, you
-        must place, in the relevant source files, a statement of the
-        additional terms that apply to those files, or a notice indicating
-        where to find the applicable terms.
-        
-          Additional terms, permissive or non-permissive, may be stated in the
-        form of a separately written license, or stated as exceptions;
-        the above requirements apply either way.
-        
-          8. Termination.
-        
-          You may not propagate or modify a covered work except as expressly
-        provided under this License.  Any attempt otherwise to propagate or
-        modify it is void, and will automatically terminate your rights under
-        this License (including any patent licenses granted under the third
-        paragraph of section 11).
-        
-          However, if you cease all violation of this License, then your
-        license from a particular copyright holder is reinstated (a)
-        provisionally, unless and until the copyright holder explicitly and
-        finally terminates your license, and (b) permanently, if the copyright
-        holder fails to notify you of the violation by some reasonable means
-        prior to 60 days after the cessation.
-        
-          Moreover, your license from a particular copyright holder is
-        reinstated permanently if the copyright holder notifies you of the
-        violation by some reasonable means, this is the first time you have
-        received notice of violation of this License (for any work) from that
-        copyright holder, and you cure the violation prior to 30 days after
-        your receipt of the notice.
-        
-          Termination of your rights under this section does not terminate the
-        licenses of parties who have received copies or rights from you under
-        this License.  If your rights have been terminated and not permanently
-        reinstated, you do not qualify to receive new licenses for the same
-        material under section 10.
-        
-          9. Acceptance Not Required for Having Copies.
-        
-          You are not required to accept this License in order to receive or
-        run a copy of the Program.  Ancillary propagation of a covered work
-        occurring solely as a consequence of using peer-to-peer transmission
-        to receive a copy likewise does not require acceptance.  However,
-        nothing other than this License grants you permission to propagate or
-        modify any covered work.  These actions infringe copyright if you do
-        not accept this License.  Therefore, by modifying or propagating a
-        covered work, you indicate your acceptance of this License to do so.
-        
-          10. Automatic Licensing of Downstream Recipients.
-        
-          Each time you convey a covered work, the recipient automatically
-        receives a license from the original licensors, to run, modify and
-        propagate that work, subject to this License.  You are not responsible
-        for enforcing compliance by third parties with this License.
-        
-          An "entity transaction" is a transaction transferring control of an
-        organization, or substantially all assets of one, or subdividing an
-        organization, or merging organizations.  If propagation of a covered
-        work results from an entity transaction, each party to that
-        transaction who receives a copy of the work also receives whatever
-        licenses to the work the party's predecessor in interest had or could
-        give under the previous paragraph, plus a right to possession of the
-        Corresponding Source of the work from the predecessor in interest, if
-        the predecessor has it or can get it with reasonable efforts.
-        
-          You may not impose any further restrictions on the exercise of the
-        rights granted or affirmed under this License.  For example, you may
-        not impose a license fee, royalty, or other charge for exercise of
-        rights granted under this License, and you may not initiate litigation
-        (including a cross-claim or counterclaim in a lawsuit) alleging that
-        any patent claim is infringed by making, using, selling, offering for
-        sale, or importing the Program or any portion of it.
-        
-          11. Patents.
-        
-          A "contributor" is a copyright holder who authorizes use under this
-        License of the Program or a work on which the Program is based.  The
-        work thus licensed is called the contributor's "contributor version".
-        
-          A contributor's "essential patent claims" are all patent claims
-        owned or controlled by the contributor, whether already acquired or
-        hereafter acquired, that would be infringed by some manner, permitted
-        by this License, of making, using, or selling its contributor version,
-        but do not include claims that would be infringed only as a
-        consequence of further modification of the contributor version.  For
-        purposes of this definition, "control" includes the right to grant
-        patent sublicenses in a manner consistent with the requirements of
-        this License.
-        
-          Each contributor grants you a non-exclusive, worldwide, royalty-free
-        patent license under the contributor's essential patent claims, to
-        make, use, sell, offer for sale, import and otherwise run, modify and
-        propagate the contents of its contributor version.
-        
-          In the following three paragraphs, a "patent license" is any express
-        agreement or commitment, however denominated, not to enforce a patent
-        (such as an express permission to practice a patent or covenant not to
-        sue for patent infringement).  To "grant" such a patent license to a
-        party means to make such an agreement or commitment not to enforce a
-        patent against the party.
-        
-          If you convey a covered work, knowingly relying on a patent license,
-        and the Corresponding Source of the work is not available for anyone
-        to copy, free of charge and under the terms of this License, through a
-        publicly available network server or other readily accessible means,
-        then you must either (1) cause the Corresponding Source to be so
-        available, or (2) arrange to deprive yourself of the benefit of the
-        patent license for this particular work, or (3) arrange, in a manner
-        consistent with the requirements of this License, to extend the patent
-        license to downstream recipients.  "Knowingly relying" means you have
-        actual knowledge that, but for the patent license, your conveying the
-        covered work in a country, or your recipient's use of the covered work
-        in a country, would infringe one or more identifiable patents in that
-        country that you have reason to believe are valid.
-        
-          If, pursuant to or in connection with a single transaction or
-        arrangement, you convey, or propagate by procuring conveyance of, a
-        covered work, and grant a patent license to some of the parties
-        receiving the covered work authorizing them to use, propagate, modify
-        or convey a specific copy of the covered work, then the patent license
-        you grant is automatically extended to all recipients of the covered
-        work and works based on it.
-        
-          A patent license is "discriminatory" if it does not include within
-        the scope of its coverage, prohibits the exercise of, or is
-        conditioned on the non-exercise of one or more of the rights that are
-        specifically granted under this License.  You may not convey a covered
-        work if you are a party to an arrangement with a third party that is
-        in the business of distributing software, under which you make payment
-        to the third party based on the extent of your activity of conveying
-        the work, and under which the third party grants, to any of the
-        parties who would receive the covered work from you, a discriminatory
-        patent license (a) in connection with copies of the covered work
-        conveyed by you (or copies made from those copies), or (b) primarily
-        for and in connection with specific products or compilations that
-        contain the covered work, unless you entered into that arrangement,
-        or that patent license was granted, prior to 28 March 2007.
-        
-          Nothing in this License shall be construed as excluding or limiting
-        any implied license or other defenses to infringement that may
-        otherwise be available to you under applicable patent law.
-        
-          12. No Surrender of Others' Freedom.
-        
-          If conditions are imposed on you (whether by court order, agreement or
-        otherwise) that contradict the conditions of this License, they do not
-        excuse you from the conditions of this License.  If you cannot convey a
-        covered work so as to satisfy simultaneously your obligations under this
-        License and any other pertinent obligations, then as a consequence you may
-        not convey it at all.  For example, if you agree to terms that obligate you
-        to collect a royalty for further conveying from those to whom you convey
-        the Program, the only way you could satisfy both those terms and this
-        License would be to refrain entirely from conveying the Program.
-        
-          13. Use with the GNU Affero General Public License.
-        
-          Notwithstanding any other provision of this License, you have
-        permission to link or combine any covered work with a work licensed
-        under version 3 of the GNU Affero General Public License into a single
-        combined work, and to convey the resulting work.  The terms of this
-        License will continue to apply to the part which is the covered work,
-        but the special requirements of the GNU Affero General Public License,
-        section 13, concerning interaction through a network will apply to the
-        combination as such.
-        
-          14. Revised Versions of this License.
-        
-          The Free Software Foundation may publish revised and/or new versions of
-        the GNU General Public License from time to time.  Such new versions will
-        be similar in spirit to the present version, but may differ in detail to
-        address new problems or concerns.
-        
-          Each version is given a distinguishing version number.  If the
-        Program specifies that a certain numbered version of the GNU General
-        Public License "or any later version" applies to it, you have the
-        option of following the terms and conditions either of that numbered
-        version or of any later version published by the Free Software
-        Foundation.  If the Program does not specify a version number of the
-        GNU General Public License, you may choose any version ever published
-        by the Free Software Foundation.
-        
-          If the Program specifies that a proxy can decide which future
-        versions of the GNU General Public License can be used, that proxy's
-        public statement of acceptance of a version permanently authorizes you
-        to choose that version for the Program.
-        
-          Later license versions may give you additional or different
-        permissions.  However, no additional obligations are imposed on any
-        author or copyright holder as a result of your choosing to follow a
-        later version.
-        
-          15. Disclaimer of Warranty.
-        
-          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-        
-          16. Limitation of Liability.
-        
-          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-        SUCH DAMAGES.
-        
-          17. Interpretation of Sections 15 and 16.
-        
-          If the disclaimer of warranty and limitation of liability provided
-        above cannot be given local legal effect according to their terms,
-        reviewing courts shall apply local law that most closely approximates
-        an absolute waiver of all civil liability in connection with the
-        Program, unless a warranty or assumption of liability accompanies a
-        copy of the Program in return for a fee.
-        
-                             END OF TERMS AND CONDITIONS
-Project-URL: Homepage, https://codeberg.org/mmatous/seal
-Project-URL: Bug Tracker, https://codeberg.org/mmatous/seal/issues
-Keywords: area,distance decay,ecology,extent,grain,richness,SAR,scale,species,species-area
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: alive-progress~=3.1
-Requires-Dist: numba~=0.59
-Requires-Dist: numexpr~=2.9
-Requires-Dist: pandas[plot]~=2.2
-Requires-Dist: pyhocon~=0.3
-Requires-Dist: seaborn~=0.13.2
-Provides-Extra: dev
-Requires-Dist: mypy~=1.6; extra == "dev"
-Requires-Dist: pandas-stubs~=2.0; extra == "dev"
-Requires-Dist: pytest~=7.4; extra == "dev"
-Requires-Dist: pytest-cov~=4.1; extra == "dev"
-Requires-Dist: ruff~=0.2.0; extra == "dev"
-Provides-Extra: alt-plot
-Requires-Dist: plotly; extra == "alt-plot"
-
-# seal
-
-Perform richness-extent-grain analyses inspired by Palmer & White
-([doi:10.1086/285704](https://doi.org/10.1086/285704), [doi:10.17615/n84a-pd17](https://doi.org/10.17615/n84a-pd17))
-
-## Setup
-
-### Installation
-
-Simply download `seal` from Codeberg [releases](https://codeberg.org/mmatous/seal)
-or clone the repository using git.
-
-### First run
-
-Done only when installing and running the tool for the first time.
-
-Open the project directory in your
-command-line interface.
-
-#### Linux
-
-In POSIX-compatible shell run:
-```bash
-source ./src/firstrun.sh
-```
-
-#### Windows
-
-In PowerShell Run:
-```
-./src/firstrun.ps1
-```
-
-If you encounter an error such as `./src/firstrun.ps1 cannot be loaded because running scripts is disabled on this system`
-on Windows, it means the script was blocked by your
-security settings. In that case either unblock
-the script e.g. using the [`Unblock-File` or `Set-ExecutionPolicy` cmdlets](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.security/set-executionpolicy?view=powershell-7.4#example-7-unblock-a-script-to-run-it-without-changing-the-execution-policy) or run the
-necessary commands manually.
-
-```
-python -m venv ./venv
-./venv/Scripts/Activate.ps1
-pip install .[dev]
-```
-
-
-You should see `(venv)` before your shell prompt now and `seal --help`
-should run the tool without errors. Continue with [Usage](#Usage).
-
-### Subsequent runs
-
-Done when running the tool any time after the first initial installation.
-
-Linux:
-```
-source ./venv/bin/activate
-seal <subcommand>
-```
-
-Windows PowerShell:
-```
-./venv/Scripts/activate.ps1
-seal <subcommand>
-```
-
-## Usage
-
-One would generally want to use `preprocess`, `analyse` and `plot` subcommands in this order.
-`misc` subcommand contains several scripts that
-may be useful while converting or modifying either datasets or quadrat
-lists for analysis.
-
-More detailed help can be accesed by `seal --help`
-or `seal <subcommand> --help`.
-
-### Preprocess
-
-Preprocess will ensure given dataset is fit to be processed
-by the `analyse` command by e.g. sanitizing strings,
-warning for missing values or
-checking whether species column remains consistent with
-name, morph and phase.
-
-Example:
-```
-seal preprocess --dataset ./datasets/raw.csv --output ./datasets/clean.csv
-```
-
-
-### Analysis
-
-`analyse` subcommand ingests [taskfile](./tasks/example-task.conf)
-to perform analyses requested therein.
-
-Example:
-```
-seal analyse --taskfile ./tasks/example-task.conf
-```
-
-Currently supported analyses are:
-
-#### a1 - Overview
-
-This analysis calculates per-quadrat species number
-and number of encountered individuals for each level.
-
-The additional data contain general description of given dataset and various smaller statistics for each level.
-Such statistics include, for example, the most common value, mean, median, min and such for each data column.
-
-This helps familiarize oneself with the data and serves as a basic check of the levels-creating strategy.
-
-#### a2 - Species-area relationship
-
-This analysis shows relationship between species richness and area sampled.
-
-Species-area curve is calculated for each level by accumulating quadrats
-and tallying the number of species. Since this method is sensitive to order of the
-quadrats, number of permutations must be specified and their arithmetic mean is plotted.
-
-The additional data contain statistics of the calculated results.
-
-#### a3 - Distance-dependent species difference
-
-This analysis creates pairwise difference of sets of encountered species
-in two quadrats.
-
-Result is the difference as a function of distance of the quadrats.
-
-#### a4 - Radius richness
-
-This analysis calculates the number of species within various distance intervals (interval's width is set by
-the `interval-step` parameter)
-from each quadrat. The radius forms a belt of sorts with a specified width.
-
-We recommend using the size of the smallest quadrat as the smallest possible step.
-
-#### a5 - Ratio of observed and expected species
-
-This analysis calculates the ratio of observed and expected number of species for each
-quadrat. The expected value is calculated as $$\sum_{}P_i * (1 - P_i)$$  where P<sub>i</sub> is the proportion
-of quadrats occupied by species _i_ and the summation is over all the species in the study grid.
-
-#### a6 - Ratio of shared and unique species
-
-This analysis calculates several ratios for pairs of quadrats based on their distance.
-1) Ratio of shared species among the quadrats and exclusive species among the quadrats.
-2) Ratio of shared species among the quadrats and all
-the species in the dataset.
-3) Ratio of shared species among the quadrats and
-all the species in the study grid.
-
-
-#### a7 - Jaccard dissimilarity
-
-This analysis calculates Jaccard dissimilarity with regards to species between
-all possible pairs of quadrats.
-
-Result is plotted as dissimilarity against the distance
-of the quadrats.
-
-Jaccard dissimilarity between quadrats _a_ and _b_ is calculated as:
-$$J(a, b) = 1 - \frac{intersect_{ab}}{intersect_{ab} + exclusive_a + exclusive_b}$$
-
-
-
-### Ploting
-
-`plot` subcommand ingests [taskfile](./tasks/example-task.conf) to detect results of previous analyses
-and present them as graphs.
-
-Generated graphs will be saved to the same directory as
-analysis results.
-
-Example:
-```
-seal plot --taskfile ./tasks/example-task.conf
-```
-
-### Misc
-
-`misc` subcommand is a kitchen sink of opinionated
-convenience tools.
-
-## Development
-
-For unit tests run `python -m doctest ./src/seal/<file>`.
-
-For functional tests run `pytest`.
-
-### License
-The source code—including the tests and documentation—is licensed under [GPLv3](./LICENSE)
-
-`./datasets/data-bmd-sl.csv` is licensed under [CC-BY-SA-4.0](./datasets/LICENSE)
-
-[aopk-fish.csv](./datasets/aopk-fish.csv) was provided under [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/)
-by AOPK ČR, Nálezová databáze ochrany přírody, on-line database portal.nature.cz. Downloaded 2024-02-05.
+Metadata-Version: 2.1
+Name: seal-tool
+Version: 0.11.0
+Summary: A tool to perform richness-extent-grain analyses
+Author-email: Martin Matouš <m@matous.dev>, Barbora Winterová <winterova@mail.muni.cz>
+License:                     GNU GENERAL PUBLIC LICENSE
+                               Version 3, 29 June 2007
+        
+         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+         Everyone is permitted to copy and distribute verbatim copies
+         of this license document, but changing it is not allowed.
+        
+                                    Preamble
+        
+          The GNU General Public License is a free, copyleft license for
+        software and other kinds of works.
+        
+          The licenses for most software and other practical works are designed
+        to take away your freedom to share and change the works.  By contrast,
+        the GNU General Public License is intended to guarantee your freedom to
+        share and change all versions of a program--to make sure it remains free
+        software for all its users.  We, the Free Software Foundation, use the
+        GNU General Public License for most of our software; it applies also to
+        any other work released this way by its authors.  You can apply it to
+        your programs, too.
+        
+          When we speak of free software, we are referring to freedom, not
+        price.  Our General Public Licenses are designed to make sure that you
+        have the freedom to distribute copies of free software (and charge for
+        them if you wish), that you receive source code or can get it if you
+        want it, that you can change the software or use pieces of it in new
+        free programs, and that you know you can do these things.
+        
+          To protect your rights, we need to prevent others from denying you
+        these rights or asking you to surrender the rights.  Therefore, you have
+        certain responsibilities if you distribute copies of the software, or if
+        you modify it: responsibilities to respect the freedom of others.
+        
+          For example, if you distribute copies of such a program, whether
+        gratis or for a fee, you must pass on to the recipients the same
+        freedoms that you received.  You must make sure that they, too, receive
+        or can get the source code.  And you must show them these terms so they
+        know their rights.
+        
+          Developers that use the GNU GPL protect your rights with two steps:
+        (1) assert copyright on the software, and (2) offer you this License
+        giving you legal permission to copy, distribute and/or modify it.
+        
+          For the developers' and authors' protection, the GPL clearly explains
+        that there is no warranty for this free software.  For both users' and
+        authors' sake, the GPL requires that modified versions be marked as
+        changed, so that their problems will not be attributed erroneously to
+        authors of previous versions.
+        
+          Some devices are designed to deny users access to install or run
+        modified versions of the software inside them, although the manufacturer
+        can do so.  This is fundamentally incompatible with the aim of
+        protecting users' freedom to change the software.  The systematic
+        pattern of such abuse occurs in the area of products for individuals to
+        use, which is precisely where it is most unacceptable.  Therefore, we
+        have designed this version of the GPL to prohibit the practice for those
+        products.  If such problems arise substantially in other domains, we
+        stand ready to extend this provision to those domains in future versions
+        of the GPL, as needed to protect the freedom of users.
+        
+          Finally, every program is threatened constantly by software patents.
+        States should not allow patents to restrict development and use of
+        software on general-purpose computers, but in those that do, we wish to
+        avoid the special danger that patents applied to a free program could
+        make it effectively proprietary.  To prevent this, the GPL assures that
+        patents cannot be used to render the program non-free.
+        
+          The precise terms and conditions for copying, distribution and
+        modification follow.
+        
+                               TERMS AND CONDITIONS
+        
+          0. Definitions.
+        
+          "This License" refers to version 3 of the GNU General Public License.
+        
+          "Copyright" also means copyright-like laws that apply to other kinds of
+        works, such as semiconductor masks.
+        
+          "The Program" refers to any copyrightable work licensed under this
+        License.  Each licensee is addressed as "you".  "Licensees" and
+        "recipients" may be individuals or organizations.
+        
+          To "modify" a work means to copy from or adapt all or part of the work
+        in a fashion requiring copyright permission, other than the making of an
+        exact copy.  The resulting work is called a "modified version" of the
+        earlier work or a work "based on" the earlier work.
+        
+          A "covered work" means either the unmodified Program or a work based
+        on the Program.
+        
+          To "propagate" a work means to do anything with it that, without
+        permission, would make you directly or secondarily liable for
+        infringement under applicable copyright law, except executing it on a
+        computer or modifying a private copy.  Propagation includes copying,
+        distribution (with or without modification), making available to the
+        public, and in some countries other activities as well.
+        
+          To "convey" a work means any kind of propagation that enables other
+        parties to make or receive copies.  Mere interaction with a user through
+        a computer network, with no transfer of a copy, is not conveying.
+        
+          An interactive user interface displays "Appropriate Legal Notices"
+        to the extent that it includes a convenient and prominently visible
+        feature that (1) displays an appropriate copyright notice, and (2)
+        tells the user that there is no warranty for the work (except to the
+        extent that warranties are provided), that licensees may convey the
+        work under this License, and how to view a copy of this License.  If
+        the interface presents a list of user commands or options, such as a
+        menu, a prominent item in the list meets this criterion.
+        
+          1. Source Code.
+        
+          The "source code" for a work means the preferred form of the work
+        for making modifications to it.  "Object code" means any non-source
+        form of a work.
+        
+          A "Standard Interface" means an interface that either is an official
+        standard defined by a recognized standards body, or, in the case of
+        interfaces specified for a particular programming language, one that
+        is widely used among developers working in that language.
+        
+          The "System Libraries" of an executable work include anything, other
+        than the work as a whole, that (a) is included in the normal form of
+        packaging a Major Component, but which is not part of that Major
+        Component, and (b) serves only to enable use of the work with that
+        Major Component, or to implement a Standard Interface for which an
+        implementation is available to the public in source code form.  A
+        "Major Component", in this context, means a major essential component
+        (kernel, window system, and so on) of the specific operating system
+        (if any) on which the executable work runs, or a compiler used to
+        produce the work, or an object code interpreter used to run it.
+        
+          The "Corresponding Source" for a work in object code form means all
+        the source code needed to generate, install, and (for an executable
+        work) run the object code and to modify the work, including scripts to
+        control those activities.  However, it does not include the work's
+        System Libraries, or general-purpose tools or generally available free
+        programs which are used unmodified in performing those activities but
+        which are not part of the work.  For example, Corresponding Source
+        includes interface definition files associated with source files for
+        the work, and the source code for shared libraries and dynamically
+        linked subprograms that the work is specifically designed to require,
+        such as by intimate data communication or control flow between those
+        subprograms and other parts of the work.
+        
+          The Corresponding Source need not include anything that users
+        can regenerate automatically from other parts of the Corresponding
+        Source.
+        
+          The Corresponding Source for a work in source code form is that
+        same work.
+        
+          2. Basic Permissions.
+        
+          All rights granted under this License are granted for the term of
+        copyright on the Program, and are irrevocable provided the stated
+        conditions are met.  This License explicitly affirms your unlimited
+        permission to run the unmodified Program.  The output from running a
+        covered work is covered by this License only if the output, given its
+        content, constitutes a covered work.  This License acknowledges your
+        rights of fair use or other equivalent, as provided by copyright law.
+        
+          You may make, run and propagate covered works that you do not
+        convey, without conditions so long as your license otherwise remains
+        in force.  You may convey covered works to others for the sole purpose
+        of having them make modifications exclusively for you, or provide you
+        with facilities for running those works, provided that you comply with
+        the terms of this License in conveying all material for which you do
+        not control copyright.  Those thus making or running the covered works
+        for you must do so exclusively on your behalf, under your direction
+        and control, on terms that prohibit them from making any copies of
+        your copyrighted material outside their relationship with you.
+        
+          Conveying under any other circumstances is permitted solely under
+        the conditions stated below.  Sublicensing is not allowed; section 10
+        makes it unnecessary.
+        
+          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+        
+          No covered work shall be deemed part of an effective technological
+        measure under any applicable law fulfilling obligations under article
+        11 of the WIPO copyright treaty adopted on 20 December 1996, or
+        similar laws prohibiting or restricting circumvention of such
+        measures.
+        
+          When you convey a covered work, you waive any legal power to forbid
+        circumvention of technological measures to the extent such circumvention
+        is effected by exercising rights under this License with respect to
+        the covered work, and you disclaim any intention to limit operation or
+        modification of the work as a means of enforcing, against the work's
+        users, your or third parties' legal rights to forbid circumvention of
+        technological measures.
+        
+          4. Conveying Verbatim Copies.
+        
+          You may convey verbatim copies of the Program's source code as you
+        receive it, in any medium, provided that you conspicuously and
+        appropriately publish on each copy an appropriate copyright notice;
+        keep intact all notices stating that this License and any
+        non-permissive terms added in accord with section 7 apply to the code;
+        keep intact all notices of the absence of any warranty; and give all
+        recipients a copy of this License along with the Program.
+        
+          You may charge any price or no price for each copy that you convey,
+        and you may offer support or warranty protection for a fee.
+        
+          5. Conveying Modified Source Versions.
+        
+          You may convey a work based on the Program, or the modifications to
+        produce it from the Program, in the form of source code under the
+        terms of section 4, provided that you also meet all of these conditions:
+        
+            a) The work must carry prominent notices stating that you modified
+            it, and giving a relevant date.
+        
+            b) The work must carry prominent notices stating that it is
+            released under this License and any conditions added under section
+            7.  This requirement modifies the requirement in section 4 to
+            "keep intact all notices".
+        
+            c) You must license the entire work, as a whole, under this
+            License to anyone who comes into possession of a copy.  This
+            License will therefore apply, along with any applicable section 7
+            additional terms, to the whole of the work, and all its parts,
+            regardless of how they are packaged.  This License gives no
+            permission to license the work in any other way, but it does not
+            invalidate such permission if you have separately received it.
+        
+            d) If the work has interactive user interfaces, each must display
+            Appropriate Legal Notices; however, if the Program has interactive
+            interfaces that do not display Appropriate Legal Notices, your
+            work need not make them do so.
+        
+          A compilation of a covered work with other separate and independent
+        works, which are not by their nature extensions of the covered work,
+        and which are not combined with it such as to form a larger program,
+        in or on a volume of a storage or distribution medium, is called an
+        "aggregate" if the compilation and its resulting copyright are not
+        used to limit the access or legal rights of the compilation's users
+        beyond what the individual works permit.  Inclusion of a covered work
+        in an aggregate does not cause this License to apply to the other
+        parts of the aggregate.
+        
+          6. Conveying Non-Source Forms.
+        
+          You may convey a covered work in object code form under the terms
+        of sections 4 and 5, provided that you also convey the
+        machine-readable Corresponding Source under the terms of this License,
+        in one of these ways:
+        
+            a) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by the
+            Corresponding Source fixed on a durable physical medium
+            customarily used for software interchange.
+        
+            b) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by a
+            written offer, valid for at least three years and valid for as
+            long as you offer spare parts or customer support for that product
+            model, to give anyone who possesses the object code either (1) a
+            copy of the Corresponding Source for all the software in the
+            product that is covered by this License, on a durable physical
+            medium customarily used for software interchange, for a price no
+            more than your reasonable cost of physically performing this
+            conveying of source, or (2) access to copy the
+            Corresponding Source from a network server at no charge.
+        
+            c) Convey individual copies of the object code with a copy of the
+            written offer to provide the Corresponding Source.  This
+            alternative is allowed only occasionally and noncommercially, and
+            only if you received the object code with such an offer, in accord
+            with subsection 6b.
+        
+            d) Convey the object code by offering access from a designated
+            place (gratis or for a charge), and offer equivalent access to the
+            Corresponding Source in the same way through the same place at no
+            further charge.  You need not require recipients to copy the
+            Corresponding Source along with the object code.  If the place to
+            copy the object code is a network server, the Corresponding Source
+            may be on a different server (operated by you or a third party)
+            that supports equivalent copying facilities, provided you maintain
+            clear directions next to the object code saying where to find the
+            Corresponding Source.  Regardless of what server hosts the
+            Corresponding Source, you remain obligated to ensure that it is
+            available for as long as needed to satisfy these requirements.
+        
+            e) Convey the object code using peer-to-peer transmission, provided
+            you inform other peers where the object code and Corresponding
+            Source of the work are being offered to the general public at no
+            charge under subsection 6d.
+        
+          A separable portion of the object code, whose source code is excluded
+        from the Corresponding Source as a System Library, need not be
+        included in conveying the object code work.
+        
+          A "User Product" is either (1) a "consumer product", which means any
+        tangible personal property which is normally used for personal, family,
+        or household purposes, or (2) anything designed or sold for incorporation
+        into a dwelling.  In determining whether a product is a consumer product,
+        doubtful cases shall be resolved in favor of coverage.  For a particular
+        product received by a particular user, "normally used" refers to a
+        typical or common use of that class of product, regardless of the status
+        of the particular user or of the way in which the particular user
+        actually uses, or expects or is expected to use, the product.  A product
+        is a consumer product regardless of whether the product has substantial
+        commercial, industrial or non-consumer uses, unless such uses represent
+        the only significant mode of use of the product.
+        
+          "Installation Information" for a User Product means any methods,
+        procedures, authorization keys, or other information required to install
+        and execute modified versions of a covered work in that User Product from
+        a modified version of its Corresponding Source.  The information must
+        suffice to ensure that the continued functioning of the modified object
+        code is in no case prevented or interfered with solely because
+        modification has been made.
+        
+          If you convey an object code work under this section in, or with, or
+        specifically for use in, a User Product, and the conveying occurs as
+        part of a transaction in which the right of possession and use of the
+        User Product is transferred to the recipient in perpetuity or for a
+        fixed term (regardless of how the transaction is characterized), the
+        Corresponding Source conveyed under this section must be accompanied
+        by the Installation Information.  But this requirement does not apply
+        if neither you nor any third party retains the ability to install
+        modified object code on the User Product (for example, the work has
+        been installed in ROM).
+        
+          The requirement to provide Installation Information does not include a
+        requirement to continue to provide support service, warranty, or updates
+        for a work that has been modified or installed by the recipient, or for
+        the User Product in which it has been modified or installed.  Access to a
+        network may be denied when the modification itself materially and
+        adversely affects the operation of the network or violates the rules and
+        protocols for communication across the network.
+        
+          Corresponding Source conveyed, and Installation Information provided,
+        in accord with this section must be in a format that is publicly
+        documented (and with an implementation available to the public in
+        source code form), and must require no special password or key for
+        unpacking, reading or copying.
+        
+          7. Additional Terms.
+        
+          "Additional permissions" are terms that supplement the terms of this
+        License by making exceptions from one or more of its conditions.
+        Additional permissions that are applicable to the entire Program shall
+        be treated as though they were included in this License, to the extent
+        that they are valid under applicable law.  If additional permissions
+        apply only to part of the Program, that part may be used separately
+        under those permissions, but the entire Program remains governed by
+        this License without regard to the additional permissions.
+        
+          When you convey a copy of a covered work, you may at your option
+        remove any additional permissions from that copy, or from any part of
+        it.  (Additional permissions may be written to require their own
+        removal in certain cases when you modify the work.)  You may place
+        additional permissions on material, added by you to a covered work,
+        for which you have or can give appropriate copyright permission.
+        
+          Notwithstanding any other provision of this License, for material you
+        add to a covered work, you may (if authorized by the copyright holders of
+        that material) supplement the terms of this License with terms:
+        
+            a) Disclaiming warranty or limiting liability differently from the
+            terms of sections 15 and 16 of this License; or
+        
+            b) Requiring preservation of specified reasonable legal notices or
+            author attributions in that material or in the Appropriate Legal
+            Notices displayed by works containing it; or
+        
+            c) Prohibiting misrepresentation of the origin of that material, or
+            requiring that modified versions of such material be marked in
+            reasonable ways as different from the original version; or
+        
+            d) Limiting the use for publicity purposes of names of licensors or
+            authors of the material; or
+        
+            e) Declining to grant rights under trademark law for use of some
+            trade names, trademarks, or service marks; or
+        
+            f) Requiring indemnification of licensors and authors of that
+            material by anyone who conveys the material (or modified versions of
+            it) with contractual assumptions of liability to the recipient, for
+            any liability that these contractual assumptions directly impose on
+            those licensors and authors.
+        
+          All other non-permissive additional terms are considered "further
+        restrictions" within the meaning of section 10.  If the Program as you
+        received it, or any part of it, contains a notice stating that it is
+        governed by this License along with a term that is a further
+        restriction, you may remove that term.  If a license document contains
+        a further restriction but permits relicensing or conveying under this
+        License, you may add to a covered work material governed by the terms
+        of that license document, provided that the further restriction does
+        not survive such relicensing or conveying.
+        
+          If you add terms to a covered work in accord with this section, you
+        must place, in the relevant source files, a statement of the
+        additional terms that apply to those files, or a notice indicating
+        where to find the applicable terms.
+        
+          Additional terms, permissive or non-permissive, may be stated in the
+        form of a separately written license, or stated as exceptions;
+        the above requirements apply either way.
+        
+          8. Termination.
+        
+          You may not propagate or modify a covered work except as expressly
+        provided under this License.  Any attempt otherwise to propagate or
+        modify it is void, and will automatically terminate your rights under
+        this License (including any patent licenses granted under the third
+        paragraph of section 11).
+        
+          However, if you cease all violation of this License, then your
+        license from a particular copyright holder is reinstated (a)
+        provisionally, unless and until the copyright holder explicitly and
+        finally terminates your license, and (b) permanently, if the copyright
+        holder fails to notify you of the violation by some reasonable means
+        prior to 60 days after the cessation.
+        
+          Moreover, your license from a particular copyright holder is
+        reinstated permanently if the copyright holder notifies you of the
+        violation by some reasonable means, this is the first time you have
+        received notice of violation of this License (for any work) from that
+        copyright holder, and you cure the violation prior to 30 days after
+        your receipt of the notice.
+        
+          Termination of your rights under this section does not terminate the
+        licenses of parties who have received copies or rights from you under
+        this License.  If your rights have been terminated and not permanently
+        reinstated, you do not qualify to receive new licenses for the same
+        material under section 10.
+        
+          9. Acceptance Not Required for Having Copies.
+        
+          You are not required to accept this License in order to receive or
+        run a copy of the Program.  Ancillary propagation of a covered work
+        occurring solely as a consequence of using peer-to-peer transmission
+        to receive a copy likewise does not require acceptance.  However,
+        nothing other than this License grants you permission to propagate or
+        modify any covered work.  These actions infringe copyright if you do
+        not accept this License.  Therefore, by modifying or propagating a
+        covered work, you indicate your acceptance of this License to do so.
+        
+          10. Automatic Licensing of Downstream Recipients.
+        
+          Each time you convey a covered work, the recipient automatically
+        receives a license from the original licensors, to run, modify and
+        propagate that work, subject to this License.  You are not responsible
+        for enforcing compliance by third parties with this License.
+        
+          An "entity transaction" is a transaction transferring control of an
+        organization, or substantially all assets of one, or subdividing an
+        organization, or merging organizations.  If propagation of a covered
+        work results from an entity transaction, each party to that
+        transaction who receives a copy of the work also receives whatever
+        licenses to the work the party's predecessor in interest had or could
+        give under the previous paragraph, plus a right to possession of the
+        Corresponding Source of the work from the predecessor in interest, if
+        the predecessor has it or can get it with reasonable efforts.
+        
+          You may not impose any further restrictions on the exercise of the
+        rights granted or affirmed under this License.  For example, you may
+        not impose a license fee, royalty, or other charge for exercise of
+        rights granted under this License, and you may not initiate litigation
+        (including a cross-claim or counterclaim in a lawsuit) alleging that
+        any patent claim is infringed by making, using, selling, offering for
+        sale, or importing the Program or any portion of it.
+        
+          11. Patents.
+        
+          A "contributor" is a copyright holder who authorizes use under this
+        License of the Program or a work on which the Program is based.  The
+        work thus licensed is called the contributor's "contributor version".
+        
+          A contributor's "essential patent claims" are all patent claims
+        owned or controlled by the contributor, whether already acquired or
+        hereafter acquired, that would be infringed by some manner, permitted
+        by this License, of making, using, or selling its contributor version,
+        but do not include claims that would be infringed only as a
+        consequence of further modification of the contributor version.  For
+        purposes of this definition, "control" includes the right to grant
+        patent sublicenses in a manner consistent with the requirements of
+        this License.
+        
+          Each contributor grants you a non-exclusive, worldwide, royalty-free
+        patent license under the contributor's essential patent claims, to
+        make, use, sell, offer for sale, import and otherwise run, modify and
+        propagate the contents of its contributor version.
+        
+          In the following three paragraphs, a "patent license" is any express
+        agreement or commitment, however denominated, not to enforce a patent
+        (such as an express permission to practice a patent or covenant not to
+        sue for patent infringement).  To "grant" such a patent license to a
+        party means to make such an agreement or commitment not to enforce a
+        patent against the party.
+        
+          If you convey a covered work, knowingly relying on a patent license,
+        and the Corresponding Source of the work is not available for anyone
+        to copy, free of charge and under the terms of this License, through a
+        publicly available network server or other readily accessible means,
+        then you must either (1) cause the Corresponding Source to be so
+        available, or (2) arrange to deprive yourself of the benefit of the
+        patent license for this particular work, or (3) arrange, in a manner
+        consistent with the requirements of this License, to extend the patent
+        license to downstream recipients.  "Knowingly relying" means you have
+        actual knowledge that, but for the patent license, your conveying the
+        covered work in a country, or your recipient's use of the covered work
+        in a country, would infringe one or more identifiable patents in that
+        country that you have reason to believe are valid.
+        
+          If, pursuant to or in connection with a single transaction or
+        arrangement, you convey, or propagate by procuring conveyance of, a
+        covered work, and grant a patent license to some of the parties
+        receiving the covered work authorizing them to use, propagate, modify
+        or convey a specific copy of the covered work, then the patent license
+        you grant is automatically extended to all recipients of the covered
+        work and works based on it.
+        
+          A patent license is "discriminatory" if it does not include within
+        the scope of its coverage, prohibits the exercise of, or is
+        conditioned on the non-exercise of one or more of the rights that are
+        specifically granted under this License.  You may not convey a covered
+        work if you are a party to an arrangement with a third party that is
+        in the business of distributing software, under which you make payment
+        to the third party based on the extent of your activity of conveying
+        the work, and under which the third party grants, to any of the
+        parties who would receive the covered work from you, a discriminatory
+        patent license (a) in connection with copies of the covered work
+        conveyed by you (or copies made from those copies), or (b) primarily
+        for and in connection with specific products or compilations that
+        contain the covered work, unless you entered into that arrangement,
+        or that patent license was granted, prior to 28 March 2007.
+        
+          Nothing in this License shall be construed as excluding or limiting
+        any implied license or other defenses to infringement that may
+        otherwise be available to you under applicable patent law.
+        
+          12. No Surrender of Others' Freedom.
+        
+          If conditions are imposed on you (whether by court order, agreement or
+        otherwise) that contradict the conditions of this License, they do not
+        excuse you from the conditions of this License.  If you cannot convey a
+        covered work so as to satisfy simultaneously your obligations under this
+        License and any other pertinent obligations, then as a consequence you may
+        not convey it at all.  For example, if you agree to terms that obligate you
+        to collect a royalty for further conveying from those to whom you convey
+        the Program, the only way you could satisfy both those terms and this
+        License would be to refrain entirely from conveying the Program.
+        
+          13. Use with the GNU Affero General Public License.
+        
+          Notwithstanding any other provision of this License, you have
+        permission to link or combine any covered work with a work licensed
+        under version 3 of the GNU Affero General Public License into a single
+        combined work, and to convey the resulting work.  The terms of this
+        License will continue to apply to the part which is the covered work,
+        but the special requirements of the GNU Affero General Public License,
+        section 13, concerning interaction through a network will apply to the
+        combination as such.
+        
+          14. Revised Versions of this License.
+        
+          The Free Software Foundation may publish revised and/or new versions of
+        the GNU General Public License from time to time.  Such new versions will
+        be similar in spirit to the present version, but may differ in detail to
+        address new problems or concerns.
+        
+          Each version is given a distinguishing version number.  If the
+        Program specifies that a certain numbered version of the GNU General
+        Public License "or any later version" applies to it, you have the
+        option of following the terms and conditions either of that numbered
+        version or of any later version published by the Free Software
+        Foundation.  If the Program does not specify a version number of the
+        GNU General Public License, you may choose any version ever published
+        by the Free Software Foundation.
+        
+          If the Program specifies that a proxy can decide which future
+        versions of the GNU General Public License can be used, that proxy's
+        public statement of acceptance of a version permanently authorizes you
+        to choose that version for the Program.
+        
+          Later license versions may give you additional or different
+        permissions.  However, no additional obligations are imposed on any
+        author or copyright holder as a result of your choosing to follow a
+        later version.
+        
+          15. Disclaimer of Warranty.
+        
+          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+        
+          16. Limitation of Liability.
+        
+          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+        SUCH DAMAGES.
+        
+          17. Interpretation of Sections 15 and 16.
+        
+          If the disclaimer of warranty and limitation of liability provided
+        above cannot be given local legal effect according to their terms,
+        reviewing courts shall apply local law that most closely approximates
+        an absolute waiver of all civil liability in connection with the
+        Program, unless a warranty or assumption of liability accompanies a
+        copy of the Program in return for a fee.
+        
+                             END OF TERMS AND CONDITIONS
+Project-URL: Homepage, https://codeberg.org/mmatous/seal
+Project-URL: Bug Tracker, https://codeberg.org/mmatous/seal/issues
+Keywords: area,distance decay,ecology,extent,grain,richness,SAR,scale,species,species-area
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: alive-progress~=3.1
+Requires-Dist: numba~=0.59
+Requires-Dist: numexpr~=2.9
+Requires-Dist: pandas~=2.2
+Requires-Dist: pydantic~=2.6
+Requires-Dist: scipy~=1.12
+Requires-Dist: seaborn~=0.13.2
+Provides-Extra: dev
+Requires-Dist: mypy==1.9; extra == "dev"
+Requires-Dist: pandas-stubs~=2.2; extra == "dev"
+Requires-Dist: pytest~=8.1; extra == "dev"
+Requires-Dist: pytest-cov~=5.0; extra == "dev"
+Requires-Dist: ruff==0.3.4; extra == "dev"
+Provides-Extra: alt-plot
+Requires-Dist: plotly; extra == "alt-plot"
+
+# seal
+
+Perform richness-extent-grain analyses inspired by Palmer & White
+([doi:10.1086/285704](https://doi.org/10.1086/285704), [doi:10.17615/n84a-pd17](https://doi.org/10.17615/n84a-pd17))
+
+## Setup
+
+### Installation
+
+From PyPI via `pip`:
+```
+pip install seal-tool
+```
+
+
+Or simply download `seal` from Codeberg [releases](https://codeberg.org/mmatous/seal)
+or clone the repository using git.
+
+
+### First run
+
+Done only when installing and running the tool for the first time
+and necessary only for non-PyPI installations.
+
+Open the project directory in your
+command-line interface.
+
+#### Linux
+
+In POSIX-compatible shell run:
+```bash
+source ./src/firstrun.sh
+```
+
+#### Windows
+
+In PowerShell Run:
+```
+./src/firstrun.ps1
+```
+
+If you encounter an error such as `./src/firstrun.ps1 cannot be loaded because running scripts is disabled on this system`
+on Windows, it means the script was blocked by your
+security settings. In that case either unblock
+the script e.g. using the [`Unblock-File` or `Set-ExecutionPolicy` cmdlets](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.security/set-executionpolicy?view=powershell-7.4#example-7-unblock-a-script-to-run-it-without-changing-the-execution-policy) or run the
+necessary commands manually.
+
+```
+python -m venv ./venv
+./venv/Scripts/Activate.ps1
+pip install .[dev]
+```
+
+
+You should see `(venv)` before your shell prompt now and `seal --help`
+should run the tool without errors. Continue with [Usage](#Usage).
+
+### Subsequent runs
+
+Done when running the tool any time after the first initial installation.
+
+Linux:
+```
+source ./venv/bin/activate
+seal <subcommand>
+```
+
+Windows PowerShell:
+```
+./venv/Scripts/activate.ps1
+seal <subcommand>
+```
+
+## Usage
+
+One would generally want to use `preprocess`, `analyse` and `plot` subcommands in this order.
+`misc` subcommand contains several scripts that
+may be useful while converting or modifying either datasets or quadrat
+lists for analysis.
+
+More detailed help can be accessed by `seal --help`
+or `seal <subcommand> --help`.
+
+### Preprocess
+
+Preprocess will ensure given dataset is fit to be processed
+by the `analyse` command by e.g. sanitizing strings,
+warning for missing values or
+checking whether species column remains consistent with
+name, morph and phase.
+
+Example:
+```
+seal preprocess --dataset ./datasets/raw.csv --output ./datasets/clean.csv
+```
+
+
+### Analysis
+
+`analyse` subcommand ingests a [taskfile](./tasks/0-example-task.toml)
+to perform analyses requested therein.
+
+Example:
+```
+seal analyse --taskfile ./tasks/0-example-task.toml
+```
+
+More example taskfiles are available at our [Codeberg repository](./tasks/)
+along with some [datasets](./datasets/).
+
+Currently supported analyses are:
+
+#### a1 - Overview
+
+This analysis calculates per-quadrat species number
+and number of encountered individuals for each level.
+
+The additional data contain general description of given dataset and various smaller statistics for each level.
+Such statistics include, for example, the most common value, mean, median, min and such for each data column.
+
+This helps familiarize oneself with the data and serves as a basic check of the levels-creating strategy.
+
+#### a2 - Species-area relationship
+
+This analysis shows relationship between species richness and area sampled.
+
+Species-area curve is calculated for each level by accumulating quadrats
+and tallying the number of species. Since this method is sensitive to order of the
+quadrats, number of permutations must be specified and their arithmetic mean is plotted.
+
+The additional data contain statistics of the calculated results.
+
+#### a3 - Distance-dependent species difference
+
+This analysis creates pairwise difference of sets of encountered species
+in two quadrats.
+
+Result is the difference as a function of distance of the quadrats.
+
+#### a4 - Radius richness
+
+This analysis calculates the number of species within various distance intervals (interval's width is set by
+the `interval-step` parameter)
+from each quadrat. The radius forms a belt of sorts with a specified width.
+
+We recommend using the size of the smallest quadrat as the smallest possible step.
+
+#### a5 - Ratio of observed and expected species
+
+This analysis calculates the ratio of observed and expected number of species for each
+quadrat. The expected value is calculated as $$\sum_{}P_i * (1 - P_i)$$  where P<sub>i</sub> is the proportion
+of quadrats occupied by species _i_ and the summation is over all the species in the study grid.
+
+#### a6 - Ratio of shared and unique species
+
+This analysis calculates several ratios for pairs of quadrats based on their distance.
+1) Ratio of shared species among the quadrats and exclusive species among the quadrats.
+2) Ratio of shared species among the quadrats and all
+the species in the dataset.
+3) Ratio of shared species among the quadrats and
+all the species in the study grid.
+
+
+#### a7 - Jaccard dissimilarity
+
+This analysis calculates Jaccard dissimilarity with regards to species between
+all possible pairs of quadrats.
+
+Result is plotted as dissimilarity against the distance
+of the quadrats.
+
+Jaccard dissimilarity between quadrats _a_ and _b_ is calculated as:
+$$J(a, b) = 1 - \frac{intersect_{ab}}{intersect_{ab} + exclusive_a + exclusive_b}$$
+
+
+
+### Plotting
+
+`plot` subcommand ingests [taskfile](./tasks/0-example-task.toml) to detect results of previous analyses
+and present them as graphs.
+
+Generated graphs will be saved to the same directory as
+analysis results.
+
+Example:
+```
+seal plot --taskfile ./tasks/0-example-task.toml
+```
+
+### Misc
+
+`misc` subcommand is a kitchen sink of opinionated
+convenience tools.
+
+## Development
+
+For unit tests run `python -m doctest ./src/seal/<file>`.
+
+For functional tests run `pytest`.
+
+### License
+The source code—including the tests and documentation—is licensed under [GPLv3](./LICENSE)
+
+`./datasets/data-bmd-sl.csv` is licensed under [CC-BY-SA-4.0](./datasets/LICENSE)
+
+[aopk-fish.csv](./datasets/aopk-fish.csv) was provided under [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/)
+by AOPK ČR, Nálezová databáze ochrany přírody, on-line database portal.nature.cz. Downloaded 2024-02-05.
```

