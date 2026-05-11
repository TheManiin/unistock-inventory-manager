# Análise Crítica dos Modelos de Pesquisa Operacional - UniStock

---

# Objetivo da Análise

Este documento apresenta uma análise crítica dos modelos matemáticos desenvolvidos para a UniStock utilizando conceitos de Pesquisa Operacional e Programação Linear.

Os modelos foram aplicados com o objetivo de apoiar decisões estratégicas relacionadas à maximização de lucro e minimização de custos operacionais da empresa.

---

# Contexto do Projeto

A UniStock é uma empresa fictícia que possui recursos limitados de desenvolvimento e suporte técnico.

Diante dessas limitações, foi necessário utilizar modelagem matemática para identificar estratégias mais eficientes de operação, equilibrando:

- Rentabilidade
- Custos operacionais
- Capacidade técnica
- Atendimento mínimo aos clientes
- Utilização de recursos

Os modelos foram implementados em Python utilizando a biblioteca PuLP no Google Colab.

---

# Modelo de Maximização de Lucro

## Objetivo

O primeiro modelo teve como foco identificar a combinação de projetos que gera o maior lucro possível para a empresa.

Foram considerados dois tipos de projetos:

- Projetos Básicos
- Projetos Premium

Cada projeto possui consumo diferente de horas técnicas e lucro associado.

---

## Resultados Obtidos

O algoritmo identificou que o cenário mais lucrativo para a UniStock ocorre com:

- 5 projetos Básicos
- 2 projetos Premium
- Lucro máximo de R$ 49.000

---

## Análise do Resultado

Os resultados demonstram que os projetos Premium possuem maior capacidade de geração de lucro, porém também consomem mais recursos técnicos.

O modelo matemático conseguiu equilibrar os dois tipos de projeto para maximizar a rentabilidade sem ultrapassar os limites operacionais da empresa.

Isso evidencia como a Programação Linear pode auxiliar empresas na tomada de decisão baseada em restrições reais de negócio.

---

# Cenário What-If de Maximização

Para analisar possíveis impactos operacionais, foi criado um cenário de crise reduzindo a capacidade da equipe de desenvolvimento.

A disponibilidade foi reduzida de:

- 200 horas
para:
- 100 horas

---

## Resultado do Cenário de Crise

O algoritmo identificou o seguinte cenário ótimo:

- 5 projetos Básicos
- 0 projetos Premium
- Lucro máximo de R$ 25.000

---

## Interpretação

A redução da capacidade operacional impactou diretamente a rentabilidade da empresa.

Os projetos Premium deixaram de ser viáveis devido ao alto consumo de horas de desenvolvimento.

Nesse cenário, concentrar a operação apenas em projetos Básicos tornou-se a estratégia mais eficiente para evitar sobrecarga operacional.

---

# Modelo de Minimização de Custos

## Objetivo

O segundo modelo teve como objetivo minimizar os custos operacionais da UniStock mantendo uma capacidade mínima de atendimento aos clientes.

O modelo considerou:

- Custos de desenvolvimento
- Custos de suporte técnico
- Demandas mínimas da empresa
- Restrições operacionais

---

## Resultados Obtidos

O algoritmo encontrou a seguinte solução ótima:

- 6 projetos Básicos
- 2 projetos Premium
- Custo mínimo de R$ 32.000

---

## Análise do Resultado

O modelo demonstrou que é possível reduzir custos operacionais sem interromper completamente os serviços prestados pela empresa.

A solução encontrada mantém o funcionamento mínimo da operação respeitando todas as restrições matemáticas definidas.

Isso demonstra a eficiência da Pesquisa Operacional na otimização de recursos empresariais.

---

# Cenário What-If de Minimização

Também foi criado um cenário de restrição operacional reduzindo a capacidade da equipe de suporte técnico.

A disponibilidade foi reduzida de:

- 90 horas
para:
- 60 horas

---

## Resultado do Cenário Restritivo

O algoritmo identificou:

- 6 projetos Básicos
- 1 projeto Premium
- Custo mínimo de R$ 25.000

---

## Interpretação

Com menos recursos disponíveis, os projetos Premium passaram a ser mais limitados devido ao maior consumo de suporte técnico.

O modelo ajustou automaticamente a operação para reduzir custos e evitar sobrecarga das equipes.

Esse comportamento demonstra a capacidade dos modelos matemáticos de adaptação a cenários críticos.

---

# Benefícios da Pesquisa Operacional

A utilização de Programação Linear trouxe diversos benefícios para a análise da UniStock:

- Apoio à tomada de decisão
- Melhor utilização de recursos
- Redução de desperdícios
- Previsão de impactos operacionais
- Simulação de cenários críticos
- Otimização financeira
- Planejamento estratégico

---

# Ferramentas Utilizadas

- Python
- Google Colab
- Biblioteca PuLP
- Programação Linear
- Modelagem Matemática
- GitHub

---

# Conclusão

Os modelos desenvolvidos demonstraram como técnicas de Pesquisa Operacional podem auxiliar empresas na resolução de problemas complexos envolvendo recursos limitados.

A aplicação da Programação Linear permitiu transformar problemas reais de negócio em modelos matemáticos capazes de gerar soluções otimizadas.

Além disso, a análise de cenários What-If mostrou como mudanças operacionais impactam diretamente os resultados financeiros e estratégicos da empresa.

Os resultados obtidos reforçam a importância da análise quantitativa e da modelagem computacional no apoio à tomada de decisões empresariais.
