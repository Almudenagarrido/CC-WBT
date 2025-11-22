# CC-WBT – Execution Guide (Demo Version)

This document provides a simple step-by-step guide to run the demo version of the CC-WBT platform locally.
Please note that the platform is still under development, and some features may be incomplete or subject to change.

## 1. Create a Virtual Environment

From the root directory of the project (CC-WBT), create a virtual environment:

python -m venv venv

## 2. Activate the Virtual Environment
Windows
venv\Scripts\activate

macOS / Linux
source venv/bin/activate

## 3. Install Dependencies

Once the environment is active, ensure you are in the root CC-WBT folder and install all required packages:

pip install -r requirements.txt


Note:
All required libraries should already be listed in requirements.txt.
If anything is missing, you can install it manually:

pip install <package_name>

## 4. Running the Demo Platform

You will need two terminals, both with the virtual environment activated.

Terminal 1 – Run the Frontend

From the project root:

cd frontend
streamlit run app.py

Terminal 2 – Run the Backend

From another terminal (with the environment activated):

cd backend
uvicorn main:app --reload --port 8001


Once both services are running, you will be able to interact with the demo version of the platform.
Some features, calculations, and validations are still in progress and not representative of the final product.