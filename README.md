\# Arabic Text-to-Gloss Translation for Egyptian Sign Language



\## TAFAHOM Graduation Project



This repository contains the AI models used in the TAFAHOM platform for translating Arabic text into Egyptian Sign Language (EgSL) gloss representations.



\---



\## Project Goal



The objective of the project is to bridge the communication gap between hearing and deaf individuals using Artificial Intelligence and Sign Language technologies.



\---



\## Repository Structure



```text

text-to-gloss/

│

├── AraT5/

│   ├── README.md

│   └── model files

│

├── gloss\_lora/

│   ├── README.md

│   └── adapter files

│

├── README.md

└── LICENSE

```



\---



\## Dataset



\### Arabic-to-Gloss Dataset



| Item              | Value |

| ----------------- | ----- |

| Original Samples  | 624   |

| Augmented Samples | 2,726 |

| Total Samples     | 3,350 |



The dataset consists of Arabic sentence–gloss pairs used to train the translation model.



\---



\## Data Augmentation



A Blank Replacement (BR) augmentation strategy was applied to improve dataset diversity and model generalization.



\---



\## Model Performance



| Metric               | Score  |

| -------------------- | ------ |

| BLEU-1               | 77.96  |

| BLEU-4               | 64.91  |

| chrF++               | 72.81  |

| METEOR               | 0.6326 |

| Exact Match Accuracy | 11.94% |



\---



\## Models



\### AraT5



Fine-tuned AraT5v2-base-1024 model for Arabic-to-Gloss translation.



\### Gloss LoRA



Parameter-efficient LoRA adapter trained for the same translation task.



\---



\## Application



The models are part of the TAFAHOM platform, which supports:



\* Arabic Text to Sign Language Translation

\* Sign Language Avatar Generation

\* Accessibility Technologies

\* Communication Assistance for Deaf Individuals



\---



\## License



GPL-3.0 License



