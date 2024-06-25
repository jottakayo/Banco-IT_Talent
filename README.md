# Dockerização do Banco de Dados


![Construção da Imagem Docker](script/img1.png)
![Verificação do Banco de Dados](script/img2.png)

## Passos

1. Construir a imagem:
    ```sh
    docker build -t desafio_it_talent_junho_01 .
    ```
2. Iniciar o contêiner:
    ```sh
    docker run --name desafio_it_talent_junho_01 -d --network host -e MYSQL_ROOT_PASSWORD=root_password desafio_it_talent_junho_01
    ```
3. Banco de dados:
    ```sh
    docker exec -it desafio_it_talent_junho_01 mysql -u root -p
    ```
