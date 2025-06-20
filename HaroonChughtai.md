# ReDAI (Research Data for AI) - Information Capture Sheet

## Project background
| Question    | Response |
| -------- | ------- |
| Project Title | Haroon's PhD - Machine learning approaches for accelerated dementia MRI |
| Principal Investigator and any other key contacts (name, department, email address, etc) | Haroon Chughtai |
| External funder(s) (if any) [[1]](#endnote-1) | ADMIRA is funded by UCLH and Alzheimers Society. Haroon's PhD is being funded and hosted by the  Hawkes Institute |
| Project partners | Geoff Parker and Danny Alexander are supervisors. Data provider is National Hospital for Neurology and Neurosurgery (NHNN), which is part of UCL - project which is capturing data is called ADMIRA (Accelerated MRI for Alzheimer's Disease). ADMIRA PI is Geoff Parker. |
| Short summary of research purpose | See title for the moment |
| Describe the AI component of the research [[2]](#endnote-2) | Using paired (i.e. same patient in same scanner) and deidentified clinical and fast MRI scans to train a supervised model to predict clinical scans from fast scans. Fast scans can be performed at 63% the time of a clinical quality scan. Motivating factors: save time, more patients can be treated, increases accessibility, individuals spend less time in the scanner. Elderly people may struggle with MRI as it's a loud and enclosed environment. |
| Describe the data collection (or access) process. Will you be creating/capturing original data, or reusing existing data? [[3]](#endnote-3) | Reusing ADMIRA data |
| If reusing third-party data, will (e.g.) data access or sharing agreements be in place? Is copyright an issue? [[4]](#endnote-4) | No separate DSA or consent required, as analysis/training is done on deidentified images |
| Does the research require any specific forms of High Performance Computing? [[5]](#endnote-5) | Some of the analysis carried out on HC's laptop, some on a desktop PC under HC's office desk at work (which houses a GPU, which means to queueing), and some on UCL Computing Science HPC. May use ARC's Myriad system in the future. |

## About the data and models

| Question | Input/training data | AI model | Output data |
| -------- | ------- | -------- | ------- |
| Short description of what it is  | Deidentified fast and clinical MRI scans |  Pytorch based model - convolutional neural network (CNN)  |  Reconstructed clinical quality scans   |
| Will the data be sensitive (ethically, commercially or for security reasons)? [[6]](#endnote-6) [[7]](#endnote-7) |  No as scans are deidentified   | No | No |
| If yes, what protective measures will be put in place? (participant consent, anonymisation, encryption, access controls, etc) | N/A  | N/A |  |  
| What data/file formats will be used?  | DICOM  |  Pytorch, Onnx  | NIFTI |
| What is the scale of data volume? (MB/GB/TB/PB) |  100s of GB  |  Few GB |  100s of GB   |
| Does your data comprise large files (>4GB) or many small files, or a mixture? |  Many small files (100s per scan, approx 200 scans) - maybe 40,000   |  Single large file probably | A few large files  |
| Where will the data be stored during the project? | XNAT. Dowloaded to ARC's RDSS and mounted onto compute to perform analysis | RDSS |  RDSS   |
| How will it be protected/backed-up? | Role-based project access, backed up by CS according to their policy |  RDSS bacckup regimne  |  RDSS backup regime   |
| Who will be responsible for data documentation/creating metadata? [[8]](#endnote-8) | Haroon himself - split role as PhD student and ARC staff |  HC  |   HC  |

## After the project

| Question | Input/training data | AI model | Output data |
| -------- | ------- | -------- | ------- |
| What data will you want to keep for the longer-term? (types, volumes, etc) [[9]](#endnote-9) | This belongs to ADMIRA project so it's their call | Model in entirety | Output data in entirety  |
| Where will it be stored? [[10]](#endnote-10) | As above | RDSS at first, then made available via HuggingFace/ Research Data Repository (figshare) | RDR - note that it would be great if RDR could render DICOM/NIFTI files, but that's a figshare feature request |
| How will longer-term storage be resourced? | N/A | ARC/HuggingFace | ARC  |
| Do any additional materials (code etc) need to be kept in order to support longer-term reproducibility? Where will they be stored? [[11]](#endnote-11) | Code for data preprocessing, and deploying the model - currently on GitHub, expected to remain there. |

## About
| Question | Response |
| -------- | ------- |
| Information provided by (project member): | Haroon Chughtai |
| Any other comments from interviewee? | |
| Information collected by (ARC member): | Martin Donnelly |
| Any other comments from interviewer? | |
| Date of information collection: | 12 June 2025 |

**NOTES FOR FORM REVISION:
**Does the research require any specific forms of High Performance Computing? - this question is ambiguous, perhaps reword to "specific compute resources"? "What compute resources are used/required/expected?" something like that
Change about the data to avout data and m,odels 
Second section is too data-centric - revise language to be more open 
Addd "affiliation" to "department" in admin info 

### Endnotes
1. Does the external funder have a research data policy, or is a data access agreement or plan in place/required? If a data management plan is required, create one using [DMPonline](https://dmponline.dcc.ac.uk/). [↑](#endnote-ref-1)
2. You should consider issues around Effectiveness, Fairness and Transparency here. See the ReDAI (Research Data for AI) service page and the Unified AI documentation – links to follow. [↑](#endnote-ref-2)
3. Useful resources: [UCL’s Harbour service](https://www.ucl.ac.uk/advanced-research-computing/harbour-ucls-external-data-service) for accessing third-party data; [re3data](https://www.re3data.org/) – the registry of research data repositories. [↑](#endnote-ref-3)
4. Link to Library's copyright advice page? [↑](#endnote-ref-4)
5. If HPC = Yes, see <https://github.com/ucl-arc/condenser-users> [↑](#endnote-ref-5)
6. Does the data management environment require specific accreditation, e.g. NHS DSP Toolkit, ISO27001, etc? If so, see [UCL’s Information Governance pages](https://www.ucl.ac.uk/isd/user/login?destination=node/4175). [↑](#endnote-ref-6)
7. If ethically sensitive, consult the [UCL Research Ethics Service](https://www.ucl.ac.uk/research-innovation-services/compliance-and-assurance/research-ethics-service). If personal data will be processed, a Data Protection Impact Assessment (DPIA) is likely to be required. [↑](#endnote-ref-7)
8. Useful resource: [ARC metadata model](https://liveuclac-my.sharepoint.com/personal/ccaemdo_ucl_ac_uk/Documents/UCL%20%282023-%29/Unified%20AI/ARC%20metadata%20model%20-%20https%3A/liveuclac.sharepoint.com/sites/RITSstaff/Shared%20Documents/Forms/AllItems.aspx?csf=1&web=1&e=KDvi6V&CID=fcdeb7ee%2D1c19%2D425f%2Db45f%2Da2be2d43fa25&FolderCTID=0x01200008C0B7F85E2CFC4F92262A497FFA8D20&id=%2Fsites%2FRITSstaff%2FShared%20Documents%2FData%20Stewardship%2FARC%20Metadata%20Model) [↑](#endnote-ref-8)
9. [UCL Library guidance](https://www.ucl.ac.uk/library/open-science-research-support/research-data-management/best-practices/how-guides/archiving) on identifying a suitable repository, determining what should be kept and what can be safely discarded, etc. [↑](#endnote-ref-9)
10. Link to UCL guidance on recommended long-term storage (to follow) [↑](#endnote-ref-10)
11. Useful resources: [HuggingFace](https://huggingface.co/); [GitHub](https://github.com/). [↑](#endnote-ref-11)

If you need help completing this form, please use MyServices (link) to contact the Research Data Stewards team.
