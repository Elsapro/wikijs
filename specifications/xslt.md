<!-- TITLE: XSLT -->
<!-- SUBTITLE: A quick summary of XSLT -->

# XSLT
## XSLT 3.0
XSLT 3.0 is a Recommendation



### key features:

* Streaming

* Separately compiled packages

* Higher-order functions

* JSON, maps, and arrays

and of course lots of goodies like trigonometric functions, dynamic XPath evaluation, a string concatenation operator, text value templates, a random number generator, and a function chaining operator.

As a bonus, we thought you'd like an open-source implementation.

So Saxon 9.8 is released today, and the open source Saxon-HE version now includes core support for XSLT 3.0 with XPath 3.1.

There are lots of other new things in Saxon 9.8:

* just-in-time compilation to reduce the cost of loading vast stylesheets like DocBook and DITA when you're only using a fraction of the template rules

* hot-spot bytecode generation, again to put the compilation effort where it's needed

* optimization of template rule sets like those found in DITA where the matching is all on attribute values rather than element names

* a new approach to processing of DOM trees, which are now only twice as slow as Saxon's native TinyTree compared with 5-10 times slower the old way

* some experimental syntax enhancements to enrich the type system: tuple types, union types, and type aliases

* bytecode generation for validation of user-defined simple types in XSD

At the same time as moving foward to XSLT 3.0, we're dropping support for older versions of the specs, so you can no longer run in XQuery 1.0 or XSLT 2.0 mode, for example - your code should continue to work, because the specs have a high level of backwards compatibility. A particular decision that will affect some of you is that we're dropping XSLT 1.0 backwards compatibility mode from Saxon-HE, and hope to eliminate it entirely in due course.