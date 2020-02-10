# Visual Semantic Textual Similariy

We present present Visual Semantic Textual Similarity (vSTS) that extends
the Semantic Textual Similarity to the visual modality, a task and dataset
which allows to study whether better sentence representations can be
built when having access to the corresponding images, in contrast with
having access to the text alone. The example below illustrates the
need to re-score the similarity values, as the text-only similarity is
not applicable to the multimodal version of the dataset: the
annotators return a low similarity when using only text, while, when
having access to the corresponding image, they return a high
similarity

![]({{ oierldl.github.io }}/vsts/images/vsts-motivation.png)


The vSTS dataset aims to become a standard benchmark to test the
contribution of visual information when evaluating the similarity of
sentences and the quality of multimodal representations, allowing to
test the complementarity of visual and textual information for
improved language understanding.


# Visual STS Dataset

The vSTS assesses the degree to which two sentences are semantically
equivalent to each other. The annotators measure the similarity among
sentences with the help of associated images. The annotations of
similarity were guided by the scale shown in the table below,
ranging from 0 for no meaning overlap to 5 for meaning
equivalence. Intermediate values reflect interpretable levels of
partial overlap in meaning.


|Similarity | definitions|
|-----------|------------|
| 5 | Completely equivalent: They mean the same thing. |
| 4 | Mostly equivalent: Some unimportant details differ. |
| 3 | Roughly equivalent: Some important information differs/missing. |
| 2 | Not equivalent but share some details. |
| 1 | Not equivalent but on the same topic. |
| 0 | Completely dissimilar. |


## Data Collection

The data collection of sentence-image pairs comprised several steps,
including the selection of pairs to be annotated, the annotation
methodology, and a final filtering stage.

1. __Sampling data for manual annotation__. We make use of two
well-known image-caption datasets. On one hand, Flickr30K dataset and
Microsoft COCO dataset, each one contains 5 manually generated
captions per images.

2. __Manual annotations__. In order to annotate the sample of 2639
pairs, we used Amazon Mechanical Turk (AMT). We got up to 5 scores per
item, and we discarded annotators that showed low correlation with the
rest of the annotators ($\rho < 0.75$).

3. __Selection of difficult examples__. We defined easiness as an
amount of discrepancy provided by an example regarding the whole
dataset. We removed 30\% of the _easiest_ examples and create a more
challenging dataset of 1858 pairs.


The full dataset comprises both the sample mentioned above and the 819
pairs from our preliminary work, totalling 2677
pairs. The figure shows the final item similarity
distribution. Although the distribution is skewed towards lower
similarity values, we consider that all the similarity ranges are
sufficiently well covered.


![]({{ oierldl.github.io }}/vsts/images/vsts20_ggplots.png)




# Explore 

link to dashboard

# Paper


# Authors


# Experiments
