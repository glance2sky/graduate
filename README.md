

## 1. 环境

* python 3.6
* PyTorch 1.1.0 (0.3.0 for calculating optical flow)
* torchvision 0.3.0
* cuda 9.0.176
* cudnn 7.0.5
* mmcv 0.2.14 (might use `pip install mmcv==0.2.14` to install old version)
* [mmdetection](https://github.com/open-mmlab/mmdetection/tree/v1.0rc0) 1.0rc0 (might use `git clone -b v1.0rc0 https://github.com/open-mmlab/mmdetection.git` to clone old version)
* numpy 1.17.2
* scikit-learn 0.21.3

Refer to the full environment in [issue](https://github.com/yuguangnudt/VEC_VAD/issues/2).  Note that our project is based on mmdet v1.0rc0. Run the program strictly according to our environment, or might try the newer versions of mmdet, PyTorch and mmcv.

Recently (2021.1) the interface of mmdet v1.0rc0 seems to have changed. If you install mmdet v1.0rc0 and get "No module named 'mmdet.datasets.pipelines' " when running the program, please refer to [issue](https://github.com/yuguangnudt/VEC_VAD/issues/9#issuecomment-768020917) to fix the bug.

## 2. 下载数据集


## 3. 光流计算

(1) 安装FlowNet2.0(https://github.com/vt-vl-lab/flownet2.pytorch), 下载预训练的模型：https://drive.google.com/file/d/1hF8vS6YeHkx3j2pfCeQqqZGwA_PJq_Da/view?usp=sharing

(2) 运行 `calc_optical_flow.py` (PyTorch 0.3.0，只有pytorch版本小于等于0.4.0才可成功运行计算光流)

## 4.  环境安装

(1) 安装mmdet:https://github.com/open-mmlab/mmdetection/tree/v1.0rc0

(2) 运行 `test.py`: `python test.py`.

## 5. Train

 `train.py`: `python train.py`.