ATUM-CoSiNet

Adaptive Template Update Mechanism for Collaborative Siamese Visual Tracking

📌 Overview

ATUM-CoSiNet is an enhanced single-object visual tracking framework that extends CoSiNet, a collaborative dual-branch Siamese tracker proposed by Dr. Wenjun Zhou.
This work introduces an Adaptive Template Update Mechanism (ATUM) to address the limitation of static templates in long-term tracking scenarios.

ATUM enables reliable online template adaptation by combining:

confidence evaluation,

adaptive thresholding,

temporal interval constraints,

and occlusion-aware filtering.

The proposed mechanism improves tracking robustness under appearance variations and occlusions while maintaining real-time performance.

📄 Related Work

This repository is based on the original implementation of:

“Dual-Branch Collaborative Siamese Network for Visual Tracking (CoSiNet)”

The original CoSiNet framework was developed by Dr. Wenjun Zhou and Ms. Yao Liu
from the Image Processing and Parallel Computing Laboratory,
School of Computer Science and Software Engineering, Southwest Petroleum University.

👥 Authors

Alhou Harouna Adamou
Master Student, Southwest Petroleum University
ATUM design, implementation, experiments, and evaluation

Wenjun Zhou (Supervisor, Corresponding Author)
Southwest Petroleum University
Original CoSiNet design, research guidance, and validation

Yao Liu
Southwest Petroleum University
Technical support and training debugging

📧 Contact:

zhouwenjun@swpu.edu.cn

⚠️ Usage Notice

If you use this code for testing or academic research, you are welcome to download and use it.

If you intend to use this code in a publication, please inform us in advance and cite the corresponding paper.

🖥️ Environment Setup

This code has been tested on the following environment:

OS: Ubuntu 22.04 LTS

Python: 3.7.12 (conda-forge)

PyTorch: 1.9.0

CUDA: 11.1

GPU: NVIDIA GeForce RTX 4060 Ti

OpenCV: 4.5.5

NumPy: 1.21.6

🔧 Quick Environment Check
PyTorch: 1.9.0
CUDA Available: True
GPU: NVIDIA GeForce RTX 4060 Ti
Python: 3.7.12
CUDA Version: 11.1

📦 Installation

Please install the required dependencies before running the code:

pip install -r requirements.txt

🚀 Running the Tracker

▶️ Test the Tracker

python test.py

📊 Evaluate the Tracker

python eval.py

🏋️ Training
Dataset

GOT-10K

Please download the dataset manually and organize it following the instructions of:

siamfc-pytorch

SiamTrackers

Train the Model

python train.py


⚠️ Note:
The ATUM module is only activated during online tracking and does not require additional offline training.

🧩 ATUM: Adaptive Template Update Mechanism

ATUM performs template updates only when tracking conditions are reliable by checking:

response confidence,

adaptive quality thresholds,

update intervals,

occlusion conditions.

This prevents template contamination and tracking drift in long sequences.

🙏 Acknowledgement

This project is built upon:

siamfc-pytorch

CoSiNet

We sincerely thank the original authors and contributors for their valuable work.

📅 Date

December 2025
