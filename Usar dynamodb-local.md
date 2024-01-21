

# Usar Dynamodb-local y Dynamodb-admin

## Forma 1:
- Descargar imagen de docker de dynamodb-local:
  - docker pull amazon/dynamodb-local

- Iniciar contenedor:
  - docker run -p 8000:8000 amazon/dynamodb-local
      - (Luego de esto ya se puede conectar a dynamodb-local desde una API)

- Instalar globalmente dynamodb-admin con npm:
  - npm install -g dynamodb-admin

- Iniciar dynamodb-admin:
  - set DYNAMO_ENDPOINT=http://localhost:8000 && dynamodb-admin

- Acceder al admin web:
  - http://localhost:8001

Fuentes:
- https://codestax.medium.com/building-scalable-serverless-crud-apis-with-fastapi-and-aws-dynamodb-local-a-step-by-step-guide-794e146278e1
- https://www.npmjs.com/package/dynamodb-admin


## Forma 2:
- Descargar imagen de docker que ya posee dynamodb-local + dynamodb-admin:
  - docker pull instructure/dynamo-local-admin

- Iniciar contenedor:
  - docker run -p 8000:8000 -it --rm instructure/dynamo-local-admin

- Acceder al admin web:
  - http://localhost:8000

Fuente:
- https://github.com/instructure/dynamo-local-admin-docker
