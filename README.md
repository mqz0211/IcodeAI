# iCodeMath Gemini Gem Setup

## 🚀 Project Overview

This project sets up a **Gemini-powered visual language model GEM** to analyze visual mathematical concepts from images and provide explanations based on a fine-tuned dataset.

It uses Google Gemini's **Gem creation feature**, not local hosting or APIs. Users trigger image analysis using prompts that start with `!`.

---

## 📁 What You Need to Do

1. **Download the Provided Resources**

   * [Download All 25 Images](./images/) (10 → 10 → 5 order)
   * [Download `dataset.jsonl`](./dataset.jsonl)

2. **Upload Them into Your Gemini Chat**

   * Upload all 25 images to the `images/` folder
   * Upload `dataset.jsonl` to the root

> ⚠️ **All 25 image filenames must match the entries in `dataset.jsonl`. Place them in the `images/` folder. Any mismatch will cause the GEM to say: “This image is not found in the dataset.”**

---

## 🧠 GEM Prompt Setup

Paste this into your GEM creation interface:

---

### 📜 GEM Behavior Instruction:

```
You are an expert AI tutor specialized in analyzing mathematical concept illustrations. You are connected to a reference database (dataset.jsonl) that links image filenames to their explanations.

Your purpose is to help students learn visual math concepts from the uploaded image set.

Rules:
1. Ask the user to download and upload the provided image set and dataset.jsonl during the first three messages:
   - "Please download and upload the 25 iCodeMath concept images. (I WILL UPLOAD EXACTLY 25 PHOTOS FOLLOWING 10-10-5. YOU WILL ANALYZE AND FULLY UNDERSTAND. IT ALSO HAS CONNECTION WITH DATASET.JSONL.)"
   - "Also download and upload the dataset.jsonl file to link the images with their explanations."
2. Only analyze an image if the user’s message starts with `!`. Otherwise, ignore image input.
3. When the prompt starts with `!`, match the image filename to dataset.jsonl and explain its concept in full.
4. If a filename is not found, say: "This image is not found in the dataset."
5. Be clear, accurate, and helpful. Your tone is that of a friendly expert tutor.
```

---

## ⚙️ How to Setup the GEM

1. Go to [Google Gemini App](https://gemini.google.com/app)
2. Click **"Create a custom Gemini"**
3. Paste the above instruction into the "Custom behavior" box
4. Name it `iCodeMath Tutor`
5. Set visibility (private, link-only, or public)
6. Save and test by uploading the files

---

## 💡 How to Use It

* Upload the downloaded images in 3 batches: **10 → 10 → 5** into the `images/` folder
* Upload the `dataset.jsonl` file to the root
* Ask questions using `!`, like:

```
!Explain the uploaded concept
```

* The model will analyze the image(s) and answer using the dataset

---

## 📝 Example dataset.jsonl

```json
{"image": "triangle_area.png", "text": "This image explains how to calculate the area of a triangle using the formula: 1/2 * base * height."}
{"image": "pie_chart_parts.png", "text": "This shows a pie chart divided into fractions representing data distribution."}
```

---

## 📜 License

This project is licensed under the **Apache License 2.0**.

> ⚠️ **Please read the LICENSE before using, modifying, or distributing this project.**

You are free to use, modify, and distribute this project as long as you comply with the terms of the Apache License.

---

## ✅ Final Notes

* No local environment or API is needed
* Fully cloud-hosted using Gemini UI
* Perfect for students, educators, or visual learners

Let me know if you’d like to expand the GEM to include quizzes, multilingual support, or concept progress tracking!
