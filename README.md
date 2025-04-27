# Audio-Video Text Generation (Ongoing Project)

### 📚 Project Overview

This project aims to develop a system that generates subtitles based on both **audio signals** and **lip movement analysis**.  
The system is tailored specifically for the **Polish language**.

Currently, there is no fully functional system for Polish lip reading; while for English, models like **AV-HuBERT** exist.  
This project adapts AV-HuBERT using **transfer learning**, fine-tuning the last four layers for Polish data.

The **audio** and **video** models are being developed **separately**, but eventually, they will be merged into a unified architecture to improve subtitle generation — especially under **harsh audio conditions**.

---

### 🎯 Goals

- Build a system capable of generating Polish subtitles based on audio and visual information.
- Investigate whether adding visual (lip movement) information improves transcription accuracy in noisy environments.
- Develop a Polish adaptation of an AV-HuBERT-like model for lip reading.
- Test and compare different architectures for the audio model (pure **Transformer** vs hybrid **CNN-RNN**).

---

### 🏗️ Current Progress

- **Video model**:  
  - Based on **AV-HuBERT**.  
  - Fine-tuning the last 4 layers on Polish datasets.
- **Audio model**:  
  - Developed from scratch.  
  - Testing **Transformer** and **CNN-RNN hybrid** architectures.
- **Dataset**:  
  - Data collected from YouTube (lectures, interviews for high-quality frontal views and audio).
  - Transcriptions and precise word-level alignments generated using [Turboscribe](https://turboscribe.ai/pl).
- **Status**:  
  - Full system setup complete.
  - Currently gathering more data to improve model training, as limited data is causing underfitting.

---

### 🔥 Technologies Used

- PyTorch
- Transformers
- CNN-RNN hybrids
- AV-HuBERT (modified)
- Data augmentation for audio and video
- Automatic word alignment and transcription tools

---

### 🚀 Future Plans

- Merge audio and video branches into a single model.
- Extensive evaluation under clean and noisy conditions.
- Further model optimization once larger datasets are available.
- Open-sourcing the Polish AV-HuBERT adaptation if successful.

---

> **Note:** This project is in an active development phase.  
> Contributions, suggestions, and ideas are very welcome!
