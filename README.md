# Telecom-2-
# Projeto Telecom X – Análise de Churn

## 1. Descrição do Projeto
Este projeto tem como objetivo analisar a evasão de clientes (churn) da empresa **Telecom X** e identificar fatores que influenciam a decisão de saída dos clientes. A partir disso, foram construídos modelos preditivos para prever a probabilidade de churn e propor estratégias de retenção.

O projeto inclui:
- Limpeza e preparação do dataset;
- Transformação de variáveis categóricas em numéricas;
- Análise exploratória e visualizações;
- Criação e avaliação de modelos preditivos (Regressão Logística e Random Forest);
- Identificação das variáveis mais relevantes para churn;
- Estratégias de retenção baseadas nos insights obtidos.

---

## 2. Dataset
O dataset utilizado contém informações de clientes da Telecom X, incluindo:
- Tempo de contrato (`tenure`);
- Tipo de contrato (`Contract`);
- Gastos mensais e totais (`MonthlyCharges`, `TotalCharges`);
- Serviços adicionais contratados (Internet, Segurança Online, etc.);
- Método de pagamento e outras informações demográficas.

> Observação: O dataset foi previamente **limpo e padronizado**, removendo colunas irrelevantes e tratando valores faltantes.

---

## 3. Pré-processamento
- Remoção de identificadores únicos (ex.: `customerID`);
- Transformação de variáveis categóricas e

## 4. Modelos Utilizados
### 4.1 Regressão Logística
- Permite interpretar a contribuição de cada variável para a probabilidade de churn.
- Normalização aplicada para melhorar convergência e desempenho.

### 4.2 Random Forest
- Captura relações não lineares e interações entre variáveis.
- Não requer normalização das variáveis.
- Permite análise da importância relativa das features.

---

## 5. Avaliação dos Modelos
Métricas utilizadas:
- **Acurácia**
- **Precisão**
- **Recall**
- **F1-score**
- **Matriz de Confusão**

> Observação: O Random Forest apresentou melhor desempenho geral, enquanto a Regressão Logística fornece insights interpretáveis sobre a contribuição das variáveis.

---

## 6. Variáveis Mais Relevantes
- **Tempo de contrato (`tenure`)**: clientes novos têm maior risco de churn.
- **Tipo de contrato (`Contract_Month-to-month`)**: contratos mensais apresentam maior evasão.
- **Gastos (`MonthlyCharges` e `TotalCharges`)**: clientes com gastos extremos tendem a evadir.
- **Serviços adicionais (`OnlineSecurity`, `InternetService_Fiber`)**: ausência de serviços ou tipo de internet influencia churn.

---

## 7. Estratégias de Retenção
1. Incentivar contratos de longo prazo com benefícios;
2. Programas de fidelidade e onboarding para clientes novos;
3. Oferecer upgrades de serviços adicionais;
4. Ofertas personalizadas baseadas em perfil de gastos;
5. Atendimento proativo e comunicação contínua com clientes de risco.

---

## 8. Tecnologias e Bibliotecas
- Python 3.x
- Pandas, NumPy (manipulação de dados)
- Scikit-learn (modelos preditivos)
- Seaborn, Matplotlib (visualizações)
- Jupyter Notebook / Google Colab

---

## 9. Como Executar
1. Clonar o repositório:  
```bash
git clone <URL_DO_REPOSITORIO>
