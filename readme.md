# CRUD AWS DynamoDB con FastAPI
https://www.youtube.com/watch?v=vm2vXdTfZI8

---

## Create environment:
- python -m venv venv

## Activate environment:
- source venv/Scripts/activate

## Install dependencies:
- pip install -r requirements.txt

## Prepare .env file:
- Copy and rename ".env.example" to ".env"

## Download dynamodb-local + dynamodb-admin docker image:
- docker pull instructure/dynamo-local-admin

## Start dynamodb docker container (in another shell):
- docker run -p 8000:8000 -it --rm instructure/dynamo-local-admin

## Start app:
- uvicorn main:app --reload --port 80 --env-file=".env"

## Visit Swagger website to interact:
- http://localhost/docs

## Visit dynamodb-admin website to check database:
- http://localhost:8000
