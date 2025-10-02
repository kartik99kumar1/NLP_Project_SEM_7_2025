# 🎬 Speech-Driven Video Summarization

### Powered by **OpenAI Whisper + BART + PySceneDetect**
---
#[GOOGLE COLAB NOTEBOOK]([https://github.com/openai/whisper](https://colab.research.google.com/drive/1oZ-G_vubB6vwYYtojiaFXhPvrLhGXCtg?usp=sharing)) – Click here to view the full implementation.

---

## 📌 Project Overview

This project aims to **automatically generate concise summaries of videos** by combining **speech recognition**, **scene detection**, and **NLP summarization techniques**.

* 🗣️ **Speech-to-Text** with **Whisper (ASR)**
* 🎥 **Scene Detection** using **PySceneDetect**
* 📝 **Summarization** with **BART (Transformer model)**
* ⚡ **Smart Framing** for more natural, explanation-oriented summaries

The output is:

1. **Full Transcription** of the video (`TRANSCRIBE.TXT`)
2. **Shot-wise Smart Summaries** (`SUMMARIZED_TEXT.TXT`)

---

## 🚀 Features

* 🎬 **Automatic shot boundary detection**
* 🎤 **Accurate speech transcription** using Whisper
* ✨ **Context-aware summarization** with BART
* 🧠 **Smart framing of sentences** for a natural explanation flow
* 📂 **Output files for transcription and summary**

---

## 🛠️ Tech Stack

* [OpenAI Whisper](https://github.com/openai/whisper) – Speech Recognition
* [PySceneDetect](https://github.com/Breakthrough/PySceneDetect) – Shot/Scene Detection
* [Hugging Face Transformers](https://huggingface.co/transformers/) – BART Summarization
* [MoviePy](https://zulko.github.io/moviepy/) – Video Editing & Processing
* [NLTK](https://www.nltk.org/) – Sentence Tokenization
* [FuzzyWuzzy](https://github.com/seatgeek/fuzzywuzzy) – String Matching

---

## 📂 Project Workflow

1. **Setup & Installations** – Install dependencies (Whisper, PySceneDetect, BART, etc.)
2. **Load Input Video** – Upload your `.mp4` file into the notebook
3. **Scene Detection** – Detect video shot boundaries
4. **Audio Demux + Transcription** – Extract audio and generate transcripts
5. **Summarization & Framing** – Summarize transcripts using BART and frame them naturally
6. **Save Outputs** – Export transcription (`TRANSCRIBE.TXT`) and summaries (`SUMMARIZED_TEXT.TXT`)

---

## 📖 Example Output

**Input Video Scene:**

```
[0 – 15.4s]:
Today, we will discuss how to implement object-oriented programming in C++...
```

**Generated Summary:**

```
[0 – 15.4s]: The speaker explains that object-oriented programming in C++ is implemented using classes and objects.
```

---

## ▶️ How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```
2. Open the notebook in **Google Colab**
3. Upload your video file into `/content/input/`
4. Run the notebook cells step by step
5. Find the outputs:

   * `/content/TRANSCRIBE.TXT`
   * `/content/SUMMARIZED_TEXT.TXT`

---

## 📌 Use Cases

* 🎓 **Educational Videos** – Summarize long lectures into concise notes
* 🎥 **Media & Entertainment** – Extract scene-wise highlights
* 📊 **Business Meetings** – Get quick summaries of recorded sessions
* 📰 **Journalism** – Condense interviews into structured takeaways

---

## 📢 Future Enhancements

* 🤖 Integrate with **GPT-based abstractive summarization** for richer outputs
* 🌐 Deploy as a **web app** for easy video uploads
* 🔎 Add **topic-based search** inside summaries

---

## 👨‍💻 Author

**KARTIK KUMAR**
USN: `1CD22CS061`
Semester 7, **CITECH Bangalore**

---
