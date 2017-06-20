## Slots and Types

A slot is a data structure that holds a value within a
particular domain at any given time. Slots represent
abstract types and the values held at any given time represent instances
of the types, where the domain is the set of known instances of the type. Each possible value
is mutually exclusive with the rest, and the presence of one value
entails the absence of the others.

![Slot](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/docs/img/slot.png)

## Properties and Classes

Slots are applied when representing properties of an object. An instance of 
a class is an object whose properties are such that every
null property-type of the class is satisfied by an equivalent non-null
property of the instance. In other words, a set of slots defining the
properties of a class (which may or may not contain default values) are completed 
by an object if the class is instantiated by the object.

Given that a class is defined by a partially-filled set of slots and an
object is defined by a sufficiently-filled set of slots, the union set 
between a class and an object is complete if and only if the object
fills all null-slots contained within the class.

Slots are useful when representing prototypes of a class as well. A
prototype is a partially-filled set of slots, the non-null properties
being derived from repeated instantiation, and those particular combinations
being generalized over a set a observations. A class is not defined by one
prototype, but by multiple prototypes distinguishing between common
variations of a class.

![Hierarchy](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/docs/img/datatypes.png)

## Objects and Relations

Relations represent contrasts of objects in terms of property deltas over space and time. 
Spatial difference refers to property deltas of objects in a set, while temporal difference
refers to property deltas of the same object as it changes over time.

![Relations](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/docs/img/Relations.PNG)

References to structures like “object” and “set” are relative. An object may very well
be considered a set of properties, while at the same time a property
is an object in and of itself.This recursive functionality is complimented
by the hierarchical structure of data within the system.
