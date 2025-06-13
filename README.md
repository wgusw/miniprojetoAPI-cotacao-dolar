# 📊 Análise da Cotação do Dólar via API Pública (AwesomeAPI)

Este projeto demonstra como consumir uma API pública para coletar dados da cotação do dólar (USD/BRL), tratar os dados com Python e visualizar os principais indicadores econômicos usando gráficos.

---

## 📌 Objetivo

- Coletar cotações do dólar dos últimos 10 dias usando a [AwesomeAPI](https://docs.awesomeapi.com.br/api-de-moedas).
- Tratar e formatar os dados com `pandas`.
- Visualizar métricas como: **compra (bid)**, **venda (ask)**, **alta (high)**, **baixa (low)** e **variação percentual (pctChange)**.
- Exportar os dados em `.csv` para uso posterior em Excel, Power BI ou banco de dados.

---

## 🚀 Tecnologias e Bibliotecas Utilizadas

- Python 3
- [requests](https://pypi.org/project/requests/) – para fazer a requisição HTTP
- [pandas](https://pandas.pydata.org/) – para tratamento e estruturação dos dados
- [matplotlib](https://matplotlib.org/) – para criação de gráficos
- Google Colab (ambiente de desenvolvimento)

---

## 🔗 Fonte dos Dados

- **API:** [AwesomeAPI - Moedas](https://docs.awesomeapi.com.br/api-de-moedas)
- **Endpoint utilizado:**  
  `https://economia.awesomeapi.com.br/json/daily/USD-BRL/10`

---

## 📊 Métricas Analisadas

| Métrica       | Descrição                                                                 |
|---------------|---------------------------------------------------------------------------|
| `bid`         | Cotação de compra (quanto você paga para comprar 1 USD)                  |
| `ask`         | Cotação de venda (quanto você recebe ao vender 1 USD)                   |
| `high`        | Maior valor do dólar no dia                                              |
| `low`         | Menor valor do dólar no dia                                              |
| `pctChange`   | Variação percentual em relação ao dia anterior                           |
| `timestamp`   | Data/hora da cotação (convertida de UNIX para formato legível)           |

---

## 📈 Visualização Gráfica

O projeto gera um gráfico com as linhas representando cada métrica acima. A linha de variação percentual foi incluída com estilo tracejado para facilitar a leitura da tendência de valorização ou desvalorização do dólar.

![Gráfico de Cotação do Dólar] ![image](https://github.com/user-attachments/assets/b782c613-b122-4b54-ad2f-fd7ea7ab5448)

![image](https://github.com/user-attachments/assets/e7bedf8f-c516-47f6-b536-63a14d603ab5)

---

## 📤 Exportação dos Dados

Os dados tratados são salvos em um arquivo `.csv` com a seguinte linha de código:

