# 🚀 PROJETO 1: Análise de Desempenho Multifatorial de Vendas por Área

## Sumário Executivo
Este projeto de Análise de Dados focou na avaliação do desempenho de fechamento de contratos em cinco áreas da empresa, correlacionando as métricas de **Eficiência por Funcionário (Produtividade)**, **Talento Individual (Top Performers)** e **Qualidade Financeira (Ticket Médio)**.

A análise revelou que o **tamanho da equipe não é o único fator determinante** para o sucesso, destacando a Área Comercial como o ponto mais crítico e a Área Operações como um *benchmark* de alta performance.

## 🎯 Objetivos da Análise

1.  **Avaliar a Eficiência (Volume):** Calcular a Taxa de Produtividade (Contratos Fechados por Funcionário) de cada área.
2.  **Identificar Talentos:** Criar um ranking dos 5 colaboradores com mais contratos fechados (Top Performers).
3.  **Avaliar Qualidade (Valor):** Calcular o Ticket Médio Mensal por Área e compará-lo com o Ticket Médio geral da empresa (R$ 2.502,56).
4.  **Gerar Insights Acionáveis:** Propor uma estratégia para otimizar o desempenho da área Comercial, que se mostrou a de menor performance.

## ⚙️ Metodologia Técnica

* **Linguagem:** Python
* **Bibliotecas:** Pandas (para manipulação, agregação e junção de dados), Matplotlib (para visualização de dados).
* **Técnicas:**
    * Utilização de `pd.merge()` com `how='left'` e `how='inner'` para unir diferentes fontes de dados.
    * Agregação de dados usando `pd.groupby()` para calcular médias (`.mean()`) e contagens (`.count()`).
    * Criação de KPIs personalizados, como **Taxa de Produtividade** e **Ticket Médio por Área**.

## 📈 Principais Insights e Descobertas

| Área | Taxa de Produtividade | Ticket Médio Mensal | Top 5 Vendedores | Conclusão |
| :--- | :---: | :---: | :---: | :--- |
| **Administrativo** | **242.31%** (Alta) | **R$ 2.512,14** | 2 | Lidera em eficiência e qualidade (valor). |
| **Operações** | 209.0% (Média/Alta) | R$ 2.477,81 | 1 (Vendedor Líder) | Alto volume e melhor *benchmark* de talento. |
| Financeiro | 233.0% (Alta) | R$ 2.392,50 | 1 | Alta eficiência por funcionário. |
| Logística | 190.0% (Média) | R$ 2.291,62 | 1 | |
| **Comercial** | 169.0% (Baixa) | R$ 2.466,82 | 0 | **Ponto Crítico:** Baixa em todas as métricas. |

### 🔑 Recomendação de Ação
A área **Comercial** deve ser o foco da otimização. Recomenda-se a implementação de um programa de **Benchmarking Interno** que utilize os métodos e *pipelines* de vendas do Top Performer da **Operações** (ID 47) e as estratégias de negociação da área **Administrativo** para elevar a produtividade e o valor dos contratos do setor.
