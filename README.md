# Alzheimer's Disease AI
The aim of this project is the developing and evaluation of an AI to classify patients affected by various stages of dementia and/or Alzheimer's Disease. We will focus on data inspection and analysis, then proceed on the realization of an AI through the use of machine learning methods.
## The data
All the data were provided by OASIS[[1]](https://www.oasis-brains.org/) (Open Access Series of Imaging Studies), in particular from their third and biggest study OASIS-3.
> _OASIS-3 is a retrospective compilation of data for >1000 participants that were collected across several ongoing projects through the WUSTL Knight ADRC over the course of 30 years. Participants include 609 cognitively normal adults and 489 individuals at various stages of cognitive decline ranging in age from 42-95yrs. All participants were assigned a new random identifier and all dates were removed and normalized to reflect days from entry into study. The dataset contains over 2000 MR sessions which include T1w, T2w, FLAIR, ASL, SWI, time of flight, resting-state BOLD, and DTI sequences. Many of the MR sessions are accompanied by volumetric segmentation files produced through Freesurfer processing. PET imaging from 3 different tracers, PIB, AV45, and FDG, totaling over 1500 raw imaging scans and the accompanying post-processed files from the Pet Unified Pipeline (PUP) are also available in OASIS-3._

Among these information, demographical data and MRI scans reports was of particular relevance.
### Overview
The following were extracted and calculated based on the OASIS-3 Dataset.
- **ID**: Unique dentifier for the patients
- **Sex**: Where 1 stands for male, and 0 for female
- **Age**: Age in years
- **Height**: Measured in mm, has an accurancy of &#177;13mm
- **Weight**: Measured in kg
- **Education**: Total years of education
- **Hand**: Where 1 stands for right handed, 0 for left handed and 2 for ambidextrous
- **mmse**: MMSE[[3]](https://en.wikipedia.org/w/index.php?title=Mini%E2%80%93Mental_State_Examination&oldid=1076211630) (Mini Mental State Examination) score from 0 to 30
- **cdr**: Clinical Dementia Rating, measures the severity of dementia: 0	none, 0.5	very mild, 1	mild, 2	moderate, 3	severe
- **dx1**: Dementia related clinical diagnosis
- **dx2-5**: Other conditions the patient is affected by
- **eTIV**: Estimated Total Intracranical Volume in mm<sup>3</sup>[[2]](https://www.oasis-brains.org/files/OASIS-3_Imaging_Data_Dictionary_v1.5.pdf)
- **brainVol**: Brain valume in mm<sup>3</sup>
- **nWBV**: brainVol/eTIV ratio
- **ventricleVol**: Sum of the volums of left lateral ventricle, right lateral ventricle, 3rd ventricle, 4th ventricle and 5th ventricle in mm<sup>3</sup>
- **ventricleRatio**: ventricleVol/eTIV ratio
- **hcVol**: Total hippocampus volume in mm<sup>3</sup>
- **hcRatio**: hcVol/eTIV ratio

<sub>Note: brain volumes were calculated by OASIS using FreeSurfer[[4]](https://surfer.nmr.mgh.harvard.edu/) software to analyse MRI scans</sub>


