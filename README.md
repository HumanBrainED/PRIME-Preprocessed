# PRIME-Preprocessed
ongoing project: preprocess PRIME-DE data

Goal: 
- 1. Quality assessment
- 2. Minimal preprocess
- 3. End-to-end preprocess 

Datasets:
- 5 core fMRI sites (n≥10 per site, function data)
    - Newcastle University (N=14)
    - UC-Davis (N=19)
    - Oxford (N=20)
    - University of Wisconsin-Madison (N=592)
    - University of Western Ontario (N=12, 7 MP2RAGE + 5 MPRAGE)
- 5 core T1+T2 sites (n≥5 per site, T1w+T2w)
    - Mount Sinai-Philips (n=8 total, 5 T1+T2, 6 func+T1)
    - Mount Sinai-Siemens (n=5)
    - Newcastle (n=14)
    - UC-Davis (N=19)
    - University of Western Ontario (N=12, MP2RAGE)

Example data: 2 subjects for each of 5 core sites above
Brain masks for example data: [link](https://github.com/HumanBrainED/PRIME-Preprocessed/blob/main/ExampleData/ExampleData_Masks.tar.gz)


----
## Anatomical brain mask (pre-release, all T1w masks)
https://github.com/HumanBrainED/PRIME-Preprocessed/releases

## v0.1_anat_brainmask: brain masks for T1w images from PRIME-DE
Masks are generated using the U-Net model (https://github.com/HumanBrainED/NHP-BrainExtraction)

- Masks for all sites except site-uwmadison are created based on [brainmask_T1w_136macaques.tar](https://github.com/HumanBrainED/NHP-BrainExtraction/blob/master/PRIME-DE_BrainMask/brainmasks/brainmask_T1w_136macaques.tar) (Ref: Reference: [Wang et al.,2021](https://www.sciencedirect.com/science/article/pii/S1053811921002780))
- U-Net model for site-uwmadison can be downloaded [here](https://github.com/HumanBrainED/NHP-BrainExtraction/blob/master/UNet_Model/models/Site_uwmadison_update_epoch_39.model) 
- Join [Quality Control](https://dev.swipesforscience.org/#/?config=https://raw.githubusercontent.com/HumanBrainED/PRIME-Preprocessed/main/vcheck_anat_brainmask/config.json)

**Note**: The masks are not perfect here. Use them as initial masks

----






