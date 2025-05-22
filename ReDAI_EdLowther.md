# ReDAI (Research Data for AI) - Information Capture Sheet

## About
| Question | Response |
| -------- | ------- |
| Information provided by (project member): | Ed Lowther, PhD candidate |
| Information collected by (ARC member): | Martin Donnelly |
| Date of information collection: | 21 May 2025 |

## Project background
| Question | Response |
| -------- | ------- |
| Project Title | PhD - a new method of time-series analysis for different types of data (multi-modal) |
| Principal Investigator and any other key contacts (name, department, email address, etc) | Ed Lowther |
| External funder(s) (if any)[[1]](#endnote-1) | |
| Project partners | Moorfields Eye Hospital, UCL Ophthalmology |
| Short summary of research purpose | Anticipating likely clinical outcomes for glaucoma patients. Glaucoma is a degenerative condition. Not known why some patients deteriorate more quickly than others. |
| Will you be creating/capturing original data, or reusing existing data?[[4]](#endnote-4) | Reusing existing anonymised/depersonalised datasets |
| Describe the AI component of the research[[2]](#endnote-2) | Training a machine-learning model, learning lots of parameters |
| Does the research require High Performance Computing?[[3]](#endnote-3) | Not currently able to use ARC infrastructure. Data currently stored on UCL's computing science cluster. Potential to utilise ARC's TRE.|

## About the data

(N.B. If you are creating/using multiple datasets, just add another column to this table)

| Question | Dataset 1 |
| -------- | ------- |
| Short title of dataset | Alzeye. Ed may need to access BioBank dataset later, can expand this table to record info around that as and when. For more info on this dataset see https://bmjopen.bmj.com/content/12/3/e058552 |
| Describe the data collection (or access) process, e.g. for reusing third-party data. For example, will data sharing agreements be in place? | Not an open dataset - data sharing agreements between NHS digital, Moorfields and UCL. Ed had to join the Alzeye team in order to access dataset. Honorary contract with Moorfields. |
| Will the data be sensitive (ethically, commercially or for security reasons)?[[5]](#endnote-5) [[6]](#endnote-6) | Anonymised, non-sensitive - but access is restricted. |
| If yes, what protective measures will be put in place? (participant consent, anonymisation, encryption, access controls, etc) | Access is controlled via SSH to HPC resource. |
| What data/file formats will be used? | Multiple data sets, inc. Image data. ECT scans of eyes. 3D arrays. 2D images. Tabular data/metadata, dates of appointment etc. |
| What is the scale of data volume? (MB/GB/TB/PB) | Full dataset is 18 TB approx. Ed currently only interested in a subset of this, but interest may broaden in time! |
| Does your data comprise large files (>4GB) or many small files, or a mixture? | Image files can be gigabyte scale. Tabular data much smaller. Small number of large files, large number of small-to-medium files. |
| Where will the data be stored during the project? | UCL Computing Science cluster. On premises. |
| How will it be protected/backed-up? | Backed up by in-house team. |
| Who will be responsible for data documentation/creating metadata? [[7]](#endnote-7) | Metadata created by original research team (Alzeye) |

## After the project

| Question | Response |
| -------- | ------- |
| What data will you want to keep for the longer-term? (types, volumes, etc)[[8]](#endnote-8) | Not yet known! Results/evidence. |
| Where will it be stored? | Where it already is. |
| How will longer-term storage be resourced? | Not known - dealt with by CS colleagues. |
| What additional materials (code, models, etc) must be kept in order to support longer-term reproducibility? Where will they be stored?[[9]](#endnote-9) | AI model will be shared if it works! Likely to be shared via HuggingFace unless anything major changes in the meantime. |

Any other notes?
- Add an any other comments field (MD)
- Need to separate training data from output data/results, and consider model more equitably. (MD)
- Is there an easy way to spellcheck GitHub pages? (MD)
- Need to create a dedicated repository for this. Within UCL-ARC?

### Endnotes

1. Does the external funder have a research data policy, or is a data access agreement or plan in place/required? If a data management plan is required, create one using [DMPonline](https://dmponline.dcc.ac.uk/). [↑](#endnote-ref-1)
2. You should consider issues around Effectiveness, Fairness and Transparency here. See the ReDAI (Research Data for AI) service page and the Unified AI documentation – links to follow. [↑](#endnote-ref-2)
3. If HPC = Yes, see <https://github.com/ucl-arc/condenser-users> [↑](#endnote-ref-3)
4. Useful resources: [UCL’s Harbour service](https://www.ucl.ac.uk/advanced-research-computing/harbour-ucls-external-data-service) for accessing third-party data; [re3data](https://www.re3data.org/) – the registry of research data repositories. [↑](#endnote-ref-4)
5. Does the data management environment require specific accreditation, e.g. NHS DSP Toolkit, ISO27001, etc? If so, see [UCL’s Information Governance pages](https://www.ucl.ac.uk/isd/user/login?destination=node/4175). [↑](#endnote-ref-5)
6. If ethically sensitive, consult the [UCL Research Ethics Service](https://www.ucl.ac.uk/research-innovation-services/compliance-and-assurance/research-ethics-service). If personal data will be processed, a Data Protection Impact Assessment (DPIA) is likely to be required. [↑](#endnote-ref-6)
7. Useful resource: [ARC metadata model](https://liveuclac-my.sharepoint.com/personal/ccaemdo_ucl_ac_uk/Documents/UCL%20%282023-%29/Unified%20AI/ARC%20metadata%20model%20-%20https%3A/liveuclac.sharepoint.com/sites/RITSstaff/Shared%20Documents/Forms/AllItems.aspx?csf=1&web=1&e=KDvi6V&CID=fcdeb7ee%2D1c19%2D425f%2Db45f%2Da2be2d43fa25&FolderCTID=0x01200008C0B7F85E2CFC4F92262A497FFA8D20&id=%2Fsites%2FRITSstaff%2FShared%20Documents%2FData%20Stewardship%2FARC%20Metadata%20Model) [↑](#endnote-ref-7)
8. [UCL Library guidance](https://www.ucl.ac.uk/library/open-science-research-support/research-data-management/best-practices/how-guides/archiving) on identifying a suitable repository, determining what should be kept and what can be safely discarded, etc. [↑](#endnote-ref-8)
9. Useful resources: [HuggingFace](https://huggingface.co/); [GitHub](https://github.com/). [↑](#endnote-ref-9)

If you need help completing this form, please use MyServices to contact the Research Data Stewards team.
