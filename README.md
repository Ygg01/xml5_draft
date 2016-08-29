Draft for XML5 proposal.
==========

The original version of this proposal is hosted on [XML5 code repository](https://github.com/annevk/xml5).

What's XML5
==========

XML5 is simply put, a more relaxed version of XML syntax. Basically, take the best aspects of HTML(5) syntax and apply it to XML. What this means in practice is following:

   * DOCTYPE is simplified and optional. Also no known laughing bomb exploits.
   * Creates a detailed rules for state transitions, to simplify implementations.
   * Allows mixed content everywhere `<text>A <b>bold</b> new world</test>` becomes:  
```
    Tag('text')
     |
     +---Text('A ')
     |
     +---Tag('b')
     |    |
     |    +---Text('bold')
     |
     +---Text(' new world')
```
   * Writing one of escaped character inside tags automatically escapes them `<tag>Tom & Jerry</tag>` when parsed becomes:
```
    Tag('tag')
     |
     +---Text('Tom & Jerry')
```
   * XML comments are a lot more flexible (and a bit more difficult to parse), i.e. `--` is allowed in comments. Nested comments are prohibited.

What XML5 strive to do is, to drop all notion of well-formedness out of the window and replace it with HTML-like error handling. XML5 parser will be able to parse any XML 1.0 and XML 1.1 documents, but a valid XML5 document wouldn't be parseable by a XML 1.0 or even XML 1.1 parser.
Motivation behind this is to allow easier parsing of XML generated using string concatenation and used often on the web.

How to read this?
=================

Here is the [rendered version](https://ygg01.github.io/xml5_draft/).

Otherwise you can download and compile the source yourself

1. [Install bikeshed](https://github.com/tabatkins/bikeshed/blob/master/docs/install.md)
2. Clone the the repository ````$ git clone https://github.com/Ygg01/xml5_draft````
3. Change to xml5_draft the repository ````$ cd xml5_draft````
4. Run bikeshed ````$ bikeshed````
