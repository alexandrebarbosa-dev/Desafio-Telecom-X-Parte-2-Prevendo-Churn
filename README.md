# Desafio-Telecom-X-Parte-2-Prevendo-Churn

# 📊 Previsão de Churn: Projeto Telecom X
(gerado por IA a partir de informações fornecidas)

## 📝 Sobre o Projeto

Este projeto foi desenvolvido para a **Telecom X** com o objetivo de reduzir a taxa de evasão de clientes (Churn). Utilizando técnicas de Machine Learning, criamos um sistema capaz de identificar clientes com alta probabilidade de cancelamento, permitindo ações preventivas de retenção.

## 🧠 Modelagem e Metodologia

O projeto foi dividido em etapas rigorosas de Ciência de Dados:

1. **Pré-processamento:** Tratamento de dados, *One-Hot Encoding* e Normalização.
2. **Engenharia de Features:** Seleção das variáveis mais relevantes para o negócio.
3. **Modelagem:** - **Regressão Logística:** Utilizada para entender a direção do impacto de cada variável.
* **Random Forest:** Modelo de alta precisão regularizado para evitar *overfitting*.

4. **Avaliação:** Alcançamos uma **acurácia de 80%** na base de teste, garantindo previsões confiáveis.

## 📈 Principais Insights (Fatores de Evasão)

Através da análise de importância de variáveis, identificamos os pilares da evasão na empresa:

* **Contratos Mensais (Month-to-month):** O maior fator de risco identificado.
* **Fibra Óptica:** Segmento com churn acima da média, demandando revisão de oferta.
* **Tempo de Contrato (Tenure):** Clientes nos primeiros 6 meses são os mais vulneráveis.

## 🛠️ Tecnologias Utilizadas

* **Pandas & Numpy:** Manipulação e tratamento de dados.
* **Scikit-Learn:** Construção do pipeline de Machine Learning.
* **Matplotlib & Seaborn:** Visualização de dados.
* **Yellowbrick:** Visualização avançada de performance de modelos e importância de features.

---

## 🎓 Aprendizados e Competências Desenvolvidas

Este desafio foi um divisor de águas na compreensão do ciclo completo de um projeto de Ciência de Dados aplicado ao mundo real. Os principais pilares de aprendizado foram:

### 1. Engenharia de Dados e Transformação (Pipeline)

Aprendi a construir um fluxo de dados robusto utilizando o `ColumnTransformer` e `OneHotEncoder`.

* **Decisão Crítica:** Implementei a técnica de `drop='first'` para evitar a armadilha da multicolinearidade (Dummy Variable Trap), garantindo a estabilidade matemática da Regressão Logística.
* **Limpeza de Metadados:** Desenvolvi funções para limpar prefixos técnicos gerados automaticamente (`onehotencoder__`), tornando os resultados interpretáveis para áreas de negócio.

### 2. Interpretabilidade de Modelos (XAI)

Mais do que prever, aprendi a explicar o "porquê" das previsões.

* **Regressão Logística:** Entendi como os coeficientes indicam a direção do risco (âncoras de retenção vs. gatilhos de evasão).
* **Random Forest:** Aprendi a extrair a importância relativa das variáveis para identificar os "órgãos vitais" que definem o comportamento do cliente.
* **Visualização Avançada:** Utilizei a biblioteca **Yellowbrick** para criar gráficos profissionais que traduzem pesos estatísticos em insights visuais.

### 3. Regularização e Generalização

Enfrentei o desafio do *overfitting* no modelo de Random Forest.

* Aprendi a ajustar hiperparâmetros (como profundidade da árvore e número de estimadores) para garantir que o modelo performe bem em dados novos, e não apenas nos dados que ele já conhece. Isso resultou em uma acurácia consistente de **80% no teste**.

### 4. Visão Analítica de Negócio

Desenvolvi a habilidade de traduzir métricas técnicas (como acurácia e pesos) em estratégias de retenção reais:

* Identificação do contrato **mensal** como principal gargalo.
* Análise de anomalias no churn de **Fibra Óptica**.
* Foco em **LTV (Lifetime Value)** através da análise da variável *Tenure*.

## 🚀 Como Executar o Projeto

1. Clone o repositório: `git clone https://github.com/seu-usuario/telecom-x-churn.git`
2. Instale as dependências: `pip install -r requirements.txt`
3. Abra o notebook: `Desafio_Telecom_X_–_Parte_2_Prevendo_Churn.ipynb`

Se tiver alguma dúvida ou sugestão, sinta-se à vontade para entrar em contato!
