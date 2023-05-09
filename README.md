## pertemuan untuk mencontoh docker
di sini adalah contoh untuk membuat docker dari python
## Penggunaan
di sesi ini diasumsikan sudah install docker
## tanpa docker
```
pip install -r requirements.txt
uvicorn main:app --host 0.0.0.0 --port 8080 --reload
```
## dengan docker
build image local
````
docker build -t contoh-api .
docker run -d -p 8080:80 contoh-api
```

## dengan docker-compose
```
docker-compose up --build
```
menggunakan docker compose bisa kelihatan ketika update dan image terestart otomatis
