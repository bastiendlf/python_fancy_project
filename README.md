# Python fancy app

Install dependencies :
```bash
pip install -r requirements.txt  
```

Run app :
```bash
uvicorn app.main:app --reload
```

-> Uvicorn running on http://127.0.0.1:8000

Build docker image : 
```bash
docker build -t myfastapi . 
```

Docker run container and use port 80:
```bash
docker run -d --name mycontainer -p 80:80 myfastapi
```

Optional, clean old docker containers:
```bash
docker rm $(docker ps -aq)
```