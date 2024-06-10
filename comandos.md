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


# Parte 2
| Ação                                                               | Comando                                                   |
| ------------------------------------------------------------------ | --------------------------------------------------------- |
| Listar imagens disponíveis                                         | `docker images`                                           |
| Criar uma tag para uma imagem (-t)                                 | `docker build -t <image-name>:<tag-name> .`               |
| Executar imagem no modo interativo (-it) no shell                  | `docker run -it <image-name> sh`                          |
| Mapear e executar na porta do container  (-p) e em background (-d) | `docker run -dp 3000:3000 <image-name>`                   |
| Adicionar uma tag a uma imagem existente                           | `docker image tag <image> <image-name>:<tag-name>`        |
| Realizar login no Docker Hub                                       | `docker login`                                            |
| Fazer push de uma imagem para um repositório                       | `docker push <image-name>:<tag-name>`                     |
| Remover uma imagem                                                 | `docker image rm <image>`                                 |
| Remover o arquivo de configuração do Docker                        | `rm ~/.docker/config.json`                                |
| Salvar imagem local em .tar                                        | `docker image save -o <arch-name> <image-name>:<tag-name>`|
| Carregar uma imagem de um arquivo (upload)                         | `docker image load -i <arquivo>.tar`                      |