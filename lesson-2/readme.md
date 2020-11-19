# lesson-2


### Simple NodeJS menggunakan docker

1. Build Docker Image
    ```
    docker build -t node-test .
    ```
2. Run

    ```
    docker run -p 8080:8080 --name node-test-1 -d node-test
    ```