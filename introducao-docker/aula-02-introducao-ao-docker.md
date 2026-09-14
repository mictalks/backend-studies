# Aula 02 - Imagens e Containers no Docker

## O que são imagens no Docker?

As imagens Docker são modelos prontos usados para criar containers.

Elas contêm os arquivos, dependências e configurações necessárias para executar uma aplicação.

**Imagem = modelo pronto**

**Container = imagem em execução**

## Comandos WSL

| Comando | O que faz |
|---|---|
| `wsl -l -v` | Lista as distribuições Linux instaladas no WSL e mostra detalhes como estado e versão do WSL. |
| `wsl --install -d <name>` | Instala uma distribuição Linux específica no WSL. Ex.: `wsl --install -d Ubuntu-24.04`. |
| `wsl --list --online` | Lista as distribuições Linux disponíveis para instalação. |
| `wsl --set-version <name> 1` | Altera uma distribuição específica para usar o WSL 1. |
| `wsl --list --verbose` | Mesma função de `wsl -l -v`: lista as distribuições instaladas, estado e versão. |
| `mkdir <nome>` | Cria um novo diretório. Ex.: `mkdir fiap`. |
| `cd <diretório>` | Acessa um diretório. Ex.: `cd fiap`. |
| `pwd` | Mostra o caminho do diretório atual. |
| `ls -la` | Lista os arquivos e diretórios, incluindo arquivos ocultos e informações detalhadas. |

## Comandos Docker

| Comando | O que faz |
|---|---|
| `docker version` | Mostra as versões do Docker Client e Docker Server/Engine. |
| `docker container` | Mostra os comandos disponíveis para gerenciamento de containers. |
| `docker container ls` | Lista os containers que estão em execução. |
| `docker container ls -a` | Lista todos os containers, inclusive os que já foram finalizados. |
| `docker image ls` | Lista as imagens Docker disponíveis na máquina. |
| `docker container run -it node:18-slim` | Cria e executa um container utilizando a imagem `node:18-slim` em modo interativo. |
| `docker --help` | Exibe os comandos e opções disponíveis no Docker. |

## Containers executados

### Hello World

```bash
docker container run hello-world