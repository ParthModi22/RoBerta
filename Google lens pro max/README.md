# Image Captioning and Web Search Application

This repository contains a Streamlit-based application that allows users to upload an image, optionally provide a text prompt, and receive an AI-generated caption based on the image and prompt. Additionally, the app performs a web search using DuckDuckGo API to retrieve relevant web results based on the generated caption or user input.

## Features
- **Image Captioning**: Automatically generate descriptive captions for uploaded images using BLIP (Bootstrapping Language-Image Pre-training) model.
- **Custom Text Prompts**: Influence caption generation by providing custom text prompts.
- **Web Search**: Perform a web search based on the generated caption or user input using DuckDuckGo API.
- **Streamlit Interface**: User-friendly interface for uploading images, entering prompts, and viewing search results.

## Setup Instructions

### 1. Get Your Public IP
To ensure your app is accessible, first get your public IP by running:
```bash
!wget -q -O - ipv4.icanhazip.com
3. Run the Streamlit App
To start the Streamlit app locally, use the following command:

bash
Copy code
streamlit run app.py
4. Create Public URL with LocalTunnel
To make your app accessible via a public URL, use LocalTunnel by running this command:

bash
Copy code
npx localtunnel --port 8501
This will provide you with a public-facing URL in the format https://<random-string>.loca.lt.

5. Access the App
Click on the provided LocalTunnel URL to access the Streamlit app in your browser.

6. Upload Image and Enter Text Prompt
Upload an image using the "Upload Image" button.
Optionally, enter a text prompt to guide the caption generation.
7. Get Search Results
Once the image and prompt (if any) are processed, the app will return relevant search results from the web based on the input.

Key Components
BLIP Image Captioning: The BLIP model is used to generate captions based on the uploaded image. Optionally, the caption can be influenced by a user-provided text prompt.
DuckDuckGo Web Search: The app uses DuckDuckGo's API to retrieve web search results based on the generated caption or the user's input query.
Streamlit Interface: Provides an interactive UI to upload images, generate captions, and display web search results.