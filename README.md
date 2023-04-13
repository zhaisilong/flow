# Flow

## 对抗

使用 EDBO 与预测器进行对抗生成，查看数据拟合情况。

[对抗脚本](adversial/adv.ipynb)

## EDBO

[Nature 贝叶斯反应条件推荐](https://github.com/b-shields/edbo)


### 化学反应产率与贝叶斯

## EDA

[EDA.ipynb](EDA.ipynb)
Features Importances: [shap.ipynb](shap.ipynb)
Condition Predictions: [openbox.ipynb](openbox.ipynb)

## 环境与安装

```bash
mamba create -nflow python=3.7
mamba activate flow
mamba install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia
mamba install -c rdkit rdkit
mamba install -c rdkit -c mordred-descriptor mordred
mamba install cudatoolkit=11.7 py-xgboost-gpu shap
mamba install jupyter ipykernel rich fire pandas

# openbox
pip install "openbox[extra]"  # for HTML Visualization

# edbo
cd software
git clone https://github.com/b-shields/edbo
cd edbo
pip install -e .
```
