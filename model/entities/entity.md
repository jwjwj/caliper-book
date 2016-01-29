#### Entity

__@type:__ [http://purl.imsglobal.org/caliper/v1/Entity](http://purl.imsglobal.org/caliper/v1/Entity)

__Description:__ a Caliper entity provides the minimal set of properties for representing an item in a learning graph. It is analogous to a schema.org [Thing](http://schema.org/Thing).  For an Entity to be linkable, dereferencing the Entity's @id should result in a representation of the node.

__Properties__

| Property | Type | Conformance | Description |
| -------- | ---- |  ----------- | ----------- |
| @context | String | required | JSON-LD context represented by an IRI |
| @id | String | required | Identifier of resource represented by an IRI |
| @type | String |  required | http://purl.imsglobal.org/caliper/v1/Entity |
| name | String |  optional | Analogous to http://schema.org/name |
| description | String |  optional | Analogous to  http://schema.org/description |
| extensions | Map<String, String> | optional | |
| dateCreated | DateTime | optional | Analogous to http://schema.org/dateCreated ([ISO 8601](https://en.wikipedia.org/wiki/ISO_8601#Combined_date_and_time_representations) format) |
| dateModified | DateTime | optional | Analogous to http://schema.org/dateModified ([ISO 8601](https://en.wikipedia.org/wiki/ISO_8601#Combined_date_and_time_representations) format) |