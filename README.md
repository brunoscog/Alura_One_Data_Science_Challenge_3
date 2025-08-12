<p align="center">
  <img src="https://raw.githubusercontent.com/brunoscog/Alura_One_Data_Science_Challenge_1/refs/heads/main/brunoscog-cover.jpg" alt="Imagem de capa do projeto">
</p>

<h1 align="center"> ONE | Alura - Challenge 3: Prevendo Evasão de Clientes (Churn) </h1>

<p align="center">
  <img src="http://img.shields.io/static/v1?label=STATUS&message=PROJETO%20CONCLUÍDO&color=GREEN&style=for-the-badge"/>
  <br>
  <img src="https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458.svg?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" />
  <img src="https://img.shields.io/badge/imbalanced--learn-753BBD?style=for-the-badge&logo=imbalanced-learn&logoColor=white" />
  <img src="https://img.shields.io/badge/Matplotlib-20232A?style=for-the-badge&logo=matplotlib&logoColor=white" />
  <img src="https://img.shields.io/badge/seaborn-20232A?style=for-the-badge&logo=seaborn&logoColor=white" />
</p>

# 📌 Índice

* [Descrição do Projeto](#descrição-do-projeto)
* [Objetivos do Desafio](#objetivos-do-desafio)
* [Tecnologias Utilizadas](#tecnologias-utilizadas)
* [Como Executar](#como-executar)
* [Estrutura do Projeto](#estrutura-do-projeto)
* [Resultado da Análise](#resultado-da-análise)
* [Acesse o projeto completo](#acesse-o-projeto-completo)
* [Desenvolvido por](#desenvolvido-por)

---

## 🧾 Descrição do Projeto

Este projeto aborda o desafio de **prever a evasão de clientes (Churn)** da **Telecom X**. A missão principal foi evoluir da análise exploratória para a construção de modelos preditivos robustos, capazes de identificar clientes com alta probabilidade de cancelamento de serviços. O trabalho envolveu a aplicação de um pipeline completo de Machine Learning, desde o pré-processamento avançado dos dados até a interpretação dos modelos e a geração de insights estratégicos para a retenção de clientes.

---

## 🎯 Objetivos do Desafio

* Preparar os dados para a modelagem (tratamento, encoding, balanceamento e normalização).
* Realizar análise de correlação e seleção de variáveis.
* Treinar e avaliar modelos de classificação (Regressão Logística e Random Forest).
* Avaliar o desempenho dos modelos com métricas como Acurácia, Precisão, Recall, F1-score e Matriz de Confusão.
* Interpretar os resultados, incluindo a análise da importância das variáveis do melhor modelo.
* Criar uma conclusão estratégica com os principais fatores que influenciam a evasão e propor estratégias de retenção.

---

## 💻 Tecnologias Utilizadas

* Python 3.x
* pandas
* scikit-learn
* imbalanced-learn
* matplotlib
* seaborn
* Google Colab / Jupyter Notebook

---

## ▶️ Como Executar

```bash
# Clone o repositório 
git clone [https://github.com/brunoscog/Alura_One_Data_Science_Challenge_3.git](https://github.com/brunoscog/Alura_One_Data_Science_Challenge_3.git)
cd Alura_One_Data_Science_Challenge_3

# Instale as bibliotecas necessárias para o projeto
pip install pandas scikit-learn imbalanced-learn matplotlib seaborn
```

Abra o arquivo Challenge 3 - TelecomX - Parte 2.ipynb no Jupyter Notebook ou Google Colab para executar o código e replicar a análise.

## 📁 Estrutura do Projeto
```bash
├── Challenge 3 - TelecomX - Parte 2.ipynb  # Notebook principal com a análise, modelos e relatório
├── dados_tratados.csv                   # Dados limpos da Parte 1
├── dados_balanceados_padronizados.csv   # Dados finais processados para a modelagem
├── README.md                            # Documentação principal do projeto
├── .gitignore
└── requirements.txt
```

## 📊 Resultado da Análise
O modelo **Random Forest**, que apresentou o melhor desempenho na avaliação, destacou os seguintes fatores como os mais influentes na previsão de evasão:

* **Fatores de Maior Evasão (Churn)**:
    * **Gasto Mensal** (`account_Charges.Monthly`): O fator mais relevante, indicando uma alta sensibilidade ao preço.
    * **Forma de Pagamento Cheque Eletrônico** (`account_PaymentMethod_Electronic check`): Principal indicador de risco de evasão.
    * **Serviço de Fibra Óptica** (`internet_InternetService_Fiber optic`): Associado a um maior risco de churn, o que sugere possíveis problemas de qualidade ou forte concorrência no segmento.
* **Fatores de Retenção (Menor Churn)**:
    * **Tempo de Contrato** (`customer_tenure`): O segundo fator mais importante; quanto maior o tempo de serviço, menor a chance de evasão.
    * **Contratos de Dois Anos** (`account_Contract_Two year`): Atuam como um forte fator de proteção contra a evasão.
    * **Serviços de Segurança e Suporte** (`internet_OnlineSecurity`, `internet_TechSupport`): Clientes que assinam esses serviços adicionais têm menor probabilidade de cancelar.

---

## 📝 Conclusão e Recomendações Estratégicas

O projeto estabeleceu uma base sólida para a utilização de inteligência preditiva na gestão de clientes da Telecom X. O modelo Random Forest é uma ferramenta eficaz, capaz de identificar os clientes em risco de evasão. Os principais impulsionadores de evasão são o **alto custo mensal, o baixo tempo de contrato e o método de pagamento**.

Para prevenir ativamente o churn, as seguintes estratégias são recomendadas:

* **Programas de Engajamento para Clientes Novos**: Focar em clientes com `tenure` baixo, oferecendo benefícios para estender o tempo de contrato.
* **Revisão de Preços**: Criar ofertas personalizadas ou descontos para clientes com altos gastos mensais.
* **Incentivos para Pagamento Automático**: Promover a migração para métodos de pagamento automáticos, afastando o risco associado ao cheque eletrônico.
* **Monitoramento da Qualidade**: Dar atenção especial à qualidade do serviço de fibra óptica e ao suporte técnico para garantir a satisfação do cliente.

---

## 📘 Acesse o projeto completo

O notebook com toda a análise, modelos e relatório final está disponível em:

👉 [`Challenge 3 - TelecomX - Parte 2.ipynb`](./Challenge%203%20-%20TelecomX%20-%20Parte%202.ipynb)

---

## 👨‍💻 Desenvolvido por

<img src="https://media.licdn.com/dms/image/v2/D4D03AQE5oHHVZzjwIg/profile-displayphoto-shrink_200_200/profile-displayphoto-shrink_200_200/0/1727484820568?e=2147483647&v=beta&t=JuBlRoJK5c2EUbs18LthUHalzmlM4A_2Zi16PzAlwmc" width=115>
<br/>
[Bruno Farias Scognamiglio](https://www.linkedin.com/in/bruno-scognamiglio-432243a7/)
