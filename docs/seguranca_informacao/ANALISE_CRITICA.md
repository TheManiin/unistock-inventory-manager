# Análise Crítica de Segurança - UniStock

## Objetivo

Analisar criticamente a vulnerabilidade mais crítica identificada na Matriz GUT do sistema UniStock, explicando como ela poderia ser explorada no contexto da plataforma e quais medidas técnicas foram adotadas para mitigação do risco.

---

# Vulnerabilidade Crítica Identificada

## SQL Injection

A vulnerabilidade com maior prioridade identificada na Matriz GUT foi o SQL Injection, recebendo nota máxima devido ao alto impacto operacional, urgência de correção e potencial crescimento do problema caso não tratado.

No contexto do UniStock, um invasor poderia explorar campos de login, busca de produtos ou formulários administrativos para inserir comandos SQL maliciosos diretamente nas consultas do banco de dados.

Exemplo de ataque:

```sql
' OR 1=1 --
