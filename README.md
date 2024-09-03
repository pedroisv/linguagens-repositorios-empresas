# Linguagens de Programação em Empresas

Este repositório contém dados sobre as linguagens de programação usadas por algumas empresas de tecnologia em seus repositorios publicos no git hub.

## Descrição dos CSVs

O repositório é composto por quatro arquivos CSV:

* **linguagens_amzn.csv:** Contém informações sobre as linguagens de programação usadas pela Amazon.
* **linguagens_apple.csv:** Contém informações sobre as linguagens de programação usadas pela Apple.
* **linguagens_netflix.csv:** Contém informações sobre as linguagens de programação usadas pela Netflix.
* **linguagens_spotify.csv:** Contém informações sobre as linguagens de programação usadas pelo Spotify.



#Repositório de Dados de Repositórios do GitHub (ARQUIVOS .PY)
Este repositório contém os arquivos de código Python utilizados para coletar dados sobre as linguagens de programação mais utilizadas em repositórios de empresas no GitHub.

##Estrutura
dados_repos.py: Este arquivo contém a classe DadosRepositorios, responsável por:

Obter informações sobre os repositórios de um usuário do GitHub.

Criar um DataFrame Pandas com as linguagens de programação mais utilizadas nos repositórios.


instanciando.py: Este arquivo contém o código para instanciar a classe DadosRepositorios e coletar dados para diferentes empresas.

manipula_dados.py: Este arquivo contém funções para manipular os dados coletados, como:

Limpar e organizar os dados.

Salvar os dados em arquivos CSV.



##Instanciando.py
O arquivo instanciando.py demonstra como utilizar a classe DadosRepositorios para coletar dados de diferentes empresas. Ele instancia a classe para cada empresa, coleta os dados e salva os resultados em arquivos CSV.
'''
from dados_repos import DadosRepositorios

amazon_rep = DadosRepositorios('amzn')
ling_mais_usadas_amzn = amazon_rep.cria_df_linguagens()

netflix_rep = DadosRepositorios('netflix')
ling_mais_usadas_netflix = netflix_rep.cria_df_linguagens()

spotify_rep = DadosRepositorios('spotify')
ling_mais_usadas_spotify = netflix_rep.cria_df_linguagens()

apple_rep = DadosRepositorios('apple')
ling_mais_usadas_apple = netflix_rep.cria_df_linguagens()

# Salvando os dados
ling_mais_usadas_amzn.to_csv('dados/linguagens_amzn.csv')
ling_mais_usadas_netflix.to_csv('dados/linguagens_netflix.csv')
ling_mais_usadas_spotify.to_csv('dados/linguagens_spotify.csv')
ling_mais_usadas_apple.to_csv('dados/linguagens_apple.csv')
'''                    
                
##Como usar

*Clone este repositório.
*Substitua SEU_TOKEN_DE_ACESSO no arquivo dados_repos.py pelo seu próprio token de acesso do GitHub.
*Execute o arquivo instanciando.py para coletar os dados e salvá-los em arquivos CSV.

##Observações

Os dados foram coletados em uma data específica e podem estar desatualizados.
As informações sobre as linguagens de programação foram obtidas através da API do GitHub e podem não refletir a realidade completa dos repositórios das empresas.
