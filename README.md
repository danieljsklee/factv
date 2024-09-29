# FACT-V: Factual Accuracy in Content Translation to Video

[**Task Description**](#task-description) |
[**FactT2V-50**](#wikikge-10) |
[**Paper**](Paper Link TBD) |
[**Citation**](#citation) |
[**License**](#license)

Text-to-Video (T2V) models, despite recent advancements, struggle with factual accuracy, especially for knowledge-dense content. We introduce FACT-V (Factual Accuracy in Content Translation to Video), a system integrating multi-source knowledge retrieval into T2V pipelines. FACT-V offers two key benefits: i) improved factual accuracy of generated videos through dynamically retrieved information, and ii) increased interpretability by providing users with the augmented prompt information. A lightweight evaluation demonstrates the potential of knowledge-augmented approaches in improving T2V systems' accuracy and reliability, particularly for entity-specific or time-sensitive prompts.

Please refer to our (Under Review) paper for more details, [Rewind and Render: Towards Factually Accurate Text-to-Video Generation with Distilled Knowledge Retrieval](Paper Link TBD). 

## Task Description


### Data Organization
The data is organized in the following way:

```
data
└── prompts
    ├── t2vprompts.json
    ... 
└── results
    ├── runwaygen2.json
    ├── cogvideox.json
    ... 
└── videos
    ├── runwaygen-2
    │   ├── standard
    │   │   ├── 1_gen2.mp4
    │   │   ├── 2_gen2.mp4
    │   ├── factv
    │   │   ├── 1_gen2_factv.mp4
    │   │   ├── 2_gen2_factv.mp4
    ... ... ...
    ├── cogvideox
    │   ├── standard
    │   │   ├── 1_cvx.mp4
    │   │   ├── 2_cvx.mp4
    │   ├── factv
    │   │   ├── 1_cvx_factv.mp4
    │   │   ├── 2_cvx_factv.mp4
```

Where:
* `data/prompts/t2vprompts.json` contains the t2v prompts.
* `data/results/modelcomparisons.json` contains comparisons between models. 
* `data/videos/runwaygen-2/` contains generated videos from RunwayML's Gen-2 and FACT-V.
* `data/videos/cogvideox/` contains generated videos from CogVideoX and FACT-V.

## Prompt Directory
Description

Here's an sample of the prompts in `data/prompts/t2vprompts.json`:

```json
{
    "prompt_id": "6",
    "prompt_text": "Scientist discovering the first leprosy treatment.",
    "common_errors": "Alice Ball first discovered the first treatment for leprosy. She was a black female scientist."
}
```

## Model Comparison
Description

Here's an example result in `data/results/...`:

```json
{
    "prompt_id": "1",
    "metric": "factuality",
    "human_annotation": ["factv", "same'", "standard"]
}
```

## Citation
Please cite our work if you found FACT-V, our [paper](), or these resources useful.

```bibtex
tbd
```
