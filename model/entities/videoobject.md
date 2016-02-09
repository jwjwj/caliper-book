### VideoObject

__subClassOf:__ [MediaObject](./mediaobject.md)

__Node type:__ {{ book.class.caliper.entity.VideoObject }}

__Comment:__ a Caliper VideoObject represents a visual recording stored in digital form. It is analogous to {{ book.class.sdo.VideoObject }}.

__Sample JSON-LD__

```JSONLD
{
  "@context": "http://purl.imsglobal.org/ctx/caliper/v1/Context",
  "@id": "https://example.com/super-media-tool/video/1225",
  "@type": "http://purl.imsglobal.org/caliper/v1/VideoObject",
  "name": "American Revolution - Key Figures Video",
  "alignedLearningObjective": [
    {
      "@id": "https://example.edu/american-revolution-101/personalities/learn",
      "@type": "http://purl.imsglobal.org/caliper/v1/LearningObjective",
      "dateCreated": "2015-08-01T06:00:00.000Z"
    }
  ],
  "duration": 1420,
  "dateCreated": "2015-08-01T06:00:00.000Z",
  "dateModified": "2015-09-02T11:30:00.000Z",
  "version": "1.0"
}
```