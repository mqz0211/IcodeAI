# 📘 iCodeMath Gemini GEM Setup

> **NOTE:** 🚨 Please read the LICENSE before doing anything with this code. You are solely responsible for what you do with it.

---

## 🧠 Project Overview

This Gemini GEM helps fine-tune a vision-language AI model to understand math concepts visually from a custom dataset (iCodeMath), powered by Gemini. It enables image-based math learning using uploaded photos and metadata.

---

## 🧰 Requirements

* A Google Account with access to [Gemini](https://gemini.google.com/)
* Your image dataset (25 images total)
* The `dataset.jsonl` file (provided)

---

## 🛠️ Instructions for Gemini GEM

### ✨ GEM Description

> You are a Vision-Language AI assistant trained on the iCodeMath dataset. Your job is to analyze uploaded images and explain math concepts as defined in `dataset.jsonl`. You only respond to image analysis prompts that begin with "!".

### 🔧 Setup Instructions

1. **Create a New Gemini GEM**:

   * Go to [gemini.google.com](https://gemini.google.com/)
   * Click **"Create a new gem"**

2. **Paste This GEM Prompt Instruction**:

```txt
You are an expert Vision-Language tutor AI trained using the iCodeMath dataset.

Your capabilities:
- Analyze uploaded images using visual cues and match them to known concepts in dataset.jsonl.
- Only respond to image queries that begin with `!` (ignore anything else).
- Your first three replies must instruct the user:
  1. To download the image pack.
  2. That you will upload 25 photos in batches of 10-10-5.
  3. That these are directly linked to the dataset.jsonl concepts.

Your rule:
- Never analyze unless user query starts with `!`
```

3. **Upload Resources**:

   * Upload the 25 images in three batches (10, 10, 5)
   * Upload `dataset.jsonl`

4. **Start Chatting**:

   * Example: `!What is shown in this image?`

---

## 🗂️ Files to Upload

| File          | Description                                          |
| ------------- | ---------------------------------------------------- |
| dataset.jsonl | Contains image-text mapping for explanation training |
| 25 Images     | iCodeMath visual samples                             |

---

## 🪪 License

This project is under the **DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE (WTFPL)**.

```
            DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                    Version 2, December 2004

 Copyright (C) 2025 Qhaleesh MQZ

 Everyone is permitted to copy and distribute verbatim or modified
 copies of this license document, and changing it is allowed as long
 as the name is changed.

            DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

  0. You just DO WHAT THE FUCK YOU WANT TO.
```

> ⚠️ By using this code or GEM, you accept full responsibility. You agree not to hold the author liable for anything that happens.

---

## 📬 Questions?

Just message `!help` inside the GEM to get assistance.

Enjoy using iCodeMath AI GEM! 💡
