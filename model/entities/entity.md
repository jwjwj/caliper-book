### Entity

__Node type:__ {{ book.class.caliper.entity.Entity }}

__Comment:__ a Caliper Entity represents a generic class that lacks the type specificity rendered explicit in its several subclasses.  It is analogous to an {{ book.class.sdo.Thing }}.  It is *recommended* that only subclasses of Entity be employed to represent nodes in the learning graph.  Caliper entities should be provisioned with a globally-scoped, dereferenceable IRI in order to ensure that Caliper [Event](../events/event.md) data can be linked and shared across contexts.  In cases where an IRI is inappropriate, an Entity can be assigned a blank node identifier.

__Properties__

| Property | Type | Description | Conformance |
| :------- | :--- | :---------- | :---------- |
| @context | {{ book.dataType.xsd.string }} | JSON-LD context represented by a globally-scoped IRI. | required |
| @id | {{ book.dataType.xsd.string }} | JSON-LD identifier represented as a globally-scoped IRI or a locally-scoped blank node identifier. | required |
| @type | {{ book.dataType.xsd.string }} | JSON-LD type represented as a globally-scoped IRI. | required |
| name | {{ book.dataType.xsd.string }} | A word or phrase by which the Entity is known.  Analogous to {{ book.dataProperty.sdo.name }} | optional |
| description | {{ book.dataType.xsd.string }} | A short representation of the Entity in written form.  Analogous to {{ book.dataProperty.sdo.description }} | optional |
| extensions | Map&lt;{{ book.dataType.xsd.string }}, {{ book.dataType.xsd.string }}&gt;   | &nbsp; | optional |
| dateCreated | {{ book.dataType.xsd.dateTime }}  | The date and time expressed with millisecond precision that represents when the Entity was created or added to a data set (ISO 8601 format required).  Analogous to {{ book.dataProperty.sdo.dateCreated }}. | optional |
| dateModified | {{ book.dataType.xsd.dateTime }} | The date and time expressed with millisecond precision that represents when the Entity was last modified (ISO 8601 format required).  Analogous to {{ book.dataProperty.sdo.dateModified }} | optional |