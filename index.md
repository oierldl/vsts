# Visual Semantic Textual Similariy

In this paper we extend STS to the visual modality, and present Visual
Semantic Textual Similarity (vSTS), a task and dataset which allows to
study whether better sentence representations can be built when having
access to the corresponding images, in contrast with having access to
the text alone. The example below illustrates the need to re-score the
similarity values, as the text-only similarity is not applicable to
the multimodal version of the dataset: the annotators return a low
similarity when using only text, while, when having access to the
corresponding image, they return a high similarity

![]({{ oierldl.github.io }}/vsts/images/vsts-motivation.png)


The vSTS dataset aims to become a standard benchmark to test the
contribution of visual information when evaluating the similarity of
sentences and the quality of multimodal representations, allowing to
test the complementarity of visual and textual information for
improved language understanding.


# Visual STS Dataset

The vSTS assesses the degree to which two sentences are semantically
equivalent to each other. The annotators measure the similarity among
sentences with the help of associated images.

The annotations of similarity were guided by the scale in
Table~\ref{tab:sim_def}, ranging from 0 for no meaning overlap to 5
for meaning equivalence. Intermediate values reflect interpretable
levels of partial overlap in meaning.


|Similarity | definitions|
|-----------|------------|
| 5 | Completely equivalent: They mean the same thing. |
| 4 | Mostly equivalent: Some unimportant details differ. |
| 3 | Roughly equivalent: Some important information differs/missing. |
| 2 | Not equivalent but share some details. |
| 1 | Not equivalent but on the same topic. |
| 0 | Completely dissimilar. |



Summary stats and plot of the dataset


# Explore 

link to dashboard

# Paper


# Authors


# Experiments
