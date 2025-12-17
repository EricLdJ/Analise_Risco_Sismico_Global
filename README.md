# Pipeline de ETL para análise de dados sísmicos integrando Python, MySQL e Power BI

Analisar tendências de terremotos e tsunamis ao redor do mundo. | Demonstrar a automação do tratamento de dados com Pandas e persistência em banco de dados relacional.

## Descrição

O projeto de análise de risco sísmico global é um trabalho que foi feito entre 01/12/2025 – Atualmente. 

Seu objetivo é evidenciar com base em dados reais disponibilizados no site Kaggle, os riscos sísmicos em diversos países, fazendo comparações entre magnitudes e frequências similares até de extrema diferença, tudo em um ciclo completo de ETL, além disso, por motivos de perpetuação do código ele é integrado em um banco de dados no mySQL e para melhor visualização foi criado um dashboard interativo com o Power BI. 

Tudo nesse projeto foi feito com minha base de conhecimento e estudos a fundo sobre as bibliotecas utilizadas. 
##Arquitetura do Projeto
O fluxo de dados segue a seguinte esteira:
1.  **Extract:** Leitura de dados brutos (CSV/Kaggle).
2.  **Transform:** Limpeza, filtragem, categorização de risco e Geocodificação Reversa (Python/Pandas).
3.  **Load:** Carga automatizada no banco de dados MySQL via SQLAlchemy.
4.  **Viz:** Conexão do Power BI com o MySQL para geração de Dashboards.
## Primeiros passos
### Dependências 
* Python
* IDE de sua escolha - Utilizada: VScode
* Jupyter notebook
* MySQL
* Power BI
* Git
### Instalação
Além do que está nas dependências, é necessário verificar o "requirements.txt" e instalar as bibliotecas com suas devidas versões para o funcionamento do código.

Instale as referências com "pip install -r requirements.txt"
### Execução

Instale e abra o bash do Git na pasta que desejar, execute o comando git clone. 

Ou se desejar, baixe o arquivo no github e abra o arquivo na sua IDE. 

Configure as Variáveis de Ambiente: Por segurança, as credenciais do banco não estão no código.

Crie um arquivo chamado .env na raiz do projeto.

Adicione suas credenciais do MySQL no seguinte formato:

**DB_USER=root**

**DB_SENHA=sua_senha_aqui**

Prepare o Banco de Dados: Abra seu terminal MySQL ou Workbench e crie o banco vazio:

**CREATE DATABASE projeto_terremotos;**

**Execute o Pipeline**: Execute célula por célula para compreender o funcionamento do código.
## Autor
Eric Lima de Jesus 

email: ericlj333@gmail.com

LinkedIn: https://www.linkedin.com/in/eric-l-jesus/