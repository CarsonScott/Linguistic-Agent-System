# Linguistic Competence in Multi-Agent Systems

The following is a theoretical model for a multi-agent system that specializes in linguistic comprehension and language production. The system is composed of two interacting agents that together produce meaningful representations of concepts in order to understand the world.

The first agent, the recognition agent, is responsible for transforming input patterns into meaningful semantic units called words, which are sent through a transmission line called the queue to the second agent. The second agent, the rewriting agent, is in charge of taking words from the queue and constructing relational diagrams which model the structure of sentences as a tree.

![](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/Structure.png)

## Recognition Agents

A recognition agent B is initialized with a set of built-in classes or categories for low-level information. Certain patterns are classified automatically, for instance the perceived changes caused by an action are automatically placed in a “verb” category, while perceived objects in the environment are placed in a “noun” category. Each new category that B learns over time is contained by an existing category, making it a subcategory to an already-known supercategory. Thus the buit-in classes are required in order for B to successfully acquire more complex categories.

## Rewriting Agents

A rewrite agent R is initialized with a set of decision rules that constrain how it chooses the actions it performs when constructing sentences. Specifically, constraints influence the ordering of words, as well as the combination of words, in a sentence. Certain requirements must be met in order for a sentence to be valid, for example a sentence that contains a verb with no subject or object is not a valid sentence. The requirement therefore states that a sentence containing a verb must also contain a subject or an object to be valid, otherwise it is nonsensical.

The properties of a given sentence form a feature vector, which is passed to every constraint function to calculate the total error of the feature vector, which equates to a point on a feature space, on which every constraint function is related to an assigned subspace that defines the valid range of compositions that are deemed acceptable by a given constraint function. Simply put, the subspace of a given constraint function is the range of compositions which result in a non-negative output.

The performance of R is indicated by the sum of results from each constraint, called the net error. This value acts as an output error used in the backpropagation of R's neural network, which is responsible for the selection of R's behavioral outputs. The result is a sort of indoctrination, where R is adapted to minimize the expected cumulative error received in the future.

