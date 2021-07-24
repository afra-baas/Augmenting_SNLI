# Augmenting_SNLI
Mitigating hypothesis-only bias in SNLI dataset with data augmentation


Table of Content
=============
  * [Table of Contents](#table-of-content)
  * [Project Description](#project-description)
  * [Method](#method)
  * [Code](#code)

## Project Description
For my Thesis I mitigated the hypothesis-only bias in the SNLI dataset.
Recent studies like (ref ...) have shown that the hypothesis annotation artifacts that enable hypothesis-only classifiers to already classify hypothesis with a high accuracy. The inferences with these correctly classified hypotheses are called easy examples. Then they give a big boost to the NLI performance when in these cases it's cheating the task of classifying inference. 
The approach to mitigate this hypothesis-only bias is explained in the section Method.

## Method
Right now each premise in SNLI has three hypothesis, each with a different label. So a
premise can lead to three labels, but an hypothesis has a unique label.
The approach is balancing the annotation artifacts other all labels by adding more examples to the SNLI dataset. (data augmentation)
We will use pertubations functions to generate new premises. These premises need to be generated in a way the the same hypothesis can get a different label. 
Resulting in multiple premises for one hypothesis. Now one hypothesis can have different labels, when related to a different premises. Thus the system can no
longer associate hypotheses with certain artifacts with only one label. 

## Code(Notebooks)
I tried to make the notebooks easy to follow. However any questions or suggestions for improvement are very welcome.

