# Matriz GUT - UniStock

## Objetivo

Mapear ameaças reais de segurança que podem afetar o sistema UniStock, classificando-as com base na metodologia GUT (Gravidade, Urgência e Tendência).

---

| # | Ameaça | Como ocorreria no UniStock | G | U | T | Total |
|---|---|---|---|---|---|---|
| 1 | SQL Injection | Um invasor pode inserir comandos SQL em formulários de login ou busca de produtos para acessar ou modificar o banco de dados do sistema. | 5 | 5 | 5 | 125 |
| 2 | XSS (Cross-Site Scripting) | Um atacante pode inserir scripts maliciosos em campos de texto para roubar sessões de usuários. | 4 | 4 | 4 | 64 |
| 3 | IDOR | Um usuário pode alterar IDs na URL para acessar pedidos ou dados de outros clientes. | 5 | 4 | 5 | 100 |
| 4 | Força Bruta | Tentativas automatizadas de login podem comprometer contas com senhas fracas. | 4 | 4 | 5 | 80 |
| 5 | Vazamento de JWT | Tokens expostos podem permitir acesso indevido às contas dos usuários. | 5 | 5 | 4 | 100 |
| 6 | Exposição de API | APIs do UniStock podem expor dados de produtos, pedidos ou usuários sem autenticação adequada. | 5 | 4 | 4 | 80 |
| 7 | Upload Malicioso de Arquivos | Um atacante pode enviar arquivos infectados na área de upload de comprovantes ou imagens de produtos. | 4 | 4 | 4 | 64 |
| 8 | Sessão Sem Expiração | Usuários podem permanecer logados indefinidamente em computadores públicos, permitindo acesso indevido. | 4 | 3 | 4 | 48 |
| 9 | Vazamento de Banco de Dados | Falhas no servidor podem expor informações de clientes, pedidos e estoque do UniStock. | 5 | 5 | 5 | 125 |
| 10 | Falha de Backup | A perda do banco de dados sem backup atualizado pode interromper completamente o funcionamento do sistema. | 5 | 4 | 5 | 100 |
| 11 | DDoS | Ataques de sobrecarga podem deixar a plataforma UniStock indisponível para clientes e administradores. | 5 | 5 | 4 | 100 |
| 12 | Credenciais Vazadas | Senhas reutilizadas por administradores podem permitir invasões ao painel administrativo. | 5 | 5 | 5 | 125 |
| 13 | Permissões Excessivas | Usuários comuns podem acessar funções administrativas devido a falhas de autorização. | 5 | 4 | 5 | 100 |
| 14 | Malware no Servidor | Softwares maliciosos podem comprometer o servidor e capturar dados do sistema. | 5 | 4 | 4 | 80 |
| 15 | Engenharia Social | Funcionários podem ser enganados por e-mails falsos solicitando acesso ao sistema. | 4 | 4 | 5 | 80 |
| 16 | Configuração Incorreta do Firebase/Cloud | Arquivos ou banco podem ficar públicos devido a permissões incorretas na nuvem. | 5 | 4 | 5 | 100 |
| 17 | Exposição de Chaves Secretas | Tokens JWT, chaves de API ou senhas podem ser publicados acidentalmente no GitHub. | 5 | 5 | 5 | 125 |
| 18 | Falta de HTTPS | Dados sensíveis podem ser interceptados durante o tráfego entre cliente e servidor. | 5 | 5 | 4 | 100 |
| 19 | Ataque de Bot em Compras | Bots podem gerar compras falsas ou consultas excessivas, prejudicando o estoque e desempenho. | 3 | 4 | 4 | 48 |
| 20 | Exclusão Acidental de Dados | Funcionários podem apagar registros importantes de estoque ou vendas sem confirmação adequada. | 4 | 3 | 4 | 48 |

---

## Critérios da Matriz GUT

- Gravidade (G): impacto causado caso a ameaça aconteça.
- Urgência (U): velocidade necessária para correção.
- Tendência (T): probabilidade de crescimento do problema caso não seja tratado.
