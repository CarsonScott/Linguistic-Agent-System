# Emergence of Linguistic Capacity in Evolving Multi-Agent Systems
The following paper describes a theoretical model of language acquisition, comprehension, and production using a distributed multi-agent system. The system is composed of a society of agents who communicate by sending and receiving phonological signals across a social network. Every individual agent contains an internal system of subagents that are specialized to each perform a small number of tasks which collectively make up the cognitive process.   

## Description
The initial subagent is called a recognition agent and is responsible for receiving input patterns from the environment and extracting  semantic representations, called words, of the observed patterns. Every time step the agent produces a set of words that were detected from the input and places them into a temporary storage-unit called a queue.

The next subagent is called a construction agent and is responsive for observing a sequence of words from the queue and creating hierarchical diagrams, called trees, of the observed sequences. Every time steps the agent selects a set of operators that were determined by the contents of the queue with respect to the current state of the tree and applies them to the tree in order to add, remove, or change certain properties that define its structure.

![Agent](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Agent.png)

## Recognition
Recognitive agents have built-in base classes that are used to kickstart the categorization process, prior to learning any knowledge that might otherwise be useful in the category-selection process, primarily to assist in reasoning about which world-classes most accurately label a given input pattern. These base classes have very few constraints on membership, so few in fact that every possible input pattern fits into at least one base category, and the particular category for which it belongs is easily determined using a decision rule to find the truth value of whether a particular property is possessed by the input pattern, and thus whether the pattern is a member of the class. 

An agent's cateogorical decision rules are determined genetically and are subject to mutation during reproduction. The effect of which is a gradual convergance to a near optimal set of decison rules which result in homeostasis. That is, a set of decision rules that result in the necessary conditions for agent reproduction, or the successful passing-on of genes to the next generation. Reaching such a state requires one to bypass certain environmental constraints that threaten an agent's reproductive fitness. For example, a deadly plant is hazardous to a deer because, if ingested, the deer's ability to reproduce is hindered through sickness behaviors in response to the toxins or even death.

![Category](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Categories.png)

## Construction
Construction agents have built-in syntactic templates that are used to kickstart the construction process, prior to learning any knowledge that might otherwise be usefule in the sentence-construction process, primarily to assist in reasoning about which sentence-models most accurately resemble a given partially-constructed tree. These syntactic templates have very few constraints on composition, albeit more than the recognition agent's base classes. In any case, a small list of properties must be present in the partial tree for a template to be matched, and the particular template for which it is matched is easily determined using a decision rule to find the truth value of whether a particular set of word-classes are possessed the by the partial tree, as well as whether said word-classes were placed into the queue in a specific order, and thus whether the tree is a member of the template class. 

An agent's template decision rules are determined genetically and are subject to mutation, exactly like the recognition agent's decision rules. Another set of decision rules (which are also genetic) are applied universally regardless of template class which determines whether a given sentence is syntactically valid. The validity measurement of a given sentence is also referred to as its fitness. If there exists a sentence space with each possible formation of a sentence corresponding to one point on the space, then the composition of all constraints applied to each point on the sentence space will result in a fitness landscape which may be used to calculate the success of any given sentence formation with respect to the construction agent's universal decision rules. 

![Constraints](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Constraints.png)

## Organization

Phonological patterns and their corresponding words are connected through bidirectional links in memory, such that the phonological patterns and the semantic representations are stored as individual nodes, and bidirectional links transmit activation signals to-and-from associated nodes. 

Motor patterns are also connected to words, where the associated phonological pattern of a word is emulated when passed through a motor system that carries out verbal actions. The output signal propagates across the social landscape via transmission lines- links that connect each agent to a set of other agents called a neighborhood- in the form of phonological data. 

![Knowledge](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Memory.png)

## Communication

The signal is received by the neighboring agents, where a given phonological pattern in memory will respond (activate) to the input pattern if it bares a strong enough resemblance to that stored pattern. The semantic representation associated with the phonological pattern also becomes active, which in turn facilitates the power to carry out the verbal action associated with said semantic representation, provided the agent selects said verbal action to pass through the motor system into the social environment.

![Society](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Society.png)

***
# System Data Procedure

The following is an explaination of the various forms of information, as well their applications, within the system.

## Classes

Data is passed through sensors and stored in an input vector, where local contrast is measured over space to extract feature vectors. Spatial patterns, called objects, are detected as relationships between features over space, while temporal patterns, called events, are recognized as relationships between features over time. 

![Process](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Data%20Process.png)

Visual/auditory data compose morphological/phonological patterns, which are combined to form classes. A class represents an abstract concept, and exists independently of its real-world signifiers.  When a class becomes active, its corrosponding morphological/phonological signifiers become active as well, triggering a sort of “mental image” or simulation of the signifiers' visual/auditory stimuli.

## Relations

Classes are associated with one another through relations, which are links that represent various logic statements about classes. The fundamental relations are as follows:

![Relations](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Relations.PNG)

The motivation behind an initial set of relations is that almost all associations in the real world can fit into a relatively short number of categories. Low-level patterns with corresponding relations allow the automatic generation of relations between classes, and thus lay a foundation for higher-level relations to form. Similarities between classes can be measured independent of relative scale, and therefore analogies can be found be relating selected properties from one class and mapping them to antother. This enables the ability to detect relations regardless of scale, simply by forming an analogy with the low-level patterns that correspond with said relations.    

## Sentences

A sentence is a structure that defines associations between words (i.e. classes).  A word is classified into specific types, which relate to their role within a sentence, and correspond to dependencies dictating the validity of a sentence. If all dependencies have been met, then a sentence is considered meaningful and thus can move on to higher levels of analysis, where the domains in which meaning is processed become increasingly concrete and specific.

Templates are sentences with slots instead of words which correspond to syntactic categories, applying restrictions on the acceptable type allowed within a slot. Templates are developed through repeated experience with a wide variety of sentences. While forming a sentence from observed auditory patterns, the partial construction at each time step is compared to various templates in order to calculate the similarity between them. Matching templates are used to make predictions about the sentence structure, and results in greater efficiency due to the fact that it bypasses the search process by simply checking each new word and only initiated search if the current template fails to account for a new word.

![Template](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Template.png)

Cost is the measured violation of the current template by a newly received word. A given template is violated when a word deviates from the expected type, rendering the template invalid and removing it from the active status. Templates may respond to deactivation by triggering a variation to become active, which retain the central structure of the template while resolving the previous violation with the original. The new template is selected without any extensive search.

***

# Knowledge Representation

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

![Hierarchy](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/docs/img/datatypes.png)

Slots are useful when representing prototypes of a class as well. A
prototype is a partially-filled set of slots, the non-null properties
being derived from repeated instantiation, and those particular combinations
being generalized over a set a observations. A class is not defined by one
prototype, but by multiple prototypes distinguishing between common
variations of a class.

## Objects and Relations

Relations represent contrasts of objects in terms of property deltas over space and time. 
Spatial difference refers to property deltas of objects in a set, while temporal difference
refers to property deltas of the same object as it changes over time.

![Relations](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/docs/img/Relations.PNG)

References to structures like “object” and “set” are relative. An object may very well
be considered a set of properties, while at the same time a property
is an object in and of itself.This recursive functionality is complimented
by the hierarchical structure of data within the system.
