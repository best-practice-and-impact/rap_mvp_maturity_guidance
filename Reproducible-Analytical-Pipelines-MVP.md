# Reproducible Analytical Pipelines Minimum Viable Product Guidance (RAP MVP)

## Things to be aware of

This guidance has been agreed upon by a working group of the [Reproducible Analytical Pipelines Champion](https://gss.civilservice.gov.uk/about-us/champion-networks/reproducible-analytical-pipeline-rap-champions/).
It will be reviewed periodically by the RAP Champions and the Best Practice and Impact data science team.

Your department may have standards that you have to work to when it comes to writing code or developing analytical products.
This guidance is a general set of advice and guidelines for any and all analytical pipelines.
Producers of analysis may incorporate some or all of these guidelines into their work depending on their needs and users.

## Introduction

### Reproducible analytical pipelines are a guarantee for users and producers

In the future, analytical processes should be reproducible to a proportionate level.
They must be backed up by a clear history of analytical decisions and implementation.
Good quality assurance processes will help to identify errors or upstream changes quicker.
Working in the open, these reproducible analytical pipelines will guarantee to users and producers alike that the analysis is trustworthy, high-quality and efficient.

### Who is this guidance for?

This guidance is for official statisticians and analysts working in the UK government.
This guidance may also be helpful for users of official statistics.

This guidance has been developed by the Best Practice and Impact division at the Office for National Statistics.
The Best Practice and Impact division supports government analysis by providing guidance, consultancy and training.

### Lessons learned in software engineering can be translated to official statistics and analysis

For producers, processes for analysis have often been constrained by inappropriate, proprietary software that makes them inefficient and quality assurance difficult.
This has caused frustration for producers and their managers as quality issues recur and analysis becomes resource-intensive.
Developing bespoke software using some best practices from software engineering helps to alleviate this.

The practices we suggest should:
- improve the quality of the analysis,
- increase trust in ther analysis by producers, their managers and users,
- create a more efficient process,
- and improve business continuity and knowledge management.

Users must trust the processes by which government analysis, research and statistics are produced.
Trust is diminished where processes are not transparent or produce low quality outputs.
When analysts and reserachers work in the open they increase transparency about both how the analysis is produced and to what degree of quality.

## The RAP Minimum Viable Product

In order to achieve these benefits, at a minimum a RAP must:
- Augment extant technical and quality assurance processes with **peer review** to ensure that the process is reproducible and that the below requirements have been met.
- **Minimise manual steps**, for example copy-paste, point-click or drag-drop steps. Where it is absolutely necessary to include a manual step in the process this must be documented as described below. 
- Be built using **open source software** which is available to anyone, preferably R or python.
- Guarantee an **audit trail** using version control software, preferably Git.
- Be **open to anyone**. This can be facilitated most easily through the use of file and code sharing platforms.
- Follow **existing good practice for quality assurance** - guidance set by departments or organisations, and by the Good Practice Team for the Government Statistical Service.
- Contain **well-commented** code and have **documentation embedded** within the product, rather than saved elsewhere.


Notes:
- There may be restrictions, such as access to databases, which stop analysis producers building a RAP for their full end-to-end process. In this case, the above requirements apply to the selected part of the process.
- There may be restrictions, such as sensitive or confidential content, which stop analysis producers from sharing their RAP publicly. In this case, it may be possible to share the RAP within a department or organisation instead.
- It is recommended that when possible a RAP should be built collaboratively - this will improve the quality of the final product and helps to facilitate knowledge sharing.
- There is not a specific tool that is required to build a RAP, but both R and Python provide the power and flexibility to carry out end-to-end analytical processes, from data source to final presentation.

### Further RAP developments
- Functions/code modularity
- Unit testing of functions
- Error handling for functions
- Documentation of functions
- Package
- Code style
- Input data validation
- Logging of data
- Continuous integration
- Dependency management
- Containerisation
