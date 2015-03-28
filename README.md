Draft for XML5 proposal.
==========

The original version of this proposal is hosted on [XML5 code repository](https://github.com/annevk/xml5).

What's XML5
==========

XML5 is simply put, a more relaxed version of XML syntax. Basically, take the best aspects of HTML(5) syntax and apply it to XML.
And no, I don't mean [quirks mode](https://developer.mozilla.org/en-US/docs/Quirks_Mode_and_Standards_Mode) or the [adoption agency algorithm](https://html.spec.whatwg.org/#adoptionAgency).
Also dealing with Doctype in a way that doesn't cause horrible security exploits.

What XML5 strive to do is, to drop all notion of well-formedness out of the window and replace it with HTML-like error handling. XML5 parser will be able to parse any XML 1.0 and XML 1.1 documents, but a valid XML5 document wouldn't be parsable by a XML 1.0 or even XML 1.1 parser.
Motivation behind this is to allow easier parsing of XML generated using string concatenation and used often on the web.

How to read this?
=================

Here is the [rendered version](http://ygg01.github.io/xml5_draft/).

Otherwise you can download and compile he source sourself

1. [Install bikeshed](https://github.com/tabatkins/bikeshed/blob/master/docs/install.md)
2. Clone the the repository ````$ git clone https://github.com/Ygg01/xml5_draft````
3. Change to xml5_draft the repository ````$ cd xml5_draft````
4. Run bikeshed ````$ bikeshed````


