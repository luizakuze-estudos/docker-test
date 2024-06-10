| Ação                                                        | Comando                                      |
|-------------------------------------------------------------|----------------------------------------------|
| Executar um shell em um contêiner                           | docker run -it <app> sh                        |
| Construir uma imagem                                        | docker build -t <nome> .                     |
| Listar imagens disponíveis                                  | docker images                                |
| Executar um contêiner em segundo plano                      | docker run -dp 3000:3000 <nome>              |
| Criar uma tag para uma imagem                               | docker build -t <nome>:v1.0.0 .              |
| Remover uma imagem                                          | docker image remove <nome>:v1.0.0            | 
| Construir uma imagem                                        | docker build -t <nome>:<tag> .               |
| Adicionar uma tag a uma imagem                              | docker image tag <id_da_imagem> <nome>:v1    |
| Realizar login no Docker Hub                                | docker login                                 |
| Realizar login no Docker Hub com nome de usuário específico | docker login -u <usuário>                    |
| Inicializar o pass                                          | pass init                                    |
| Realizar login no Docker Hub com nome de usuário específico | docker login -u <usuário>                    |
| Inicializar o pass com token de acesso                      | pass init <token_de_acesso>                  |
| Realizar login no Docker Hub com nome de usuário específico | docker login -u <usuário>                    |
| Fazer push de uma imagem para um repositório                | docker push <nome>:v1                        |
| Limpar construtores não utilizados                          | docker builder prune                         |
| Realizar logout do Docker Hub                               | docker logout                                |
| Realizar login no Docker Hub com nome de usuário específico | docker login -u <usuário>                    |
| Remover o arquivo de configuração do Docker                 | rm ~/.docker/config.json                     | 
| Fazer push de uma imagem para um repositório                | docker push <nome>:v1                        | 
| Salvar uma imagem em um arquivo                             | docker image save -o <arquivo>.tar <nome>:v1 |
| Remover uma imagem                                          | docker image rm <id_da_imagem>               |
| Carregar uma imagem de um arquivo                           | docker image load -i <arquivo>.tar           |
