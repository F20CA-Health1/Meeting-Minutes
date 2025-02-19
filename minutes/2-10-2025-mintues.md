# Minutes

Note: Meeting online during several sudden problems

Present: Ka2023, rv2009, zj2009, lh2020, zy2017, am2102, jk2023s, yj2012

Minutes taken by: zj2009

## Agenda

- Progress presentation for the project
- Prepare for the project presentation in Week 7

## Minutes

Topics:

- Progress presentation
- Detail discussion
- Preparation for project presentation in Week 7

## Progress presentation

PPT: https://heriotwatt-my.sharepoint.com/:p:/g/personal/am2102_hw_ac_uk/ESi5-PIRxBdCrfTS6qoR71sBfmVvxEKRpwRVNl9Afj4l2w?e=ikv2Bo

### TTS Engineer

presentater: Yujing Ju

detialed deploy for tts can be seen in the PPT and following github link

Github: https://github.com/juyujing/multilang-tts

### Safety Evaluation

Presenter: Zewei Yan

Attempt the evaluation code SafetyBench, it is used to evaluate the safety of the model. The seven perspectives are the types of the questions, compare the origin_pred with the answer in the json file to see the safety situation.

![alt text](image.png)

EmoLLM can help us to improve in the future: General Evaluation Output(currently including BLEU and ROUGE scores), Professional Output(Turn-Based Dialogue Evaluation)

Github: https://github.com/F20CA-Health1/safety-benchmarking

### Performance Evaluation

Presenter: Zhaorui Jiang

Github: https://github.com/F20CA-Health1/performance--benchmarking

Evaluation Metrics​

- Accuracy​
- F1-score(optional)​

Using "sklearn" Python Package to calculate them​

The Medical-LLM Leaderboard includes a variety of tasks​

- Uses accuracy as its primary evaluation metric ​
- Accuracy measures the percentage of correct answers provided by a language model across the various medical QA datasets

Evaluation Health Base Dataset（Consider biology dataset to evaluate？）​

- MMLU Subsets (college_medicine and professional_medicine)​
- MMLU-Pro Subset (Health）​
- PubMedQA​
- MedMCQA​
- MedQA​
- ToxiGen ​
- USMLE​
- NHS（Our unique Dataset, also requirement)​
  //upload to hugggingface （better label and format like MMLU-Pro dataset）

Attention: NHS dataset needs to be reorganized by us.

#### Pipline for Performance Benchmarking

##### Evaluation

To run local inference, modify the model name in the following script and execute it:

```bash
cd scripts/examples/
sh eval_llama_2_7b.sh
```

##### 🏆 Leaderboard

| Model           | MMLU-PRO | MMLU-1 | MMLU-2 |
| :-------------- | :------- | :----- | :----- |
| Llama3-Med42-8B | 0.529    | 0.790  | 0.676  |

##### Benchmarking Answer Extraction

We provide different alternatives to do answer extraction. We found that different answer extraction mechanisms have minor impact on the results.

```
python compute_accuracy.py results/llama-3-8b-quantized/CoT/all/
```

### Heuristic Evaluation

Presenter: Lanting Huang

It needs the GUI design combined with Heuristic Evaluation.

Useful material: https://hci.stanford.edu/courses/cs147/2024/au/lectures/11-heuristic-evaluation.pdf

### NLU language understanding

Presenter: Jiahui Kang

### RAG

presentater: Rohan Veit

Github: https://github.com/F20CA-Health1/rohan_playground

Video: https://streamable.com/gc8rw9

### Interface/GUI + Voice/Audio Input

presentater: Kareem Al-Hasan

![alt text](image-1.png)

detialed codes can be seen in teams like autio test.py

It may need find some benchmarks to evaluate the effects

### Role Allocation Detials

- Zhaorui Jiang - Project Coordinator
- Rohan Veit - Deputy Coordinator
- Kareem Al-Hasan - RAG Manager
- Jiahui Kang - NLU language understanding
- Ameen - App/GUI developement + TTS Engineer
- Zhaorui Jiang + Zewei Yan - Model Evaluation/Research/Implementation (Safety + Performance + Bias (Gender/Race) + Interpret + Finetuning + Prompting)
- Yujing Ju - TTS Engineer
- Lanting Huang - System Engineer/Ethics Consideration/Heuristic Evaluation

## Prepare for the project presentation in Week 7

Need another time to prepare for presentation's outline and detailed contents.

Time control for presentation is quite important (within 10 min)
