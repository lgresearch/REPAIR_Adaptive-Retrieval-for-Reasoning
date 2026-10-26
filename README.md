# Plan-and-Rerank Framework for Reasoning-Intensive Retrieval

## setup
Use separate virtual environments for inference and training, which use different PyTorch and vLLM versions.
Set `JAVA_HOME` to your Java installation before constructing a corpus graph.

- For inference,
```
pip install -r requirements.txt
```

- For training,
```
pip install -r train/requirements.txt
```


## Training
- Train data generation
```
bash bash/train_sft.sh
```

## Graph construction

- Graph construction
```
bash bash/construct_graph.sh
```

## Inference

- Inference (e.g. BRIGHT)
```
bash bash/rank_bright.sh
```

## Evaluation
- Evaluation (e.g. BRIGHT)
```
bash bash/eval_bright.sh
```

## Contact

For questions regarding this repository, please contact [Jongho Kim](mailto:jongh97@snu.ac.kr).

## Citation

If you find REPAIR useful in your research, please cite our paper.

```bibtex
@inproceedings{kim-etal-2026-adaptive,
  title = "Adaptive Retrieval for Reasoning",
  author = "Kim, Jongho and Kim, Jaeyoung and Kim, Jihyuk and Kim, Yu Jin and Hwang, Seung-won and Lee, Moontae",
  booktitle = "Proceedings of the 64th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
  year = "2026",
  pages = "37366--37381",
  publisher = "Association for Computational Linguistics",
  url = "https://aclanthology.org/2026.acl-long.1734/",
  doi = "10.18653/v1/2026.acl-long.1734"
}
