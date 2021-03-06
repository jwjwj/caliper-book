### ePubPart

__subClassOf:__ [DigitalResource](./digitalresource.md)

__Node type:__ {{ book.class.caliper.entity.ePubPart }}

__Comment:__ a Caliper ePubPart is analogous to a {{ book.class.idpf.ePubPart }} and represents a major structural division within a piece of written content, typically encapsulating a set of related [ePubChapters](./epubchapter.md).

__Sample JSON-LD__

```JSONLD
{
  "@context": "http://purl.imsglobal.org/ctx/caliper/v1/Context",
  "@id": "https://example.com/viewer/book/34843#epubcfi(/4/3/1)",
  "@type": "http://www.idpf.org/epub/vocab/structure/#part",
  "name": "Part One",
  "dateCreated": "2015-08-01T06:00:00.000Z",
  "dateModified": "2015-09-02T11:30:00.000Z",
  "isPartOf": {
    "@id": "https://example.com/viewer/book/34843#epubcfi(/4/3)",
    "@type": "http://www.idpf.org/epub/vocab/structure/#volume",
    "name": "The American Revolution, 1763-1789",
    "dateCreated": "2015-08-01T06:00:00.000Z",
    "dateModified": "2015-09-02T11:30:00.000Z",
    "version": "2nd ed."
  }
}
```