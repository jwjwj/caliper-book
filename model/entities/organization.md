### Organization

__subClassOf:__ [Agent](./agent.md)

__Node type:__ {{ book.class.caliper.entity.Organization }}

__Comment:__ a Caliper Organization represents a group of people organized into a community or other social, commercial, educational or political structure.  The group has a common purpose or reason for existence that spans beyond the set of people belonging to it and can act as an [Agent](./agent.md). Organizations are often decomposable into hierarchical structures.  It is analogous to a {{book.class.org.Organization }}.

__Properties__

| Property | Type | Description | Conformance |
| -------- | ---- | ----------- | ----------- |
| subOrganizationOf | [Organization](./organization.md) | The Organization's parent Organization. | optional |

__Sample JSON-LD__

```JSONLD
{
  "@context": "http://purl.imsglobal.org/ctx/caliper/v1/Context",
  "@id": "https://example.edu/colleges/1/departments/2",
  "@type": "http://purl.imsglobal.org/caliper/v1/w3c/Organization",
  "name": "Department of History",
  "subOrganizationOf": {
    "@context": "http://purl.imsglobal.org/ctx/caliper/v1/Context",
    "@id": "https://example.edu/colleges/1",
    "@type": "http://purl.imsglobal.org/caliper/v1/w3c/Organization",
    "name": "College of Social Science"
  }
}
```