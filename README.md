# 💰 Pipeline de dados: extração de dados de bitcoin com ETL em PySpark e Databricks

## 💡  Sobre o projeto

Esse projeto tem o objetivo criar um pipeline completo que vai extrair os dados de APIs transforma e armazena em Delta Tables e automatizar esse processo, e cria um dashboard interativo. Além de explorar o poder do Databricks

## 🔧 Ferramentas utilizadas

- Python 3.8+
- Databricks
- API Coinbase
- API CurrencyFreaks
- requests
- pyspark
- datetime

## Arquitetura do projeto

<div align="center" >
<img width="566" height="938" alt="Image" src="https://github.com/user-attachments/assets/260ef6d6-944c-4e5a-b593-5a77609ce54c" />
</div>

## 📈 Dashboard 
Dashboard atualizado em tempo real criado no Databricks

<div align="center" >
<img width="800" height="938" alt="Image" src="https://github.com/user-attachments/assets/fc7c743b-cd8b-4e22-8e90-665ac5e719be" />
</div>

## Visualização da pipeline

<div align="center" >
<img width="800" height="1000" alt="Image" src="https://github.com/user-attachments/assets/2cc71035-5602-47d8-a39d-6025f8104b5d" />
</div>

## 🚀 Como usar

**Pré-requisitos**
- Conta no Databricks
- Chave de API da CurrencyFreaks
- Cluster Databricks ou SQL Warehouse configurado
- Catálogo Unity
- Instalação

**Clonar o repositório**
```bash
 git clone igortnt8/pipeline_api_bitcoin_databricks
 cd pipeline_api_bitcoin_databricks
```
**Importe os notebooks no Databricks:**
- Acesse seu espaço de trabalho Databricks
- Vá em Workspace → Import
- Selecione os arquivos `.py`  da pasta `PROJETO_ETL_Bitcoin/`

**Configuração do Pipeline**

**Criar fluxo de trabalho no Databricks:**
- Acesse Fluxos de Trabalho → Criar
- Adicione uma tarefa do tipo Notebook
- Selecione o Notebook `Pipeline_api_biticoin_auto.ipynb`

**Configurar Parâmetros (Valor-Chave):**

Na seção Parâmetros da tarefa
Estado:
Chave: `chave_api`
Valor: `sua_chave_api_aqui`

**Aglomerado:**

- Selecione um cluster existente ou crie um novo

**Pipeline do Executor:**

- Clique em Executar agora para manual de execução
- Ou configure um agendamento para execução automática
