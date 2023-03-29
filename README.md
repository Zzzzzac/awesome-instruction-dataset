# awesome-instruction-dataset
A collection of open-source dataset to train chat-based LLMs (ChatGPT,LLaMA,Alpaca)

Instruction Tuning is a key component of instruction-following LLMs such as ChatGPT. This repo is dedicated to providing a comprehensive list of datasets used for instruction tuning in various LLMs, making it easier for researchers and developers to access and utilize these resources.

Lingual-Tags:
-   EN: Instruction datasets in English
-   CN: Instruction datasets in Chinese
-   ML: [Multi-lingual] Instruction datasets in multiple languages

Task-Tags:
-  MT: [Multi-task] Datasets containing multiple tasks
-  TS: [Task-specific] Datasets tailored for specific tasks

Generation-method:
- HG: [Human Generated Dataset] Datasets created by humans
- SI: [Self-Instruct] Datasets generated using self-instruct methods
- MIX: [Mixed Dataset] Dataset contains both human and machine generated data

# Table of Contents
1. [The template](#The-template)
2. [The Dataset](#The-Instruction-following-Dataset)
   - [(tatsu-lab/Alpaca)|52K|EN|MT|SI](https://github.com/tatsu-lab/stanford_alpaca)
   - [(gururise/Cleaned Alpaca)|52K|EN|MT|SI](https://github.com/gururise/AlpacaDataCleaned)
   - [(XueFuzhao/InstructionWild)|52K|EN|CN|MT|SI](https://github.com/XueFuzhao/InstructionWild)
   - [(JosephusCheung/GuanacoDataset)|534K|ML|MT|SI](https://huggingface.co/datasets/JosephusCheung/GuanacoDataset)
   - [(Hello-SimpleAI/HC3)|24K|EN|MT|MIX](https://huggingface.co/datasets/Hello-SimpleAI/HC3)
   - [(Hello-SimpleAI/HC3-Chinese)|13K|CN|MT|MIX](https://huggingface.co/datasets/Hello-SimpleAI/HC3)
   - [(allenai/prosocial-dialog)|58K|EN|MT|MIX](https://huggingface.co/datasets/allenai/prosocial-dialog)
 

# The template

Append the new project at the end of file

```markdown
## [({owner}/{project-name)|Tags}]{https://github.com/link/to/project}

- summary:
- Data generation model:
- paper:
- Cost:
```

# The Instruction-following Dataset

## [(tatsu-lab/Alpaca)|52K|EN|MT|SI](https://github.com/tatsu-lab/stanford_alpaca)

 - Summary:`52K` data generated from modified `self-instruct` pipeline with human written `175 seed task`.
 - Data generation model: `text-davinci-003`
 - paper: [alpaca-blog](https://crfm.stanford.edu/2023/03/13/alpaca.html)
 - Cost: $600 

## [(gururise/Cleaned Alpaca)|52K|EN|MT|SI](https://github.com/gururise/AlpacaDataCleaned)

 - Summary: A project that manually cleaned the Alpaca 52K Dataset
 - Data generation model: `text-davinci-003`
 - paper: N/A
 - Cost: N/A
 
## [(XueFuzhao/InstructionWild)|52K|EN|CN|MT|SI](https://github.com/XueFuzhao/InstructionWild)

 - Summary:`52K` data generated from modified `self-instruct` pipeline with human written `429 seed task`.
 - Data generation model: `text-davinci-003`
 - paper: N/A
 - Cost: $880
 
 ## [(JosephusCheung/GuanacoDataset)|534K|ML|MT|SI](https://huggingface.co/datasets/JosephusCheung/GuanacoDataset)

 - Summary:`52K` data generated from modified `self-instruct` pipeline with human written `429 seed task`.
 - Data generation model: `text-davinci-003`
 - Cost: $6000

 ## [(Hello-SimpleAI/HC3)|24K|EN|MT|MIX](https://huggingface.co/datasets/Hello-SimpleAI/HC3)

 - Summary:The the first human-ChatGPT comparison corpus (English Version), named HC3 dataset
 - Data generation model: `gpt-3.5`, `human`
 - paper: [How Close is ChatGPT to Human Experts? Comparison Corpus, Evaluation, and Detection](https://arxiv.org/abs/2301.07597)
 - Cost: N/A

 ## [(Hello-SimpleAI/HC3-Chinese)|13K|CN|MT|MIX](https://huggingface.co/datasets/Hello-SimpleAI/HC3)

 - Summary:The the first human-ChatGPT comparison corpus (Chinese Version), named HC3 dataset
 - Data generation model: `gpt-3.5`, `human`
 - paper: [How Close is ChatGPT to Human Experts? Comparison Corpus, Evaluation, and Detection](https://arxiv.org/abs/2301.07597)
 - Cost: N/A

 ## [(allenai/prosocial-dialog)|58K|EN|MT|MIX](https://huggingface.co/datasets/allenai/prosocial-dialog)

 - Summary: ProsocialDialog is the first large-scale multi-turn English dialogue dataset to teach conversational agents to respond to problematic content following social norms.
 - Data generation model: `gpt-3.5`, `human`
 - paper: [ProsocialDialog: A Prosocial Backbone for Conversational Agents](https://arxiv.org/abs/2205.12688)
 - Cost: N/A


