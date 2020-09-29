# An example of finetuning BERT-base, BERT-large and Megatron-BERT with NeMo

### Environment
---
Docker container of NeMo (v0.11) pulled from <a href="https://ngc.nvidia.com/">NVIDIA GPU Cloud (NGC)</a>
- Nemo: https://ngc.nvidia.com/catalog/containers/nvidia:nemo

### Dataset
---
<a href="https://www.kaggle.com/bittlingmayer/amazonreviews/home">Amazon reviews for sentiment analysis</a>
</br>
Unzipping to ./data

### Checkpoints
---
The pre-trained checkpoints of BERT-base, BERT-large and Megatron-BERT can be downloaded from <a href="https://ngc.nvidia.com/">NGC</a>.
- BERT-base: https://ngc.nvidia.com/catalog/models/nvidia:bertbaseuncasedfornemo

- BERT-large: https://ngc.nvidia.com/catalog/models/nvidia:bertlargeuncasedfornemo

- Megatron-BERT: https://ngc.nvidia.com/catalog/models/nvidia:megatron_bert_345m
(replace "v0.1_cased/zip" with "v0.1_uncased/zip" in the pulling command.)
</br>
Unzipping to ./checkpoint/ENCODER_NAME
</br>


### Results
---
- After 3 epochs of finetuning, we can get the results below:

| Encoder | No. of params | Accuracy |
| --- | --- | --- |
| BERT-base     | 109 m | 0.948 |
| BERT-large    | 335 m | 0.956 |
| Megatron-BERT | 334 m | 0.967 |

### Reference:
---
- https://github.com/NVIDIA/NeMo
- https://developer.nvidia.com/nvidia-nemo 


