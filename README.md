Installation
Make sure you have Python 3.7 or higher installed.

Install the required packages:
pip install fastapi uvicorn textblob httpx pytest
Clone the repository or deploy it to AWS AppRunner as shown in this video.
Running the app
Start the app by running:

uvicorn main:app --host 0.0.0.0 --port 8080
The app will be available at http://127.0.0.1:8080.

API Endpoints
/sentiment (POST)
Takes a JSON payload with a "text" field and returns the sentiment score.

Example request:

{
  "text": "I love this!"
}
Example response:

{
  "sentiment_score": 10
}
Testing
To run the tests, execute:

pytest test_app.py
# or just
pytest
License
This project is licensed under the Apache License.
