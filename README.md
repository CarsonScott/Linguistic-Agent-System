# Linguistic Agent Systems

## Recognition Agents

A recognition agent B is initialized with a set of built-in classes or categories that hold intimate ties to the sensory-motor system. Certain low-level patterns of information are classified automatically to assigned categories, for example the perceived changes resulting from an action are automatically sent to a “verb” category, while passive observations of objects are placed in a “noun” category. Each new category learned by B is contained within an existing supercategory. Thus the classes built into B make up the basis for every future class acquired by B through experience.

## Rewriting Agents

A rewrite agent R is initialized with a set of decision rules that constrain how it chooses the actions it performs when constructing sentences. Specifically, constraints influence the ordering of words, as well as the combination of words, in a sentence. Certain requirements must be met in order for a sentence to be valid, for example a sentence that contains a verb with no subject or object is not a valid sentence. The requirement therefore states that a sentence containing a verb must also contain a subject or an object to be valid, otherwise it is nonsensical.

The properties of a given sentence form a feature vector, which is passed to every constraint function to calculate the total error of the feature vector, which equates to a point on a feature space, on which every constraint function is related to an assigned subspace that defines the valid range of compositions that are deemed acceptable by a given constraint function. Simply put, the subspace of a given constraint function is the range of compositions which result in a non-negative output.

The performance of R is indicated by the sum of results from each constraint, called the net error. This value acts as an output error used in the backpropagation of R's neural network, which is responsible for the selection of R's behavioral outputs. The result is a sort of indoctrination, where R is adapted to minimize the expected cumulative error received in the future.


