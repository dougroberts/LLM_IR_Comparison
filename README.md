# Comparing Information Retrieval Mechanisms Supplementing Language Models for Question Answering

## Purpose
This project consists of a systematic comparison between a large language model by itself (GPT-3) and a large language model supplemented by an external information resource (ReTro and QA-GNN). Each model was evaluated with SQuAD for accuracy performing question answering. This benchmark was used to see whether, in the current state of the practice, incorporating information from external resources into a language model can improve upon the performance of a language model by itself. In the implementation of the models performed in this project, supplementing a large language model with an external information resource failed to improve question answering performance.<br/>
## Environment Requirements
**Note**: Some notebooks require a GPU to work correctly<br/>
### CONDA Environment Setup for Each Notebook
* **gpt3.ipynb**: conda create -n qaproject python=3.9
* **retro.ipynb**: conda create -n qaproject python=3.9
* **qagnn.ipynb**: conda create -n qagnn python=3.7
* **Generate_Multiple_Choice_Questions.ipynb**: conda create -n qaproject python=3.9

## Notebooks
### GPT-3
* Notebook: [gpt3.ipynb](gpt3.ipynb)
* Purpose: Access OpenAI API to receive model generated answers for prompted questions from SQuAD 1.1
* Link to Paper: [Language Models are Few-Shot Learners](https://arxiv.org/pdf/2005.14165.pdf)
* Adapted code: [Stanford's CS224U OpenQA Homework](https://github.com/cgpotts/cs224u/blob/master/hw_openqa.ipynb)

### Retrieval Transformers (ReTro)
* Notebook: [retro.ipynb](retro.ipynb)
* Purpose: Adaptation of the ReTro model to generate answers to a given prompt from SQuAD 1.1
* Link to Paper: [Improving language models by retrieving from trillions of tokens](https://arxiv.org/abs/2112.04426)
* Adapted code: [LabML ReTro Implementation](https://github.com/labmlai/annotated_deep_learning_paper_implementations/tree/master/labml_nn/transformers/retro)

### QA-GNN
* Notebook: [qagnn.ipynb](qagnn.ipynb)
* Purpose: Adaptation of the QA-GNN model to perform multiple choice question answering from SQuAD 1.1
* Link to Paper: [QA-GNN: Reasoning with Language Models and Knowledge Graphs for Question Answering](https://arxiv.org/abs/2104.06378)
* Adapted code: [Stanford Official Implementation](https://github.com/michiyasunaga/qagnn)
#### Generate Multiple Choice Questions
* Notebook: [Generate_Multiple_Choice_Questions.ipynb](Generate_Multiple_Choice_Questions.ipynb)
* Purpose: Adapt the SQuAD 1.1 dataset to have multiple choice answers instead of a single right answer
* Source Explanation: [Ramsri Goutham's Practical AI](https://towardsdatascience.com/practical-ai-automatically-generate-multiple-choice-questions-mcqs-from-any-content-with-bert-2140d53a9bf5)
* Adapted code: [Generate_MCQ_BERT_Wordnet_Conceptnet Repo](https://github.com/ramsrigouthamg/Generate_MCQ_BERT_Wordnet_Conceptnet.git)
