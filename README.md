<!--
SPDX-FileCopyrightText: 2026 Eugenie Modolo <eugenie@modolo.fr>

SPDX-License-Identifier: AGPL-3.0-or-later
-->

# cancer_survival

## Objective
Project using the existing model [BulkRNABert](https://huggingface.co/InstaDeepAI/BulkRNABert) in order to predict the survival (OS and/or PFS) of patients based on the transcriptome (bulk RNA-Seq) of their tumor biopsy.


## Files structure

- root:
	* .gitmodules: Git configuration
	* requirements.txt: dependencies required to run the project locally
	* README.md: general project documentation

- BulkRNABert: external repository cloned via the Git tool submodules

- data: folder used for the project's data: bulk RNA-Seq and clinical data from 193 patients (25 with pancreatic cancer, 67 with cervix carcinoma and 101 with endometrial carcinoma). They are not loaded into this repository as they contain sensible information

- LICENSES: folder used for the project's license (GNU AFFERO GENERAL PUBLIC LICENSE)

- model: Machine- and Deep Learning models developed in-house for this project

- results: folder used for the project's results and temporary files. They are not loaded into this repository as they contain sensible information

- src: source codes
	* model: BulkRNABert model downloaded from [Hugging Face](https://huggingface.co/InstaDeepAI/BulkRNABert)
	* Notebooks: elements of data exploration and model eligibility testing


## Local environment 

### Prerequisite

- python 3.11.x

### Installation

The following commands create the virtual environment, activate it, and install the dependencies listed in the file requirements.txt.

Windows:

```
python3 -m venv .venv

.\.venv\Scripts\Activate.ps1

uv pip install -r requirements.txt
```

Mac/Linux:

```
python3 -m venv .venv

source .venv/bin/activate

uv pip install -r requirements.txt
```


