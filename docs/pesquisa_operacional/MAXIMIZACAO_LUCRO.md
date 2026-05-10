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
