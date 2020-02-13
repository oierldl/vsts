# __vSTS__: Visual Semantic Textual Similarity

We present present Visual Semantic Textual Similarity (vSTS) that
extends the Semantic Textual Similarity to the visual modality, a task
and dataset which allows to study whether better sentence
representations can be built when having access to the corresponding
images, in contrast with having access to the text alone.

The vSTS dataset aims to become a standard benchmark to test the
contribution of visual information when evaluating the similarity of
sentences and the quality of multimodal representations, allowing to
test the complementarity of visual and textual information for
improved language understanding.


For more details check out our ECAI paper [__Evaluating Multimodal
Representations on Visual Semantic Textual
Similarity__](https://oierldl.github.io/vsts/paper/ECAI_2020___vSTS.pdf),
and [website](https://oierldl.github.io/vsts/).

The code and models presented in our [paper](https://oierldl.github.io/vsts/paper/ECAI_2020___vSTS.pdf), see our repository at: **TBD**

Full dataset can be downloaded [here](http://ixa2.si.ehu.eus/~jibloleo/visual_sts.v2.0.tar.gz).


## Data description and format

Each instance contains a pair of images and their description and a
similarity value that ranges from 0 to 5. In total, we obtained 2677
pairs.

Each row contains one instance with tab separated values. Each row
contains the following information:

- **``id``**: instances ID.
- **``source``**: Source of the sentence pairs: STS2014, STS2015, MS-COCO and Flickr30k.
- **``sent1``**: First sentence of the pair.
- **``image1``**: Path to the image file associated with the first sentence.
- **``sent2``**: Second sentence of the pair.
- **``image2``**: Path to the image file associated with the secpmd sentence.
- **``sim``**: Similarity value that ranges from 0 to 5. 


The file ``visual_sts.v2.0.all.tsv`` ([download](https://github.com/oierldl/vsts/visual_sts.v2.0.all.tsv)) contains the whole
dataset without the actual images. Train, development, and test
partition used in the
[paper]((https://oierldl.github.io/vsts/paper/ECAI_2020___vSTS.pdf))
can be found in [``train-dev-test``](https://github.com/oierldl/vsts/dataset/train-dev-test) folder in the GitHub
repository. Partitions are divied in the following files:

- **Training set**: ``dataset/train-dev-test/visual_sts.v2.0.train.tsv``
- **Development set**: ``dataset/train-dev-test/visual_sts.v2.0.dev.tsv``
- **Test set**: ``dataset/train-dev-test/visual_sts.v2.0.test.tsv``

In
order to obtain the images you can download the whole dataset from our
servers: [vSTS
dataset](http://ixa2.si.ehu.eus/~jibloleo/visual_sts.v2.0.tar.gz).

