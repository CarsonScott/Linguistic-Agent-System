## Slots and Types

A slot is a data structure that holds an equivalent value to a
particular element in a domain set at any given time. Slots represent
abstract types and the values held at any given time represent instances
of types, where the domain set is a set of known instances of a type,
and thus a set of states that are known to be possible for a given type.

For all possible values that a slot may hold, an equivalent value is
held by a specific element in the domain. Therefore, each possible value
is mutually exclusive with the rest, and the presence of one value
entails the absence of the others.

![Slot](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/docs/img/slot.png)

## Properties and Classes

Slots are applied when representing properties of an object, given that
an instance of a class is an object whose properties are such that every
null property-type of the class is satisfied by an equivalent non-null
property of the instance. In other words, a set of slots defining the
properties of a class, which may or may not contain a default value, are
satisfied if and only if they are completed by an object considered to
be an instance of that class.

Given that a class is defined by a partially-filled set of slots and an
object is defined by a sufficiently-filled set of slots, the union set
of slots between a class and an object is considered satisfied if and
only if the object is an instance of the class and therefore completes
(or fills) the remaining slots.

Slots are useful when representing prototypes of a class, where a
prototype is a partially-filled set of slots with non-null properties
derived from repeated instantiation, in which the properties of an
instance tend to gravitate toward distinguishable combinations of
values, and those particular combinations are generalized by a finite
collection of prototypes. Therefore a class is not defined by a single
prototype, but by multiple prototypes that distinguish between common
variations of a class.

![Hierarchy](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/docs/img/datatypes.png)
