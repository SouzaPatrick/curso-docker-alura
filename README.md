# curso-docker-alura


Comandos bashos docker
- Comando basicos do docker
executar container
```
docker run <nome_imagem>
```
executar container podendo escrever no terminal
```
docker run -it <nome_imagem>
```
iniciar container
```
docker start <id_container>
```
iniciar container podendo escrever no terminal
```
docker start -a -i <id_container>
```
Apagar container
```
docker rm  <id_container>
```
Listar container ativos
```
docker ps
```
Listar todos os containers 
```
docker ps -a
```
Listar todas as imagens
```
docker images
```
Apagar todos os container parados
```
docker container prune
```
Apagar imagem
```
docker rmi  <id_imagem>
```
Apagar todas as imagens
```
docker rmi  $(docker images -q)
```
Parar todos os containers de uma vez
```
docker stop -t 0  $(docker ps -q)
```
Mostras as configuracoes do container
```
docker inspect <id_container>
```
Criar uma rede bridge para a comunicacao entre containes pelo nome
```
docker network create --driver bridge minha-rede
```