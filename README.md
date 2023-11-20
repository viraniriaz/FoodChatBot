# Chatbot with Generative Model using Dialogflow, FastAPI, and MySQL

## Overview

This project implements a chatbot using Google's generative model through Dialogflow. The backend is built with FastAPI, and data is stored in a MySQL database. The chatbot understands natural language through the use of intents and entities.

## Features

- **Generative Model**: Utilizes Google's generative model via Dialogflow for natural language understanding.
- **FastAPI Backend**: Implements a FastAPI backend to handle communication with the chatbot.
- **MySQL Database**: Uses MySQL to store and retrieve data for a seamless user experience.
- **Intent and Entities**: Leverages Dialogflow's intent and entity recognition for better comprehension of user inputs.

## Setup

### Prerequisites

- [Dialogflow](https://cloud.google.com/dialogflow): Set up a Dialogflow project and obtain API credentials.
- [FastAPI](https://fastapi.tiangolo.com/): Install FastAPI for the backend.
- [MySQL](https://www.mysql.com/): Set up a MySQL server and configure the database.
- [Ngrok](https://ngrok.com/): Install Ngrok for secure HTTPS connections.

### Installation

1. **Clone the repository:**

    ```bash
    cd FoodChatBot
    ```

2. **Install dependencies:**

    ```bash
    pip install fastapi[all]
    ```

3. **Configure your credentials:**

    - Update the MySQL connection details in `db_helper`.

4. **Run the FastAPI server:**

    ```bash
    uvicorn main:app --reload
    ```
5. **Secure the connection with Ngrok (for HTTPS):**

    - Start Ngrok to expose your local server securely:

      ```bash
      ngrok http 8000
      ```

    - Obtain the Ngrok HTTPS URL and update your Dialogflow webhook settings accordingly.
6. **Open the app in your browser:**

    ```
    http://localhost:8000/
    ```

## Usage

1. Use the provided endpoints to interact with the chatbot and manage data stored in the MySQL database.

## Contributing

Feel free to contribute by opening issues or creating pull requests. Your feedback and enhancements are welcome!


