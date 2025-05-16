# project-1-Speech-to-Text-for-transcription-services-

**`project_1_Speech_to_Text_for_transcription_services (2).ipynb`**



---

### 📘 **Notebook Overview: Speech-to-Text for Transcription Services**

This project notebook implements a **Speech-to-Text transcription system**, likely using audio input and converting it into written text using pre-trained models.

#### 🔍 Key Components:

1. **Libraries and Setup**

   * Imports include `torch`, `transformers`, `datasets`, `IPython.display.Audio`, etc.
   * GPU availability is checked for better performance.

2. **Model and Tokenizer**

   * Uses **Wav2Vec2** from the Hugging Face `transformers` library:

     ```python
     from transformers import Wav2Vec2ForCTC, Wav2Vec2Tokenizer
     ```
   * Model: `facebook/wav2vec2-base-960h`

3. **Data Preprocessing**

   * Loads audio files (WAV format), resamples to 16kHz.
   * Audio is processed into input values using the tokenizer.

4. **Transcription**

   * Audio input is passed through the model to get logits.
   * Uses `argmax` to get the most likely tokens and decodes them into text.

5. **Example**

   * Contains at least one test audio sample.
   * Plays the audio and prints the transcribed text.

---
