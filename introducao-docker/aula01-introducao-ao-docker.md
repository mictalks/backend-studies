# Aula 01 - Introdução ao Docker

O que veremos nessa aula:

* Instalação do WSL via PowerShell no Windows
* Instalação do Docker Desktop e configuração
* Comandos relacionados ao Docker
* Execução do primeiro container

---

## Qual problema o Docker pretende resolver?

Um dos problemas que o Docker ajuda a resolver é a execução de várias aplicações de forma isolada, evitando a necessidade de utilizar uma máquina virtual completa para cada aplicação e, consequentemente, reduzindo o consumo de recursos como CPU e memória RAM.

O Docker e os containers possuem um objetivo parecido com o de uma VM (Virtual Machine), que é isolar ambientes, porém os containers são mais leves e compartilham o Kernel do sistema operacional.

---

## O que é um Container?

O Container é um ambiente isolado que permite executar diferentes aplicações em uma mesma máquina, mantendo seus processos separados uns dos outros.

No Docker, é muito comum utilizar containers Linux. Alguns recursos importantes do Linux para o funcionamento dos containers são:

* **Kernel:** responsável pela comunicação entre o hardware e o software.
* **Cgroups (Control Groups):** responsáveis por controlar e limitar o uso de recursos, como CPU e memória RAM.
* **Namespaces:** responsáveis por isolar processos e recursos, como rede e sistema de arquivos, entre os containers.

## O que é o Ubuntu?

O Ubuntu é uma distribuição Linux. No Windows, podemos utilizá-lo por meio do WSL para ter um ambiente Linux dentro da máquina.

Nesse ambiente, podemos criar e navegar entre arquivos e diretórios, executar comandos Linux e trabalhar com ferramentas utilizadas no desenvolvimento e com o Docker.

> O Ubuntu não é responsável por gerenciar os containers. Quem realiza esse gerenciamento é o Docker Engine.

## Comandos úteis

| Comando                      | O que faz                                                                                     |
| ---------------------------- | --------------------------------------------------------------------------------------------- |
| `wsl -l -v`                  | Lista as distribuições Linux instaladas no WSL e mostra detalhes como estado e versão do WSL. |
| `wsl --install -d <name>`    | Instala uma distribuição Linux específica no WSL. Ex.: `wsl --install -d Ubuntu-24.04`.       |
| `wsl --list --online`        | Lista as distribuições Linux disponíveis para instalação.                                     |
| `wsl --set-version <name> 1` | Altera uma distribuição específica para usar o WSL 1.                                         |
| `wsl --list --verbose`       | Mesma função de `wsl -l -v`: lista as distribuições instaladas, estado e versão.              |
| `mkdir <nome>`               | Cria um novo diretório. Ex.: `mkdir fiap`.                                                    |
| `cd <diretório>`             | Acessa um diretório. Ex.: `cd fiap`.                                                          |
| `pwd`                        | Mostra o caminho do diretório atual.                                                          |
| `ls -la`                     | Lista os arquivos e diretórios, incluindo arquivos ocultos e informações detalhadas.          |
