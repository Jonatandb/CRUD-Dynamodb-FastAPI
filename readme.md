# CRUD AWS DynamoDB con FastAPI
https://www.youtube.com/watch?v=vm2vXdTfZI8

---
## Create environment
- python -m venv venv

## Activate environment
- source venv/Scripts/activate

## Install dependencies
- pip install -r requirements.txt

## Download dynamodb-local + dynamodb-admin docker image
- docker pull instructure/dynamo-local-admin

## Start dynamodb docker container
- docker run -p 8000:8000 -it --rm instructure/dynamo-local-admin

## Visit dynamodb-admin website
- http://localhost:8000

## Start app
- uvicorn main:app --reload --port 80 --env-file=".env"

## Visit root URL
- http://localhost/

