# 🎙️ Audio-to-Text Translation Pipeline

## 📝 Description
This project demonstrates the power of **Model Chaining** using the **Hugging Face** ecosystem. It implements a sequential pipeline that processes audio input to generate translated text.

The system works in two stages:
1.  **Speech-to-Text (ASR):** Converts the input audio file (voice recording) into a textual transcript using a state-of-the-art ASR model.
2.  **Machine Translation:** Automatically takes the transcribed text and translates it into the target language using a secondary translation model.

## 🚀 Key Features
* **Hugging Face Integration:** Seamlessly utilizes pre-trained models from the Hugging Face Hub.
* **Sequential Pipeline:** Demonstrates how to pass outputs from one AI model as inputs to another.
* **Audio Processing:** Handles audio input decoding and processing.
* **Automated Translation:** Provides instant translation from spoken audio.

## 🛠️ Technologies Used
* **Library:** Hugging Face Transformers
* **Language:** Python
* **Audio Handling:** Librosa / SoundFile
* **Models Used:**
    * *ASR Model:* (e.g., openai/whisper-base or facebook/wav2vec2)
    * *Translation Model:* (e.g., Helsinki-NLP/opus-mt-en-ar)

## 💻 How it Works
1.  **Input:** User provides an audio file (e.g., `.wav` or `.mp3`).
2.  **Stage 1 (Transcription):** The ASR model processes the audio and outputs a string of text.
3.  **Stage 2 (Translation):** The text is passed to the Translation model.
4.  **Output:** The final translated text is displayed.

## 🏃‍♀️ How to Run
1.  Clone the repository.
2.  Install dependencies:
    ```bash
    pip install transformers torch librosa
    ```
3.  Run the script:
    ```bash
    python Huggingface_task.ipynb
    ```
