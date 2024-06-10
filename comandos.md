# Parte 1
| Ação                                                                       | Comando                                           |
|----------------------------------------------------------------------------|---------------------------------------------------|
| Procurando por imagens no Docker Hub                                       | `docker search openjdk`                           |
| Baixando uma imagem do Docker Hub                                          | `docker pull ubuntu`                              |
| Listando as imagens armazenadas (baixadas ou geradas) em seu computador    | `docker image ls`                                 |
| Apagando as imagens que não são usadas por qualquer contêiner              | `docker image prune`                              |
| Listando o espaço ocupado em disco por imagens, contêineres, etc.          | `docker system df`                                |
| Listando os contêineres que estão em execução                              | `docker ps`                                       |
| Listando os contêineres que estão em execução e os inativos                | `docker ps -a`                                    |
| Verificando estatísticas (uso de CPU, memória, I/O) dos contêineres ativos | `docker stats`                                    |
| Finalizando a execução de um contêiner                                     | `docker stop <container ID ou nome do contêiner>` |
| Removendo um contêiner                                                     | `docker rm <container ID ou nome do contêiner>`   |
| Removendo todos os contêineres inativos de uma só vez                      | `docker container prune`                          |


# Parte 2 - Imagens
| Ação                                                               | Comando                                                    |
|--------------------------------------------------------------------|------------------------------------------------------------|
| Listar imagens disponíveis                                         | `docker images`                                            |
| Criar uma tag para uma imagem (-t)                                 | `docker build -t <image-name>:<tag-name> .`                |
| Executar imagem no modo interativo (-it) no shell                  | `docker run -it <image-name> sh`                           |
| Mapear e executar na porta do conteiner  (-p) e em background (-d) | `docker run -dp 3000:3000 <image-name>`                    |
| Adicionar uma tag a uma imagem existente                           | `docker image tag <image> <image-name>:<tag-name>`         |
| Realizar login no Docker Hub                                       | `docker login`                                             |
| Fazer push de uma imagem para o DockerHub                       | `docker push <image-name>:<tag-name>`                      |
| Remover uma imagem                                                 | `docker image rm <image>`                                  |
| Remover o arquivo de configuração do Docker                        | `rm ~/.docker/config.json`                                 |
| Salvar imagem local em .tar                                        | `docker image save -o <arch-name> <image-name>:<tag-name>` |
| Carregar uma imagem de um arquivo (upload)                         | `docker image load -i <arquivo>.tar`                       |


# Parte 3 - Conteiners

| Ação                                                | Comando                                             |
| --------------------------------------------------- | --------------------------------------------------- |
| Rodar conteiner em background, não trava o terminal | docker run -d  app:v1                               |
| Rodar conteiner com um noem específico              | docker run -d --name <name-conteiner>               |
| Verificar os logs, quando há erros                  | docker logs <id-conteiner>                          |
| Mapear e executar conteiner                         | docker run -d -p <host-port>:<docker-port>          |
| Parar execução do conteiner                         | docker stop <conteiner-name>                        |
| Iniciar conteiner que já existe                     | docker start <conteiner-name>                       |
| Executar um comando dentro do conteiner             | docker exec <conteiner-name> <commands (ls, cd...)> |
| Remover um conteiner                                | docker rm <conteiner-name>                          |




_nota: `docker run` para criar conteiner (+iniciar) e `docker start` se já existe (+iniciar)_