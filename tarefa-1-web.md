# Tarefa 1 — Formulário web "Para quem é a scooter"

Testes do primeiro formulário de pedido do Urban Scooter, executados no **Google Chrome** e no **Opera**, na resolução **1280x720**. Os casos foram desenhados com **partição de equivalência** e **análise de valor limite** para os campos Nome, Sobrenome, Endereço, Estação de metrô e Telefone.

**Resultado:** 52 casos — 36 aprovados e 16 reprovados, com o mesmo resultado nos dois navegadores.

| ID | Caso de teste | Classe de equivalência | Valor limite | Dado de teste | Chrome | Opera | Bug |
|---|---|---|---|---|---|---|---|
| T-1 | "Nome" com 2 caracteres (limite mínimo) é aceito | 2 até 15 caracteres (letras, espaços e traços) - Válido | 2 - limite mínimo | "Jo" | Aprovado | Aprovado | — |
| T-2 | "Nome" com 3 caracteres (mínimo + 1) é aceito | 2 até 15 caracteres (letras, espaços e traços) - Válido | 3 - mínimo + 1 | "Ana" | Aprovado | Aprovado | — |
| T-3 | "Nome" com 8 caracteres (dentro da classe) é aceito | 2 até 15 caracteres (letras, espaços e traços) - Válido | — | "Fernanda" | Aprovado | Aprovado | — |
| T-4 | "Nome" com 14 caracteres (máximo - 1) é aceito | 2 até 15 caracteres (letras, espaços e traços) - Válido | 14 - máximo - 1 | "Mariaclarasous" | Aprovado | Aprovado | — |
| T-5 | "Nome" com 15 caracteres (limite máximo) é aceito | 2 até 15 caracteres (letras, espaços e traços) - Válido | 15 - limite máximo | "Mariaclarasouza" | Aprovado | Aprovado | — |
| T-6 | "Nome" com espaço no meio é aceito | Espaço no meio - Válido | — | "Ana Luz" | Aprovado | Aprovado | — |
| T-7 | "Nome" com hífen é aceito | Um hífen - Válido | — | "Ana-Luz" | Aprovado | Aprovado | — |
| T-8 | "Nome" vazio exibe mensagem de erro | Campo vazio - Inválido | 0 - campo vazio | [] | Aprovado | Aprovado | — |
| T-9 | "Nome" com 1 caractere (abaixo do mínimo) exibe mensagem de erro | Menor que 2 caracteres - Inválido | 1 - mínimo - 1 | "J" | Aprovado | Aprovado | — |
| T-10 | "Nome" com 16 caracteres (acima do máximo) exibe mensagem de erro | Maior que 15 caracteres - Inválido | 16 - máximo + 1 | "Mariaclarasouzaa" | Aprovado | Aprovado | — |
| T-11 | "Nome" com números exibe mensagem de erro | Alfanumérico - Inválido | — | "Ana123" | Aprovado | Aprovado | — |
| T-12 | "Nome" com caracteres especiais exibe mensagem de erro | Caractere especial - Inválido | — | "Ana@#" | Aprovado | Aprovado | — |
| T-13 | "Sobrenome" com 2 caracteres (limite mínimo) é aceito | 2 até 15 caracteres (letras, espaços e traços) - Válido | 2 - limite mínimo | "Jo" | Aprovado | Aprovado | — |
| T-14 | "Sobrenome" com 3 caracteres (mínimo + 1) é aceito | 2 até 15 caracteres (letras, espaços e traços) - Válido | 3 - mínimo + 1 | "Ana" | Aprovado | Aprovado | — |
| T-15 | "Sobrenome" com 8 caracteres (dentro da classe) é aceito | 2 até 15 caracteres (letras, espaços e traços) - Válido | — | "Fernanda" | Aprovado | Aprovado | — |
| T-16 | "Sobrenome" com 14 caracteres (máximo - 1) é aceito | 2 até 15 caracteres (letras, espaços e traços) - Válido | 14 - máximo - 1 | "Mariaclarasous" | Aprovado | Aprovado | — |
| T-17 | "Sobrenome" com 15 caracteres (limite máximo) é aceito | 2 até 15 caracteres (letras, espaços e traços) - Válido | 15 - limite máximo | "Mariaclarasouza" | Aprovado | Aprovado | — |
| T-18 | "Sobrenome" com espaço no meio é aceito | Espaço no meio - Válido | — | "Ana Luz" | Aprovado | Aprovado | — |
| T-19 | "Sobrenome" com hífen é aceito | Um hífen - Válido | — | "Ana-Luz" | Aprovado | Aprovado | — |
| T-20 | "Sobrenome" vazio exibe mensagem de erro | Campo vazio - Inválido | 0 - campo vazio | [] | Aprovado | Aprovado | — |
| T-21 | "Sobrenome" com 1 caractere (abaixo do mínimo) exibe mensagem de erro | Menor que 2 caracteres - Inválido | 1 - mínimo - 1 | "J" | Aprovado | Aprovado | — |
| T-22 | "Sobrenome" com 16 caracteres (acima do máximo) exibe mensagem de erro | Maior que 15 caracteres - Inválido | 16 - máximo + 1 | "Mariaclarasouzaa" | Reprovado | Reprovado | [KAN-84](https://ingridmatos.atlassian.net/browse/KAN-84) |
| T-23 | "Sobrenome" com números exibe mensagem de erro | Alfanumérico - Inválido | — | "Ana123" | Aprovado | Aprovado | — |
| T-24 | "Sobrenome" com caracteres especiais exibe mensagem de erro | Caractere especial - Inválido | — | "Ana@#" | Aprovado | Aprovado | — |
| T-25 | "Endereço" com 5 caracteres (limite mínimo) é aceito | 5 até 50 caracteres (letras, números, espaços, traços, pontos e vírgulas) - Válido | 5 - limite mínimo | "Rua 1" | Aprovado | Aprovado | — |
| T-26 | "Endereço" com 6 caracteres (mínimo + 1) é aceito | 5 até 50 caracteres (letras, números, espaços, traços, pontos e vírgulas) - Válido | 6 - mínimo + 1 | "Rua 10" | Aprovado | Aprovado | — |
| T-27 | "Endereço" com letras, números, ponto, vírgula e traço é aceito | 5 até 50 caracteres (letras, números, espaços, traços, pontos e vírgulas) - Válido | — | "Av. Brasil-Norte, 250" | Aprovado | Aprovado | — |
| T-28 | "Endereço" com 49 caracteres (máximo - 1) é aceito | 5 até 50 caracteres (letras, números, espaços, traços, pontos e vírgulas) - Válido | 49 - máximo - 1 | "Rua Augusta, 1000, apto 12, bloco B, Centro. Lade" | Aprovado | Aprovado | — |
| T-29 | "Endereço" com 50 caracteres (limite máximo) é aceito | 5 até 50 caracteres (letras, números, espaços, traços, pontos e vírgulas) - Válido | 50 - limite máximo | "Rua Augusta, 1000, apto 12, bloco B, Centro. Ladei" | Reprovado | Reprovado | [KAN-85](https://ingridmatos.atlassian.net/browse/KAN-85) |
| T-30 | Espaços no início e no fim do "Endereço" são removidos ao tirar o foco | Espaço no início e no fim - Válido (espaços excluídos) | — | " Rua Augusta, 100 " | Aprovado | Aprovado | — |
| T-31 | "Endereço" vazio exibe mensagem de erro | Campo vazio - Inválido | 0 - campo vazio | [] | Reprovado | Reprovado | [KAN-86](https://ingridmatos.atlassian.net/browse/KAN-86) |
| T-32 | "Endereço" com 4 caracteres (abaixo do mínimo) exibe mensagem de erro | Menor que 5 caracteres - Inválido | 4 - mínimo - 1 | "Rua1" | Reprovado | Reprovado | [KAN-87](https://ingridmatos.atlassian.net/browse/KAN-87) |
| T-33 | "Endereço" com 51 caracteres (acima do máximo) exibe mensagem de erro | Maior que 50 caracteres - Inválido | 51 - máximo + 1 | "Rua Augusta, 1000, apto 12, bloco B, Centro. Ladeir" | Reprovado | Reprovado | [KAN-93](https://ingridmatos.atlassian.net/browse/KAN-93) |
| T-34 | "Endereço" com caracteres especiais exibe mensagem de erro | Caractere especial - Inválido | — | "Rua #10 @ casa" | Reprovado | Reprovado | [KAN-94](https://ingridmatos.atlassian.net/browse/KAN-94) |
| T-35 | "Endereço" com 3 caracteres depois de remover os espaços exibe mensagem de erro | Menor que 5 caracteres após excluir os espaços - Inválido | 3 - após excluir os espaços | " Rua " | Reprovado | Reprovado | [KAN-95](https://ingridmatos.atlassian.net/browse/KAN-95) |
| T-36 | Estação de metrô escolhida na lista é aceita | Estação da lista - Válido | — | Primeira estação da lista | Aprovado | Aprovado | — |
| T-37 | Digitar parte do nome filtra a lista de estações de metrô | Parte do nome de uma estação - Válido | — | 3 primeiras letras de uma estação da lista | Aprovado | Aprovado | — |
| T-38 | "Estação de metrô" vazia impede o avanço | Campo vazio - Inválido | — | [] | Aprovado | Aprovado | — |
| T-39 | Texto que não é estação da lista não é aceito em "Estação de metrô" | Texto fora da lista - Inválido | — | "Estacao Inexistente" | Aprovado | Aprovado | — |
| T-40 | "Telefone" com 10 caracteres (limite mínimo) é aceito | 10 até 12 caracteres (números e "+") - Válido | 10 - limite mínimo | "+123456789" | Reprovado | Reprovado | [KAN-88](https://ingridmatos.atlassian.net/browse/KAN-88) |
| T-41 | "Telefone" com 11 caracteres (mínimo + 1 / máximo - 1) é aceito | 10 até 12 caracteres (números e "+") - Válido | 11 - mínimo + 1 / máximo - 1 | "+1234567890" | Aprovado | Aprovado | — |
| T-42 | "Telefone" com 12 caracteres (limite máximo) é aceito | 10 até 12 caracteres (números e "+") - Válido | 12 - limite máximo | "+12345678901" | Aprovado | Aprovado | — |
| T-43 | "Telefone" vazio exibe mensagem de erro | Campo vazio - Inválido | 0 - campo vazio | [] | Reprovado | Reprovado | [KAN-96](https://ingridmatos.atlassian.net/browse/KAN-96) |
| T-44 | "Telefone" com 9 caracteres (abaixo do mínimo) exibe mensagem de erro | Menor que 10 caracteres - Inválido | 9 - mínimo - 1 | "+12345678" | Reprovado | Reprovado | [KAN-91](https://ingridmatos.atlassian.net/browse/KAN-91) |
| T-45 | "Telefone" com 13 caracteres (acima do máximo) exibe mensagem de erro | Maior que 12 caracteres - Inválido | 13 - máximo + 1 | "+123456789012" | Reprovado | Reprovado | [KAN-89](https://ingridmatos.atlassian.net/browse/KAN-89) |
| T-46 | "Telefone" sem o sinal "+" exibe mensagem de erro | Sem o sinal "+" - Inválido | — | "12345678901" | Reprovado | Reprovado | [KAN-90](https://ingridmatos.atlassian.net/browse/KAN-90) |
| T-47 | "Telefone" com letras exibe mensagem de erro | Alfanumérico - Inválido | — | "+12345abcde" | Reprovado | Reprovado | [KAN-97](https://ingridmatos.atlassian.net/browse/KAN-97) |
| T-48 | "Telefone" com espaço e traço exibe mensagem de erro | Espaço e traço - Inválido | — | "+12 345-6789" | Reprovado | Reprovado | [KAN-98](https://ingridmatos.atlassian.net/browse/KAN-98) |
| T-49 | "Telefone" com parênteses exibe mensagem de erro | Caractere especial - Inválido | — | "+(12)345678" | Reprovado | Reprovado | [KAN-99](https://ingridmatos.atlassian.net/browse/KAN-99) |
| T-50 | Formulário com todos os campos válidos abre o formulário "Locação" | Todos os campos válidos - Válido | — | Nome "Ana", Sobrenome "Silva", Endereço "Rua Augusta, 100", Estação de metrô: primeira da lista, Telefone "+1234567890" | Aprovado | Aprovado | — |
| T-51 | Formulário vazio mostra erro em todos os campos e não avança | Todos os campos vazios - Inválido | — | [] | Reprovado | Reprovado | [KAN-92](https://ingridmatos.atlassian.net/browse/KAN-92) |
| T-52 | Dados preenchidos continuam no formulário ao voltar de "Locação" | Todos os campos válidos - Válido | — | Nome "Ana", Sobrenome "Silva", Endereço "Rua Augusta, 100", Estação de metrô: primeira da lista, Telefone "+1234567890" | Aprovado | Aprovado | — |
