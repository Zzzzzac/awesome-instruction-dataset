# awesome-text/visual-instruction-tuning-dataset
A collection of open-source instruction tuning datasets to train (text and multi-modal) chat-based LLMs (GPT-4, ChatGPT,LLaMA,Alpaca). We currently include image-instruction-answer (e.g. visual-instruction-tuning) and instruction-answer datasets.

Instruction Tuning / Reinforcement Learning from Human Feedback (RLHF) Dataset is a key component of instruction-following LLMs such as ChatGPT. This repo is dedicated to providing a comprehensive list of datasets used for instruction tuning in various LLMs, making it easier for researchers and developers to access and utilize these resources.

Other relevant awesome-list: [nichtdax/awesome-totally-open-chatgpt](https://github.com/nichtdax/awesome-totally-open-chatgpt): A codebase of totally open alternatives to ChatGPT

Size: The number of instruction tuning pairs

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
- COL: [Collection of Dataset] Dataset made from a collection of other datasets

# Table of Contents
1. [The template](#the-template)
2. [The Multi-modal Instruction Dataset](#the-multi-modal-instruction-datasets)
   - [(Vision-CAIR/MiniGPT-4)|5K|EN|MT|MIX](https://minigpt-4.github.io/)
   - [(haotian-liu/LLaVA)|150K|EN|MT|MIX](https://huggingface.co/datasets/liuhaotian/LLaVA-Instruct-150K)
3. [The Instruction tuning Dataset](#the-instruction-following-datasets)
   - [(tatsu-lab/Alpaca)|52K|EN|MT|SI](https://github.com/tatsu-lab/stanford_alpaca)
   - [(gururise/Cleaned Alpaca)|52K|EN|MT|SI](https://github.com/gururise/AlpacaDataCleaned)
   - [(XueFuzhao/InstructionWild)|52K|EN|CN|MT|SI](https://github.com/XueFuzhao/InstructionWild)
   - [(JosephusCheung/GuanacoDataset)|534K|ML|MT|SI](https://huggingface.co/datasets/JosephusCheung/GuanacoDataset)
   - [(Hello-SimpleAI/HC3)|24K|EN|MT|MIX](https://huggingface.co/datasets/Hello-SimpleAI/HC3)
   - [(Hello-SimpleAI/HC3-Chinese)|13K|CN|MT|MIX](https://huggingface.co/datasets/Hello-SimpleAI/HC3)
   - [(allenai/prosocial-dialog)|58K|EN|MT|MIX](https://huggingface.co/datasets/allenai/prosocial-dialog)
   - [(allenai/natural-instructions)|1.6K|ML|MT|HG](https://github.com/allenai/natural-instructions)
   - [(bigscience/xP3)|N/A|ML|MT|MIX](https://huggingface.co/datasets/bigscience/xP3)
   - [(nomic-ai/gpt4all)|437k|EN|MT|COL](https://github.com/nomic-ai/gpt4all)
   - [(PhoebusSi/Alpaca-CoT)|500k|ML|MT|COL](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT)
   - [(google-research/FLAN)|N/A|EN|MT|MIX](https://github.com/google-research/FLAN/tree/main/flan/v2)
   - [(thunlp/UltraChat)|280k|EN|TS|MIX](https://github.com/thunlp/UltraChat)
   - [(cascip/ChatAlpaca)|10k|EN|MT|MIX](https://github.com/cascip/ChatAlpaca)
   - [(YeungNLP/firefly-train-1.1M)|1100k|CN|MT|COL](https://huggingface.co/datasets/YeungNLP/firefly-train-1.1M)
   - [(orhonovich/unnatural-instructions)|240K|EN|MT|MIX](https://github.com/orhonovich/unnatural-instructions)
   - [(Instruction-Tuning-with-GPT-4/GPT-4-LLM)|52K|EN|CN|MT|SI](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
   - [(databrickslabs/dolly)|15K|EN|MT|HG](https://github.com/databrickslabs/dolly/tree/master/data)
   - [(OpenAssistant/oasst1)|161K|ML|MT|HG](https://huggingface.co/datasets/OpenAssistant/oasst1)
   - [(RyokoAI/ShareGPT52K)|90K|ML|MT|SI](https://huggingface.co/datasets/RyokoAI/ShareGPT52K)
4. [Reinforcement Learning from Human Feedback (RLHF) Datasets](#reinforcement-learning-from-human-feedback-rlhf-datasets)
   - [(Anthropic/hh-rlhf)|22k|EN|MT|MIX](https://huggingface.co/datasets/Anthropic/hh-rlhf)
   - [(HuggingFaceH4/stack-exchange-preferences)|10741k|EN|TS|HG](https://huggingface.co/datasets/HuggingFaceH4/stack-exchange-preferences)
   - [(stanfordnlp/SHP)|385k|EN|MT|HG](https://huggingface.co/datasets/stanfordnlp/SHP)
   - [(Instruction-Tuning-with-GPT-4/GPT-4-LLM)|52K|EN|MT|MIX](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
 

# The template

Append the new project at the end of file

```markdown
## [({owner}/{project-name)|Tags}]{https://github.com/link/to/project}

- summary:
- Data generation model:
- paper:
- License:
- Related: (if applicable)
```
# The Multi-modal Instruction Datasets

 ## [(Vision-CAIR/MiniGPT-4)|5K|EN|MT|MIX](https://minigpt-4.github.io/)
  
 - Summary: A high-quality, well-aligned (e.g. more detailed image desciption) image-text dataset created using conversation between two bots, similar to [ChatCaptioner](https://github.com/Vision-CAIR/ChatCaptioner). This image-text dataset can then be used with some predefined instruction template for image-instruction-answer finetuning.
 - Modality: Text, Image
 - Data generation model: N/A
 - paper: [MiniGPT-4: Enhancing Vision-language Understanding with Advanced Large Language Models](https://github.com/Vision-CAIR/MiniGPT-4/blob/main/MiniGPT_4.pdf)
 - License: BSD 3-Clause
 - Related: 
     -[Interactive ChatCaptioner for image and video](https://github.com/Vision-CAIR/ChatCaptioner)
     
 ## [(haotian-liu/LLaVA)|150K|EN|MT|MIX](https://huggingface.co/datasets/liuhaotian/LLaVA-Instruct-150K)
  
 - Summary: LLaVA Visual Instruct 150K is a set of GPT-generated multimodal instruction-following data. It is constructed for visual instruction tuning and for building large multimodal towards GPT-4 vision/language capability.
 - Modality: Text, Image
 - Data generation model: `GPT-4-0314` 
 - paper: [Visual Instruction Tuning](https://arxiv.org/abs/2304.08485)
 - License: cc-by-nc-4.0

     
# The Instruction-following Datasets

 ## [(tatsu-lab/Alpaca)|52K|EN|MT|SI](https://github.com/tatsu-lab/stanford_alpaca)

 - Summary:`52K` data generated from modified `self-instruct` pipeline with human written `175 seed task`.
 - Data generation model: `text-davinci-003`
 - paper: [alpaca-blog](https://crfm.stanford.edu/2023/03/13/alpaca.html)
 - License: Attribution-NonCommercial 4.0 International

 ## [(gururise/Cleaned Alpaca)|52K|EN|MT|SI](https://github.com/gururise/AlpacaDataCleaned)

 - Summary: A project that manually cleaned the Alpaca 52K Dataset
 - Data generation model: `text-davinci-003`
 - paper: N/A
 - License: Attribution-NonCommercial 4.0 International
 
 ## [(XueFuzhao/InstructionWild)|52K|EN|CN|MT|SI](https://github.com/XueFuzhao/InstructionWild)

 - Summary:`52K` data generated from modified `self-instruct` pipeline with human written `429 seed task`.
 - Data generation model: `text-davinci-003`
 - paper: N/A
 - License: InstructWild dataset is intended for non-commercial research purpose only.
 
 ## [(JosephusCheung/GuanacoDataset)|534K|ML|MT|SI](https://huggingface.co/datasets/JosephusCheung/GuanacoDataset)

 - Summary:`52K` instruction data generated from modified `self-instruct` pipeline with human written `429 seed task`.
 - Data generation model: `text-davinci-003`
 - License: gpl-3.0

 ## [(Hello-SimpleAI/HC3)|24K|EN|MT|MIX](https://huggingface.co/datasets/Hello-SimpleAI/HC3)

 - Summary:The the first human-ChatGPT comparison corpus (English Version), named HC3 dataset
 - Data generation model: `gpt-3.5`, `human generated`
 - paper: [How Close is ChatGPT to Human Experts? Comparison Corpus, Evaluation, and Detection](https://arxiv.org/abs/2301.07597)
 - License: cc-by-sa-4.0

 ## [(Hello-SimpleAI/HC3-Chinese)|13K|CN|MT|MIX](https://huggingface.co/datasets/Hello-SimpleAI/HC3-Chinese)

 - Summary:The the first human-ChatGPT comparison corpus (Chinese Version), named HC3 dataset
 - Data generation model: `gpt-3.5`, `human generated`
 - paper: [How Close is ChatGPT to Human Experts? Comparison Corpus, Evaluation, and Detection](https://arxiv.org/abs/2301.07597)
 - License: cc-by-sa-4.0

 ## [(allenai/prosocial-dialog)|58K|EN|MT|MIX](https://huggingface.co/datasets/allenai/prosocial-dialog)

 - Summary: ProsocialDialog is the first large-scale multi-turn English dialogue dataset to teach conversational agents to respond to problematic content following social norms.
 - Data generation model: `gpt-3.5`, `human generated`
 - paper: [ProsocialDialog: A Prosocial Backbone for Conversational Agents](https://arxiv.org/abs/2205.12688)
 - License: cc-by-4.0

 ## [(allenai/natural-instructions)|1.6K|ML|MT|HG](https://github.com/allenai/natural-instructions)

 - Summary: A community effort to create a large collection of `1,616 diverse NLP tasks` and their natural language definitions/instructions.
 - Data generation model: `Human generated`
 - paper: [Super-NaturalInstructions: Generalization via Declarative Instructions on 1600+ NLP Tasks](https://arxiv.org/abs/2204.07705)
 - License: Apache License 2.0
 
 ## [(bigscience/xP3)|N/A|ML|MT|MIX](https://huggingface.co/datasets/bigscience/xP3)

 - Summary: [Prompt-resource] xP3 (Crosslingual Public Pool of Prompts) is a collection of prompts & datasets across 46 of languages & 16 NLP tasks.
 - Data generation model: N/A
 - paper: [Crosslingual Generalization through Multitask Finetuning](https://arxiv.org/abs/2211.01786)
 - License: Apache License 2.0

 ## [(PhoebusSi/Alpaca-CoT)|500k|ML|MT|COL](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT)

 - Summary: A datset for Chain-of-Thoughts reasoning based on LLaMA and Alpaca. Note: Their repository will continuously collect various instruction tuning datasets. [Github Repo](https://github.com/PhoebusSi/Alpaca-CoT)
 - paper: N/A
 - License: Apache License 2.0
 
 ## [(nomic-ai/gpt4all)|437k|EN|MT|COL](https://github.com/nomic-ai/gpt4all)

 - Summary: gpt4all leverages three publicly available datasets: 1.[laion/OIG](https://huggingface.co/datasets/laion/OIG), 2.[pacovaldez/stackoverflow-questions](https://huggingface.co/datasets/pacovaldez/stackoverflow-questions) 3. subset of [bigscience/bloomz-p3](https://huggingface.co/bigscience/bloomz-p3)
 - Data generation model: N/A
 - paper: [GPT4All: Training an Assistant-style Chatbot with Large Scale Data Distillation from GPT-3.5-Turbo](https://s3.amazonaws.com/static.nomic.ai/gpt4all/2023_GPT4All_Technical_Report.pdf)
 - License: MIT License
 
 ## [(teknium1/GPTeacher)|20k+|EN|MT|SI](https://github.com/teknium1/GPTeacher)

 - Summary: A collection of modular datasets generated by GPT-4, General-Instruct - Roleplay-Instruct - Code-Instruct - and Toolformer
 - Data generation model: `GPT-4`
 - paper: N/A
 - License: MIT License
 
 ## [(google-research/FLAN)|N/A|EN|MT|MIX](https://github.com/google-research/FLAN/tree/main/flan/v2)

 - Summary: The Flan Collection compiles datasets from Flan 2021, P3, Super-Natural Instructions, along with dozens more datasets into one place, formats them into a mix of zero-shot, few-shot and chain-of-thought templates
 - Data generation model: N/A
 - paper: [The Flan Collection: Designing Data and Methods for Effective Instruction Tuning](https://arxiv.org/abs/2301.13688)
 - License: N/A

 ## [(thunlp/UltraChat)|280k|EN|TS|MIX](https://github.com/thunlp/UltraChat)

 - Summary: UltraChat aims to construct an open-source, large-scale, and multi-round dialogue data. The first part of UltraChat (i.e., the Questions about the World sector) is released, which contains 280k diverse and informative dialogues. More dialogues about writing and creation, assistance on existing materials are to come.
 - Data generation model: `GPT-3.5-turbo`
 - paper: N/A
 - License: Attribution-NonCommercial 4.0 International
 
 ## [(cascip/ChatAlpaca)|10k|EN|MT|MIX](https://github.com/cascip/ChatAlpaca)

 - Summary: Based on the Stanford Alpaca data, ChatAlpaca extends the data to multi-turn instructions and their corresponding responses. More data (20k) and the Chinese translated version are to come.
 - Data generation model: `GPT-3.5-turbo`
 - paper: N/A
 - License: Apache License 2.0
 - Related: [(tatsu-lab/Alpaca)|52K|EN|MT|SI](https://github.com/tatsu-lab/stanford_alpaca)
  
 ## [(YeungNLP/firefly-train-1.1M)|1100k|CN|MT|COL](https://huggingface.co/datasets/YeungNLP/firefly-train-1.1M)
 
 - Summary: Chinese datasets of 23 tasks combined with human-written instruction templates. 
 - Data generation model: N/A
 - paper: N/A
 - License: N/A
 
 ## [(orhonovich/unnatural-instructions)|240K|EN|MT|MIX](https://github.com/orhonovich/unnatural-instructions)
  
 - Summary: 64K examples by prompting a language model with three seed examples of instructions and eliciting a fourth. Then the set is expanded to 240K by prompting the model to rephrase each instruction.
 - Data generation model: `text-davinci-002`
 - paper: [Unnatural Instructions: Tuning Language Models with (Almost) No Human Labor](https://arxiv.org/abs/2212.09689)
 - License: MIT License
 
 ## [(Instruction-Tuning-with-GPT-4/GPT-4-LLM)|52K|EN|CN|MT|SI](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
 
 - Summary: 52K instruction-following data generated by GPT-4 with the original Alpaca prompts & Alpaca prompts translated into Chinese by ChatGPT + 9K instruction-following data generated by GPT-4 with prompts in Unnatural Instruction.
 - Data generation model: `GPT-4`
 - paper: [Instruction Tuning with GPT-4](https://arxiv.org/abs/2304.03277)
 - License: Attribution-NonCommercial 4.0 International
 - Related: 
     -[(tatsu-lab/Alpaca)|52K|EN|MT|SI](https://github.com/tatsu-lab/stanford_alpaca)
     -[(orhonovich/unnatural-instructions)|240K|EN|MT|MIX](https://github.com/orhonovich/unnatural-instructions)
 
 ## [(databrickslabs/dolly)|15K|EN|MT|HG](https://github.com/databrickslabs/dolly/tree/master/data)
 
 - Summary: This datset was generated by thousands of Databricks employees in several of the behavioral categories outlined in the InstructGPT paper, including brainstorming, classification, closed QA, generation, information extraction, open QA, and summarization.
 - Data generation model: N/A
 - paper: [Free Dolly](https://www.databricks.com/blog/2023/04/12/dolly-first-open-commercially-viable-instruction-tuned-llm)
 - License: CC BY-SA 3.0
 
 ## [(OpenAssistant/oasst1)|161K|ML|MT|HG](https://huggingface.co/datasets/OpenAssistant/oasst1)
 
 - Summary: OpenAssistant Conversations (OASST1), a human-generated, human-annotated assistant-style conversation corpus consisting of 161,443 messages distributed across 66,497 conversation trees, in 35 different languages, annotated with 461,292 quality ratings. 
 - Data generation model: N/A
 - paper: [OpenAssistant Conversations - Democratizing Large Language Model Alignment](https://drive.google.com/file/d/10iR5hKwFqAKhL3umx8muOWSRm7hs5FqX/view)
 - License: apache-2.0
 
 ## [(RyokoAI/ShareGPT52K)|90K|ML|MT|SI](https://huggingface.co/datasets/RyokoAI/ShareGPT52K)
 
 - Summary: 90,000 conversations scraped via the ShareGPT API before it was shut down. These conversations include both user prompts and responses from OpenAI's ChatGPT.
 - Data generation model: `GPT-4`,`GPT-3.5`
 - paper: N/A
 - License: cc0-1.0
 
# Reinforcement Learning from Human Feedback (RLHF) Datasets

  ## [(Anthropic/hh-rlhf)|22k|EN|MT|MIX](https://huggingface.co/datasets/Anthropic/hh-rlhf)

 - Summary: This RLHF dataset is an iterated 'online' dataset that includes data from 52B language models. It contains 22k helpfulness comparisons and no red-teaming data. 
 - Data generation model: `Anthropic RL-CAI 52B`
 - paper: [Training a Helpful and Harmless Assistant with Reinforcement Learning from Human Feedback](https://arxiv.org/abs/2204.05862)
 - License: mit
 - Related: 
     -[(Hello-SimpleAI/HC3)|24K|EN|MT|MIX](https://huggingface.co/datasets/Hello-SimpleAI/HC3)
     -[(Hello-SimpleAI/HC3-Chinese)|13K|CN|MT|MIX](https://huggingface.co/datasets/Hello-SimpleAI/HC3-Chinese)

  ## [(HuggingFaceH4/stack-exchange-preferences)|10741k|EN|TS|HG](https://huggingface.co/datasets/HuggingFaceH4/stack-exchange-preferences)

 - Summary: This dataset contains questions and answers from the Stack Overflow Data Dump for the purpose of preference model training.
 - Data generation model: N/A
 - paper: [A General Language Assistant as a Laboratory for Alignment](https://arxiv.org/abs/2112.00861)
 - License: cc-by-sa-4.0
 
  ## [(stanfordnlp/SHP)|385k|EN|MT|HG](https://huggingface.co/datasets/stanfordnlp/SHP)

 - Summary: Each example is a Reddit post with a question/instruction and a pair of top-level comments for that post, where one comment is more preferred by Reddit users (collectively).
 - Data generation model: N/A
 - paper: N/A
 - License: N/A
 
  ## [(Instruction-Tuning-with-GPT-4/GPT-4-LLM)|52K|EN|MT|MIX](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
 
 - Summary: Ranked responses (Note: Data is evaluated by `GPT-4` model NOT human) of Alpaca prompts from three models (GPT-4, GPT-3.5 and OPT-IML) by asking GPT-4 to rate the quality. Author believes "GPT-4 is capable of identifying and fixing its own mistakes, and accurately judging the quality of responses" 
 - Data generation model: `GPT-4`
 - paper: [Instruction Tuning with GPT-4](https://arxiv.org/abs/2304.03277)
 - License: Attribution-NonCommercial 4.0 Internationals
 - Related: 
     -[(tatsu-lab/Alpaca)|52K|EN|MT|SI](https://github.com/tatsu-lab/stanford_alpaca)
