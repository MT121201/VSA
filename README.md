## Machine Learning Final Project: Vision Search Assistant

This repository is a clone of the excellent [Vision Search Assistant](https://arxiv.org/abs/2410.21220) repository.

### Modifications and Improvements:
- The original workflow is retained.
- A new prompt template has been applied based on the original prompt.
- Various code modifications have been made to fix bugs and improve stability.

For more details, please refer to the original paper and our modifications documented in this repository.

## ⚙️ Setup

1. Clone this repository and navigate to the VSA folder.
```
git clone https://github.com/MT121201/VSA.git
cd VSA
```

2. Create a conda environment.
```
conda create -n vsa python=3.10
conda activate vsa
```

3. Install LLaVA.
```
cd models/LLaVA
pip install -e .
```

4. Install other requirements.
```
pip install -r requirements.txt
```

## 🚀 Demo
```
python cli.py \
    --vlm-model "liuhaotian/llava-v1.6-vicuna-7b" \
    --ground-model "IDEA-Research/grounding-dino-base" \
    --search-model "internlm/internlm2_5-7b-chat" \
    --vlm-load-4bit
```

## 🙌 Acknowledgements
Our work is greatly inspired by **Vision Search Assistant** and other open-source projects: [GroundingDINO](https://github.com/IDEA-Research/GroundingDINO), [LLaVA](https://github.com/haotian-liu/LLaVA), [MindSearch](https://github.com/InternLM/MindSearch).

## 📖 Citation
Original pipeline, source code, and prompt are from:
```
@article{zhang2024visionsearchassistantempower,
  title={Vision Search Assistant: Empower Vision-Language Models as Multimodal Search Engines},
  author={Zhang, Zhixin and Zhang, Yiyuan and Ding, Xiaohan and Yue, Xiangyu},
  journal={arXiv preprint arXiv:2410.21220},
  year={2024}
}
```