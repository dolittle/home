---
title: Naming
description: Learn about how Doolittle's naming conventions
keywords: General
author: einari
weight: 3
---

One of the most important aspects of maintainable code is readability.
Being able to identify what something does just by reading the name.
This applies to files, type names, functions / methods - all the way through.

## Abbreviations

You should not use abbreviations, unless they are well known and understood abbreviations,
such as `XML` or `JSON` or similar.

## Prefix / postfix

Having prefixes or postfixes to type names is often considered a code-smell.
It can be an indication that the name alone is not saying what it is actually doing.
There is no reason to add the technical concern as a pre-/postfix.
Examples of pre-/postfixes you should avoid:

* Controller
* ViewModel
* Exception

Make the naming of unambiguous instead.

## Upper CamelCase vs lower camelCase

All C# code consistently uses upper CamelCase - also called Pascal Case.
While all JavaScript is consistently using lower camelCase - with the exception of
types that can be instantiated. These have upper CamelCase. This last convention is
a convention that is common in the JavaScript space.

Going between the two worlds, Dolittle makes sure to translate everything.
During serialization for instance, translation is done for naming - both ways - making
it feel natural to a C# developer as well as a JavaScript developer.