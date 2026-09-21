# Aula 01 - Gerenciamento de Contâineres I

O que veremos nessa aula:

* Como gerenciar containers
* Como criar imagens
* Como usar comandos de forma aprofundada
* Criar o primeiro Dockerfile
* Como a rede de um container funciona
* Criar um volume persistente de container
* Montar logs no container
* Registro de containers em cloud

## Comandos Docker / Contâineres executados

| Comando | O que faz |
|---|---|
| `docker container run -it ubuntu` | Cria e executa um container Ubuntu em modo interativo. |
| `exit` | Sai do terminal do container. |
| `docker container run -it node:18 /bin/bash` | Cria e executa um container com Node.js 18 e abre o terminal Bash dentro dele. |
| `docker container stats` | Mostra, em tempo real, o consumo de recursos dos containers, como CPU e memória. |
| `docker container attach [ID]` | Conecta o terminal a um container que está em execução. |
| `docker container restart [ID]` | Reinicia um container. |
| `docker container stop [ID]` | Para um container de forma controlada. |
| `docker container start [ID]` | Inicia novamente um container que está parado. |
| `docker container kill [ID]` | Interrompe imediatamente a execução de um container. |
| `docker container rm [ID]` | Remove um container. |
| `docker container top [ID]` | Mostra os processos em execução dentro de um container. |