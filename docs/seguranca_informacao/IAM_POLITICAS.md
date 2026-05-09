# IAM e Políticas de Segurança - UniStock

## Objetivo

Definir políticas de autenticação, autorização e controle de acesso do sistema UniStock, garantindo proteção de dados, segurança operacional e conformidade com boas práticas modernas de segurança da informação.

---

## Conceitos Utilizados

- IAM (Identity and Access Management)
- Zero Trust
- RBAC (Role-Based Access Control)
- JWT Authentication
- MFA (Multi-Factor Authentication)
- Least Privilege

---

# Políticas de Segurança e Controle de Acesso

| # | Política | Tipo | Justificativa Técnica |
|---|---|---|---|
| 1 | Senhas com mínimo de 8 caracteres | Autenticação | Reduz vulnerabilidade a ataques de força bruta. |
| 2 | Obrigatoriedade de caracteres especiais em senhas | Autenticação | Aumenta complexidade das credenciais. |
| 3 | Hashing de senhas com bcrypt | Autenticação | Impede leitura direta das senhas caso o banco seja comprometido. |
| 4 | JWT com tempo de expiração | Sessão | Evita reutilização de tokens antigos. |
| 5 | Logout automático após inatividade | Sessão | Reduz riscos em computadores públicos. |
| 6 | MFA para administradores | Autenticação | Adiciona camada extra de proteção para contas críticas. |
| 7 | Controle RBAC para usuários e administradores | Autorização | Restringe acesso conforme perfil do usuário. |
| 8 | Apenas administradores podem alterar estoque | Autorização | Evita manipulação indevida de inventário. |
| 9 | Clientes só podem visualizar próprios pedidos | Autorização | Previne ataques IDOR. |
| 10 | Bloqueio temporário após múltiplas tentativas de login | Proteção | Mitiga ataques de força bruta. |
| 11 | Uso obrigatório de HTTPS | Comunicação Segura | Impede interceptação de dados sensíveis. |
| 12 | Tokens JWT armazenados de forma segura | Sessão | Evita roubo de sessão por scripts maliciosos. |
| 13 | Logs de auditoria para ações administrativas | Auditoria | Permite rastreamento de alterações críticas. |
| 14 | Restrição de upload apenas para formatos permitidos | Upload Seguro | Reduz risco de malware no servidor. |
| 15 | Sanitização de entradas de formulário | Proteção Web | Evita SQL Injection e XSS. |
| 16 | Expiração de sessão após troca de senha | Sessão | Impede reutilização de sessões antigas. |
| 17 | Permissões mínimas no banco de dados | Infraestrutura | Minimiza impacto de invasões. |
| 18 | Rotação periódica de chaves secretas | Segurança de Tokens | Reduz risco de vazamento permanente. |
| 19 | Monitoramento de acessos suspeitos | Monitoramento | Detecta possíveis invasões rapidamente. |
| 20 | Backup criptografado dos dados | Proteção de Dados | Garante recuperação segura em incidentes. |

---

## Modelo de Perfis de Acesso (RBAC)

| Perfil | Permissões |
|---|---|
| Cliente | Comprar produtos, visualizar pedidos próprios, editar perfil |
| Funcionário | Gerenciar estoque e pedidos |
| Administrador | Controle total do sistema |
| Analista | Visualizar relatórios e dashboards |

---

## Princípios de Segurança Aplicados

### Zero Trust
Nenhum usuário ou dispositivo é considerado confiável automaticamente.

### Least Privilege
Cada usuário possui apenas as permissões necessárias para executar suas funções.

### Defesa em Camadas
O sistema utiliza múltiplas barreiras de proteção:
- autenticação
- autorização
- criptografia
- logs
- monitoramento

---

## Conclusão

As políticas IAM do UniStock foram definidas com foco em segurança operacional, proteção de dados e mitigação de ameaças identificadas na Matriz GUT. A combinação de autenticação segura, RBAC, criptografia e monitoramento contínuo reduz significativamente os riscos de invasão, vazamento de dados e acesso indevido ao sistema.
