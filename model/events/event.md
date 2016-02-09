#### Event

__Node type:__ {{ book.class.caliper.event.Event }}

__Comment:__ a Caliper Event . . . . For enhanced specificity utilize the many subclasses of Event when constructing an Event rather than instantiating instances of the Event class itself.

__Properties__

| Property | Type | Description | Conformance |
| -------- | ---- | ----------- | ----------- |
| @context | {{ book.dataType.xsd.string }} | JSON-LD context represented by a globally-scoped IRI. | required |
| @type | {{ book.dataType.xsd.string }} | JSON-LD type represented as a globally-scoped IRI. | required |
| actor | [Agent](../entities/agent.md) | The Agent who initiated the event, typically a [Person](../entities/person.md), [Organization](../entities/organization.md) or [Software Application](../entities/softwareapplication.md). | required |
| action | {{ book.dataType.xsd.string }} | . . . | optional |
| object | [Entity](../entities/entity.md) | . . . | required |
| eventTime | {{ book.dataType.xsd.dateTime }}  | The date and time expressed with millisecond precision and formatted per ISO 8601 that represents when the Event was generated. | required |
| target | [Entity](../entities/entity.md) | . . . | optional |
| generated | [Entity](../entities/entity.md) | . . . | optional |
| edApp | [Software Application](../entities/softwareapplication.md) | . . . | optional |
| group | [Organization](../entities/organization.md) | . . . | optional |
| membership | [Membership](../entities/membership.md) | . . . | optional |
| session | [Session](../entities/session.md) | . . . | optional |