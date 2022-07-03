# Domain-Adaptive-Building-Counting
**Paper Title:** Cross-Region Building Counting in Satellite Imagery using Counting Consistency

**Pre-print** available [here]()

**Dataset** available [here](https://drive.google.com/drive/folders/1CIYGCJucyJ9dnwjt0BZJ7pnyiKIDuRQC?usp=sharing)

**Dataset Name:** IML-DAC

Estimating the number of buildings in any geographical region is a vital component of urban analysis, disaster management, and public policy decision. Deep learning methods for building localization and counting in satellite imagery, can serve as a viable and cheap alternative. However, these algorithms suffer performance degradation when applied to the regions on which they have not been trained. Current large datasets mostly cover the developed regions and collecting such datasets for every region is a costly, time-consuming, and difficult endeavor. In this paper, we propose an unsupervised domain adaptation method for counting buildings where we use a labeled source domain (developed regions) and adapt the trained model on an unlabeled target domain (developing regions). We initially align distribution maps across domains by aligning the output space distribution through adversarial loss. We then exploit counting consistency constraints, within-image count consistency, and across-image count consistency, to decrease the domain shift. Within-image consistency enforces that building count in the whole image should be greater than or equal to count in any of its sub-image. Across-image consistency constraint enforces that if an image contains considerably more buildings than the other image, then their sub-images shall also have the same order. These two constraints encourage the behavior to be consistent across and within the images, regardless of the scale. To evaluate the performance of our proposed approach, we collected and annotated a large-scale dataset consisting of challenging South Asian regions having higher building densities and irregular structures as compared to existing datasets. We perform extensive experiments to verify the efficacy of our approach and report improvements of approximately 7% to 20% over the competitive baseline methods.

![pipeline_3](https://user-images.githubusercontent.com/60637386/175949883-f9a81aff-0ae3-489c-868a-c616ec26250c.jpg)

# Dataset Details

To evaluate the accuracy of the proposed approach in cross-region building counting, in our experiments, we use the IML-DAC and South Asian regions of xView as target (test) datasets. The geographical locations of areas from which IML-DAC are collected are mainly South Asian regions. 
The dataset contains a total of 4935 patches non-overlapping patches of dimension 500x500 pixels.

### Dataset Link and Contents

The dataset can be downloaded from [here](https://drive.google.com/drive/folders/1CIYGCJucyJ9dnwjt0BZJ7pnyiKIDuRQC?usp=sharing).

The link will contain three folders divided into training, validation, and testing. Each folder contains two subfolders: images and ground truths.

# Implementing the Code

### Installation

The following need to be installed before proceeding:

PyTorch 0.4.1

Python 2.7

### Training the Source Model

### Adapting using L_DMA

### Adapting using L_CWI

### Adapting using L_CAI
