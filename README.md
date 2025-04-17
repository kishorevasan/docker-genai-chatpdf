# Chat PDF App using Llama2 and Docker

A simple GenAI app for [Docker's Docs](https://docs.docker.com/) based on the [GenAI Stack](https://github.com/docker/genai-stack) PDF Reader application. This app uses **Llama2, Docker, Neo4j.**

The app is built based on Tech With Tim tutorial, [watch here](https://youtu.be/Y9YbCvzAwas). I would recommend watching it if you want to build this from scratch.

If you want to learn more about Docker, I would recommend this [video](https://youtu.be/pg19Z8LL06w)

The app should be ready to go once you clone the repository;

Here are the steps:
1. Download Docker
2. Download ollama
3. Download Neo4j
4. create a `.env` file; copy contents from `env.example` to the `.env` file; change `EMBEDDING_MODEL=ollama`
5. on the directory type `docker compose --build`
6. Go to the listed localhost and you should see the chat interface!!
7. Don't forget to type `docker compose down` once you are done using the app.

A few tips:
1. The app worked best when I was using the Docker Desktop client so I would highly recommend that.
2. It took way too long to vectorize a 27Kb file. There are ways to optimize it with gpu/ openai vector embeddings if you choose to use it.s
