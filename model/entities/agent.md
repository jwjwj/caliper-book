### Agent

__subClassOf:__ [Entity](./entity.md)

__Node type:__ {{ book.class.caliper.entity.Agent }}

__Comment:__ a Caliper Agent represents an [Entity](./entity.md) that can initiate or perform an [Action](../actions.md).  It is analogous to a {{ book.class.foaf.Agent }}.  Agent is considered a generic class that lacks the type specificity rendered explicit in its several subclasses.  It is *recommended* that only subclasses of Agent be used to represent a Caliper [Event](../events/event.md) actor.

__Subclasses:__ [Person](./person.md), [Organization](./organization.md) and [SoftwareApplication](./softwareapplication.md)