<img src="img/imgecommerce.png" width="100%">

## 1. Problema de Negócio
Uma empresa de e-commerce busca entender como os descontos impactam a receita e o comportamento de compra dos clientes, a fim de otimizar estratégias de precificação e maximizar o faturamento.

O objetivo deste projeto é analisar a relação entre descontos, volume de vendas e receita, identificando padrões por categoria de produto e gerando insights para apoiar decisões mais eficientes na aplicação de descontos.

---
### Dicionário de Dados
| Atributo        | Descrição |
|----------------|----------|
| user_id        | Identificador único de cada usuário |
| product_id     | Identificador único de cada produto |
| category       | Categoria do produto |
| price          | Preço original antes do desconto |
| discount       | Percentual de desconto aplicado |
| final_price    | Preço final após o desconto |
| payment_method | Método de pagamento |
| purchase_date  | Data da compra |
| day            | Dia da compra |
| month          | Mês da compra |
| year           | Ano da compra |

---
## 2. Planejamento da Solução

### 2.1 Ferramentas Utilizadas

- **Linguagem de Programação:** Python  
  - Biblioteca de manipulação de dados: Pandas  
  - Biblioteca de visualização de dados: Matplotlib e Seaborn

### 2.2 Implementação da Solução

**Coleta de Dados:**  
Os dados foram obtidos na plataforma Kaggle (“E-commerce Dataset”) e representam transações simuladas de um e-commerce. Apesar de não serem dados reais, permitem analisar padrões de compra e comportamento dos clientes.

**Descrição das Variáveis:**  
Nesta etapa, foi realizada a descrição das variáveis presentes no conjunto de dados.

**Limpeza e Preparação dos Dados:**  
Nesta etapa, os dados foram verificados quanto a valores nulos, não sendo encontradas inconsistências. A variável de data foi convertida para o formato adequado, os nomes das colunas foram padronizados e foram criadas variáveis derivadas, como mês, ano e valor de desconto, para apoiar a análise.

**Análise Exploratória dos Dados:**  
Etapa a qual foi realizada, a análise das variáveis numéricas e categóricas por meio de abordagens univariadas, bivariadas e multivariadas, com o objetivo de identificar padrões, relações e insights sobre o impacto dos descontos na receita e no comportamento de compra.

---

## 3. Top Insights

- **Descontos elevados reduzem a receita**  
  Descontos mais altos não geram aumento no faturamento, indicando perda de margem sem ganho relevante em volume de vendas.

- **Menores descontos concentram maior receita**  
  A faixa entre 0% e 10% apresenta os maiores valores de faturamento, indicando maior eficiência em preços próximos do original.

- **Descontos não aumentam o volume de compras**  
  O número de transações se mantém relativamente estável entre os níveis de desconto, mostrando que descontos agressivos não impulsionam a demanda de forma consistente.

- **Impacto varia entre categorias**  
  O efeito dos descontos não é uniforme, com algumas categorias mais sensíveis à redução de preço do que outras.

- **Limite crítico de desconto**  
  Descontos acima de 30% tendem a diminuir significativamente a receita em diferentes categorias.

- **Redução do valor médio das compras**  
  O valor médio pago pelos clientes diminui conforme o desconto aumenta, refletindo diretamente no faturamento.

- **Mudança no comportamento de pagamento**  
  O método de pagamento varia conforme o nível de desconto, indicando alterações no comportamento do consumidor.

- **Ausência de padrão temporal**  
  Não foi identificado um padrão consistente de aumento de vendas ao longo do tempo relacionado a descontos.

---

## 4. Recomendações de Negócio

A análise mostra que o impacto dos descontos varia entre categorias e que níveis elevados não aumentam proporcionalmente a receita. Com base nisso, a estratégia pode ser segmentada:

---

### Categorias com alta receita e baixo desconto
Essas categorias mantêm alto desempenho mesmo com poucos descontos, indicando baixa sensibilidade ao preço.

**Direcionamento:**  
Manter descontos baixos e priorizar margem de lucro.

---

### Categorias com alto desconto e baixa receita
Descontos elevados não estão gerando retorno em faturamento, indicando ineficiência na estratégia atual.

**Direcionamento:**  
Reduzir a intensidade dos descontos e revisar a estratégia de precificação.

---

### Limite crítico de desconto
Descontos acima de 30% impactam negativamente a receita.

**Direcionamento:**  
Evitar o uso frequente de descontos elevados, aplicando-os de forma pontual e estratégica.

---

## 5. Conclusão

Este projeto analisou como os descontos influenciam a receita e o comportamento de compra em um e-commerce, permitindo identificar padrões relevantes para a tomada de decisão.

De forma geral, os resultados mostram que o aumento dos descontos não garante melhores resultados financeiros, reforçando a importância de uma análise mais estratégica na sua aplicação.

Além disso, a análise evidenciou que o impacto dos descontos varia entre categorias, destacando a necessidade de considerar as particularidades de cada tipo de produto ao definir estratégias de precificação.

Por fim, o projeto demonstra como a análise de dados pode ser utilizada para apoiar decisões mais eficientes, transformando dados em insights que contribuem para a melhoria do desempenho do negócio.
