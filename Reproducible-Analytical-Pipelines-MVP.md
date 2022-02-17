# Reproducible Analytical Pipelines Minimum Viable Product Guidance (RAP MVP)

## Things to be aware of

This guidance has been agreed by a working group of the [Reproducible Analytical Pipelines Champions](https://gss.civilservice.gov.uk/about-us/champion-networks/reproducible-analytical-pipeline-rap-champions/).
It will be reviewed periodically by the RAP Champions and the Reproducible Analytical Pipelines team in Methodology and Quality Directorate at the Office for National Statistics.

Your department may have standards that you have to work to when you are writing code or developing analytical products.
This guidance is a general set of advice and guidelines for any and all analytical pipelines.
Producers of analysis may incorporate some or all of these guidelines into their work depending on their needs and users.

## Introduction

### Reproducible analytical pipelines are a guarantee for users and producers

Analytical processes should be reproducible to a proportionate level.
They must be backed up by a clear history of analytical decisions and implementation.
Good quality assurance processes will help to identify errors or upstream changes more quickly.
Working in the open, these reproducible analytical pipelines will guarantee to users and producers alike that the analysis is trustworthy, high-quality and efficient.

### Who is this guidance for?

This guidance is for official statisticians and analysts working in the UK government.
The guidance may also be helpful for users of official statistics or other government analysis.

This guidance has been developed by the Reproducible Analytical Pipelines (RAP) team in the Methodology and Quality Directorate at the [Office for National Statistics](https://www.ons.gov.uk/aboutus).
Methodology and Quality Directorate supports government analysis by providing guidance, consultancy and training. We do this for the [Analysis Function](https://www.gov.uk/government/organisations/government-analysis-function).

### Lessons learned in software engineering can be translated to official statistics and analysis

For producers of analysis, processes have often been made harder by inappropriate, proprietary software. This makes them inefficient and difficult to quality assure.
This has caused frustration for producers and their managers as quality issues recur and analysis becomes resource-intensive.
Developing bespoke software using some best practices from software engineering helps to alleviate this.

The practices we suggest should:
- improve the quality of the analysis
- increase trust in the analysis by producers, their managers and users
- create a more efficient process
- improve business continuity and knowledge management

Users must trust the processes by which government analysis, research and statistics are produced.
Trust is reduced when processes are not transparent or produce low quality outputs.
When analysts and researchers work in the open they increase transparency about how the analysis is produced and to what degree of quality.

## The RAP Minimum Viable Product

In order to achieve these benefits, at a minimum a Reproducible Analytical Pipeline must:
- Minimise manual steps. Manual steps include copy and paste, point and click or drag and drop operations. Where it is absolutely necessary to include a manual step in the process this must be fully documented as described below.
- Be built using open source software which is available to anyone, preferably [python](https://www.python.org/) or [R](https://www.r-project.org/)
- Deepen technical and quality assurance processes with [peer review](https://best-practice-and-impact.github.io/qa-of-code-guidance/peer_review.html) to ensure that the process is reproducible and that the below requirements have been met
- Guarantee an audit trail using [version control software](https://best-practice-and-impact.github.io/qa-of-code-guidance/version_control.html#why-do-we-need-version-control), preferably Git
- Be [open to anyone](https://best-practice-and-impact.github.io/qa-of-code-guidance/project_documentation.html#open-source-your-code-span-role-image-aria-label-difficulty-rating-2-out-of-5-span). This can be done most easily by using file and code sharing platforms
- Follow existing good practice for quality assurance – guidance set by departments or organisations, and by the Analysis Function teams and Data Quality Hub for the Analysis Function and Government Statistical Service
- Contain [well-commented](https://best-practice-and-impact.github.io/qa-of-code-guidance/code_documentation.html#comments-span-role-image-aria-label-difficulty-rating-1-out-of-5-span) code and have [documentation embedded](https://best-practice-and-impact.github.io/qa-of-code-guidance/project_documentation.html) and version controlled within the product, rather than saved elsewhere


Notes:
- There may be restrictions, such as access to databases, which stop analysis producers building a RAP for their full end-to-end process. In this case, the above requirements apply to the selected part of the process.
- There may be restrictions, such as sensitive or confidential content, which stop analysis producers from sharing their RAP publicly. In this case, it may be possible to share the RAP within a department or organisation instead. You may be able to use synthetic data to make sharing possible.
- We recommend that when possible a RAP should be built collaboratively - this will improve the quality of the final product and helps to facilitate knowledge sharing.
- There is not a specific tool that is required to build a RAP. Both python and R provide the power and flexibility to carry out end-to-end analytical processes, from data source to final presentation.

### Further RAP developments
- Functions and code modularity
- Unit testing of functions
- Error handling for functions
- Documentation of functions
- Packaging code
- Code style
- Input data validation
- Logging of data
- Continuous integration
- Dependency management
- Containerisation
