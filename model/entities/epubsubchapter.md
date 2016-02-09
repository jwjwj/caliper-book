### ePubSubChapter

__subClassOf:__ [DigitalResource](./digitalresource.md)

__Node type:__ {{ book.class.caliper.entity.ePubSubChapter }}

__Comment:__ a Caliper ePubSubChapter is analogous to a {{ book.class.idpf.ePubSubChapter }} and represents a major division within an [ePubChapter](./epubchapter.md).

__Sample JSON-LD__

```JSONLD
{
  "@context": "http://purl.imsglobal.org/ctx/caliper/v1/Context",
  "@id": "https://example.com/viewer/book/34843#epubcfi(/4/3/1/1/1)",
  "@type": "http://www.idpf.org/epub/vocab/structure/#subchapter",
  "name": "The Grenville Administration and Taxing the Colonies",
  "dateCreated": "2015-08-01T06:00:00.000Z",
  "dateModified": "2015-09-02T11:30:00.000Z",
  "isPartOf": { 
    "@context": "http://purl.imsglobal.org/ctx/caliper/v1/Context",
    "@id": "https://example.com/viewer/book/34843#epubcfi(/4/3/1/1)",
    "@type": "http://www.idpf.org/epub/vocab/structure/#chapter",
    "name": "The Stamp Act Crisis",
    "dateCreated": "2015-08-01T06:00:00.000Z",
    "dateModified": "2015-09-02T11:30:00.000Z",
    "isPartOf": {
      "@context": "http: //purl.imsglobal.org/ctx/caliper/v1/Context",
      "@id": "https: //example.com/viewer/book/34843#epubcfi(/4/3/1)",
      "@type": "http: //www.idpf.org/epub/vocab/structure/#part",
      "name": "Part One",
      "dateCreated": "2015-08-01T06:00:00.000Z",
      "dateModified": "2015-09-02T11:30:00.000Z",
      "isPartOf": {
        "@id": "https: //example.com/viewer/book/34843#epubcfi(/4/3)",
        "@type": "http: //www.idpf.org/epub/vocab/structure/#volume",
        "name": "The American Revolution, 1763-1789",
        "dateCreated": "2015-08-01T06:00:00.000Z",
        "dateModified": "2015-09-02T11:30:00.000Z",
        "version": "2nd ed."
      }
    }
  }
}
```