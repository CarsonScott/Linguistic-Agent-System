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

An agent's template decision rules are determined genetically and are subject to mutation, exactly like the recognition agent's decision rules. Another set of decision rules are applied universally regardless of template class which determines whether a given sentence is syntactically valid. The validity measurement of a given sentence is also referred to as its fitness. If there exists a sentence space with each possible formation of a sentence corresponding to one point on the space, then the composition of all constraints applied to each point on the sentence space will result in a fitness landscape which may be used to calculate the success of any given sentence formation with respect to the construction agent's universal decision rules.

![Constraints](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Constraints.png)

## Organization

Phonological patterns and their corresponding words are connected through bidirectional links in memory, such that the phonological patterns and the semantic representations are stored as individual nodes, and bidirectional links transmit activation signals to-and-from associated nodes. 

Motor patterns are also connected to words, where the associated phonological pattern of a word is emulated when passed through a motor system that carries out verbal actions. The output signal propagates across the social landscape via transmission lines- links that connect each agent to a set of other agents called a neighborhood- in the form of phonological data. 

![Knowledge](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Memory.png)

## Communication

The signal is received by the neighboring agents, where a given phonological pattern in memory will respond (activate) to the input pattern if it bares a strong enough resemblance to that stored pattern. The semantic representation associated with the phonological pattern also becomes active, which in turn facilitates the power to carry out the verbal action associated with said semantic representation, provided the agent selects said verbal action to pass through the motor system into the social environment.

![Society](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Society.png)
