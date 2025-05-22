# C2Prompt: Class-aware Client Knowledge Interaction for Federated Continual Learning







## Installation
```shell
conda create -n C2Prompt python=3.9
conda activate C2Prompt
pip install torch==2.5.1 torchvision==0.20.1 torchaudio==2.5.1 --index-url https://download.pytorch.org/whl/cu118
pip install -r requirements.txt
```


### Data and Model Preparation

This work primarily utilizes DomainNet, ImageNet-R. Among them, DomainNet, ImageNet-R are existing datasets. And you can download DomainNet at [here](https://ai.bu.edu/M3SDA/), ImageNet-R at [here](https://github.com/hendrycks/imagenet-r?tab=readme-ov-file)  



### DC-Comp
You can directly run the pre-written shell script:
```
sh src/scripts/run_imagenetr.sh
sh src/scripts/run_domainnet.sh
```
You can get the single task training results in:
```
sh src/scripts/run_imagenetr_direct.sh
sh src/scripts/run_domainnet_direct.sh
```
Compute the five metrics in our benchmark with src/benchmark_metrics.py.
