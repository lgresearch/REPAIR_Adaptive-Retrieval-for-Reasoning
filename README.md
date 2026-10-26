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
