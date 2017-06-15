# System Data Procedure

The following attempts to break down the various forms in which information is expressed throughout the system, along with the corresponding application of each.

## Classes

Data is passed through sensors and stored in an input vector, where local contrast is measured over space to extract feature vectors. Spatial patterns, called objects, are detected as relationships between features over space, while temporal patterns, called events, are recognized as relationships between features over time. 

Visual  and auditory data forms morphological and phonological patterns/sequences, which are combined to form classes, or words, which equate to abstract concepts that are independent of real-world signifiers.  When a class becomes active, the corrosponding morphological and phonological signifiers become active as well, triggering a sort of “mental image”, or simulation of the visual and auditory stimuli. Classes are used to create environmental representations, along with a set of relations between them which define meaniningful implications of the observed environment.


![Data Process](https://github.com/CarsonScott/Linguistic-Agent-System/blob/master/img/Data%20Process.png)

 
Words are the phonological signifiers of classes. A sentence defines the interactive and comparitive associations between words, and by extension their classes, within a sequence. A word is classified into specific types, which relate to their role within a sentence, and correspond to dependencies dictating the validity of a sentence. If all dependencies have been met, then a sentence is considered meaningful and thus can move on to higher levels of analysis, where the domains in which meaning is processed become increasingly concrete and specific.

Templates are sentences with slots instead of words which correspond to syntactic categories, applying restrictions on the acceptable type allowed within a slot. Templates are developed through repeated experience with a wide variety of sentences. While forming a sentence from observed auditory patterns, the partial construction at each time step is compared to various templates in order to calculate the similarity between them. Matching templates are used to make predictions about the sentence structure, and results in greater efficiency due to the fact that it bypasses the search process by simply checking each new word and only initiated search if the current template fails to account for a new word.

Cost is the measured violation of the current template by a newly received word. A given template is violated when a word deviates from the expected type, rendering the template invalid and removing it from the active status. Templates may respond to deactivation by triggering a variation to become active, which retain the central structure of the template while resolving the previous violation with the original. The new template is selected without any extensive search.

