### DigitalResource

__subClassOf:__ [Entity](./entity.md)

__Node type:__ {{ book.class.caliper.entity.DigitalResource }}

__Comment:__ Represents a generic digital resource.  Analogous to schema.org's [CreativeWork](https://schema.org/CreativeWork).

__Properties__

| Property | Type | Description | Conformance |
| -------- | ---- | ----------- | ----------- |
| ~~objectType~~ | ~~[Collection](./collection.md)&lt;{{ book.dataType.xsd.string }}&gt;~~ | &nbsp;| deprecated |
| keywords | [Collection](./collection.md)&lt;{{ book.dataType.xsd.string }}&gt; | A short representation of the Entity in written form.  Analogous to {{ book.dataProperty.sdo.description }} | optional |
| alignedLearningObjective | [Collection](./collection.md)&lt;[LearningObjective](./learningobjective.md)&gt; | &nbsp; | optional |
| isPartOf | [DigitalResource](./digitalresource.md) | A related DigitalResource that includes or incorporates the described DigitalResource as a part of its whole.  Analogous to {{ book.dataProperty.sdo.isPartOf }} or {{ book.dataProperty.dcterms.isPartOf }}. | optional |
| datePublished | {{ book.dataType.xsd.dateTime }} | The date and time expressed with millisecond precision that represents the publication date of the DigitalResource (ISO 8601 format required).  Analogous to {{ book.dataProperty.sdo.datePublished }} | optional |
| version | {{ book.dataType.xsd.string }} | An identifier that designates the current form of the DigitalResource.  Analogous to {{ book.dataProperty.sdo.version }} | optional |

__Proposed Caliper 1.1 property additions__

| Property | Type | Description | Conformance |
| -------- | ---- | ----------- | ----------- |
| creator | [Agent](./agent.md) | The [Agent](./agent.md) responsible for bringing the described DigitalResource into being.  Analogous to {{ book.dataProperty.sdo.creator }} or {{ book.dataProperty.dcterms.creator }}. | optional |