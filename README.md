# Medical_Chatbot

MediBot is an AI-powered medical chatbot that assists users with information on various medical conditions. Leveraging advanced language models and a knowledge base of medical texts, MediBot provides informative responses based on user symptoms and queries. This project is built using Python, LangChain, and Pinecone, integrated with OpenAI’s GPT for natural language understanding.


## Features

Interactive Chat Interface: Users can interact with MediBot via a simple and intuitive web interface.
Symptom-Based Search: Provides medical information based on symptoms input by the user.
Embeddings for Fast Retrieval: Uses Pinecone for efficient storage and retrieval of medical information embeddings.
Customizable Knowledge Base: Easily update the chatbot’s knowledge with additional medical data.

## Tech Stack

Python: Core programming language used for the application.
LangChain: Manages language model workflows and integrates AI tools.
Flask: Web framework used to create a simple web interface for the chatbot.
Pinecone: Vector database used for fast and scalable embedding storage and retrieval.
OpenAI GPT: Model used for generating responses based on user input.

## Getting Started
    Follow these steps to set up and run the MediBot project on your local machine.
    Prerequisites : 
    1) Conda (for environment management)
    2) Pinecone and OpenAI API keys (sign up on their respective sites to obtain)


## Installation
    1) Clone the Repository
        ```bash
        git clone https://github.com/your-repo-name.git
        cd your-repo-name
        ```

    2) Create a Conda Environment
        ```bash
        conda create -n medibot python=3.10 -y
        conda activate medibot
        ```

## Install Requirements

    1) Install the required Python libraries:
        ```bash
        pip install -r requirements.txt
        ```

    2) Configure API Keys
    Create a .env file in the root directory of the project and add your Pinecone and OpenAI API credentials as follows:
        PINECONE_API_KEY = "your_pinecone_api_key"
        OPENAI_API_KEY = "your_openai_api_key"

    3) Initializing the Database
    Run the following command to store medical embeddings in Pinecone:

    ```bash 
    python store_index.py
    ```

    4) Running the Application
    To start the Flask web application, run:

    ```bash
    python app.py
    ```

    5)Open your browser and go to http://localhost:5000 to interact with MediBot.


## Project Structure

    app.py: Main entry point for the web application.
    store_index.py: Script for storing medical data embeddings into Pinecone.
    requirements.txt: Lists all dependencies needed for the project.
    .env: Contains environment variables, such as API keys.

## Contributing

Feel free to fork this project, make improvements, and submit pull requests. All contributions are welcome!

## License

This project is licensed under the MIT License. See the LICENSE file for more information.
