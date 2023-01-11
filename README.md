[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
![Issues](https://img.shields.io/github/issues/Galsenaicommunity/Wolof-Common-Voice)
![PR](https://img.shields.io/github/issues-pr/Galsenaicommunity/Wolof-Common-Voice)

# Wolof-Common-Voice
Wolof Text Data Collection for recording on the Mozilla [Common Voice](https://commonvoice.mozilla.org/) platform.  
We use the Wolof part of the data collected by [Masakhane](https://www.masakhane.io/) during the [MasakhaNER project](https://github.com/masakhane-io/lacuna_pos_ner). The goal is to split them into sentences so that they can be recorded in the [best conditions](https://commonvoice.mozilla.org/sentence-collector/#/en/how-to) prescribed by Mozilla.

![Drag Racing](common-voice.png)

# Structure
The project is structured as follows:
```
.
├── data
│   └── raw <- initial data from the MasakhaNER project (cf eda-cleaning.ipynb)
│   ├── intermediate <- cleaned and adapted data to common voice specifications
│   ├── processed <- ready to upload data
```
# Upload
`Processed` data have to be uploaded on the [sentence collector](https://commonvoice.mozilla.org/sentence-collector/#/add) for review __by users__.

# ToDo
The corpus after processing (intermediate) contains `13400 sentences` in total: __2400__ in [part 1](data/intermediate/wolof_to_upload_part1.txt) and __11400__ in [part 2](data/intermediate/wolof_to_upload_part2.txt). We currently need to:

- [ ] Split the data (part 2) into batches of 2000 sentences  
- [ ] Clean the data to remove punctuation, special characters, numbers and abbreviations  
- [ ] Ensures that sentences do not exceed 14 words in length  
- [ ] Makes sure the sentences make sense to facilitate recording  
- [ ] Write a Wolof reading guide to enable users to read correctly  
- [ ] Making a tutorial on how to get started with the common voice platform  
- [ ] Organize a datathon to catalyze data collection  