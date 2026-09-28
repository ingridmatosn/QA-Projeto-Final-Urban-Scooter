# QA Projeto Final — Urban Scooter (Web, Mobile e API)

Projeto final do bootcamp de **Analista de QA da TripleTen** (Sprint 9): planejamento, execução e documentação de testes do serviço de aluguel de patinetes **Urban Scooter** em três frentes — formulário web, aplicativo mobile do entregador e API do backend.

**Status:** projeto aprovado na revisão da TripleTen.

## Visão geral

| Frente | Escopo | Casos | Aprovados | Reprovados | Bloqueados | Bugs |
|---|---|---|---|---|---|---|
| [Tarefa 1 — Web](tarefa-1-web.md) | Formulário "Para quem é a scooter" em Chrome e Opera (1280x720) | 52 | 36 | 16 | — | 16 |
| [Tarefa 2 — Mobile](tarefa-2-mobile.md) | App do entregador: notificação de prazo, falha de conexão e layout (Figma) | 17 | 7 | 5 | 5 | 5 |
| [Tarefa 3 — API](tarefa-3-api.md) | Criar e excluir entregador (`POST` e `DELETE /api/v1/courier`) + datas de pedido | 36 | 16 | 20 | — | 20 |
| **Total** | | **105** | **59** | **41** | **5** | **41** |

Todos os bugs foram registrados no Jira (KAN-84 a KAN-124), **um por caso reprovado**, com passos para reproduzir, resultado esperado, resultado real, ambiente e print de evidência. Veja a lista completa em [relatorios-de-bug.md](relatorios-de-bug.md).

## Técnicas aplicadas

- **Partição de equivalência e análise de valor limite** em todos os campos com regra de tamanho ou formato (por exemplo, Endereço com 4, 5, 49, 50 e 51 caracteres; login da API com 1, 2, 10 e 11 letras).
- **Teste cross-browser**: cada caso da Tarefa 1 foi executado no Google Chrome e no Opera, na mesma resolução.
- **Testes específicos de mobile**: modo avião, notificação com data e hora controladas no emulador, comportamento de pop-ups e comparação com o design do Figma.
- **Testes de API**: validação de código de status, corpo da resposta e regras de negócio, incluindo a exclusão em cascata dos pedidos de um entregador excluído.

## Principais achados

- **Web:** mensagens de validação diferentes do requisito ("Insira um número válido" no lugar de "Digite um número válido") e campos que aceitam valores fora do limite, como Sobrenome com 16 caracteres e Telefone com 13 caracteres ou sem o sinal "+".
- **Mobile:** a notificação "2 horas para o final do pedido" não é enviada; os botões "Login", "Não lembro da minha senha" e o filtro de estações não exibem o pop-up "Sem acesso à internet"; o pop-up fecha ao tocar fora dele.
- **API:** o `POST /api/v1/courier` aceita login, firstName e senha fora das regras e responde **201 Created** em vez de **400 Bad Request**; o `DELETE` com id não numérico responde **500 Internal Server Error**; e excluir um entregador **não apaga os pedidos vinculados**, que continuam no banco com `"inDelivery": true`.

## Ferramentas

Google Sheets · Jira · Google Chrome e Opera (DevTools) · Android Studio (emulador Pixel 5, API 31) · Figma · Postman

## Estrutura do repositório

| Arquivo | Conteúdo |
|---|---|
| `tarefa-1-web.md` | 52 casos de teste do formulário web, com classe de equivalência, valor limite, dado de teste e resultado no Chrome e no Opera |
| `tarefa-2-mobile.md` | 17 casos de teste do aplicativo mobile |
| `tarefa-3-api.md` | 36 casos de teste da API, com o corpo da requisição de cada caso |
| `relatorios-de-bug.md` | Os 41 bugs do Jira, com prioridade, caso de teste relacionado, resultado esperado e resultado real |

## Aprendizado

Na revisão, a sugestão foi agrupar em **um único bug** os defeitos que têm a mesma causa e aparecem em cenários diferentes (por exemplo, a mensagem de validação do Endereço com 4 e com 51 caracteres), relacionando esse bug aos vários casos de teste. Isso reduz tickets duplicados e facilita o acompanhamento da correção pelo time de desenvolvimento — prática que passei a adotar.

## Autora

**Ingrid Matos** — QA Junior
[LinkedIn](https://linkedin.com/in/ingridmatosn) · [Portfólio de QA](https://github.com/ingridmatosn/QA-Portfolio-Main)
