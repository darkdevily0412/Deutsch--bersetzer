
#### Deutsch-Übersetzer ####
**English to German Translator**

Deutsch-Übersetzer is a Streamlit-based application that translates text between English and German using the T5 model from Hugging Face's Transformers library. This project provides a simple and intuitive interface similar to Google Translate.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Workflow](#workflow)
- [Model Details](#model-details)


## Overview
Deutsch-Übersetzer is designed to facilitate seamless translation between English and German. The application leverages the T5 (Text-To-Text Transfer Transformer) model, which is known for its efficiency and accuracy in various NLP tasks, including translation.

## Features
- Translate text from English to German and vice versa.
- Simple and intuitive UI built with Streamlit.
- Real-time translation results.
```markdown
## Installation
To set up the project, follow these steps:

1. **Clone the repository:**
    ```sh
    git clone https://github.com/darkdevily0412/deutsch-ubersetzer.git
    cd deutsch-ubersetzer
    ```

2. **Install the required packages:**
    ```sh
    pip install -r requirements.txt
    ```

3. **Download and set up ngrok:**
    ```sh
    wget -q -O ngrok.zip https://bin.equinox.io/c/4VmDzA7iaHb/ngrok-stable-linux-amd64.zip
    unzip -o ngrok.zip
    ```

4. **Install your ngrok authtoken:**
    ```sh
    ./ngrok authtoken <YOUR_NGROK_AUTHTOKEN>
    ```

## Usage
Run the Streamlit app using the following command:
```sh
streamlit run translator_app.py
```

## Workflow
1. **Load the T5 model and tokenizer:**
    - The T5 model is loaded from Hugging Face's Transformers library.
2. **Input Text:**
    - Users enter text in a text area provided in the UI.
3. **Select Translation Direction:**
    - Users select the translation direction (English to German or German to English).
4. **Translate Text:**
    - Upon clicking the "Translate" button, the input text is passed to the T5 model for translation.
5. **Display Translation:**
    - The translated text is displayed on the UI.

## Model Details
- **Model:** T5 (Text-To-Text Transfer Transformer)
- **Library:** Hugging Face Transformers
- **Pretrained Model:** `google/t5-small`
- **Time Complexity:** 
  - The translation process primarily involves encoding the input text and decoding the output text, both of which are linear in relation to the length of the input text. The overall time complexity is O(n), where n is the length of the input text.

