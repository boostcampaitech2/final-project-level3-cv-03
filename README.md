## :cat: Korean Zero-shot Cat Emotion and Action Understanding.
Official Pytorch Implementation

![Teaser image](https://kr.object.ncloudstorage.com/resume/boostcamp/teaser.png)

## :floppy_disk: Installation
For all the methods described in the paper, is it required to have:
- Anaconda
- [CLIP](https://github.com/openai/CLIP)

Specific requirements for each method are described in its section. 
To install CLIP please run the following commands:
  ```shell script
conda install --yes -c pytorch pytorch=1.7.1 torchvision cudatoolkit=<CUDA_VERSION>
pip install ftfy regex tqdm gdown
pip install git+https://github.com/openai/CLIP.git
```

## :hammer: Method
![Method image](https://kr.object.ncloudstorage.com/resume/boostcamp/main_figure.png)

### 1. CLIP-based Contrastive Latent Representation Learning.
**Dataset Curation.**

We create an MSCOCO and WiT Korean-Image-English Pair dataset.

**Training.**
```
python3 train.py
```

## :golf: Results

### Zero-shot Image Classification Accuracy.
- Cifar10

|Model| Acc. |
|:-:|:-:|
| KoCLIP(kor)  | 15% |
|  Ours(kor)  | 80%  |
|  CLIP(eng) | 95%  |



### Cat Diary Generation Results.

**Demo.**

![LSUN image](https://kr.object.ncloudstorage.com/resume/boostcamp/demo.png)
