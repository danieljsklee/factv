# FACT-V: Factual Accuracy in Content Translation to Video

[**Task Description**](#task-description) |
[**FactT2V-50**](#wikikge-10) |
[**Paper**](Paper Link TBD) |
[**Citation**](#citation) |
[**License**](#license)

Text-to-Video (T2V) models, despite recent advancements, struggle with factual accuracy, especially for knowledge-dense content. We introduce FACT-V (Factual Accuracy in Content Translation to Video), a system integrating multi-source knowledge retrieval into T2V pipelines. FACT-V offers two key benefits: i) improved factual accuracy of generated videos through dynamically retrieved information, and ii) increased interpretability by providing users with the augmented prompt information. A lightweight evaluation demonstrates the potential of knowledge-augmented approaches in improving T2V systems' accuracy and reliability, particularly for entity-specific or time-sensitive prompts.

Please refer to our (Under Review) paper for more details, [Rewind and Render: Towards Factually Accurate Text-to-Video Generation with Distilled Knowledge Retrieval](Paper Link TBD). 

## Task Description

## FactT2V-50
Description

### Dataset Organization (example placed)
The data is organized in the following way:
```
data
└── prompts
    ├── t2vprompts.json
    ... ...

└── videos
    ├── runwaygen-2
    │   ├── standard
    │   │   ├── 1.mp4
    │   │   ├── 2.mp4
    │   ├── factv
    │   │   ├── ar.m-nta.json
    │   │   ├── de.m-nta.json
    ... ...
    ├── runwaygen2-factv
    │   ├── 1.mp4
    │   ├── 2.mp4
    ... ... ...
    │   ├── cogvideox2b
    │   ├── 1.mp4
    │   ├── 2.mp4
    ... ... ...
    │   └── cogvideox2b
    │   ├── 1.mp4
    │   ├── 2.mp4
    ... ...

```
Where:
* `data/prompts/t2vprompts.json` contains the t2v prompts.
* `data/videos/...` contains the video
* `data/names/gpt/` contains the predictions from GPT-3 and GPT-3.5 (May 2023), and also GPT-4 (September 2023).
* `data/names/wikidata/` contains the data from Wikidata (May 2023).

## Citation
Please cite our work if you found FACT-V, our [paper](), or these resources useful.

```bibtex
tbd
```
