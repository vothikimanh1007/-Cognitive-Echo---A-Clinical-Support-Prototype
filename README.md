# Cognitive Echo: A Clinical Support Prototype

This repository contains the full codebase, analysis, and models for the research paper: **"The Digital Scribe: A Computational Analysis of the Thematic and Emotional Architecture of English-Language Autobiographical Memory."**

The project introduces **Cognitive Echo**, a proof-of-concept application designed to analyze the emotional and thematic content of personal narratives, bridging the gap between computational linguistics and clinical psychology.

---

## 📄 Project Overview

This research explores the structure of human memory by applying state-of-the-art Natural Language Processing (NLP) models to a corpus of autobiographical narratives. The core objectives are:

- **Emotional Valence Quantification**: To accurately measure the emotional tone of personal stories.
- **Thematic Analysis**: To discover the latent, recurring themes within these narratives.
- **Methodological Contribution**: To provide a scalable, data-driven framework for "digital phenotyping."
- **Clinical Application**: To develop 'Cognitive Echo,' a prototype tool that demonstrates how this technology could augment therapeutic practice.

This work is grounded in established psychological theories, including Conway's Self-Memory System, McGaugh's memory modulation hypothesis, and Pennebaker's expressive writing paradigm.

---

## 🔬 A Self-Contained Research Artifact

For maximum accessibility and reproducibility, this entire project—from data collection to a functional web application—is encapsulated within a single Google Colab notebook. This approach allows any researcher to replicate our findings and interact with our models with just a web browser and a Google account.

---

## 📂 Repository Structure

The repository has been simplified to support the single-notebook workflow:
...

## 🚀 Getting Started: Running the Notebook

Follow these steps to run the entire research pipeline.

### Step 1: Open in Google Colab
Click the button below to open the main notebook directly in Google Colab:

[Open in Google Colab](<your-colab-link>)

### Step 2: Configure API Credentials
The notebook needs to connect to Reddit's API for the initial data collection step. For security, you must provide your credentials using Colab's "Secrets" manager.

In the Colab notebook, click the key icon (🔑) on the left sidebar.

Add the following three secrets:

- `CLIENT_ID` -> [Your Reddit App Client ID]
- `CLIENT_SECRET` -> [Your Reddit App Client Secret]
- `USER_AGENT` -> [A unique string, e.g., "MyResearchApp/1.0 by YourUsername"]

### Step 3: Run the Notebook Sequentially
The notebook is divided into parts. Run each code cell from top to bottom:

1. **Part 0: Environment Setup**: Installs all necessary libraries.
2. **Part 1: Data Collection**: Connects to Reddit and scrapes the raw data. *(Note: This part will automatically be skipped if it finds an existing data file (`reddit_narratives_anonymized.csv`), so you only need to run it once.)*
3. **Part 2: Model Generation and Analysis**: Loads the data, trains the Sentiment and Topic models, saves them, and generates all the analytical charts from the paper.
4. **Part 3: Application Prototype**: Loads the saved models and launches the 'Cognitive Echo' Gradio web app.

### Step 4: Interact with the Prototype
The final cell will launch the Gradio application and provide a public URL (ending in `.gradio.live`). Click this link to open the interactive prototype in a new browser tab and analyze your own text.

---

## 📄 Citation

If you use the code, models, or findings from this project in your research, please cite our paper:

```bibtex
@article{YourLastName_2025_DigitalScribe,
  title   = {The Digital Scribe: A Computational Analysis of the Thematic and Emotional Architecture of English-Language Autobiographical Memory},
  author  = {[Vo Thi Kim Anh]},
  journal = {[...]},
  year    = {2025},
  volume  = {[...]},
  pages   = {[...]}
}

### Notes:
- Replace `<your-colab-link>` with the actual link to your Google Colab notebook.
- Modify the citation format with the correct author and publication details when the paper is finalized.
