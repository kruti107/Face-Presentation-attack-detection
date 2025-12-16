🛡️ Face Presentation Attack Detection using Vision Transformer (ViT)
📌 Overview

Face Presentation Attack Detection (PAD), also known as Face Anti-Spoofing, aims to protect face recognition systems from spoofing attacks such as printed photos, replayed videos, and digital manipulations.

This repository presents a Vision Transformer (ViT)–based approach for detecting face presentation attacks by leveraging global self-attention to capture subtle spatial cues that are often missed by traditional CNN-based methods.

🎯 Objectives

Detect bona-fide (real) vs spoofed (fake) face images

Improve generalization against unseen spoofing attacks

Explore the effectiveness of Vision Transformers for biometric security

🧠 Key Features

✅ Vision Transformer (ViT) backbone

✅ Patch-based self-attention for global context modeling

✅ Binary classification (Live / Spoof)

✅ PyTorch-based modular implementation

✅ Easy to extend to video-based PAD and deepfake detection

🏗️ Model Architecture

Input face image is divided into fixed-size patches

Patches are embedded into tokens

Tokens are processed using multi-head self-attention

Global representation is learned using transformer encoder layers

Classification head predicts:

0 → Presentation Attack

1 → Bona-fide Face

🗂️ Dataset

I have used reply attack (https://www.idiap.ch/en/scientific-research/data/replayattack)

This model can be trained on standard face anti-spoofing datasets such as:

CASIA-FASD

Replay-Attack

MSU-MFSD

Custom face spoof datasets

⚠️ Dataset files are not included due to license restrictions.

⚙️ Installation

1️⃣ Clone the repository
git clone https://github.com/your-username/face-pad-vit.git
cd face-pad-vit

2️⃣ Create virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows

3️⃣ Install dependencies
pip install -r requirements.txt

📦 Requirements

Python ≥ 3.9

PyTorch ≥ 2.1

Torchvision

OpenCV

NumPy

Einops

(Full list available in requirements.txt)

Output:

Prediction: Bona-fide / Spoof
Confidence Score: 0.xx

📊 Evaluation Metrics

Accuracy

Precision

Recall

F1-Score

🔐 Applications

Face recognition security systems

Biometric authentication

Deepfake and spoof detection

Access control systems

AI-based identity verification

🧩 Future Work

🔹 Video-based PAD using Temporal Transformers

🔹 Zero-shot and cross-dataset evaluation

🔹 Integration with CNN-Transformer hybrid models

🔹 Real-time deployment

🤝 Contributing

Contributions are welcome!
If you find a bug or want to improve the model:

Fork the repository

Create a new branch

Submit a pull request

📜 License

This project is released under the MIT License.
You are free to use, modify, and distribute it for research and educational purposes.

🙏 Acknowledgements

Vision Transformer (ViT)

PyTorch community

Face Anti-Spoofing research community
