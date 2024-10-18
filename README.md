# milvus-docker

https://milvus.io/docs/install_standalone-docker-compose.md

# Local setup

Create virtual environment

```
python3 -m venv milvus-docker
source milvus-docker/bin/activate
pip install -r requirements.txt
```

Install any new packages if required and update requirements.txt simultaneously

```
pip install torch && pip freeze > requirements.txt
```

Start docker containers

```
docker-compose up -d
```

Run scripts locally
```
python app/create_collection.py
python app/generate_embeddings.py
```
