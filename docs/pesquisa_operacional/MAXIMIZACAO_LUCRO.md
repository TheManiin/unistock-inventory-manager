# Maximização de Lucro - UniStock

---

# Objetivo

Aplicar Programação Linear para identificar a combinação ideal de projetos da UniStock que gera o maior lucro possível, considerando limitações operacionais da empresa.

---

# Cenário do Problema

A UniStock possui uma equipe limitada de desenvolvimento e suporte técnico.

A empresa precisa decidir quantos projetos do tipo Básico e Premium devem ser aceitos durante o mês para maximizar o lucro total sem ultrapassar os recursos disponíveis.

---

# Variáveis de Decisão

- x = quantidade de projetos Básicos
- y = quantidade de projetos Premium

---

# Informações Operacionais

## Projeto Básico

- Lucro: R$ 5.000
- Consome 20 horas de desenvolvimento
- Consome 10 horas de suporte

## Projeto Premium

- Lucro: R$ 12.000
- Consome 50 horas de desenvolvimento
- Consome 15 horas de suporte

---

# Recursos Disponíveis

## Equipe de Desenvolvimento

- 200 horas disponíveis

## Equipe de Suporte

- 80 horas disponíveis

---

# Modelagem Matemática

## Função Objetivo

Maximizar o lucro:

```math
Max Z = 5000x + 12000y
```

---

# Análise de Cenário (What-If)

Para simular um cenário de crise operacional, a restrição da equipe de desenvolvimento foi reduzida de 200 horas para 100 horas disponíveis.

## Cenário Normal

- Projetos Básicos: 5
- Projetos Premium: 2
- Lucro Máximo: R$ 49.000

## Cenário de Crise

- Projetos Básicos: 5
- Projetos Premium: 0
- Lucro Máximo: R$ 25.000

## Interpretação dos Resultados

A análise demonstrou que a redução da capacidade operacional impacta diretamente a estratégia da empresa e o lucro final obtido.

No cenário normal, a UniStock consegue equilibrar projetos básicos e premium para maximizar o retorno financeiro. Porém, quando os recursos de desenvolvimento são reduzidos pela metade, os projetos premium deixam de ser viáveis devido ao alto consumo de horas técnicas.

O algoritmo identificou automaticamente que manter apenas projetos básicos se torna a decisão mais eficiente para evitar sobrecarga operacional.

Essa análise ajuda a gestão da empresa a prever impactos de crises, atrasos ou redução de equipe, permitindo decisões mais seguras e estratégicas.
