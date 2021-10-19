# .NET CORE WEB API Project

### Project done as a side project in order to learn .Net Core Web Api, includes:
1. Basic WEB API server.
2. Unit Testing.
3. Used Docker.
4. Used kubernetes.
5. Secrets and Health Checks

3. Start a MongoDb docker image using the following command:
    ```bash
    docker run -d --rm --name mongo -p 27017:27017 -v mongodbdata:/data/db -e MONGO_INITDB_ROOT_USERNAME=mongoadmin -e MONGO_INITDB_ROOT_PASSWORD=Pass#word1 --network=net5tutorial mongo
    ```
4. Download/Run the web api image from Docker Hub using the following command:
    ```bash
    docker run -it --rm -p 8080:80 -e MongoDbSettings:Host=mongo -e MongoDbSettings:Password=Pass#word1 --network=net5tutorial gikodocker/catalog:v3
    ```

