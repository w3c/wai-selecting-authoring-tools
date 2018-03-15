---
layout: default
title: "Selecting and Using Authoring Tools for Web Accessibility"
permalink: /design-develop/authoring-tools/selecting/
footer: >
---

{::options toc_levels="2" /}

{::nomarkdown}
{% include_cached toc.html type="start" title="Page Contents" class="full" %}
{:/}

-   TOC is created automatically.
{:toc}

{::nomarkdown}
{% include_cached toc.html type="end" %}
{:/}

## Introduction

As of the last revision of this document, we were unaware of any single
authoring tool that fully supports production of accessible websites.
Some developers are improving the support of accessibility in their
authoring tools, and some utilities may help supplement gaps in existing
authoring tools.

This document provides information which may help find improved
authoring tools and/or work around the gaps in existing authoring tools.
It includes questions to ask software vendors regarding accessibility
support in current and upcoming product versions according to their
conformance with W3C's [Authoring Tool Accessibility Guidelines
(ATAG)](http://www.w3.org/WAI/intro/atag.php).

ATAG addresses all kinds of authoring tools, including content
management systems (CMS), WYSIWYG ("What You See Is What You Get")
tools, save-as-HTML conversion tools such as word processors,
database-generation tools, site management tools, etc. ATAG has a
companion set of techniques to help software developers implement ATAG
in their products. ATAG explains to authoring tool developers how to
make their products:

1.  support accessible authoring practices;
2.  generate standard markup;
3.  support the creation of accessible content;
4.  provide ways of checking and correcting inaccessible content;
5.  integrate accessibility support into the overall look and feel of
    the product;
6.  promote accessibility in help and documentation; and
7.  ensure that the tool is accessible to authors with disabilities.

## Checklists for Authoring Tool Selection {#venqu}

### Evaluating software currently in use by an organization:

-   Do authoring tools currently in use support or hinder the production
    of accessible websites? Be sure to broadly consider content
    management systems (CMS), WYSIWYG ("What You See Is What You Get")
    HTML editors; conversion tools such as word processors or
    presentation software with "save as HTML" buttons; applications that
    generate web pages from databases; image editors; multimedia
    editors; site management tools, etc.
-   Do authoring tools currently in use change or remove accessibility
    information (for instance, alternative text for images) that has
    been added by other tools or by hand mark-up?
-   For authoring tools that do not support the creation of accessible
    content, are there plug-ins or other utilities that can be used with
    those products to better support the production of accessible
    websites?

### Selecting new or replacement software:

-   Which applications are more conformant with ATAG?
-   For which applications are there plug-ins that fill gaps in
    accessibility support for the primary product?
-   Which applications carry a developer's commitment to continue to
    improve ATAG conformance in future versions?

### Reviewing software procurement practices:

-   Do procurement policies within the organization encourage or require
    purchase of applications with more advanced support for
    accessibility?
-   For organizations with a concentration of purchasing power, is there
    an avenue through which to communicate the organization's interest
    in ATAG-conformant software to vendors, so that they are aware of
    the demand for these features?

### Questioning software vendors about product support:

-   Does the product conform to W3C's [Authoring Tool Accessibility
    Guidelines (ATAG)](http://www.w3.org/WAI/intro/atag.php)?
-   If not, when does the company plan to release a conformant version?
-   Can the vendor demonstrate the existing accessibility support in
    their product(s)?
-   Are there plug-ins that can be used with their product(s) to more
    effectively support creation of accessible websites?
-   Can a suite of tools be established to provide the accessibility
    that the specific authoring tool lacks?
-   (In countries where there are government requirements for web
    accessibility) What features has the company added to their
    product(s) to support web accessibility requirements?
-   Who would be a good contact person in the company for more
    information concerning products' accessibility?

## Working around Limitations of Existing Authoring Tools {#limitations}

Until authoring tools that more fully conform to ATAG are available, it
is helpful to develop strategies to work around the limitations of
existing tools. Steps to developing such strategies include:

-   become familiar with the general concepts (at the guideline level,
    not necessarily the individual success criteria/checkpoints) in Web
    Content Accessibility Guidelines (WCAG) and ATAG;
-   identify key limitations of authoring tools currently in use within
    an organization (by noting recurring problems in inaccessible output
    from those authoring tools; reading accessibility reviews of the
    products(s); noting feature support of ATAG success
    criteria/checkpoints; etc.);
-   locate plug-ins or utilities which can be used in combination with a
    given authoring tool to correct inaccessible output;
-   develop an in-house process or checklist for correcting
    accessibility problems generated by these tools.

### Examples of strategies to work around limitations of existing authoring tools:

**Note:** ATAG 1.0 was the completed version when this document was
published. To get updated information on later versions of ATAG, see the
[ATAG Overview](http://www.w3.org/WAI/intro/atag.php).

1.  If the templates provided with an authoring tool do not conform to
    WCAG \[[ATAG 1.0 Checkpoint
    1.4](/TR/ATAG10/atag10.html#check-use-accessible-templates)\],
    develop WCAG-conformant templates appropriate to your organization's
    needs, and distribute throughout the organization.
2.  If an authoring tool does not create valid markup \[[ATAG 1.0
    Checkpoint 2.2](/TR/ATAG10/atag10.html#check-ensure-published-DTD)\]
    according to a published Document Type Definition (DTD), use it in
    conjunction with a clean-up tool such as [HTML
    Tidy](/People/Raggett/tidy/).
3.  If a multimedia authoring tool does not support the creation of
    captions for audio \[[ATAG 1.0 Checkpoint
    1.1](/TR/ATAG10/atag10.html#check-support-access-features)\], use it
    in conjunction a caption editor such as
    [Magpie](http://ncam.wgbh.org/webaccess/magpie/).
4.  For authoring systems primarily designed to produce print media (for
    example, Acrobat, PageMaker, Quark Express), rich media (Director,
    Flash, ToolBook), word processing (Word, Word Perfect),
    presentations (PowerPoint, Freelance, Visio), go back to the
    original source material where possible and generate an accessible
    HTML or XHTML version from the source; or run file through a
    converter if available then check the accuracy of the conversion; or
    recreate the materials in a known accessible format; then also post
    the accessible format on the site \[[ATAG 1.0 Checkpoint
    2.1](/TR/ATAG10/atag10.html#check-prefer-w3c)\].
5.  If an authoring tool being used to retrofit an existing site doesn't
    prompt for missing alternative text \[[ATAG 1.0 Checkpoint
    3.1](/TR/ATAG10/atag10.html#check-provide-missing-alt)\], use an
    accessibility-retrofitting tool that both prompts for missing
    accessibility information and provides a means to insert the missing
    information.
6.  If an authoring tool does not insert a Document Type Declaration
    (DTD) (necessary for validation of markup, and for conformant HTML,
    XHTML, etc.) [\[ATAG 1.0 Checkpoint
    2.2\]](/TR/ATAG10/atag10.html#check-ensure-published-DTD), look for
    an extension which inserts the appropriate DTD, or insert the DTD by
    hand.
7.  If an authoring tool does not support cascading style sheets \[[ATAG
    1.0 Checkpoint
    3.2](/TR/ATAG10/atag10.html#check-help-provide-structure) & [ATAG
    1.0 Checkpoint
    4.5](/TR/ATAG10/atag10.html#check-allow-transformation)\], use it in
    conjunction with a compatible style sheet editor.
8.  If an authoring tool does not display a linearized version of tables
    \[[ATAG 1.0 Checkpoint
    3.2](/TR/ATAG10-TECHS/#check-help-provide-structure)\], use it in
    conjunction with [Lynx](http://lynx.browser.org/) or
    [Lynx-me](http://ugweb.cs.ualberta.ca/%7Egerald/lynx-me.cgi), or
    some [other text browser](/WAI/References/Browsing) or [text browser
    emulator](/WAI/ER/existingtools.html#Filter).
9.  If an authoring tool does not preserve all accessibility information
    during authoring, transformations, and conversions \[[ATAG 1.0
    Checkpoint
    1.2](/TR/ATAG10/atag10.html#check-leave-access-content)\], either
    edit by hand and save straight to source, or get a new authoring
    tool.
10. If an authoring tool automatically generates equivalent alternatives
    \[[ATAG 1.0 Checkpoint
    1.3](/TR/ATAG10/atag10.html#check-generate-access-markup)\], e.g. by
    inserting file name as alternative text, turn off that function, or
    manually check and correct all alternative text.

## Product Reviews {#prodrev}

The [Authoring Tool Accessibility Guidelines Working Group](/WAI/AU/)
(AUWG) previously [reviewed authoring tools](/WAI/AU/2002/tools) for
conformance with ATAG. As of the last revision of this document, the
reviews were not up-to-date and therefore may not represent the latest
progress in ATAG conformance. In the future, the AUWG may update product
reviews on a collaborative basis with developers; assistance and
feedback on reviews is helpful.

In some cases developers have information on their own sites describing
the degree of accessibility support in their products. Developers'
accessibility pages may contain links to plug-ins which enhance the
capability of an authoring tool to support the production of accessible
web content.