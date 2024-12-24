# VATT-Official
This repository contains the **official code, datasets, and sample outputs** for our [NeurIPS paper](#citation)  
**"Tell What You Hear From What You See — Video to Audio Generation Through Text."**

## Table of Contents
1. [Introduction](#introduction)  
2. [Datasets](#datasets)  
   - [V2A Instruction Dataset](#v2a-instruction-dataset)  
3. [Sample Outputs](#sample-outputs)  
4. [Citation](#citation)

## Introduction
**VATT (Video-to-Audio Generation Through Text) a multi-modal generative framework that takes a video and an optional text prompt as input, and generates audio and optional textual description of the audio. Such a framework has two advantages: i) Video-to-Audio generation process can be refined and controlled via text which complements the context of visual information, and ii) The model can suggest what audio to generate for the video by generating audio captions. VATT consists of two key modules: VATT Converter, a LLM that is fine-tuned for instructions and includes a projection layer that maps video features to the LLM vector space; and VATT Audio, a transformer that generates audio tokens from visual frames and from optional text prompt using iterative parallel decoding. The audio tokens are converted to a waveform by pretrained neural codec. 

If you find this repository helpful in your research, please consider citing our paper (see [Citation](#citation)).

## Datasets
Here, we provide links to our **V2A Instruction Dataset**. Currently, we offer two versions:

### V2A Instruction Dataset
1. **VGGSound Only**  
   [Download Link](https://drive.google.com/file/d/1uo4Hx6tAnqVkU65AfPHGwFAftysTCXxs/view)  
   This subset consists solely of VGGSound data.

2. **VGGSound + AudioSet 2M**  
   [Download Link](https://drive.google.com/file/d/1ukpU69eysXnhrHOfgSVWf2BHE5E4WuzI/view)  
   This expanded version includes both VGGSound and some additional data from AudioSet, totaling 1.77 million samples.

> **Note:** Please check the appropriate licenses and usage rights for VGGSound and AudioSet data before using them in your research.

## Sample Outputs
We provide sample outputs generated by **VATT-LLama-T** on the VGGSound test set:

- **VATT-LLama-T (VGGSound Test Set)**  
  [Download Link](https://drive.google.com/file/d/10DVuVOxn_2eDUdSYLrtB0XSkkCgJMY3a/view?usp=sharing)

## Citation
If you use VATT or refer to our NeurIPS paper, please cite us:
@article{liu2024tell,
  title={Tell What You Hear From What You See--Video to Audio Generation Through Text},
  author={Liu, Xiulong and Su, Kun and Shlizerman, Eli},
  journal={arXiv preprint arXiv:2411.05679},
  year={2024}
}
