# 🍇🥑 LlamaIndex - Chat with the Nutrition AI

A chatbot powered by LlamaIndex that augments GPT 3.5 with the contents of the Human Nutrition textbook by University of Hawaii Food Science and Human Nutrition Program.

## Overview of the App

<img src="picture.png" width="75%">

- Takes user queries via Streamlit's `st.chat_input` and displays both user queries and model responses with `st.chat_message`
- Uses LlamaIndex to load and index data and create a chat engine that will retrieve context from that data to respond to each user query

## Demo App

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://nutritionbot.streamlit.app/)

## Get an OpenAI API key

You can get your own OpenAI API key by following the following instructions:
1. Go to https://platform.openai.com/account/api-keys.
2. Click on the `+ Create new secret key` button.
3. Next, enter an identifier name (optional) and click on the `Create secret key` button.
4. Add your API key to your `secrets.toml` file. If you don't already have a `secrets.toml` file, add a folder named `.streamlit`, create a file called `secrets.toml` within the folder, and add the following to it:
``` openai_key = <your key here> ```
   
Alternatively, you can use [Streamlit Community Cloud's secrets management feature](https://docs.streamlit.io/deploy/streamlit-community-cloud/deploy-your-app/secrets-management) to add your API key via the web interface.

> [!CAUTION]
> Don't commit your secrets file to your GitHub repository. The `.gitignore` file in this repo includes `.streamlit/secrets.toml` and `secrets.toml`. 

## Try out the app

Once the app is loaded, enter your question about nutrition and wait for a response.
