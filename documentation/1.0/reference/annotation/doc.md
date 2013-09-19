---
layout: reference
title: '`doc` annotation'
tab: documentation
unique_id: docspage
author: Tom Bentley
doc_root: ../../..
---

# #{page.title}

The `doc` annotation adds documentation to a declaration.

## Usage

Explict `doc` annotation:

<!-- try: -->
    doc("Some documentation")
    void example(){
    }

Implict use of `doc` via the "anonymous annotation":

<!-- try: -->
    "More documentation"
    void furtherExample() {
    }

## Description

The `doc` annotation is processed by the 
[`ceylon doc`](#{site.urls.ceylon_tool_current}/ceylon-doc.html) tool, 
which assumes it contains [Markdown formatted](../markdown/) text.

### Anonymous annotation

As shown above, the annotation can be used in two forms, 

* explicit invocation of `doc`, or
* as a string literal, when it is the first annotation 
  in the list of annotations of the declaration

The anonymous form is preferred.

## See also

* [`doc`](#{site.urls.apidoc_current}/index.html#doc)
* Reference for [annotations in general](../../structure/annotation/)
