\# Gloss LoRA Adapter



\## Description



This folder contains the LoRA adapter fine-tuned for Arabic-to-Gloss translation.



The adapter is applied on top of the AraT5 base model.



\---



\## Model Information



| Item       | Value                       |

| ---------- | --------------------------- |

| Method     | LoRA Fine-Tuning            |

| Task       | Arabic to Gloss Translation |

| Base Model | AraT5v2-base-1024           |



\---



\## Files



\* adapter\_model.safetensors

\* adapter\_config.json

\* tokenizer.json

\* tokenizer\_config.json

\* special\_tokens\_map.json



\---



\## Usage



```python

from transformers import AutoModelForSeq2SeqLM

from peft import PeftModel



base\_model = AutoModelForSeq2SeqLM.from\_pretrained("AraT5")



model = PeftModel.from\_pretrained(

&#x20;   base\_model,

&#x20;   "gloss\_lora"

)

```



