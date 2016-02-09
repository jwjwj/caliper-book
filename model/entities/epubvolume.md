### ePubVolume

__subClassOf:__ [DigitalResource](./digitalresource.md)

__Node type:__ {{ book.class.caliper.entity.ePubVolume }}

__Comment:__ a Caliper ePubVolume is analogous to a {{ book.class.idpf.ePubVolume }} and represents an item in a collection of related ePub resources.

__Sample JSON-LD__

```JSONLD
{
  "@context": "http://purl.imsglobal.org/ctx/caliper/v1/Context",
  "@id": "https://example.com/viewer/book/34843#epubcfi(/4/3)",
  "@type": "http://www.idpf.org/epub/vocab/structure/#volume",
  "name": "The American Revolution, 1763-1789",
  "dateCreated": "2015-08-01T06:00:00.000Z",
  "dateModified": "2015-09-02T11:30:00.000Z",
  "version": "2nd ed."
}
```