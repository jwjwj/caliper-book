#### Entity

__@type:__ [http://purl.imsglobal.org/caliper/v1/Entity](http://purl.imsglobal.org/caliper/v1/Entity)

__Description:__ a Caliper entity provides the minimal set of properties for representing an item in a learning graph. It is analogous to a schema.org [Thing](http://schema.org/Thing).  For an Entity to be linkable, dereferencing the Entity's @id should result in a representation of the node.

__Properties__

| Property | Type | Description | Conformance |
| :------- | :--- | :---------- | :---------- |
| @context | [xsd:string](https://www.w3.org/TR/xmlschema11-2/#string) | JSON-LD context represented by an IRI | required |
| @id | [xsd:string](https://www.w3.org/TR/xmlschema11-2/#string) | JSON-LD identifier represented as a globally-scoped IRI or a locally-scoped blank node | required |
| @type | [xsd:string](https://www.w3.org/TR/xmlschema11-2/#string) | JSON-LD type IRI | required |
| name | [xsd:string](https://www.w3.org/TR/xmlschema11-2/#string) | Analogous to http://schema.org/name |  optional |
| description | [xsd:string](https://www.w3.org/TR/xmlschema11-2/#string) | Analogous to  http://schema.org/description | optional |
| extensions | Map<[xsd:string](https://www.w3.org/TR/xmlschema11-2/#string), [xsd:string](https://www.w3.org/TR/xmlschema11-2/#string)> | &nbsp; | optional |
| dateCreated | [xsd:dateTime](https://www.w3.org/TR/xmlschema11-2/#dateTime) | &nbsp; | optional |
| dateModified | [xsd:dateTime](https://www.w3.org/TR/xmlschema11-2/#dateTime) | &nbsp; | optional |