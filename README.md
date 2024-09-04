# Generative AI, LLMs, and Ollama

## Introduction

### What is Generative AI?
Generative AI refers to artificial intelligence systems capable of generating new content, such as text, images, music, and more. Unlike traditional AI models, which perform specific tasks like classification or prediction, generative AI models create new data that mimics the style or content of the training data they were fed. These models are commonly used in natural language processing (NLP), computer vision, and creative arts.

### Large Language Models (LLMs)
Large Language Models (LLMs) are a type of generative AI specifically designed to understand and generate human-like text. These models are trained on vast amounts of text data and leverage architectures like transformers to learn the intricacies of language. Popular LLMs include GPT-3, GPT-4, LLaMA, and more. LLMs have revolutionized fields like chatbots, content creation, and question-answering systems due to their advanced language understanding capabilities.

### Ollama
Ollama is a platform that allows developers to run, package, and share Large Language Models (LLMs) locally. It simplifies the deployment and management of LLMs on personal machines or local environments without the need for cloud infrastructure. Ollama provides tools to package models into self-contained environments, making it easy to run them on different systems without compatibility issues.

## Project Setup Instructions

This repository contains a `main.py` file that leverages Ollama to create a new model based on an existing one using `langchain` and `langchain-ollama`. Follow the instructions below to set up the environment and run the project.

### Step-by-Step Setup Instructions

#### 1. Clone the Repository

First, clone the repository to your local machine:

```bash
git clone https://github.com/kariyaraj/GenAI_Session.git
cd GenAI_Session
```

#### 2. Install Python and PIP

Ensure Python 3 and PIP are installed on your system. You can check if Python and PIP are installed by running:

```bash
python3 -m venv env
source env/bin/activate  # On Windows, use `env\Scripts\activate`
```

#### 3. Create a Python Virtual Environment

To keep dependencies isolated, create a Python virtual environment:

```bash
python3 --version
pip3 --version
```

#### 4. Install Required Packages

Install the necessary Python packages, including langchain, langchain-ollama, and ollama:

```bash
pip3 install langchain langchain-ollama ollama
```

#### 5. Install Ollama and pull the model

Install the necessary Python packages, including langchain, langchain-ollama, and ollama:

```bash
curl -sSfL https://ollama.com/download | sh
ollama --version
ollama pull gemma2:2b
```

#### 6. Run Main File


```bash
python3 main.py

```


#### 7.  Model Creation and Management with Ollama

The script will use Ollama's local deployment capabilities to manage and package the new model. Follow the prompts in the script to select a base model and provide the necessary configuration parameters for the new model.

```bash
ollama create <model_name> --file <file-name>
ollama run <model_name>
```
