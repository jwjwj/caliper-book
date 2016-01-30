#### Post

__@type:__ {{ book.entity_post }}

__Description:__ a Post is an entry or message submitted to a Forum. A series of Posts may constitute a Thread if they share a common subject and are connected by a reply or by date relationships. It is analogous to an [sioc:Post](http://rfds.org/sioc/spec/#term_Post).

__subClassOf:__ [AssignableDigitalResource](AssignableDigitalResource.md)

__Properties__

| Property | Type | Description | Conformance|
| :------- | :--- |  :---------- | :-------- |
| addressedTo | [Agent](entities/agent.md) | An [Agent](entities/agent.md), typically a [Person](./person.md), to which this post is addressed. | recommended |
| body | {{ book.datatype_string }} | Plain-text rendering of the content of the post. | recommended |
| attachments | [Collection](entities/collection.md)<[DigitalResource](entities/digitalresource.md)> | An array of one or more [DigitalResources](entities/digitalresource.md). | optional |
| replyCount | {{ book.datatype_nonNegativeInteger }} | Number of messages posted in reply to this message. | optional |
| viewCount | {{ book.datatype_nonNegativeInteger }} | Number of views of this {{ book.entity_post }}. | optional |
| wordCount | {{ book.datatype_nonNegativeInteger }} | Number of words in message body. | optional |

__Sample JSON__

```JSONLD
{
  "@context": "http://purl.imsglobal.org/ctx/caliper/v1/Context",
  "@id": "https://example.edu/course/1/forum/2/topic/1/post/1",
  "@type": "http://purl.imsglobal.org/caliper/v1/Post",
  "addressedTo": {},
  "body": "I like Caliper.",
  "wordCount": 3, 
  "dateCreated": "2015-08-01T06:00:00.000Z"
}
```