---
title:      'Template for Noise Extensions'
author:
 - First Author (first@email)
 - Second Author (second@email)
revision:   '1'
status:     'unofficial/unstable'
date:       '2017-11-12'
link-citations: 'true'
---

1. Introduction
================

This is a template document for writing Noise extension specifications.

This section should contain a few sentences describing the purpose of this extension.

2. Overview
============

This section should give a brief overview of how your extension works.

Introduce new terms in **bold**.  Use internal references such as [Section
1](#introduction).  Use bibliographic references such as [@hkdfpaper], [@kudla2005], [@rfc5869] that refer to bibtex entries in either the `spectools/*.bib` files or the local `my.bib` file.


3.  More sections
===================

Some guidelines:

 0. Use bullets, `inline code` for `variable names` and similar, and pre-formatted text blocks when needed.

 1. Follow the same style as the Noise Specification.

 2. To insert pagebreaks in the PDF document, use the LaTeX `\newpage` command like so:

\newpage

 3. Use Pandoc-specific features sparingly, but Pandoc has a few nice features:

     * Subscripts~1~ and superscripts^2^
     * Tables (see later)
     * Ability to control numbering of lists (e.g. this list starts at 0).

3.1. Subsections
-----------------
Add as needed.


4.  Even more sections
=======================

Pandoc tables are helpful for displaying patterns:

+---------------------------+--------------------------------+
|     NN():                 |        KN(s):                  |
|       -> e                |          -> s                  |
|       <- e, ee            |          ...                   |
|                           |          -> e                  |
|                           |          <- e, ee, se          |
+---------------------------+--------------------------------+
|     NK(rs):               |        KK(s, rs):              |
|       <- s                |          -> s                  |
|       ...                 |          <- s                  |
|       -> e, es            |          ...                   |
|       <- e, ee            |          -> e, es, ss          |
|                           |          <- e, ee, se          |
+---------------------------+--------------------------------+


5. Security considerations
===========================

You must list security considerations for using your extension, for example a bulleted list like so:

 * **Confidentiality**:  Some stuff.

 * **Integrity**:  Other stuff.
 

6. Rationales
=============

Not required, but might be a good idea to explain nonobvious design decisions.


7. IPR
========

This document is hereby placed in the public domain.

8. Acknowledgements
=====================

Make sure to acknowledge prior and related work, and others who contributed.

9.  References
================
