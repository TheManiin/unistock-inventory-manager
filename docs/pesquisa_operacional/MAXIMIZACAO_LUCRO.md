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

# Restrição de Não Negatividade

As variáveis de decisão não podem assumir valores negativos.

x ≥ 0

y ≥ 0

# Resultados Obtidos com Python

O modelo matemático foi implementado em Python utilizando a biblioteca PuLP no Google Colab.

Após a execução do algoritmo de Programação Linear, foi encontrada a seguinte solução ótima:

- Projetos Básicos: 5
- Projetos Premium: 2
- Lucro Máximo: R$ 49.000

O algoritmo identificou automaticamente a combinação mais eficiente de projetos sem ultrapassar os limites operacionais definidos pelas restrições matemáticas.

# Análise de Cenário (What-If)

Para simular uma situação de crise operacional, a disponibilidade da equipe de desenvolvimento foi reduzida de 200 horas para 100 horas mensais.

O objetivo da análise foi verificar como a redução de recursos impactaria o lucro e a estratégia operacional da empresa.

## Cenário Normal
- Projetos Básicos: 5
- Projetos Premium: 2
- Lucro Máximo: R$ 49.000
  
## Cenário de Crise
- Projetos Básicos: 5
- Projetos Premium: 0
- Lucro Máximo: R$ 25.000

# Análise Crítica dos Resultados

Os resultados matemáticos obtidos em Python fazem sentido para a realidade operacional da UniStock, pois demonstram claramente como as limitações de recursos influenciam diretamente a capacidade produtiva da empresa.

No cenário normal, a combinação entre projetos Básicos e Premium permite alcançar maior rentabilidade, utilizando de forma equilibrada as equipes de desenvolvimento e suporte técnico.

Entretanto, quando ocorre uma redução na disponibilidade da equipe de desenvolvimento, os projetos Premium deixam de ser viáveis devido ao alto consumo de horas técnicas. Nesse cenário, o algoritmo identificou que concentrar a operação apenas em projetos Básicos se torna a alternativa mais eficiente para evitar sobrecarga operacional e reduzir riscos.

A análise What-If ajuda a gestão da empresa a prever impactos causados por crises, atrasos ou redução de equipe, permitindo tomadas de decisão mais seguras, estratégicas e baseadas em dados reais.

# Ferramentas Utilizadas

- Python
- Google Colab
- Biblioteca PuLP
- Programação Linear
- Modelagem Matemática

# Conclusão

A aplicação de Pesquisa Operacional permitiu transformar um problema real de negócios em um modelo matemático capaz de apoiar decisões estratégicas da UniStock.

O uso de Programação Linear e algoritmos em Python demonstrou como técnicas computacionais podem auxiliar empresas na maximização de lucro, otimização de recursos e análise de cenários operacionais críticos.


# Arquivo Python

O algoritmo desenvolvido em Python utilizando a biblioteca PuLP pode ser consultado no notebook abaixo:

- [Visualizar Notebook no GitHub](./UniStock_Maximizacao.ipynb)
- [Abrir no Google Colab](https://colab.research.google.com/drive/1DZWE7oLEF7ioVLMH9r6sqcshlM5pC1gq#scrollTo=LKhx7UBgoMkx)
