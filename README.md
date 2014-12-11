Draft for XML5 proposal.
==========

The original version of this proposal is hosted on [XML5 Google code repository](https://code.google.com/p/xml5/).

What's XML5 
==========

XML5 is simply put, a more relaxed version of XML syntax. Basically, take the best aspects of HTML(5) syntax and apply it to XML.
And no, I don't mean [quirks mode](https://developer.mozilla.org/en-US/docs/Quirks_Mode_and_Standards_Mode) or the [adoption agency algorithm](https://html.spec.whatwg.org/#adoptionAgency).
Also dealing with Doctype in a way that doesn't cause horrible security exploits.

What XML5 strive to do is, to drop all notion of well-formedness out of the window and replace it with HTML-like error handling. XML5 parser will be able to parse any XML 1.0 and XML 1.1 documents, but a valid XML5 document wouldn't be parsable by a XML 1.0.
Motivation behind this is to allow easier parsing of XML generated using string concatenation.

How to read this?
=================

Hopefully a link to rendered version will be up sooner or later, but in case it isn't you can compile resources yourself:

1. [Install bikeshed](https://github.com/tabatkins/bikeshed/blob/master/docs/install.md)
2. Clone the the repository ````$ git clone https://github.com/Ygg01/xml5_draft````
3. TODO


