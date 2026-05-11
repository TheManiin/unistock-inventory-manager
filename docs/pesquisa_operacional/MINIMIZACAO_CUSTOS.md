# Minimização de Custos - UniStock

---

# Objetivo

Aplicar conceitos de Programação Linear no sistema UniStock para identificar a combinação de projetos que minimize os custos operacionais da empresa, mantendo a capacidade mínima de atendimento aos clientes.

---

# Cenário do Problema

A UniStock precisa reduzir seus custos operacionais sem comprometer totalmente a entrega de projetos para clientes.

A empresa deseja determinar quantos projetos dos tipos Básico e Premium devem ser executados durante o mês, buscando minimizar os custos totais de operação e utilização de recursos técnicos.

---

# Variáveis de Decisão

- x = quantidade de projetos Básicos
- y = quantidade de projetos Premium

---

# Informações Operacionais

## Projeto Básico

- Custo operacional unitário: R$ 3.000
- Consome 15 horas de desenvolvimento
- Consome 8 horas de suporte técnico

## Projeto Premium

- Custo operacional unitário: R$ 7.000
- Consome 40 horas de desenvolvimento
- Consome 12 horas de suporte técnico

---

# Demandas Mínimas da Empresa

A UniStock precisa manter um volume mínimo de projetos para garantir funcionamento operacional e atendimento aos clientes.

## Quantidade mínima de projetos

- Pelo menos 6 projetos Básicos
- Pelo menos 2 projetos Premium

---

# Recursos Disponíveis

## Equipe de Desenvolvimento

- 180 horas disponíveis por mês

## Equipe de Suporte Técnico

- 90 horas disponíveis por mês

---

# Modelagem Matemática

## Função Objetivo

Minimizar o custo total da empresa:

```math
Min Z = 3000x + 7000y
```

# Restrições Matemáticas

## Restrição da Equipe de Desenvolvimento

A soma das horas utilizadas pelos projetos não pode ultrapassar a capacidade da equipe de desenvolvimento.

15x + 40 y ≤180

# Restrição da Equipe de Suporte Técnico

A soma das horas de suporte consumidas pelos projetos não pode ultrapassar o limite disponível da equipe.

8x + 12 y ≤90

# Restrição de Demanda Mínima

A empresa precisa atender uma quantidade mínima de projetos contratados.

x ≥ 6

y ≥ 2

# Restrição de Não Negatividade

As variáveis de decisão não podem assumir valores negativos.

x ≥ 0

y ≥ 0

# Resultados Obtidos com Python

O modelo matemático foi implementado em Python utilizando a biblioteca PuLP no Google Colab.

Após a execução do algoritmo de Programação Linear, foi encontrada a seguinte solução ótima:

- Projetos Básicos: 6
- Projetos Premium: 2
- Custo Mínimo: R$ 32.000

O algoritmo identificou automaticamente a combinação de projetos com menor custo operacional possível, respeitando todas as restrições definidas no modelo matemático.

# Análise de Cenário (What-If)

Para simular um cenário de redução orçamentária, a disponibilidade da equipe de suporte técnico foi reduzida de 90 horas para 60 horas mensais.

O objetivo da análise foi verificar como a limitação de recursos impactaria os custos e a capacidade operacional da empresa.

## Cenário Normal

- Projetos Básicos: 6
- Projetos Premium: 2
- Custo Mínimo: R$ 32.000
  
## Cenário de Restrição Operacional

- Projetos Básicos: 6
- Projetos Premium: 1
- Custo Mínimo: R$ 25.000
