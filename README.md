# Tra(c)king SDGs in the European Framework Programmes
## Introduction
In 2015, the Sustainable Development Goals (SDGs) were introduced as a universal call to action to end poverty, protect the planet, and ensure prosperity for all by 2030
Our project monitors how the European Union's research funding programs, starting from 1984, have supported these goals.
We use textual analysis and the lexicon of the [EU Joint Research Centre](https://knowsdgs.jrc.ec.europa.eu/sdgmapper) to check the alignment of funded research projects, listed on [CORDIS](https://cordis.europa.eu/), with the SDGs.
We provide a comprehensive dataset that associates these projects with the 17 SDGs and their 169 specific targets, as well as, an interactive dashboard **[insert ref here]** that is regularly updated with new data and insights. 

## Methodology
We refer to Boudt et al. (2024) to get the full methodology. We deviate from this paper by including all projects, not just those coordinated by research-oriented entities.

## Dataset
Below is a breakdown of the dataset's components:

- **`projectID`**: A unique identifier for each research project.

- **`acronym`**: The official shorthand or acronym associated with the research project.

- **`frameworkProgramme`**: IThe Framework Programme that funded the research project

- **`title`**: The formal title of the research project.

- **`abstract`**: The abstract of the research project.

- **`startingDate`**: The official start date of the project.

- **`endingDate`**: The project's designated conclusion date.

- **`budget`**: The total funding amount allocated to the project (in EUR).

- **`SDG dummies`**: A set of binary (dummy) variables representing each of the 17 SDGs. A project is marked with a '1' for a specific SDG if it is determined to align with that goal based on keyword analysis, and '0' otherwise. 

- **`target dummies`**: Similar to the SDG dummies, these binary variables are linked to the 169 specific targets under the 17 SDGs. They indicate whether a project aligns with specific targets.

- **`detected words`**: A list of keywords from the project's title and abstract that were identified as relevant to the SDGs, based on the lexicon used for textual analysis. 

- **`coordinatorName`**: Name of the coordinator.

- **`coordinatorCountry`**: Country of origin of the coordinator
 
- **`nPartners`**: The number of partners involved in the project.

## Citation
If you use data or insights derived from this project in your research, presentations, or publications, please cite the following work:

Boudt, K., Inghels, Y., & Spithoven, A. (2024). Trac(k)ing the trajectory: Mapping Sustainable Development Goal 8 in EU-funded research projects (No. 24/1084). Ghent University, Faculty of Economics and Business Administration.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

## Contact
For questions, suggestions, or collaborations, please contact yanick.inghels@ugent.be.
