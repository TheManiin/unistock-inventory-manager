# Maximização de Lucro - UniStock

---

# Objetivo

Aplicar conceitos de Programação Linear no sistema UniStock para identificar a combinação ideal de projetos que maximize o lucro da empresa, considerando limitações operacionais de desenvolvimento e suporte técnico.

---

# Cenário do Problema

A UniStock possui uma equipe limitada de desenvolvimento e suporte técnico responsável pela execução de projetos de clientes.

A empresa precisa decidir quantos projetos dos tipos Básico e Premium podem ser aceitos durante o mês sem ultrapassar os recursos disponíveis, buscando maximizar o lucro total da operação.

---

# Variáveis de Decisão

- x = quantidade de projetos Básicos
- y = quantidade de projetos Premium

---

# Informações Operacionais

## Projeto Básico

- Lucro unitário: R$ 5.000
- Consome 20 horas de desenvolvimento
- Consome 10 horas de suporte técnico

## Projeto Premium

- Lucro unitário: R$ 12.000
- Consome 50 horas de desenvolvimento
- Consome 15 horas de suporte técnico

---

# Recursos Disponíveis

## Equipe de Desenvolvimento

- 200 horas disponíveis por mês

## Equipe de Suporte Técnico

- 80 horas disponíveis por mês

---

# Modelagem Matemática

## Função Objetivo

Maximizar o lucro total da empresa:

```math
Max Z = 5000x + 12000y
```

# Restrições Matemáticas
## Restrição da Equipe de Desenvolvimento

A soma das horas utilizadas pelos projetos não pode ultrapassar a capacidade da equipe de desenvolvimento.
20x + 50y ≤ 200

# Restrição da Equipe de Suporte Técnico
A soma das horas de suporte consumidas pelos projetos não pode ultrapassar o limite disponível da equipe.
10x + 15y ≤ 80
