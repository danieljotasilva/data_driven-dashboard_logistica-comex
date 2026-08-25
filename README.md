# 📊 Data Driven Dashboard - Logística COMEX

Dashboard desenvolvido em **Power BI** para análise e acompanhamento de indicadores relacionados a operações de **Logística e Comércio Exterior (COMEX)**.

O projeto utiliza dados históricos de importação para transformar informações operacionais em uma visão analítica, permitindo acompanhar prazos, volumes, modalidades de transporte, origens, destinos e exceções ao longo das operações logísticas.

---

## 🗂️ Sumário

* [Sobre o projeto](#-sobre-o-projeto)
* [Objetivos](#-objetivos)
* [Funcionalidades](#-funcionalidades)
* [Prévia](#-prévia)
* [Tecnologias utilizadas](#-tecnologias-utilizadas)
* [Base de dados](#-base-de-dados)
* [Estrutura do projeto](#-estrutura-do-projeto)
* [Como utilizar](#-como-utilizar)
* [Autor](#-autor)
* [Licença](#-licença)

---

## 📌 Sobre o projeto

Este projeto apresenta um **dashboard analítico de operações de importação**, desenvolvido com Power BI a partir de uma base histórica de movimentações logísticas.

A proposta é transformar dados operacionais em informações que facilitem a análise de desempenho logístico e a identificação de possíveis desvios em relação aos prazos contratados.

Entre as informações disponíveis estão:

* Tipo de operação;
* Modal de transporte;
* Incoterm;
* País de origem;
* Local de destino;
* Operador logístico;
* Peso e volume das cargas;
* Data de coleta;
* Data de entrega;
* Prazo realizado;
* Prazo contratado;
* Código de exceção.

O projeto também busca demonstrar a aplicação de conceitos de **Business Intelligence, análise de dados, modelagem e visualização de informações** em um contexto de negócio.

---

## 🎯 Objetivos

O dashboard foi desenvolvido com os seguintes objetivos:

* Consolidar informações relacionadas às operações de importação;
* Facilitar o acompanhamento do desempenho logístico;
* Comparar o prazo realizado com o prazo contratado;
* Identificar operações que apresentaram desvios de prazo;
* Analisar a distribuição das operações por modal, origem e destino;
* Permitir uma exploração mais dinâmica dos dados por meio de filtros e visualizações;
* Transformar dados operacionais em informações úteis para análise e tomada de decisão.

---

## ✨ Funcionalidades

O dashboard permite explorar os dados de logística por diferentes perspectivas, incluindo:

* **Indicadores operacionais** para acompanhamento das operações;
* **Análise de prazos**, comparando o prazo realizado com o prazo contratado;
* **Análise de desempenho logístico**;
* **Segmentação por modal de transporte**;
* **Análise por país de origem**;
* **Análise por destino**;
* **Análise por operador logístico**;
* **Análise de peso e volume das cargas**;
* **Identificação de exceções nas operações**;
* **Filtros interativos** para exploração dos dados.

A utilização dos filtros permite navegar pelos dados de forma exploratória e analisar diferentes recortes da operação logística.

---

## 🖼️ Prévia

![Dashboard de Logística COMEX](assets/dash-logistica-dd.gif)

🔗 **[Acesse o dashboard interativo aqui](https://app.powerbi.com/view?r=eyJrIjoiZTBhNmFkMWEtNzgyYi00OWZjLWI2YjktZmE0Njk2YTgxY2YxIiwidCI6ImI3NTlhNjUzLWE3ZDItNDFiNS05OGNmLTVlN2NhZDIzM2EyMCJ9&embedImagePlaceholder=true)**

> Explore o dashboard com filtros, drill-down e todas as visualizações completas.

---

## 🛠️ Tecnologias utilizadas

| Tecnologia                                 | Função                                                           |
| ------------------------------------------ | ---------------------------------------------------------------- |
| [Power BI](https://powerbi.microsoft.com/) | Desenvolvimento do dashboard, modelagem e visualização dos dados |
| DAX                                        | Criação de medidas e cálculos analíticos                         |
| Power Query                                | Tratamento, transformação e preparação dos dados                 |
| Excel                                      | Fonte auxiliar para informações de apoio ao modelo               |
| CSV                                        | Armazenamento dos dados históricos de importação                 |
| PDF                                        | Fonte documental utilizada no conjunto de dados                  |

---

## 🧾 Base de dados

O principal conjunto de dados utilizado pelo dashboard está disponível em:

`data/Historico_Importacao.csv`

A base contém registros históricos de operações de importação e possui informações relacionadas a transporte, origem, destino, carga, prazos e exceções.

### Principais campos

| Campo                      | Descrição                               |
| -------------------------- | --------------------------------------- |
| `Operação`                 | Tipo da operação                        |
| `Tipo`                     | Modal/tipo de transporte                |
| `No. Invoice`              | Identificação da invoice                |
| `Incoterm`                 | Condição comercial da operação          |
| `Origem`                   | País de origem da carga                 |
| `ID País Destino`          | Identificação do país de destino        |
| `Local Destino`            | Local de destino                        |
| `ID Operador Logístico`    | Identificação do operador logístico     |
| `Doc. Embarque (AWB / BL)` | Documento de embarque                   |
| `Peso (kg)`                | Peso da carga em quilogramas            |
| `Volume (cbm)`             | Volume da carga em metros cúbicos       |
| `Tipo de serviço`          | Tipo de serviço contratado              |
| `Data da Coleta`           | Data de coleta da carga                 |
| `Data da Entrega`          | Data de entrega da carga                |
| `Prazo Realizado`          | Prazo efetivamente realizado            |
| `Prazo Contratado`         | Prazo contratado para a operação        |
| `Cód. Exceção`             | Código associado a uma eventual exceção |

Além da base principal, o projeto possui arquivos auxiliares relacionados a **cadastros de COMEX** e **bandeiras de países**.

> **Observação:** os dados disponibilizados neste repositório são destinados à demonstração do projeto e à exploração das técnicas de análise e visualização utilizadas no dashboard.

---

## 📁 Estrutura do projeto

```text
data_driven-dashboard_logistica-comex/
│
├── assets/
│   ├── dash-logistica-dd.gif    # Prévia animada do dashboard
│   ├── home.png                # Asset visual do projeto
│   └── home.svg                # Asset visual do projeto
│
├── data/
│   ├── Bandeiras Países.xlsx   # Dados auxiliares de países
│   ├── Cadastros Comex.pdf     # Informações cadastrais de COMEX
│   └── Historico_Importacao.csv # Histórico das operações
│
├── Dashboard Logística.pbix    # Arquivo principal do Power BI
├── .gitignore
└── README.md
```

---

## 🚀 Como utilizar

### Pré-requisitos

Para explorar ou editar o projeto localmente, é necessário ter:

* **Power BI Desktop** instalado;
* Acesso aos arquivos disponíveis no repositório;
* Os arquivos de dados mantidos em seus respectivos diretórios.

### Passo a passo

1. Clone o repositório:

```bash
git clone https://github.com/danieljotasilva/data_driven-dashboard_logistica-comex.git
```

2. Acesse a pasta do projeto:

```bash
cd data_driven-dashboard_logistica-comex
```

3. Abra o arquivo:

```text
Dashboard Logística.pbix
```

4. No **Power BI Desktop**, atualize as fontes de dados caso necessário.

5. Explore o dashboard utilizando os filtros e visualizações disponíveis.

> O arquivo `.pbix` contém o modelo e as visualizações desenvolvidas para o projeto.

---

## 📚 Conceitos aplicados

Este projeto reúne conceitos relacionados a:

* **Business Intelligence (BI)**
* **Análise de Dados**
* **Data Visualization**
* **Data Modeling**
* **ETL / ELT**
* **Power Query**
* **DAX**
* **Indicadores de desempenho (KPIs)**
* **Análise de operações logísticas**
* **Comércio Exterior (COMEX)**

---

## 👤 Autor

Desenvolvido por **Daniel João da Silva**.

* GitHub: [@danieljotasilva](https://github.com/danieljotasilva)
* Repositório: [data_driven-dashboard_logistica-comex](https://github.com/danieljotasilva/data_driven-dashboard_logistica-comex)

---

## 📄 Licença

Este projeto não possui uma licença definida no repositório.

Caso o projeto seja disponibilizado para reutilização ou distribuição, recomenda-se adicionar um arquivo `LICENSE` especificando os termos de uso.
