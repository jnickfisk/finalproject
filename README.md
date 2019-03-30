# Final Project

## Instructions
Reminder: 
Do not commit large data files to the repository. Provide paths to where they can be downloaded if they
are from public sources, or track them with [git-lfs](https://git-lfs.github.com).

## Introduction

This is a final project for the [Comparative Genomics](https://github.com/Yale-EEB723/syllabus) seminar in the spring of 2019. This project aims to construct time calibrated phylogenies of tumors sampled at different sites using exome data. Additionally, effect size of mutations will be calculated and aligned with interesting annotations from the patients' life histories. 

## The goal

With improvements in both computing power and theory, phylogenetic analysis of large swaths of sequencing data has become both feasible and powerful.
The development of cancer is, fundamentally, an evolutionary process.  
This is all the more evident when cancer cell populations acquire immunity to targeted therapies, leading to profound challenges in continued care. 
Modern sequencing technology can be leveraged to obtain clinically relevant data on which methods born in evolutionary biology can be applied. 
The structure of tumor lineages can be obtained and calibrated to real-time, allowing for estimates for temporal resolution of metastasis and mutations of interest.
Further, selection intensity can be used to determine the effect size of somatic single nucleotide variants (SNVs) for well-defined cancer subtypes. 
Here, we examine the whole-exome data of a cohort of lung cancer patients in the broad context of their medical history. Specifically, we focus on the effect sizes of mutations in EGFR positive samples and the overall lineage structure of subsequent metastases. 

## The data
The data comes from 2 main sources:
The first set comes from data previously published in the PNAS paper "Early and multiple origins of metastatic lineages within primary tumors
Zi-Ming Zhao, Bixiao Zhao, Yalai Bai, Atila Iamarino, Stephen G. Gaffney, Joseph Schlessinger, Richard P. Lifton, David L. Rimm, and Jeffrey P. Townsend
From that patient pool, two had cancers (lung adenocarcinomas) that developed resistance to an EGFR targetted therapy. Further, they had greater than 5 samples, including normal somatic, primary sampling, and multiple metatises. 
For their biological and biomedical interest, as well as the sampling robustness, they make for good data to prototype the methodology employeed here.

The second set of day come from a collaboration with Gilead (which I believe is unpublished [check this]) but has been approved for my use in the project at present. From there, I have usable whole exome data from 17 patients (4 excluded for quality reasons). These patients all have at least 3 samples; normal somatic, pre treatment, and post treatment. 

The human exome sequencing data are paired with patient medical histories. The medical histories have been well-annonomized and the sequencing data has been previously published or otherwise made available. 
Variants have been previously called; however, the raw reads have been retained and will be consulted in case of anomalousness. 

--Illumina sequencing, but need to check on the kit used to enrich for exome and what specific sequencer was used. 
## Background

Implementation of these evolutionary techniques affords opportunities not only to further understand the nature of tumorigenesis and the acquisition of therapeutic resistance, but also to guide the continuing treatment of individuals while identifying the most important mutations at the population level towards which funding and time can be directed. 
Continued development and application of these techniques will ultimately encapsulate other somatic aberrations, such as copy number variation, and concurrently incorporate them into measures of selection intensity.
In non-smoker lung carcinomas, EGFR mutations are incredibly common and, thus, a great target for the synthesis of topological information and effect size calculation in an expected way as a proof of concept for the utility of the methods described here. 
Indeed, a small case study of 2 patients has already been completed and is pending publication; however, 2 patients does not give sufficient power to answer questions of effect size. 


--I think some of my goal section can be moved here.

--A bit more about EGFR

--A bit more about lung carcinmoas


## Methods
--Maybe validate SNV calls?

--Also investigate using CNVs to constrain clades (subclones)

IQTree for ML estimation of tree

BEAST for Chronogram 

  -birth death model

  -coalescent

  -GTR 

Ancestral state reconstruction in phangorn 

 -investigate using parameters optimized in BEAST to do so

Use ggtree for visualization? 

CancerEffectSize.R https://github.com/Townsend-Lab-Yale/cancereffectsizeR

Investigate structural methods if time permits.


## Results


## Assessment

Was it successful in achieving the initial goal?

What are the main obstacles encountered?

What would you have done differently?

What are future directions this could go in?

## References
