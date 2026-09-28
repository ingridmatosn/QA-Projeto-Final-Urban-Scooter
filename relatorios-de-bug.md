# Relatórios de bug

41 bugs registrados no Jira (KAN-84 a KAN-124), um por caso reprovado, cada um com passos para reproduzir, resultado esperado, resultado real, ambiente e evidência (print).

| Bug | Título | Prioridade | Caso de teste |
|---|---|---|---|
| [KAN-84](https://ingridmatos.atlassian.net/browse/KAN-84) | Campo "Sobrenome" aceita 16 caracteres sem exibir mensagem de erro | Média | Tarefa 1, T-22 |
| [KAN-85](https://ingridmatos.atlassian.net/browse/KAN-85) | Campo "Endereço" não aceita 50 caracteres (limite máximo) e exibe mensagem de erro | Média | Tarefa 1, T-29 |
| [KAN-86](https://ingridmatos.atlassian.net/browse/KAN-86) | Campo "Endereço" vazio não exibe mensagem de erro e permite avançar para o formulário "Locação" | Alta | Tarefa 1, T-31 |
| [KAN-87](https://ingridmatos.atlassian.net/browse/KAN-87) | Campo "Endereço" com 4 caracteres exibe a mensagem "Insira um número válido" em vez de "Digite um número válido" | Baixa | Tarefa 1, T-32 |
| [KAN-88](https://ingridmatos.atlassian.net/browse/KAN-88) | Campo "Telefone" não aceita 10 caracteres (limite mínimo) e exibe mensagem de erro | Média | Tarefa 1, T-40 |
| [KAN-89](https://ingridmatos.atlassian.net/browse/KAN-89) | Campo "Telefone" aceita 13 caracteres sem exibir mensagem de erro | Média | Tarefa 1, T-45 |
| [KAN-90](https://ingridmatos.atlassian.net/browse/KAN-90) | Campo "Telefone" aceita número sem o sinal "+" sem exibir mensagem de erro | Média | Tarefa 1, T-46 |
| [KAN-91](https://ingridmatos.atlassian.net/browse/KAN-91) | Campo "Telefone" com 9 caracteres exibe a mensagem "Insira um número válido" em vez de "Digite um número válido" | Baixa | Tarefa 1, T-44 |
| [KAN-92](https://ingridmatos.atlassian.net/browse/KAN-92) | Formulário "Para quem é a scooter" vazio não exibe mensagem de erro no campo "Endereço" ao clicar em "Avançar" | Alta | Tarefa 1, T-51 |
| [KAN-93](https://ingridmatos.atlassian.net/browse/KAN-93) | Campo "Endereço" com 51 caracteres exibe a mensagem "Insira um número válido" em vez de "Digite um número válido" | Baixa | Tarefa 1, T-33 |
| [KAN-94](https://ingridmatos.atlassian.net/browse/KAN-94) | Campo "Endereço" com caracteres especiais exibe a mensagem "Insira um número válido" em vez de "Digite um número válido" | Baixa | Tarefa 1, T-34 |
| [KAN-95](https://ingridmatos.atlassian.net/browse/KAN-95) | Campo "Endereço" com 3 caracteres após remover os espaços exibe a mensagem "Insira um número válido" em vez de "Digite um número válido" | Baixa | Tarefa 1, T-35 |
| [KAN-96](https://ingridmatos.atlassian.net/browse/KAN-96) | Campo "Telefone" vazio exibe a mensagem "Insira um número válido" em vez de "Digite um número válido" | Baixa | Tarefa 1, T-43 |
| [KAN-97](https://ingridmatos.atlassian.net/browse/KAN-97) | Campo "Telefone" com letras exibe a mensagem "Insira um número válido" em vez de "Digite um número válido" | Baixa | Tarefa 1, T-47 |
| [KAN-98](https://ingridmatos.atlassian.net/browse/KAN-98) | Campo "Telefone" com espaço e traço exibe a mensagem "Insira um número válido" em vez de "Digite um número válido" | Baixa | Tarefa 1, T-48 |
| [KAN-99](https://ingridmatos.atlassian.net/browse/KAN-99) | Campo "Telefone" com parênteses exibe a mensagem "Insira um número válido" em vez de "Digite um número válido" | Baixa | Tarefa 1, T-49 |
| [KAN-100](https://ingridmatos.atlassian.net/browse/KAN-100) | Ícone do filtro de estação abre a lista sem exibir o pop-up "Sem acesso à internet" quando não há conexão | Baixa | Tarefa 2, T-11 |
| [KAN-101](https://ingridmatos.atlassian.net/browse/KAN-101) | Pop-up "Sem acesso à internet" fecha ao tocar fora dele, sem tocar em "Ok" | Média | Tarefa 2, T-13 |
| [KAN-102](https://ingridmatos.atlassian.net/browse/KAN-102) | Botão "Login" não exibe o pop-up "Sem acesso à internet" quando não há conexão | Alta | Tarefa 2, T-8 |
| [KAN-103](https://ingridmatos.atlassian.net/browse/KAN-103) | "Não lembro da minha senha" exibe "Contate o gerente: 0101" em vez do pop-up "Sem acesso à internet" quando não há conexão | Média | Tarefa 2, T-9 |
| [KAN-104](https://ingridmatos.atlassian.net/browse/KAN-104) | Notificação "2 horas para o final do pedido" não é recebida às 21:59 do dia de entrega | Alta | Tarefa 2, T-1 |
| [KAN-105](https://ingridmatos.atlassian.net/browse/KAN-105) | POST /api/v1/orders aceita deliveryDate da semana passada e retorna 201 Created ao invés de 400 Bad Request | Alta | Tarefa 3, T-32 |
| [KAN-106](https://ingridmatos.atlassian.net/browse/KAN-106) | POST /api/v1/orders aceita deliveryDate de ontem e retorna 201 Created ao invés de 400 Bad Request | Alta | Tarefa 3, T-33 |
| [KAN-107](https://ingridmatos.atlassian.net/browse/KAN-107) | POST /api/v1/orders aceita deliveryDate de hoje e retorna 201 Created ao invés de 400 Bad Request | Alta | Tarefa 3, T-34 |
| [KAN-108](https://ingridmatos.atlassian.net/browse/KAN-108) | POST /api/v1/courier aceita login com 1 letra e retorna 201 Created ao invés de 400 Bad Request | Média | Tarefa 3, T-4 |
| [KAN-109](https://ingridmatos.atlassian.net/browse/KAN-109) | POST /api/v1/courier aceita login com 11 letras e retorna 201 Created ao invés de 400 Bad Request | Média | Tarefa 3, T-5 |
| [KAN-110](https://ingridmatos.atlassian.net/browse/KAN-110) | POST /api/v1/courier aceita login com números e retorna 201 Created ao invés de 400 Bad Request | Média | Tarefa 3, T-6 |
| [KAN-111](https://ingridmatos.atlassian.net/browse/KAN-111) | POST /api/v1/courier aceita login com letras cirílicas e retorna 201 Created ao invés de 400 Bad Request | Média | Tarefa 3, T-7 |
| [KAN-112](https://ingridmatos.atlassian.net/browse/KAN-112) | POST /api/v1/courier aceita login com caractere especial e retorna 201 Created ao invés de 400 Bad Request | Média | Tarefa 3, T-8 |
| [KAN-113](https://ingridmatos.atlassian.net/browse/KAN-113) | POST /api/v1/courier aceita firstName com 1 letra e retorna 201 Created ao invés de 400 Bad Request | Média | Tarefa 3, T-14 |
| [KAN-114](https://ingridmatos.atlassian.net/browse/KAN-114) | POST /api/v1/courier aceita firstName com 11 letras e retorna 201 Created ao invés de 400 Bad Request | Média | Tarefa 3, T-15 |
| [KAN-115](https://ingridmatos.atlassian.net/browse/KAN-115) | POST /api/v1/courier aceita firstName com número e retorna 201 Created ao invés de 400 Bad Request | Média | Tarefa 3, T-16 |
| [KAN-116](https://ingridmatos.atlassian.net/browse/KAN-116) | POST /api/v1/courier aceita firstName com letras cirílicas e retorna 201 Created ao invés de 400 Bad Request | Média | Tarefa 3, T-17 |
| [KAN-117](https://ingridmatos.atlassian.net/browse/KAN-117) | POST /api/v1/courier aceita firstName com caractere especial e retorna 201 Created ao invés de 400 Bad Request | Média | Tarefa 3, T-18 |
| [KAN-118](https://ingridmatos.atlassian.net/browse/KAN-118) | POST /api/v1/courier aceita firstName vazio e retorna 201 Created ao invés de 400 Bad Request | Média | Tarefa 3, T-19 |
| [KAN-119](https://ingridmatos.atlassian.net/browse/KAN-119) | POST /api/v1/courier aceita requisição sem o campo firstName e retorna 201 Created ao invés de 400 Bad Request | Média | Tarefa 3, T-20 |
| [KAN-120](https://ingridmatos.atlassian.net/browse/KAN-120) | POST /api/v1/courier aceita senha com 3 dígitos e retorna 201 Created ao invés de 400 Bad Request | Média | Tarefa 3, T-21 |
| [KAN-121](https://ingridmatos.atlassian.net/browse/KAN-121) | POST /api/v1/courier aceita senha com 5 dígitos e retorna 201 Created ao invés de 400 Bad Request | Média | Tarefa 3, T-22 |
| [KAN-122](https://ingridmatos.atlassian.net/browse/KAN-122) | POST /api/v1/courier aceita senha com letras e retorna 201 Created ao invés de 400 Bad Request | Média | Tarefa 3, T-23 |
| [KAN-123](https://ingridmatos.atlassian.net/browse/KAN-123) | DELETE /api/v1/courier/:id com id não numérico ("abc") retorna 500 Internal Server Error ao invés de 400 Bad Request | Alta | Tarefa 3, T-29 |
| [KAN-124](https://ingridmatos.atlassian.net/browse/KAN-124) | DELETE /api/v1/courier/:id exclui o entregador, mas não exclui os pedidos vinculados a ele na tabela Orders | Alta | Tarefa 3, T-31 |

## Detalhes

### KAN-84 — Campo "Sobrenome" aceita 16 caracteres sem exibir mensagem de erro

- **Prioridade:** Média
- **Caso de teste:** Tarefa 1, T-22
- **Resultado esperado:** O campo “Sobrenome” deveria aceitar somente de 2 a 15 caracteres. Com 16 caracteres, o campo deveria ficar destacado em vermelho com a mensagem “Insira um nome válido” e o usuário não deveria avançar para o formulário “Locação”.
- **Resultado real:** O campo aceitou 16 caracteres sem destaque vermelho e sem mensagem de erro, e ao clicar em “Avançar” o formulário “Locação” foi aberto.

### KAN-85 — Campo "Endereço" não aceita 50 caracteres (limite máximo) e exibe mensagem de erro

- **Prioridade:** Média
- **Caso de teste:** Tarefa 1, T-29
- **Resultado esperado:** O campo “Endereço” deveria aceitar de 5 a 50 caracteres. Com 50 caracteres (limite máximo), o valor deveria ser aceito sem mensagem de erro e o formulário “Locação” deveria ser aberto.
- **Resultado real:** O campo ficou destacado em vermelho com a mensagem “Insira um número válido” e o usuário não conseguiu avançar. Com 49 caracteres o valor é aceito normalmente.

### KAN-86 — Campo "Endereço" vazio não exibe mensagem de erro e permite avançar para o formulário "Locação"

- **Prioridade:** Alta
- **Caso de teste:** Tarefa 1, T-31
- **Resultado esperado:** O campo “Endereço” é obrigatório. Vazio, deveria ficar destacado em vermelho com a mensagem “Digite um número válido” e o usuário não deveria avançar para o formulário “Locação”.
- **Resultado real:** O campo vazio não exibiu mensagem de erro e, ao clicar em “Avançar”, o formulário “Locação” foi aberto.

### KAN-87 — Campo "Endereço" com 4 caracteres exibe a mensagem "Insira um número válido" em vez de "Digite um número válido"

- **Prioridade:** Baixa
- **Caso de teste:** Tarefa 1, T-32
- **Resultado esperado:** Com 4 caracteres, abaixo do mínimo (“Rua1”), o campo deveria ficar destacado em vermelho com a mensagem “Digite um número válido”, conforme os requisitos, e o usuário não deveria avançar.
- **Resultado real:** O campo ficou destacado em vermelho e o usuário não avançou, mas a mensagem exibida foi “Insira um número válido” em vez de “Digite um número válido”.

### KAN-88 — Campo "Telefone" não aceita 10 caracteres (limite mínimo) e exibe mensagem de erro

- **Prioridade:** Média
- **Caso de teste:** Tarefa 1, T-40
- **Resultado esperado:** O campo “Telefone” deveria aceitar de 10 a 12 caracteres, incluindo o sinal “+”. Com 10 caracteres (limite mínimo), o valor deveria ser aceito sem mensagem de erro e o formulário “Locação” deveria ser aberto.
- **Resultado real:** O campo ficou destacado em vermelho com a mensagem “Insira um número válido” e o usuário não conseguiu avançar.

### KAN-89 — Campo "Telefone" aceita 13 caracteres sem exibir mensagem de erro

- **Prioridade:** Média
- **Caso de teste:** Tarefa 1, T-45
- **Resultado esperado:** O campo “Telefone” deveria aceitar somente de 10 a 12 caracteres, incluindo o sinal “+”. Com 13 caracteres, o campo deveria ficar destacado em vermelho com a mensagem “Digite um número válido” e o usuário não deveria avançar.
- **Resultado real:** O campo aceitou 13 caracteres sem destaque vermelho e sem mensagem de erro, e ao clicar em “Avançar” o formulário “Locação” foi aberto.

### KAN-90 — Campo "Telefone" aceita número sem o sinal "+" sem exibir mensagem de erro

- **Prioridade:** Média
- **Caso de teste:** Tarefa 1, T-46
- **Resultado esperado:** O sinal “+” é obrigatório no campo “Telefone”. Sem ele, o campo deveria ficar destacado em vermelho com a mensagem “Digite um número válido” e o usuário não deveria avançar.
- **Resultado real:** O campo aceitou o número sem o sinal “+”, sem destaque vermelho e sem mensagem de erro, e ao clicar em “Avançar” o formulário “Locação” foi aberto.

### KAN-91 — Campo "Telefone" com 9 caracteres exibe a mensagem "Insira um número válido" em vez de "Digite um número válido"

- **Prioridade:** Baixa
- **Caso de teste:** Tarefa 1, T-44
- **Resultado esperado:** Com 9 caracteres, abaixo do mínimo (“+12345678”), o campo deveria ficar destacado em vermelho com a mensagem “Digite um número válido”, conforme os requisitos, e o usuário não deveria avançar.
- **Resultado real:** O campo ficou destacado em vermelho e o usuário não avançou, mas a mensagem exibida foi “Insira um número válido” em vez de “Digite um número válido”.

### KAN-92 — Formulário "Para quem é a scooter" vazio não exibe mensagem de erro no campo "Endereço" ao clicar em "Avançar"

- **Prioridade:** Alta
- **Caso de teste:** Tarefa 1, T-51
- **Resultado esperado:** Todos os campos obrigatórios deveriam ficar destacados em vermelho com a mensagem de erro de cada um, inclusive o campo “Endereço”, e o usuário não deveria avançar.
- **Resultado real:** Os campos “Nome”, “Sobrenome”, “Estação de metrô” e “Telefone” exibiram mensagem de erro, mas o campo “Endereço” não ficou destacado em vermelho e não exibiu mensagem de erro.

### KAN-93 — Campo "Endereço" com 51 caracteres exibe a mensagem "Insira um número válido" em vez de "Digite um número válido"

- **Prioridade:** Baixa
- **Caso de teste:** Tarefa 1, T-33
- **Resultado esperado:** Com 51 caracteres, acima do máximo (“Rua Augusta, 1000, apto 12, bloco B, Centro. Ladeir”), o campo deveria ficar destacado em vermelho com a mensagem “Digite um número válido”, conforme os requisitos, e o usuário não deveria avançar.
- **Resultado real:** O campo ficou destacado em vermelho e o usuário não avançou, mas a mensagem exibida foi “Insira um número válido” em vez de “Digite um número válido”.

### KAN-94 — Campo "Endereço" com caracteres especiais exibe a mensagem "Insira um número válido" em vez de "Digite um número válido"

- **Prioridade:** Baixa
- **Caso de teste:** Tarefa 1, T-34
- **Resultado esperado:** Com caracteres especiais (“Rua #10 @ casa”), o campo deveria ficar destacado em vermelho com a mensagem “Digite um número válido”, conforme os requisitos, e o usuário não deveria avançar.
- **Resultado real:** O campo ficou destacado em vermelho e o usuário não avançou, mas a mensagem exibida foi “Insira um número válido” em vez de “Digite um número válido”.

### KAN-95 — Campo "Endereço" com 3 caracteres após remover os espaços exibe a mensagem "Insira um número válido" em vez de "Digite um número válido"

- **Prioridade:** Baixa
- **Caso de teste:** Tarefa 1, T-35
- **Resultado esperado:** Ao tirar o foco, os espaços do início e do fim deveriam ser removidos, restando “Rua” (3 caracteres, abaixo do mínimo). O campo deveria ficar destacado em vermelho com a mensagem “Digite um número válido”, conforme os requisitos, e o usuário não deveria avançar.
- **Resultado real:** Os espaços foram removidos e o campo ficou destacado em vermelho, mas a mensagem exibida foi “Insira um número válido” em vez de “Digite um número válido”.

### KAN-96 — Campo "Telefone" vazio exibe a mensagem "Insira um número válido" em vez de "Digite um número válido"

- **Prioridade:** Baixa
- **Caso de teste:** Tarefa 1, T-43
- **Resultado esperado:** Vazio, o campo “Telefone” deveria ficar destacado em vermelho com a mensagem “Digite um número válido”, conforme os requisitos, e o usuário não deveria avançar.
- **Resultado real:** O campo ficou destacado em vermelho e o usuário não avançou, mas a mensagem exibida foi “Insira um número válido” em vez de “Digite um número válido”.

### KAN-97 — Campo "Telefone" com letras exibe a mensagem "Insira um número válido" em vez de "Digite um número válido"

- **Prioridade:** Baixa
- **Caso de teste:** Tarefa 1, T-47
- **Resultado esperado:** Com letras (“+12345abcde”), o campo deveria ficar destacado em vermelho com a mensagem “Digite um número válido”, conforme os requisitos, e o usuário não deveria avançar.
- **Resultado real:** O campo ficou destacado em vermelho e o usuário não avançou, mas a mensagem exibida foi “Insira um número válido” em vez de “Digite um número válido”.

### KAN-98 — Campo "Telefone" com espaço e traço exibe a mensagem "Insira um número válido" em vez de "Digite um número válido"

- **Prioridade:** Baixa
- **Caso de teste:** Tarefa 1, T-48
- **Resultado esperado:** Com espaço e traço (“+12 345-6789”), o campo deveria ficar destacado em vermelho com a mensagem “Digite um número válido”, conforme os requisitos, e o usuário não deveria avançar.
- **Resultado real:** O campo ficou destacado em vermelho e o usuário não avançou, mas a mensagem exibida foi “Insira um número válido” em vez de “Digite um número válido”.

### KAN-99 — Campo "Telefone" com parênteses exibe a mensagem "Insira um número válido" em vez de "Digite um número válido"

- **Prioridade:** Baixa
- **Caso de teste:** Tarefa 1, T-49
- **Resultado esperado:** Com parênteses (“+(12)345678”), o campo deveria ficar destacado em vermelho com a mensagem “Digite um número válido”, conforme os requisitos, e o usuário não deveria avançar.
- **Resultado real:** O campo ficou destacado em vermelho e o usuário não avançou, mas a mensagem exibida foi “Insira um número válido” em vez de “Digite um número válido”.

### KAN-100 — Ícone do filtro de estação abre a lista sem exibir o pop-up "Sem acesso à internet" quando não há conexão

- **Prioridade:** Baixa
- **Caso de teste:** Tarefa 2, T-11
- **Resultado esperado:** Sem conexão com a internet, ao tocar em qualquer botão ativo deveria aparecer a janela pop-up “Sem acesso à internet” com o botão “Ok”. O ícone do filtro é um botão ativo, então o pop-up deveria ser exibido.
- **Resultado real:** O filtro abre normalmente, mostrando a lista de estações (“1st Street”) e o botão “Aplicar”, sem exibir o pop-up “Sem acesso à internet”. O pop-up só aparece depois, ao tocar em “Aplicar”.

### KAN-101 — Pop-up "Sem acesso à internet" fecha ao tocar fora dele, sem tocar em "Ok"

- **Prioridade:** Média
- **Caso de teste:** Tarefa 2, T-13
- **Resultado esperado:** O pop-up “Sem acesso à internet” deveria continuar aberto, pois ele só desaparece quando o botão “Ok” é tocado.
- **Resultado real:** O pop-up “Sem acesso à internet” fecha ao tocar fora dele, sem tocar no botão “Ok”.

### KAN-102 — Botão "Login" não exibe o pop-up "Sem acesso à internet" quando não há conexão

- **Prioridade:** Alta
- **Caso de teste:** Tarefa 2, T-8
- **Resultado esperado:** A janela pop-up “Sem acesso à internet” deveria ser exibida com o botão “Ok”.
- **Resultado real:** Nada acontece ao tocar em “Login”: o pop-up “Sem acesso à internet” não é exibido e o usuário permanece na tela de login, sem nenhum aviso.

### KAN-103 — "Não lembro da minha senha" exibe "Contate o gerente: 0101" em vez do pop-up "Sem acesso à internet" quando não há conexão

- **Prioridade:** Média
- **Caso de teste:** Tarefa 2, T-9
- **Resultado esperado:** A janela pop-up “Sem acesso à internet” deveria ser exibida com o botão “Ok”.
- **Resultado real:** É exibida a notificação “Contate o gerente: 0101” com o botão “OK”, como se houvesse conexão. O pop-up “Sem acesso à internet” não aparece.

### KAN-104 — Notificação "2 horas para o final do pedido" não é recebida às 21:59 do dia de entrega

- **Prioridade:** Alta
- **Caso de teste:** Tarefa 2, T-1
- **Resultado esperado:** Às 21:59 do dia de entrega, o entregador deveria receber uma notificação do app Urban Scooter com o texto “2 horas para o final do pedido. O pedido "State St" deve ser concluído. Se você não chegar a tempo, entre em contato com o suporte: 0101”.
- **Resultado real:** Nenhuma notificação do app Urban Scooter foi recebida às 21:59 nem depois (verificado até 22:02). Na gaveta de notificações aparece apenas a notificação do sistema “Serial console enabled”.

### KAN-105 — POST /api/v1/orders aceita deliveryDate da semana passada e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Alta
- **Caso de teste:** Tarefa 3, T-32
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro, pois só é possível pedir a scooter a partir do dia seguinte. O pedido não deveria ser criado.
- **Resultado real:** Código de resposta 201 Created e o pedido é criado (corpo da resposta com o número de rastreio "track"). O pedido aparece na lista de pedidos disponíveis para os entregadores.

### KAN-106 — POST /api/v1/orders aceita deliveryDate de ontem e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Alta
- **Caso de teste:** Tarefa 3, T-33
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro, pois só é possível pedir a scooter a partir do dia seguinte. O pedido não deveria ser criado.
- **Resultado real:** Código de resposta 201 Created e o pedido é criado (corpo da resposta com o número de rastreio "track"). O pedido aparece na lista de pedidos disponíveis para os entregadores.

### KAN-107 — POST /api/v1/orders aceita deliveryDate de hoje e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Alta
- **Caso de teste:** Tarefa 3, T-34
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro, pois só é possível pedir a scooter a partir do dia seguinte. O pedido não deveria ser criado.
- **Resultado real:** Código de resposta 201 Created e o pedido é criado (corpo da resposta com o número de rastreio "track"). O pedido aparece na lista de pedidos disponíveis para os entregadores.

### KAN-108 — POST /api/v1/courier aceita login com 1 letra e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Média
- **Caso de teste:** Tarefa 3, T-4
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro. O entregador não deveria ser criado, pois o login deve ter somente letras latinas, de 2 a 10 caracteres.
- **Resultado real:** Código de resposta 201 Created com o corpo {"ok": true} . O entregador é criado no banco de dados.

### KAN-109 — POST /api/v1/courier aceita login com 11 letras e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Média
- **Caso de teste:** Tarefa 3, T-5
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro. O entregador não deveria ser criado, pois o login deve ter somente letras latinas, de 2 a 10 caracteres.
- **Resultado real:** Código de resposta 201 Created com o corpo {"ok": true} . O entregador é criado no banco de dados.

### KAN-110 — POST /api/v1/courier aceita login com números e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Média
- **Caso de teste:** Tarefa 3, T-6
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro. O entregador não deveria ser criado, pois o login deve ter somente letras latinas, de 2 a 10 caracteres.
- **Resultado real:** Código de resposta 201 Created com o corpo {"ok": true} . O entregador é criado no banco de dados.

### KAN-111 — POST /api/v1/courier aceita login com letras cirílicas e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Média
- **Caso de teste:** Tarefa 3, T-7
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro. O entregador não deveria ser criado, pois o login deve ter somente letras latinas, de 2 a 10 caracteres.
- **Resultado real:** Código de resposta 201 Created com o corpo {"ok": true} . O entregador é criado no banco de dados.

### KAN-112 — POST /api/v1/courier aceita login com caractere especial e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Média
- **Caso de teste:** Tarefa 3, T-8
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro. O entregador não deveria ser criado, pois o login deve ter somente letras latinas, de 2 a 10 caracteres.
- **Resultado real:** Código de resposta 201 Created com o corpo {"ok": true} . O entregador é criado no banco de dados.

### KAN-113 — POST /api/v1/courier aceita firstName com 1 letra e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Média
- **Caso de teste:** Tarefa 3, T-14
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro. O entregador não deveria ser criado, pois o firstName deve ter somente letras latinas, de 2 a 10 caracteres.
- **Resultado real:** Código de resposta 201 Created com o corpo {"ok": true} . O entregador é criado no banco de dados.

### KAN-114 — POST /api/v1/courier aceita firstName com 11 letras e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Média
- **Caso de teste:** Tarefa 3, T-15
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro. O entregador não deveria ser criado, pois o firstName deve ter somente letras latinas, de 2 a 10 caracteres.
- **Resultado real:** Código de resposta 201 Created com o corpo {"ok": true} . O entregador é criado no banco de dados.

### KAN-115 — POST /api/v1/courier aceita firstName com número e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Média
- **Caso de teste:** Tarefa 3, T-16
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro. O entregador não deveria ser criado, pois o firstName deve ter somente letras latinas, de 2 a 10 caracteres.
- **Resultado real:** Código de resposta 201 Created com o corpo {"ok": true} . O entregador é criado no banco de dados.

### KAN-116 — POST /api/v1/courier aceita firstName com letras cirílicas e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Média
- **Caso de teste:** Tarefa 3, T-17
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro. O entregador não deveria ser criado, pois o firstName deve ter somente letras latinas, de 2 a 10 caracteres.
- **Resultado real:** Código de resposta 201 Created com o corpo {"ok": true} . O entregador é criado no banco de dados.

### KAN-117 — POST /api/v1/courier aceita firstName com caractere especial e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Média
- **Caso de teste:** Tarefa 3, T-18
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro. O entregador não deveria ser criado, pois o firstName deve ter somente letras latinas, de 2 a 10 caracteres.
- **Resultado real:** Código de resposta 201 Created com o corpo {"ok": true} . O entregador é criado no banco de dados.

### KAN-118 — POST /api/v1/courier aceita firstName vazio e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Média
- **Caso de teste:** Tarefa 3, T-19
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro. O entregador não deveria ser criado, pois o firstName é um campo obrigatório e deve ter de 2 a 10 letras latinas.
- **Resultado real:** Código de resposta 201 Created com o corpo {"ok": true} . O entregador é criado no banco de dados.

### KAN-119 — POST /api/v1/courier aceita requisição sem o campo firstName e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Média
- **Caso de teste:** Tarefa 3, T-20
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro. O entregador não deveria ser criado, pois o firstName é um campo obrigatório para criar o entregador.
- **Resultado real:** Código de resposta 201 Created com o corpo {"ok": true} . O entregador é criado no banco de dados.

### KAN-120 — POST /api/v1/courier aceita senha com 3 dígitos e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Média
- **Caso de teste:** Tarefa 3, T-21
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro. O entregador não deveria ser criado, pois a senha deve ter somente números inteiros, exatamente 4 caracteres.
- **Resultado real:** Código de resposta 201 Created com o corpo {"ok": true} . O entregador é criado no banco de dados.

### KAN-121 — POST /api/v1/courier aceita senha com 5 dígitos e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Média
- **Caso de teste:** Tarefa 3, T-22
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro. O entregador não deveria ser criado, pois a senha deve ter somente números inteiros, exatamente 4 caracteres.
- **Resultado real:** Código de resposta 201 Created com o corpo {"ok": true} . O entregador é criado no banco de dados.

### KAN-122 — POST /api/v1/courier aceita senha com letras e retorna 201 Created ao invés de 400 Bad Request

- **Prioridade:** Média
- **Caso de teste:** Tarefa 3, T-23
- **Resultado esperado:** Código de resposta 400 Bad Request e mensagem de erro. O entregador não deveria ser criado, pois a senha deve ter somente números inteiros, exatamente 4 caracteres.
- **Resultado real:** Código de resposta 201 Created com o corpo {"ok": true} . O entregador é criado no banco de dados.

### KAN-123 — DELETE /api/v1/courier/:id com id não numérico ("abc") retorna 500 Internal Server Error ao invés de 400 Bad Request

- **Prioridade:** Alta
- **Caso de teste:** Tarefa 3, T-29
- **Resultado esperado:** Código de resposta 400 Bad Request (erro do cliente) com mensagem de erro, informando que o id é inválido. O servidor não deveria falhar.
- **Resultado real:** Código de resposta 500 Internal Server Error com o corpo {"code": 500, "message": "invalid input syntax for integer: \"abc\""} . O erro interno do banco de dados é exposto na resposta.

### KAN-124 — DELETE /api/v1/courier/:id exclui o entregador, mas não exclui os pedidos vinculados a ele na tabela Orders

- **Prioridade:** Alta
- **Caso de teste:** Tarefa 3, T-31
- **Resultado esperado:** O entregador é excluído (200 OK, {"ok": true} ) e, conforme o requisito, os pedidos vinculados a ele na tabela Orders também são apagados. O GET pelo track deveria retornar 404 Not Found.
- **Resultado real:** O entregador é excluído (200 OK, {"ok": true} ), mas o pedido vinculado continua no banco de dados: o GET /api/v1/orders/track?t=346363 retorna 200 OK com o pedido id 4 e "inDelivery": true, ligado a um entregador que não existe mais.
