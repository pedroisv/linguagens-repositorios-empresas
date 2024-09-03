# Linguagens de Programação em Empresas

Este repositório contém dados sobre as linguagens de programação usadas por algumas empresas de tecnologia em seus repositorios publicos no git hub.

## Descrição dos CSVs

O repositório é composto por quatro arquivos CSV:

* **linguagens_amzn.csv:** Contém informações sobre as linguagens de programação usadas pela Amazon.
* **linguagens_apple.csv:** Contém informações sobre as linguagens de programação usadas pela Apple.
* **linguagens_netflix.csv:** Contém informações sobre as linguagens de programação usadas pela Netflix.
* **linguagens_spotify.csv:** Contém informações sobre as linguagens de programação usadas pelo Spotify.



# Repositório de Dados de Repositórios do GitHub (ARQUIVOS .PY)
Este repositório contém os arquivos de código Python utilizados para coletar dados sobre as linguagens de programação mais utilizadas em repositórios de empresas no GitHub.

## Estrutura
**dados_repos.py:** Este arquivo contém a classe DadosRepositorios, responsável por:
* Obter informações sobre os repositórios de um usuário do GitHub.
* Criar um DataFrame Pandas com as linguagens de programação mais utilizadas nos repositórios.

**instanciando.py:** Este arquivo contém o código para instanciar a classe DadosRepositorios e coletar dados para diferentes empresas.

**manipula_dados.py:** Este arquivo contém funções para manipular os dados coletados, como:
* Limpar e organizar os dados.
* Salvar os dados em arquivos CSV.
