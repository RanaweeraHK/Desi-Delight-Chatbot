# Desi Delight Chatbot for Royal Spice

![Try Magic Design (2)](https://github.com/RanaweeraHK/Food-Chatbot/assets/129282753/04c51c35-5869-4051-85f4-d3e1c10b5640)


Desi Delight is a chatbot developed for the Indian food website Royal Spice. It uses Dialogflow for chatbot functionalities, FastAPI for the backend, and HTML/CSS for the frontend.

## Directory Structure

- **backend:** Contains Python FastAPI backend code.
- **db:** Contains the dump of the database. Import this into your MySQL database using MySQL Workbench.
- **dialogflow_assets:** Contains training phrases and other assets for Dialogflow intents.
- **frontend:** Contains website code using HTML and CSS.

## Installation

Install the required Python modules using pip:

```bash
pip install mysql-connector
pip install "fastapi[all]"
```


## Starting the FastAPI Backend Server

1. Navigate to the backend directory in your command prompt.
2. Run the following command to start the FastAPI server:

```bash
uvicorn main:app --reload
```

## Ngrok for HTTPS Tunneling

1. Download Ngrok from [https://ngrok.com/download](https://ngrok.com/download) and install the version suitable for your OS.
2. Extract the zip file and place ngrok.exe in a folder.
3. Open Windows Command Prompt, navigate to that folder, and run the following command to create an HTTPS tunnel:

```bash
ngrok http 8000
```

Note: Ngrok sessions can expire, so restart if you encounter a session expiration message.

## Usage

Once the backend server and Ngrok tunnel are running, access the frontend by visiting the Ngrok HTTPS URL generated. The chatbot will be available for interactions related to Indian cuisine and Royal Spice.
