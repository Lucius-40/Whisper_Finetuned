# Whisper Fine-Tuning Project

## Overview
This project demonstrates the process of fine-tuning OpenAI's Whisper model for speech recognition tasks. The workflow includes data preparation, augmentation, model training, evaluation, and inference. The notebook `Fine_tuning_base.ipynb` contains all the steps and code used in this project.

## Project Structure
- `Fine_tuning_base.ipynb`: Main notebook with all code and documentation.
- `LICENSE`: License file for the project.

## Steps Performed
1. **Data Preparation**
   - Loaded and preprocessed audio datasets for training and validation.
   - Converted audio files to the required format for Whisper.

2. **Data Augmentation**
   - Applied various augmentation techniques to increase dataset diversity and improve model robustness.
   - **Note:** The data augmentation code was adapted from Zarif Mahir.    Github : https://github.com/zarifmahir

3. **Model Fine-Tuning**
   - Loaded a pre-trained Whisper model.
   - Configured training parameters and callbacks.
   - Trained the model on the prepared dataset.

### Base Model Metrics
- The base version of the model shows a Levenshtein similarity of **0.87** and an approximate Word Error Rate (WER) of **20%**.

4. **Evaluation**
   - Evaluated the fine-tuned model on validation/test data.
   - Calculated relevant metrics (e.g., WER, CER).

5. **Inference**
   - Demonstrated inference using the fine-tuned model on sample audio files.

## How to Use
1. Clone this repository.
2. Install the required dependencies (see the notebook for details).

## Requirements
- `numpy==1.26.4`
- `scikit-learn==1.3.2`
- `protobuf==3.20.3`
- `datasets==3.6.0`
- `transformers==4.48.3`
- `torchaudio`
- `accelerate`
- `evaluate`
- `bitsandbytes`
- `jiwer`
- `SoundFile`
- `python-Levenshtein`

3. Run the notebook `Fine_tuning_base.ipynb` step by step.

## Credits
- Data augmentation code adapted from Zarif Mahir. [Add GitHub link here]

## License
See the `LICENSE` file for details.
