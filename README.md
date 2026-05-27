<!--
SPDX-FileCopyrightText: 2026 Eugenie Modolo <eugenie@modolo.fr>

SPDX-License-Identifier: AGPL-3.0-or-later
-->

# cancer_survival
Project using the existing model BulkRNABert (https://huggingface.co/InstaDeepAI/BulkRNABert) in order to predict the survival (OS and/or PFS) of patients based on the transcriptome (bulk RNA-Seq) of their tumor biopsy.

# Environnement local

## Prérequis

- python 3.11.x

## Installation

Les commandes suivantes créent l'environnement virtuel, l'activent et installent les dépendances listées dans le fichier requirements.txt.

Windows :

python3 -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt

Mac/Linux :

python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

