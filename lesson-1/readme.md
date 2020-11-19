# lesson-1


Simple NGINX menggunakan docker

#### Menjalankan via CLI
Di linux
```
docker run --name nginx -p "8080:80" -v $(pwd)/html/:/usr/share/nginx/html -d nginx:1.19.4-alpine
```
Di windows (powershell)
```
docker run --name nginx -p "8080:80" -v ${PWD}/html/:/usr/share/nginx/html -d nginx:1.19.4-alpine
```

### Using Dockerfile

```
docker build -t nginx-using-dockerfile .
```
Kemudian jalankan docker image yang barusan dibuat

```
docker run -p 8080:80 --name nginx-with-dockerfile-container -d nginx-using-dockerfile
```