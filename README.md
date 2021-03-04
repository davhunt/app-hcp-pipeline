[![Abcdspec-compliant](https://img.shields.io/badge/ABCD_Spec-v1.1-green.svg)](https://github.com/brain-life/abcd-spec)
[![Run on Brainlife.io](https://img.shields.io/badge/Brainlife-brainlife.app.465-blue.svg)](https://doi.org/10.25663/brainlife.app.465)

# app-hcp-pipeline

This App is a Brainlife wrapper for [HCP Pipelines](https://github.com/Washington-University/HCPpipelines). The HCP Pipelines product is a set of tools for processing Magnetic Resonance Imaging (MRI) images for the [Human Connectome Project](https://www.humanconnectome.org/). In particular, this App implements the structural preprocessing, and uses the [BIDS-app wrapper](https://github.com/BIDS-Apps/HCPPipelines), which consists of a container that includes all of the dependencies and a run script that parses a BIDS dataset (this is the reason why the latest version of this App may not correspond to the latest released version of the HCP Pipelines).

#### References and resources to consider
* HCP Pipelines main repository: https://github.com/Washington-University/HCPpipelines
* HCP Pipelines BIDS-app wrapper: https://github.com/BIDS-Apps/HCPPipelines

### Authors
- Giulia Bertò ([@giulia-berto](https://github.com/giulia-berto))
- Soichi Hayashi ([@soichih](https://github.com/soichih))

### Project director
- Franco Pestilli ([@francopestilli](https://github.com/francopestilli))

### Funding Acknowledgement
brainlife.io is publicly funded and for the sustainability of the project it is helpful to Acknowledge the use of the platform. We kindly ask that you acknowledge the funding below in your code and publications. Copy and past the following lines into your repository when using this code.

[![NSF-BCS-1734853](https://img.shields.io/badge/NSF_BCS-1734853-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1734853)
[![NSF-BCS-1636893](https://img.shields.io/badge/NSF_BCS-1636893-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1636893)
[![NSF-ACI-1916518](https://img.shields.io/badge/NSF_ACI-1916518-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1916518)
[![NSF-IIS-1912270](https://img.shields.io/badge/NSF_IIS-1912270-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1912270)
[![NIH-NIBIB-R01EB029272](https://img.shields.io/badge/NIH_NIBIB-R01EB029272-green.svg)](https://grantome.com/grant/NIH/R01-EB029272-01)

### Citations
We ask that you cite the following articles when publishing papers that used data, code or other resources created by the brainlife.io community.

1. Glasser MF, Sotiropoulos SN, Wilson JA, Coalson TS, Fischl B, Andersson JL, Xu J, Jbabdi S, Webster M, Polimeni JR, Van Essen DC, Jenkinson M; WU-Minn HCP Consortium. The minimal preprocessing pipelines for the Human Connectome Project. Neuroimage. 2013 Oct 15;80:105-24. doi: 10.1016/j.neuroimage.2013.04.127. Epub 2013 May 11. PMID: 23668970; PMCID: PMC3720813. https://pubmed.ncbi.nlm.nih.gov/23668970/

2. Avesani, P., McPherson, B., Hayashi, S. et al. The open diffusion data derivatives, brain data upcycling via integrated publishing of derivatives and reproducible open cloud services. Sci Data 6, 69 (2019). [https://doi.org/10.1038/s41597-019-0073-y](https://doi.org/10.1038/s41597-019-0073-y)

## Running the App 

### On Brainlife.io

Check out the brainlife app [here](https://doi.org/10.25663/brainlife.app.465)

### Running Locally

Information on how to run HCP Pipelines locally can be found here:
https://github.com/Washington-University/HCPpipelines/wiki/Installation-and-Usage-Instructions

### Inputs

The structural prepocessing is subdivided into 3 parts (Pre-FreeSurfer processing, FreeSurfer processing, and Post-FreeSurfer processing), and requires at least one T1w and one T2w scan. If you input a freesurfer folder (optional), the FreeSurfer step will be skipped.

### Outputs

A folder containing all the outputs.

### Dependencies

This App requires [singularity](https://www.sylabs.io/singularity/) to run. If you don't have singularity, you will need to install following dependencies. It also requires [jq](https://stedolan.github.io/jq/).

---

#### MIT Copyright (c) brainlife.io

<sub> This material is based upon work supported by the National Science Foundation Graduate Research Fellowship under Grant No. 1342962. Any opinion, findings, and conclusions or recommendations expressed in this material are those of the authors(s) and do not necessarily reflect the views of the National Science Foundation. </sub>
