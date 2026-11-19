# 🌤️ Monitoramento de Temperatura Local via Planilha & API

Este projeto demonstra uma integração automatizada entre o **Google Sheets** e a API de previsão do tempo **Open-Meteo**. O script lê coordenadas geográficas de um formulário/planilha pública e consulta em tempo real as condições meteorológicas de cada local cadastrado.

## 🚀 Funcionalidades

- **Leitura Dinâmica:** Conecta-se diretamente a uma planilha do Google via exportação de CSV para coletar nomes de locais e coordenadas (Latitude e Longitude).
- **Integração com API:** Consulta a API gratuita e sem chave da [Open-Meteo](https://open-meteo.com/) para obter dados meteorológicos precisos de forma ágil.
- **Processamento Iterativo:** Varre cada registro da planilha de forma automatizada, exibindo as respostas formatadas.

## 🛠️ Tecnologias Utilizadas

- [Python 3](https://www.python.org/)
- [Pandas](https://pandas.pydata.org/) (Manipulação de dados da planilha)
- [Requests](https://requests.readthedocs.io/) (Requisições HTTP para a API)
- [Jupyter Notebook / Google Colab](https://colab.research.google.com/)

## 📂 Estrutura dos Dados

A planilha de entrada espera as seguintes colunas:
| Coluna | Descrição |
| :--- | :--- |
| `Carimbo de data/hora` | Data e hora em que o registro foi inserido |
| `Nome do local` | Identificação do ponto de interesse (Ex: Catedral da Sé) |
| `Latitude` | Coordenada de latitude decimal (Ex: -23.55) |
| `Longitude` | Coordenada de longitude decimal (Ex: -46.63) |

## ⚙️ Como Executar o Projeto

### Pré-requisitos
Você precisará ter o Python instalado ou rodar o ambiente no Google Colab. As bibliotecas necessárias são:
```bash
pip install pandas requests
Executando o script
Clone o repositório:
git clone https://github.com/seu-usuario/seu-repositorio.git
Abra o arquivo do notebook no VS Code, Jupyter ou faça upload no Google Colab.
Execute as células em ordem para ler os dados da planilha e ver as saídas das requisições em tempo real.

Desenvolvido com 💙 por [redacted link].
