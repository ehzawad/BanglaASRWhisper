# BanglaASR
Bangla ASR model which was trained Bangla Mozilla Common Voice Dataset.
This is Fine-tuning Whisper for Bangla Mozilla common voice dataset. For training Bangla ASR model here used 40k training and 7k Validation of around 400 hours of data. We trained 12000 steps in this model and get word error rate 4.58%.

Whisper is a Transformer based encoder-decoder model, also referred to as a sequence-to-sequence model. It maps a sequence of audio spectrogram features to a sequence of text tokens. First, the raw audio inputs are converted to a log-Mel spectrogram by the action of the feature extractor. The Transformer encoder then encodes the spectrogram to form a sequence of encoder-hidden states. Finally, the decoder autoregressively predicts text tokens, conditional on both the previous tokens and the encoder's hidden states.



![Alt text](asset/whisper_architecture.svg)


| Size | Layers | Width | Heads | Parameters | Bangla-only | Training Status |
| ------------- | ------------- | --------    |--------    | ------------- | ------------- | --------    |
tiny   | 4  |384  | 6   | 39 M 	| X |  X
base   | 6 	|512  | 8 	|74 M 	| X	|  X
small  | 12 |768  | 12 	|244 M 	| ✓ |  ✓ 
medium | 24 |1024 | 16 	|769 M 	| X |  X
large  | 32 |1280 | 20 	|1550 M | X |  X




# Requirments
```
!pip install datasets>=2.6.1
!pip install transformers
!pip install librosa
!pip install evaluate>=0.30
!pip install jiwer
!pip install gradio
!pip install torchaudio
```
or

```
pip install -r requirements.txt
```

# Dataset

mozilla building an open-source, multi-language dataset of voices that anyone can use to train speech-enabled applications.

- Bangla voice dataset please click [here](https://commonvoice.mozilla.org/bn/datasets)


# Training

# Inference

# Evaluation

# Contribution

# Reference
1. https://huggingface.co/blog/fine-tune-whisper
