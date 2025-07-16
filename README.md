# 🇷🇼 Parakeet Kinyarwanda TTS Fine-Tuning Pipeline

This project implements a complete pipeline for fine-tuning the [Parakeet CTC model (v0.6b)](https://arxiv.org/abs/2104.01721) on the **Kinyarwanda TTS dataset** using NVIDIA NeMo and Hugging Face's ecosystem.

## 📌 Project Overview

- 🔉 Loads and parses 5 hours of Kinyarwanda TTS data (CSV and audio)
- 📊 Computes dataset statistics (duration, WER, vocabulary, SNR)
- 📁 Generates train/val/test JSON manifests
- 🔤 Builds a Byte Pair Encoding (BPE) tokenizer
- 🎙️ Loads and adapts a pre-trained `parakeet-ctc-0.6b` ASR model
- 🧠 Fine-tunes the model using subword tokenization and frozen encoder
- 📈 Logs metrics and training progress to [Weights & Biases (wandb)](https://wandb.ai/)
- ☁️ Optionally pushes final `.nemo` model to the Hugging Face Hub

## 📂 File Structure

