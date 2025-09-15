# NCoPEN: Topology-Informed Co-Encoding of Spectral Perturbations with Cross-Channel Interdependence Recomposition for EEG-Based Neurodegeneration Screening

![](figure/image1.png)

Figure 1: Comparative depiction of functional brain connectivity and spectral distribution

![](figure/image2.png)

Figure 2: Detailed network structure of our proposed NCoPEN.

## Methods

### NIRU

![](figure/image3.png)

Figure 3: {Illustration of six heterogeneous feature-extraction pipelines

![](figure/image4.png)

Figure 4: NIRU: multichannel descriptors are transformed by self-attention and then recomposed via a Gaussian mixture, yielding structurally refined embeddings for downstream reconstruction.

### PATMD

![](figure/image5.png)

Figure 5: PATMD: perturbation kernels quantify inter-channel functional deviations; spectral–graph eigenanalysis resolves principal perturbation orientations; spectral-response projection produces the fused descriptor $F_7$.

## Installation

We run NCoPEN and previous methods on a system running Ubuntu 22.04, with Python 3.8, PyTorch 2.1.0, and CUDA 12.1.

## Experiment

### Resting-state Parkinson Dataset

![](figure/image6.png)

Figure 6: Baseline distribution across four EEG corpora—Thessaloniki (AD/FTD/HC), CAUEEG (CN/MCI/AD), Task-state Parkinson, and Resting-state Parkinson.

![](table/table2.png)

Table 2: Resting-state PD–HC baselines across representative EEG networks.

![](figure/image7.png)

Figure 7: Three-dimensional t-SNE embeddings of latent features on the Resting-State Parkinson cohort (PD vs.\ HC) across ten architectures

### Task-Induced PD Classification

![](table/table3.png)

Table 3: Baseline classification outcomes on the task-state Parkinson’s dataset

### Multi-Class Classification on Thessaloniki Dataset

![](table/table4.png)

Table 4: Quantitative assessment of regional contributions to AD classification efficacy through cortical branch-specific ablation analysis.

### Large-Scale Evaluation on CAUEEG

![](table/table5.png)

Table 5: CAUEEG cohort, three-class CN–MCI–AD benchmark.

![](figure/image8.png)

Figure 8: Channel-level SHAP attribution maps with the NIRU enabled (left) versus ablated (right)

## Ablation study

### Feature-Processing Ablation

![](table/table6.png)

Table 6: Comparative ablation outcomes for the NIRU

### Feature-Fusion Ablation

![](table/table7.png)

Table 7: Comparative evaluation of feature-aggregation ablations within the PATMD module

### Classifier Ablation

![](table/table8.png)

Table 8: Performance comparison across ablated classifier configurations

![](figure/image9.png)

Figure 9: Two-dimensional t-SNE embeddings of features from ablated classifiers

### Feature Extraction Ablation

![](table/table9.png)

Table 9: Feature extraction ablation across backbone encoders


## Model Visualization

![](figure/image10.png)

Figure 10: Channel–wise activation heatmaps contrasting CN and PD cohorts across six feature families

![](figure/image11.png)

Figure 11: (a) Standardized multichannel EEG with superposed saliency weights—gray, (b) Scalp-averaged channel-importance topography,(c) Band-resolved PSD maps

![](figure/image12.png)

Figure 12: Top-3 discriminative EEG segments identified by the model

![](figure/image13.png)

Figure 13: Decision geometry, calibration behavior, and error structure for the PD–HC classifier


# Question

if you have any questions, please contact 'yachen.wei@hdu.edu.cn'
