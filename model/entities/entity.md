#### Entity

__@type:__ [http://purl.imsglobal.org/caliper/v1/Entity](http://purl.imsglobal.org/caliper/v1/Entity)

__Description:__ a Caliper Entity provides the minimal set of properties for representing a node in a learning graph. It is analogous to an [sdo:Thing](http://schema.org/Thing).  Dereferencing the Entity's IRI ```@id``` should provide a representation of the node.  For enhanced specificity utilize the many subclasses of Entity when constructing an [Event](../events/event.md) rather than instances of the Entity class itself.

__Properties__

| Property | Type | Description | Conformance |
| :------- | :--- | :---------- | :---------- |
| @context | {{ book.datatype_string }} | JSON-LD context represented by a globally-scoped IRI. | required |
| @id | {{ book.datatype_string }} | JSON-LD identifier represented as a globally-scoped IRI or a locally-scoped blank node. | required |
| @type | {{ book.datatype_string }} | JSON-LD type represented as a globally-scoped IRI. | required |
| name | {{ book.datatype_string }} | A word or phrase by which the Entity is known.  Analogous to [sdo:name](http://schema.org/name). | optional |
| description | {{ book.datatype_string }} | A short representation of the Entity in written form.  Analogous to [sdo:description](http://schema.org/description). | optional |
| extensions | Map<{{ book.datatype_string }}, {{ book.datatype_string }}> | &nbsp; | optional |
| dateCreated | {{ book.datatype_dateTime }}  | The date and time expressed with millisecond precision and formatted per ISO 8601 that represents when the Entity was created or added to a data set.  Analogous to [sdo:dateCreated](http://schema.org/dateCreated). | optional |
| dateModified | {{ book.datatype_dateTime }} | The date and time expressed with millisecond precision and formatted per ISO 8601 that represents when the Entity was last modified.  Analogous to [sdo:dateModified](http://schema.org/dateModified). | optional |