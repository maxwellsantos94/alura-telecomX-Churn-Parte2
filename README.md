# 📊 Previsão de Evasão de Clientes (Churn Prediction)

Este projeto realiza uma análise completa de dados de clientes do setor de telecomunicações para **identificar quem está mais propenso a cancelar o serviço (churn)** e **quais fatores influenciam esse comportamento**.  

Além disso, são geradas **recomendações estratégicas** para reduzir a evasão e melhorar a retenção de clientes.

---

## **Etapas do Projeto**

1. **Preparação dos dados**
   - Remoção de colunas sem valor preditivo (IDs, chaves únicas)
   - Tratamento de valores ausentes e inconsistências
   - Codificação de variáveis categóricas (One-Hot Encoding)
   - Análise do balanceamento das classes (churn vs. não churn)
   - Aplicação de técnicas de balanceamento (SMOTE / undersampling / oversampling)
   - Normalização ou padronização de variáveis quando necessário

2. **Análise exploratória**
   - Cálculo da proporção de clientes evadidos
   - Matriz de correlação para variáveis numéricas
   - Visualização de relações importantes (tenure × churn, gasto mensal × churn)

3. **Modelagem preditiva**
   - Divisão do conjunto de dados em treino e teste (70/30)
   - Treinamento de múltiplos modelos:
     - Regressão Logística (requer normalização)
     - KNN (requer normalização)
     - Random Forest (não requer normalização)
   - Avaliação com métricas:
     - Acurácia
     - Precisão
     - Recall
     - F1-score
     - Matriz de confusão

4. **Interpretação dos resultados**
   - Identificação das variáveis mais relevantes:
     - Importância das features (Random Forest)
     - Coeficientes (Regressão Logística)
   - Identificação de clientes com maior risco de evasão (probabilidade de churn mais alta)
   - Perfil dos clientes que precisam de maior atenção

5. **Conclusões estratégicas**
   - Principais fatores que levam à evasão
   - Recomendações para retenção de clientes:
     - Ajustes em planos e contratos
     - Ofertas personalizadas
     - Melhorias no onboarding para clientes novos

---

## **Principais Perguntas Respondidas**
- **Quem são os clientes com maior risco de evasão?**  
  → Listagem dos clientes com maior probabilidade de churn com base no modelo.  

- **Quais variáveis mais influenciam esse comportamento?**  
  → Ranking das variáveis mais relevantes para a decisão do modelo.  

- **Que tipo de perfil a empresa precisa manter mais próximo?**  
  → Identificação de padrões (ex.: clientes com contrato mensal, baixo tempo de permanência, alto gasto mensal).  

---

## **Tecnologias Utilizadas**
- Python 3.x
- Pandas, NumPy
- Matplotlib
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Jupyter Notebook

---

## **Como Executar**
1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   cd seu-repositorio
