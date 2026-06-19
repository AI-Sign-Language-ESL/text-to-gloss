\# AraT5 Model



\## Description



This folder contains the fine-tuned AraT5v2-base-1024 model used for Arabic-to-Gloss translation in the TAFAHOM project.



The model translates Arabic text into Egyptian Sign Language (EgSL) gloss representations.



\---



\## Model Information



| Item       | Value                        |

| ---------- | ---------------------------- |

| Base Model | AraT5v2-base-1024            |

| Task       | Arabic to Gloss Translation  |

| Language   | Arabic                       |

| Output     | Egyptian Sign Language Gloss |



\---



\## Files



\* model.safetensors

\* config.json

\* generation\_config.json

\* tokenizer\_config.json

\* special\_tokens\_map.json

\* spiece.model

\* added\_tokens.json



\---



\## Example



Input:



كيف حالك



Output:



حال كيف



\---



\## Usage



```python

from transformers import AutoTokenizer, AutoModelForSeq2SeqLM



model\\\_path = "AraT5"



tokenizer = AutoTokenizer.from\\\_pretrained(model\\\_path)

model = AutoModelForSeq2SeqLM.from\\\_pretrained(model\\\_path)

```

