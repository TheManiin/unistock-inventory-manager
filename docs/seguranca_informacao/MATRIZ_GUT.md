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

---

## Critérios da Matriz GUT

- Gravidade (G): impacto causado caso a ameaça aconteça.
- Urgência (U): velocidade necessária para correção.
- Tendência (T): probabilidade de crescimento do problema caso não seja tratado.
