### Session

__subClassOf:__ [Entity](./entity.md)

__Node type:__ {{ book.class.caliper.entity.Session }}

__Comment:__ a Caliper Session represents a Web application user session.  [SessionEvent](../events/sessionevent.md) log in actions generate a Session.  Log out actions treat the Session as the target of the interaction while in the case of a time out, the Session constitutes the object of the interaction. 

__Properties__

| Property | Type | Description | Conformance |
| -------- | ---- | ----------- | ----------- |
| actor | [Agent](./agent.md) | The [Agent](./agent.md) who establishes the Session.| required |
| startedAtTime | {{ book.dataType.xsd.dateTime }}  | The date and time expressed with millisecond precision that represents when a Session commenced (ISO 8601 format required).  Analogous to {{ book.dataProperty.provo.startedAtTime }}. | recommended |
| endedAtTime | {{ book.dataType.xsd.dateTime }} | The date and time expressed with millisecond precision that represents when a Session ended or was terminated (ISO 8601 format required).  Analogous to {{ book.dataProperty.provo.endedAtTime }} | recommended |
| duration | {{ book.dataType.xsd.string }} | The total interval of time required to complete the Attempt (ISO 8601 format required). | optional |

__Sample JSON-LD__

```JSONLD
{
    "@context": "http://purl.imsglobal.org/ctx/caliper/v1/Context",
    "@id": "https://example.com/viewer/session-123456789",
    "@type": "http://purl.imsglobal.org/caliper/v1/Session",
    "name": "session-123456789",
    "actor": {
        "@id": "https://example.edu/user/554433",
        "@type": "http://purl.imsglobal.org/caliper/v1/lis/Person",
        "dateCreated": "2015-08-01T06:00:00.000Z"
    },
    "dateCreated": "2015-09-15T10:15:00.000Z",
    "startedAtTime": "2015-09-15T10:15:00.000Z"
}
```