# LGPD e Proteção de Dados - UniStock

## Objetivo

Documentar os dados pessoais coletados pelo sistema UniStock, definindo finalidade, base legal e direitos do titular conforme a Lei Geral de Proteção de Dados (LGPD - Lei 13.709/18).

---

## Conceitos Aplicados

- LGPD (Lei Geral de Proteção de Dados)
- Privacidade by Design
- Minimização de Dados
- Consentimento
- Execução de Contrato
- Legítimo Interesse
- Segurança da Informação
- Governança de Dados

---

# Dados Pessoais e Tratamentos Realizados

| # | Dado Coletado | Finalidade | Base Legal | Direitos do Titular |
|---|---|---|---|---|
| 1 | Nome completo | Identificação do cliente na plataforma | Execução de Contrato (Art. 7º, V) | Solicitar correção ou exclusão da conta |
| 2 | CPF | Emissão de nota fiscal e validação fiscal | Obrigação Legal (Art. 7º, II) | Exclusão após prazo legal obrigatório |
| 3 | E-mail | Login, recuperação de senha e notificações | Execução de Contrato | Solicitar alteração ou remoção |
| 4 | Senha criptografada | Autenticação segura no sistema | Legítimo Interesse | Alteração de senha a qualquer momento |
| 5 | Número de telefone | Contato sobre pedidos e suporte | Consentimento | Solicitar remoção do cadastro |
| 6 | Endereço | Entrega de produtos | Execução de Contrato | Alteração cadastral pelo usuário |
| 7 | CEP | Validação logística de entrega | Execução de Contrato | Correção de dados incorretos |
| 8 | Endereço IP | Segurança e prevenção contra fraudes | Legítimo Interesse | Solicitar anonimização quando possível |
| 9 | Logs de acesso | Auditoria e investigação de incidentes | Legítimo Interesse | Solicitar informações sobre armazenamento |
| 10 | Cookies de sessão | Manutenção da autenticação | Legítimo Interesse | Gerenciamento via navegador |
| 11 | Histórico de pedidos | Controle operacional e suporte | Execução de Contrato | Solicitação de exportação dos dados |
| 12 | Dados bancários | Processamento de pagamentos | Execução de Contrato | Exclusão conforme legislação financeira |
| 13 | Tokens JWT | Controle de autenticação e sessão | Legítimo Interesse | Expiração automática da sessão |
| 14 | Fotos de produtos enviadas | Cadastro de itens no estoque | Execução de Contrato | Solicitação de exclusão |
| 15 | Nome de usuários administradores | Auditoria e rastreabilidade | Legítimo Interesse | Solicitar revisão de dados |
| 16 | Histórico de alterações no estoque | Segurança operacional | Legítimo Interesse | Consulta mediante solicitação |
| 17 | Dados de suporte técnico | Atendimento ao cliente | Execução de Contrato | Solicitação de exclusão após atendimento |
| 18 | Informações de navegação | Melhorias na experiência da plataforma | Consentimento | Revogação do consentimento |
| 19 | Relatórios analíticos de uso | Inteligência operacional e métricas | Legítimo Interesse | Solicitar anonimização |
| 20 | Sessões de login | Controle de acesso e segurança | Legítimo Interesse | Encerramento manual das sessões |

---

# Medidas de Segurança Aplicadas

O UniStock utiliza medidas técnicas e administrativas para proteger os dados pessoais armazenados na plataforma.

## Controles Implementados

- Criptografia de senhas com bcrypt
- Comunicação segura utilizando HTTPS
- Tokens JWT com expiração
- Controle RBAC de permissões
- Logs de auditoria
- Backup criptografado
- MFA para administradores
- Sanitização de entradas contra SQL Injection e XSS
- Controle de sessão e logout automático
- Restrição de acesso por perfil

---

# Direitos Garantidos ao Usuário

Conforme a LGPD, o titular dos dados poderá:

- Solicitar confirmação de tratamento dos dados
- Solicitar acesso aos dados armazenados
- Corrigir dados incompletos ou incorretos
- Solicitar anonimização quando aplicável
- Solicitar exclusão dos dados
- Revogar consentimentos concedidos
- Solicitar portabilidade dos dados
- Obter informações sobre compartilhamento de dados

---

# Política de Retenção de Dados

Os dados pessoais serão armazenados apenas pelo período necessário para cumprimento das finalidades operacionais, legais e fiscais do UniStock.

Após o encerramento da conta:

- Dados fiscais poderão ser mantidos pelo prazo exigido em lei
- Tokens e sessões serão invalidados imediatamente
- Dados desnecessários serão anonimizados ou excluídos
- Backups seguirão política de retenção segura

---

# Princípios da LGPD Aplicados

## Necessidade

O sistema coleta apenas os dados essenciais para funcionamento da plataforma.

## Finalidade

Todos os dados possuem finalidade específica e legítima.

## Segurança

Os dados são protegidos contra acesso não autorizado e vazamentos.

## Transparência

Os usuários possuem acesso às informações sobre tratamento dos dados.

## Prevenção

O sistema adota medidas preventivas contra incidentes de segurança.

---

# Conclusão

A adequação do UniStock à LGPD garante maior proteção aos dados pessoais dos usuários, reduzindo riscos de vazamentos, acessos indevidos e penalidades legais. As medidas aplicadas seguem boas práticas modernas de segurança da informação e governança de dados, assegurando conformidade com a Lei Geral de Proteção de Dados.
