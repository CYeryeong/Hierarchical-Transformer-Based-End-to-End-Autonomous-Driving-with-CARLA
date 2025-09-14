# Multimodal Coarse-to-Local Transformer for Reliable End-to-End Autonomous Driving
This repository contains the implementation of the Multimodal Coarse-to-Local Transformer (MC2L-Transformer) designed for reliable end-to-end autonomous driving. 
The framework integrates multimodal sensory inputs with a hierarchical transformer (global → local) for uncertainty-aware trajectory prediction.

1. Clone this repository:
   ```bash
   git clone https://github.com/CYeryeong/Multimodal-Coarse-to-Local-Transformer-for-Reliable-End-to-End-Autonomous-Driving.git
   cd Multimodal-Coarse-to-Local-Transformer-for-Reliable-End-to-End-Autonomous-Driving

2. Conda Env Setup:
   ```bash
   conda env create -f environment.yml
   conda activate e2e_ht

## 📖 Notes
  - Environment is tested with Python 3.7.12.
  - GPU acceleration (CUDA) is strongly recommended for training with LiDAR + image fusion.
  - Some packages may require system-level dependencies (ex. CARLA 9.10.1, etc.).
  - Ensure NVIDIA drivers and CUDA toolkit are properly installed before training.

## 🚀 Results
<img width="1408" height="658" alt="1200" src="https://github.com/user-attachments/assets/db70c988-6d93-4e06-9a0b-dffd3483959d" />
<img width="1408" height="658" alt="2100" src="https://github.com/user-attachments/assets/41c26263-cfdd-404b-a882-69c29962339a" />
<img width="1408" height="658" alt="2900" src="https://github.com/user-attachments/assets/73484577-b828-438f-bd37-719d7d9e1171" />



## 🚀 Training & Evaluation
  ```bash
  python train.py \
    --root /path/to/dataset \
    --logdir ./logs/exp1 \
    --batch_size 8 \
    --epochs 30
  ```

## 📜 Citation
  ```bash
  @article{cho2025mc2ltransformer,
    title   = {Multimodal Coarse-to-Local Transformer for Reliable End-to-End Autonomous Driving},
    author  = {Cho, Yeryeong and Kim, Joongheon},
    year    = {2025}
  }
  ```
