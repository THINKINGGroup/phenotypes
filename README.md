[![CC BY 4.0][cc-by-shield]][cc-by]

# About
This repository contains code lists created using the DExtER Code Builder tool, developed at the University of Birmingham.
Code Builder allows you to search for medical codes and drug codes across different medical databases such as SnomedCT, Read codes and HES simultaneously and export the results. Here you can find code lists for app. 150 medical conditions and app. 75 medications.

## Data dictionary
Each of the medical conditions and medications is in a separate folder (named for the medical condition or drug) and each of the folders contain CSV files for each of the databases that were searched, e.g. CPRD AURUM, CPRD GOLD, IMRD.

Below you can see an explanation for each of the columns of the CSV files, separately for the drug and medical condition lists.

### Drug codes

| Column name             | Description |
| ----------------------- | ----------- |
| `DRUG_CODE_ID`          | The actual term stored in the drug database. This might be a number, a short string, or a hexadecimal value. |
| `DESCRIPTION`           | The text description of the drug code. This will also include (where available) the drug substance, strength, route of administration etc. |
| `BNF1`, `BNF2`, `BNF3` | The BNF codes from this pseudo-classification are used in the prescribing dataset as a unique identifier to show what was prescribed. These BNF codes can tell you a lot about a drug or appliance. [Read more about BNF codes.](https://digital.nhs.uk/data-and-information/areas-of-interest/prescribing/practice-level-prescribing-in-england-a-summary/practice-level-prescribing-glossary-of-terms)|
| `ATC`                   | This stands for the "Anatomical Therapeutic Chemical Classification System", a drug classification system that classifies the active ingredients of drugs according to the organ or system on which they act and their therapeutic, pharmacological, and chemical properties. [Read more about ATC codes.](https://www.whocc.no/atc_ddd_index/)|
| `DATABASE`              | The database queried. |

### Medical condition codes

| Column name       | Description |
| ----------------- | ----------- |
| `MEDICAL_CODE_ID` | The actual term stored in the medical database. This might be a number, a short string, or a hexadecimal value.  |
| `DESCRIPTION`     | This is the text description of the medical code. |
| `READ_CODE`       | Read Codes are a coded thesaurus of clinical terms that have been used in the NHS since 1985. They provide a standard vocabulary for clinicians to record patient findings and procedures, in health and social care IT systems across primary and secondary care. [Read more about Read Codes](https://digital.nhs.uk/services/terminology-and-classifications/read-codes). | 
| `SNOMED_CT_CODE`  | SNOMED CT is a structured clinical vocabulary for use in electronic health records. It is the most comprehensive and precise clinical health terminology product in the world. [Read more about SNOMED CT](https://digital.nhs.uk/services/terminology-and-classifications/snomed-ct). |
| `DATABASE`        | The database queried. |

## Licence
You are free to reuse and adapt the contents of this repository, as long as you provide appropriate attribution by citing the creators of this work and noting what adaptations you have made. See the [LICENCE file](/LICENCE) for the full terms.

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
