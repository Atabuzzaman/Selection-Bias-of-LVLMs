# Benchmarking and Mitigating MCQA Selection Bias of Large Vision-Language Models (EMNLP 2025)

**Abstract**: 
Large Vision-Language Models (LVLMs) have achieved strong performance on vision-language tasks, particularly Visual Question Answering (VQA). While prior work has explored unimodal biases in VQA, the problem of selection bias in Multiple-Choice Question Answering (MCQA)—where models may favor specific option tokens (e.g., "A") or positions—remains underexplored. In this paper, we investigate both the presence and nature of selection bias in LVLMs through fine-grained MCQA benchmarks spanning easy, medium, and hard difficulty levels, defined by the semantic similarity of distractors. We further propose an inference-time logit-level debiasing method that estimates an ensemble bias vector from general and contextual prompts and applies confidence-adaptive corrections to the model’s output. Our method mitigates bias without retraining and is compatible with frozen LVLMs. Extensive experiments across several state-of-the-art models reveal consistent selection biases that intensify with task difficulty, and show that our mitigation approach significantly reduces bias while improving accuracy in challenging settings. This work offers new insights into the limitations of LVLMs in MCQA and presents a practical approach to improve their robustness in fine-grained visual reasoning.

---
## Dataset:
Please download the fine-grained MCQA dataset from the following link: https://drive.google.com/drive/folders/1405I1_6canS9caK-ZwgukR0bXWLptXlB?usp=sharing.

---
## Code
The provided notebook (cub_with_and_without_name.ipynb) includes the code used to evaluate our datasets (CUB medium/hard) with the Qwen2.5-VL-7B-Instruct model. This code can also be used for all other datasets by just changing the file name and formats. 

---
## Citation
```bibtex
@inproceedings{atabuzzaman2025benchmarking,
  title={Benchmarking and Mitigating MCQA Selection Bias of Large Vision-Language Models},
  author={Atabuzzaman, Md and Asgarov, Ali and Thomas, Chris},
  booktitle={Proceedings of the 2025 Conference on Empirical Methods in Natural Language Processing},
  pages={33536--33550},
  year={2025}
}
```
