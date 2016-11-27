**holocene** is a way of organizing a bunch of documents that could become
a static/dynamic content management system, provided I write the actual code.

Documents are nodes in a tree. Nodes have attributes.

The tree can have multiple representations, some isomorphic (e.g. files on 
disk ↔ in-memory representation ↔ database), some not (e.g. in-memory 
representation → HTML files).

The tree is mapped to an URL space (see [On short URLs][] for some related 
thoughts). This mapping should probably be one-to-one; many-to-one is more
flexible, but requires extra choices (e.g how do you represent multiple nodes
with the same URL?). 

Goals:

* finish something; files on disk → HTML files at a minimum
* write as little code as possible (libraries are OK)

In scope:

* node types
* node ordering
* inline references to other notes
* (later) resources (node attributes that are not part of the tree)
* (later) error pages
* (later) live preview
* (later) Atom/RSS
* (later) sitemap
* (later) image handling
* (later) full-text search

Out of scope:

* versioning (it is representation specific, e.g. git for files on disk)
* web UI (files on disk should be enough)
* internationalization



[On short URLs]: https://qntm.org/urls
