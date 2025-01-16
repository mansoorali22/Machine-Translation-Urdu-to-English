# Urdu to English Machine Translation using RNN with Attention

This repository contains the implementation of a custom Long Short Term Memory (LSTM) with an attention-based encoder-decoder architecture to perform machine translation from Urdu to English. The model is designed using the PyTorch framework and adheres to the following requirements:

## Project Details

### Dataset
The dataset consists of parallel sentence-aligned files provided in `.dev` and `.devtest` formats. These files have been combined and randomly shuffled into:
- **Training Data**: 70%
- **Validation Data**: 15%
- **Test Data**: 15%

### Model
The LSTM with attention-based encoder-decoder architecture has been implemented from scratch without using any pre-built RNN libraries. However, PyTorch's built-in functions have been utilized for backpropagation and optimization.

### Key Features
- **Encoder**: Processes the input Urdu sentences.
- **Attention Mechanism**: Aligns and focuses on relevant parts of the input sequence during decoding.
- **Decoder**: Generates English translations.

### Evaluation
The model's performance is evaluated using the [Moses multi-bleu.perl script](https://github.com/moses-smt/mosesdecoder/blob/master/scripts/generic/multi-bleu.perl) to calculate BLEU scores, which measure the quality of translations.
