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


## Impactos Operacionais

A exploração dessa vulnerabilidade poderia causar:

- acesso indevido a contas administrativas
- vazamento de dados de clientes
- alteração de registros de estoque
- exclusão de pedidos e produtos
- indisponibilidade parcial do sistema
- prejuízos financeiros
- violação da LGPD

Como o UniStock centraliza autenticação, estoque e pedidos, o impacto operacional dessa falha seria extremamente crítico para a plataforma.

## Técnicas de Mitigação Implementadas

Para reduzir os riscos de SQL Injection, o UniStock adotou as seguintes medidas:

### ORM (Object Relational Mapping)

O backend utiliza ORM para impedir concatenação manual de comandos SQL, evitando interpretação maliciosa de entradas do usuário.

### Sanitização de Entradas

Todos os dados enviados por formulários passam por validação e sanitização antes do processamento.

### RBAC

O controle de permissões restringe acessos administrativos apenas a usuários autorizados.

### HTTPS Obrigatório

Toda comunicação entre cliente e servidor ocorre de forma criptografada.

### Logs de Auditoria

Ações críticas são registradas para investigação de possíveis incidentes.

## Conclusão

A análise crítica demonstrou que o SQL Injection representa uma das ameaças mais graves ao UniStock devido ao potencial comprometimento do banco de dados e exposição de informações sensíveis.

As técnicas de mitigação implementadas, combinadas com políticas de IAM e conformidade com a LGPD, reduzem significativamente os riscos operacionais e fortalecem a segurança da plataforma.
