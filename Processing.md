# System Data Procedure

The following is an explaination of the various forms of information, as well their applications, within the system.

![Process](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Data%20Process.png)

## Classes

Data is passed through sensors and stored in an input vector, where local contrast is measured over space to extract feature vectors. Spatial patterns, called objects, are detected as relationships between features over space, while temporal patterns, called events, are recognized as relationships between features over time. 

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

