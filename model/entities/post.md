#### Post

__Description:__ a Post is an entry or message submitted to a Forum. A series of Posts may constitute a Thread if they share a common subject and are connected by a reply or by date relationships. It is analogous to an [sioc:Post](http://rfds.org/sioc/spec/#term_Post).

__Type IRI:__ [http://purl.imsglobal.org/caliper/v1/Post](http://purl.imsglobal.org/caliper/v1/Post)

__subClassOf:__ [AssignableDigitalResource](AssignableDigitalResource.md)

__Properties__

| Property | Type | Description | Conformance|
| :------- | :--- |  :---------- | :-------- |
| addressedTo | [Agent](entities/agent.md) | the agent, typically a person, to which this post is addressed | recommended |
| body | [xsd:string](https://www.w3.org/TR/xmlschema-2/#string) | plain-text rendering of the content of the post. | recommended |
| attachments | [Collection](entities/collection.md)<[DigitalResource](entities/digitalresource.md)> | an array of one or more Digital Resources | optional |
| ~~replyCount~~ | [~~xsd:nonNegativeInteger~~](https://www.w3.org/TR/xmlschema-2/#nonNegativeInteger) | ~~number of messages posted in reply to this message~~ | ~~optional~~ |
| ~~viewCount~~ | [~~xsd:nonNegativeInteger~~](https://www.w3.org/TR/xmlschema-2/#nonNegativeInteger) | ~~number of messages posted in reply to this message~~ | ~~optional~~ |
| wordCount | [xsd:nonNegativeInteger](https://www.w3.org/TR/xmlschema-2/#nonNegativeInteger) | number of words in message body | optional |

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