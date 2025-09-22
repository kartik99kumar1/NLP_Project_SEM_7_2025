# 🎥 Speech-Driven Video Summarizer with Whisper + BART

## 📌 Project Overview

This project is an **end-to-end NLP + Speech AI pipeline** that automatically:

1. **Detects scenes** in a video 🎬
2. **Transcribes audio** from each scene using **OpenAI Whisper** 🎤
3. **Summarizes transcripts** with **BART (transformer model)** 📝
4. **Generates structured outputs**:

   * Full transcription → `TRANSCRIBE.TXT`
   * Smart per-scene summaries → `SUMMARIZED_TEXT.TXT`

✅ Ideal for **lectures, podcasts, meetings, tutorials** → instantly create notes & highlights!

---

## ✨ Features

* 🔍 **Scene Detection** – Splits video into meaningful shots (PySceneDetect).
* 🗣 **Speech-to-Text** – Converts speech to text using Whisper (multilingual support).
* 📝 **Summarization** – Uses BART to generate concise summaries for each scene.
* 🎯 **Smart Framing** – Adds natural phrasing like “The speaker explains…” for clarity.
* 📂 **Outputs** – Saves both full transcripts & concise summaries for further use.

---

## 🛠 Tech Stack

* [Whisper](https://github.com/openai/whisper) – Speech recognition
* [BART](https://huggingface.co/facebook/bart-large-cnn) – Text summarization
* [PySceneDetect](https://github.com/Breakthrough/PySceneDetect) – Scene boundary detection
* [MoviePy](https://github.com/Zulko/moviepy) – Video editing utilities
* [NLTK](https://www.nltk.org/) – Sentence tokenization
* [FuzzyWuzzy](https://github.com/seatgeek/fuzzywuzzy) – Text similarity

---

## 🚀 Setup & Installation

Run in **Google Colab** or locally with Python 3.9+

```bash
# Install dependencies
pip install -q transformers moviepy scenedetect git+https://github.com/openai/whisper.git ffmpeg-python nltk fuzzywuzzy python-Levenshtein
```

---

## 📂 Usage

### 1️⃣ Upload Input Video

Place your video in `/content/input/test.mp4` (or update the path).

### 2️⃣ Run the Pipeline

```python
python main.py  # or run the notebook cells in Colab
```

### 3️⃣ Outputs

* `TRANSCRIBE.TXT` → Full speech-to-text transcript
* `SUMMARIZED_TEXT.TXT` → Smart per-scene summaries

---

## 📊 Example Output

**Transcript (excerpt):**

```
[0.0 – 15.3]:
Welcome to this tutorial on deep learning basics...
```

**Summary (excerpt):**

```
[0.0 – 15.3]: The speaker explains that this is a tutorial on deep learning basics.
```

---

## 🌟 Future Improvements

* 📌 Merge summaries → Create a final video abstract
* ✂️ Auto-generate **short highlight video** with key scenes
* 🧾 Add **topic classification & keyword extraction**
* 🤖 Build a **Q\&A chatbot** over the transcript

---

## 📜 License

CIT License © 2025

---

## 👨‍💻 Author

Developed By: KARTIK KUMAR
USN: 1CD22CS061
