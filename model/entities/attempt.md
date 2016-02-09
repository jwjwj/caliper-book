### Attempt

__subClassOf:__ [Entity](./entity.md)

__Node type:__ {{ book.class.caliper.entity.Attempt }}

__Comment:__ a Caliper Attempt provides a count of the number of times an [Agent](./agent.md) interacts with an [AssignableDigitalResource](./assignabledigitalresource.md).  Attempts are generated as the result of an action such as starting an [Assessment](./assessment.md). In the case of an [OutcomeEvent](../events/outcomeevent.md) graded action, the Attempt constitutes the object of the interaction. 

__Properties__

| Property | Type | Description | Conformance |
| -------- | ---- | ----------- | ----------- |
| assignable | [DigitalResource](./digitalresource.md) | The [DigitalResource](./digitalresource.md) that is the target of the Attempt. | required |
| actor | [Agent](./agent.md) | The [Agent](./agent.md) who initiates the Attempt.| required |
| count | {{ book.dataType.xsd.nonNegativeInteger }} | The total number of attempts inclusive of the current Attempt that have been registered against the assigned resource. | required |
| startedAtTime | {{ book.dataType.xsd.dateTime }}  | The date and time expressed with millisecond precision that represents when an Attempt commenced (ISO 8601 format required).  Analogous to {{ book.dataProperty.provo.startedAtTime }}. | recommended |
| endedAtTime | {{ book.dataType.xsd.dateTime }} | The date and time expressed with millisecond precision that represents when an Attempt was completed or terminated (ISO 8601 format required).  Analogous to {{ book.dataProperty.provo.endedAtTime }} | optional |
| duration | {{ book.dataType.xsd.string }} | The total interval required to complete the Attempt (ISO 8601 format required). | optional |

__Sample JSON-LD__

```JSONLD
{
  "@context": "http://purl.imsglobal.org/ctx/caliper/v1/Context",
  "@id": "https://example.edu/politicalScience/2015/american-revolution-101/assessment/001/attempt/5678",
  "@type": "http://purl.imsglobal.org/caliper/v1/Attempt",
  "actor": "https://example.edu/user/554433",
  "assignable": "https://example.edu/politicalScience/2015/american-revolution-101/assessment/001",
  "count": 1,
  "dateCreated": "2015-08-01T06:00:00.000Z",
  "startedAtTime": "2015-09-15T10:15:00.000Z"
}
```