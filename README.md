# aws-bedrock-generative-ai

# Build Generative AI applications with Amazon Bedrock

This repository contains code for building diverse AI applications using Amazon Bedrock's foundation models.

## Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites
* Python 3.9 or higher
* pip
* [get Model Access in Amazon Bedrock](https://us-east-1.console.aws.amazon.com/bedrock/home?region=us-east-1#/modelaccess)

### Installation

Clone the repo

```bash
git clone https://github.com/gitmurali/aws-bedrock-generative-ai.git
```

Install required packages

```bash
pip install -r requirements.txt
```

## Usage

This repository contains code for demonstrating how to build AI applications using Amazon Bedrock's foundation models.

### Image Generation

To generate images using Stable Diffusion, run the following command:

```bash
streamlit run image_generation.py
```

To run in docker container:

```bash
sudo docker build . -t generative-ai
sudo docker run -p 8501:8501 -d --rm -v ~/.aws:/root/.aws generative-ai
```

This will launch a Streamlit app where you can enter prompts to generate images in various styles.

### Chatbot

To interact with a chatbot built using Amazon Bedrock, LangChain, and Streamlit, run:

```bash
streamlit run chat_bedrock.py
```

Launch a Streamlit app where you can have a conversation with the chatbot, witnessing AI-powered conversational capabilities.
