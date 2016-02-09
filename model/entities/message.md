### Message

__subClassOf:__ [AssignableDigitalResource](./AssignableDigitalResource.md)

__Node type:__ {{ book.class.caliper.entity.Message }}

__Comment:__ a Caliper Message is a digital form of written communication sent to a recipient. A series of Messages may constitute a [Thread](./thread.md) if they share a common subject and are connected by a reply or by date relationships. It is analogous to an {{ book.class.sioc.Post }}.

__Properties__

| Property | Type | Description | Conformance|
| -------- | ---- | ----------- | ---------- |
| addressedTo | [Agent](./agent.md) | An [Agent](./agent.md), typically a [Person](./person.md), to which this Message is addressed. | recommended |
| body | {{ book.dataType.xsd.string }} | Plain-text rendering of the content of the Message. | recommended |
| attachments | [Collection](entities/collection.md)<[DigitalResource](./digitalresource.md)> | An array of one or more [DigitalResources](./digitalresource.md). | optional |
| replyCount | {{ book.dataType.xsd.nonNegativeInteger }} | Number of messages posted in reply to this message. | optional |
| viewCount | {{ book.dataType.xsd.nonNegativeInteger }} | Number of views of this Message. | optional |
| wordCount | {{ book.dataType.xsd.nonNegativeInteger }} | Number of words in the Message body. | optional |

__Sample JSON-LD__

```JSONLD
{
  "@context": "http://purl.imsglobal.org/ctx/caliper/v1/Context",
  "@id": "https://example.edu/course/1/forum/2/topic/1/message/1",
  "@type": "http://purl.imsglobal.org/caliper/v1/Message",
  "addressedTo": {},
  "body": "I like Caliper.",
  "wordCount": 3, 
  "dateCreated": "2015-08-01T06:00:00.000Z"
}
```