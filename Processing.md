# System Data Procedure

The following attempts to break down the various forms in which information is expressed throughout the system, along with the corresponding application of each.

![Data Process](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Data%20Process.png)

## Classes

Data is passed through sensors and stored in an input vector, where local contrast is measured over space to extract feature vectors. Spatial patterns, called objects, are detected as relationships between features over space, while temporal patterns, called events, are recognized as relationships between features over time. 

Visual  and auditory data forms morphological and phonological patterns/sequences, which are combined to form classes, or words, which equate to abstract concepts that are independent of real-world signifiers.  When a class becomes active, the corrosponding morphological and phonological signifiers become active as well, triggering a sort of “mental image”, or simulation of the visual and auditory stimuli. Classes are used to create environmental representations, along with a set of relations between them which define meaniningful implications of the observed environment.

## Sentences

A sentence is a structure that defines associations between words (i.e. classes).  A word is classified into specific types, which relate to their role within a sentence, and correspond to dependencies dictating the validity of a sentence. If all dependencies have been met, then a sentence is considered meaningful and thus can move on to higher levels of analysis, where the domains in which meaning is processed become increasingly concrete and specific.

Templates are sentences with slots instead of words which correspond to syntactic categories, applying restrictions on the acceptable type allowed within a slot. Templates are developed through repeated experience with a wide variety of sentences. While forming a sentence from observed auditory patterns, the partial construction at each time step is compared to various templates in order to calculate the similarity between them. Matching templates are used to make predictions about the sentence structure, and results in greater efficiency due to the fact that it bypasses the search process by simply checking each new word and only initiated search if the current template fails to account for a new word.

Cost is the measured violation of the current template by a newly received word. A given template is violated when a word deviates from the expected type, rendering the template invalid and removing it from the active status. Templates may respond to deactivation by triggering a variation to become active, which retain the central structure of the template while resolving the previous violation with the original. The new template is selected without any extensive search.


## Relations

Sentences are equivalent to graphs, where the nodes are classes and the links are relations. Nodes of course have semantic properties while links represent logic, where each link has a logical identity that defines how two or more classes relate to one another. The elementary logical identities are as follows:

![](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Relations.PNG)

The domains are used as the foundation for all high-level relations, which represent complex associations between classes.

The motivation behind building an initial set of relations is that almost all associations in the real world can fit into a small number of categories. Low-level sensory patterns can trigger a relation automatically, so that higher level versions of said relations bare resemblance to basic shapes, sounds, events, etc., to which they are analogous
