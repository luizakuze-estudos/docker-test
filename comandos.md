| Ação                                                             | Comando                        |
|------------------------------------------------------------------|-------------------------------|
| Procurando por imagens no Docker Hub                             | `docker search openjdk`       |
| Baixando uma imagem do Docker Hub                                | `docker pull ubuntu`          |
| Listando as imagens armazenadas (baixadas ou geradas) em seu computador | `docker image ls`             |
| Apagando as imagens que não são usadas por qualquer contêiner    | `docker image prune`          |
| Listando o espaço ocupado em disco por imagens, contêineres, etc.| `docker system df`            |
| Listando os contêineres que estão em execução                    | `docker ps`                   |
| Listando os contêineres que estão em execução e os inativos      | `docker ps -a`                |
| Verificando estatísticas (uso de CPU, memória, I/O) dos contêineres ativos | `docker stats`            |
| Finalizando a execução de um contêiner                           | `docker stop <container ID ou nome do contêiner>` |
| Removendo um contêiner                                           | `docker rm <container ID ou nome do contêiner>`   |
| Removendo todos os contêineres inativos de uma só vez            | `docker container prune`      |
