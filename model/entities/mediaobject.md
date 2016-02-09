### MediaObject

__subClassOf:__ [DigitalResource](./digitalresource.md)

__Node type:__ {{ book.class.caliper.entity.MediaObject }}

__Comment:__ a Caliper MediaObject represents a generic piece of media content analogous to {{ book.class.sdo.MediaObject }}.  Since MediaObject lacks type specificity it is *recommended* that only its subclasses be employed to represent nodes in the learning graph.

__Properties__

| Property | Type | Description | Conformance |
| -------- | ---- | ----------- | ----------- |
| duration | {{ book.dataType.xsd.long }} | The length of time to completion.  Analogous to {{ book.dataProperty.sdo.duration }}.  | optional |

__Subclasses:__ [AudioObject](./audionobject.md), [ImageObject](./imageobject.md) and [VideoObject](./videoobject.md)  