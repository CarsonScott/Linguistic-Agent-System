# Emergence of Linguistic Capacity in Evolving Multi-Agent Systems

The following paper describes a theoretical model of language acquisition, comprehension, and production using a distributed multi-agent system. The system is composed of a society or population of agents, who communicate by sending and receiving phonological signals across a social network. Every individual contains an internal system of subagents that are specialized to perform a small number of tasks which make up the cognitive process.   

## Overview

The initial subagent is called a recognition agent and is responsible for receiving input patterns from the environment and extracting  semantic representations, called words, of the observed patterns. Every time step the agent produces a set of words that were detected from the input and places them into a temporary storage-unit called a queue.

The next subagent is called a construction agent and is responsive for observing a sequence of words from the queue and creating hierarchical diagrams, called trees, of the observed sequences. Every time steps the agent selects a set of operators that were determined by the contents of the queue with respect to the current state of the tree and applies them to the tree in order to add, remove, or change certain properties that define its structure.

![Agent](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Agent.png)

## Recognition
Recognitive agents have built-in base classes that are used to 'kick-start' the categorization process, prior to learning knowledge that it would otherwise find useful in the category-selection process in reasoning about which class a given input pattern fits best. These base classes have very few constraints for determining if a pattern is an acceptable member or not, such that every possible input pattern fits into at least one base category, and the particular category for which it belongs is easily determined by an associated decision rule, which returns a binary truth value that indicates whether a particular property is possessed by a given patthern, and thus whether the pattern is a member of the class. 

An agent's cateogorical decision rules are determined genetically and are subject to mutation during reproduction. The effect of which is a gradual convergance to a near optimal set of decison rules which result in homeostasis. That is, a set of decision rules that result in the necessary conditions for agent reproduction, or the successful passing-on of genes to the next generation. Reaching such a state requires one to bypass certain environmental constraints that threaten an agent's reproductive fitness. For example, a deadly plant is hazardous to a deer because, if ingested, the deer's ability to reproduce is hindered through sickness behaviors in response to the toxins or even death.

![Category](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Categories.png)

## Construction Agent

A Construction agent R is initialized with a set of decision rules that constrain how it chooses the actions it performs when constructing sentences. Specifically, constraints influence the ordering of words, as well as the combination of words, in a sentence. Certain requirements must be met in order for a sentence to be valid, for example a sentence that contains a verb with no subject or object is not a valid sentence. The requirement therefore states that a sentence containing a verb must also contain a subject or an object to be valid, otherwise it is nonsensical.

The properties of a given sentence form a feature vector, which is passed to every constraint function to calculate the total error of the feature vector, which equates to a point on a feature space, on which every constraint function is related to an assigned subspace that defines the valid range of compositions that are deemed acceptable by a given constraint function. Simply put, the subspace of a given constraint function is the range of compositions which result in a non-negative output.

The performance of R is indicated by the sum of results from each constraint, called the net error. This value acts as an output error used in the backpropagation of R's neural network, which is responsible for the selection of R's behavioral outputs. The result is a sort of indoctrination, where R is adapted to minimize the expected cumulative error received in the future.

A finite amount of memory gives rise to constraints on the depth and breadth of constructed sentences. In other words, the amount of memory for which a Construction agent has at its disposal at any given time has direct influence on the complexity limit, or the maximum number of nodes that a Construction agent can keep track of in a constructed sentence.

![Constraints](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Constraints.png)

## Knowledge Organization

Phonological patterns and their corresponding words are connected through bidirectional links in memory, such that the phonological patterns and the semantic reperesentations are stored as individual nodes, and bidirectional links transmit activation signals to-and-from associated nodes. 

Motor patterns are also connected to words, where the associated phonological pattern of a word is emulated when passed through a motor system that carries out verbal actions. The output signal propagates across the social landscape via transmission lines- links that connect each agent to a set of other agents called a neighborhood- in the form of phonological data. 

![Knowledge](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Memory.png)

## Social Interaction

The signal is received by the neighboring agents, where a given phonological pattern in memory will respond (activate) to the input pattern if it bares a strong enough resemblence to that stored pattern. The semantic representation associated with the phonological pattern also becomes active, which in turn facilitates the power to carry out the verbal action associated with said semantic representation, provided the agent selects said verbal action to pass through the motor system into the social environment. 

![Society](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Society.png)
