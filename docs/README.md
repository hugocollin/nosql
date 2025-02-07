# README : NoSQL 

## Table of contents

- [Description](#description)
- [Prerequisites](#prerequisites)
- [Project structure](#project-structure)
- [Installation](#installation)
- [Contribution](#contribution)
- [Author](#author)

## Description

This project is a study of NoSQL databases. It is divided into 3 parts :
1. Redis database
2. MongoDB database
3. OrientDB database

## Prerequisites

- Anaconda
- Docker Desktop

## Project structure

```bash
├── data/
│   ├── movielens_movies.json
│   └── movielens_users.json
├── docs/
│   └── README.md
├── lecture/
│   └── nosql_lecture.pdf
├── notebooks/
│   ├── 1-redis.ipynb
│   ├── 2-mongo.ipynb
│   └── 3-orientdb.ipynb
└── .gitignore
```

## Installation

Remember to use the `Anaconda Powershell` prompt at the root of your project.

```
conda create -n nosql python=3.7
conda activate nosql
conda install -c anaconda mongo-tools
pip install jupyter jupyterlab redis pymongo
```

To run your jupyter notebook: `jupyter notebook` or `jupyter lab`

### Run Redis

In a separate command line prompt:

```
docker run -it --rm --name some-redis -p 6379:6379 redis
```

### Run MongoDB

In a separate command line prompt:

```
docker run -it --rm --name some-mongo -p 27017:27017 mongo:4
```

### Run OrientDB

In a separate command line prompt:

```
docker run -it --rm --name some-orientdb -p 2424:2424 -p 2480:2480 -e ORIENTDB_ROOT_PASSWORD=root orientdb:2.2
```

## Contribution

All contributions are welcome. Here's how you can help :

1. Fork the project.
2. Create your feature branch (git checkout -b feature/AmazingFeature).
3. Commit your changes (git commit -m 'Add some AmazingFeature').
4. Push to the branch (git push origin feature/AmazingFeature).
5. Open a pull request.

## Author

This project was developed by COLLIN Hugo a student from the Master 2 SISE program at the University of Lyon 2.