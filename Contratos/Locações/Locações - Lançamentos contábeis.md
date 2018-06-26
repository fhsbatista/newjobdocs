# SEGUROS – LANÇAMENTOS CONTÁBEIS DE CADASTRO DO CONTRATO
Este documento tem como objetivo descrever quais são os lançamentos contábeis que o New Job precisa gerar quando for cadastrado um contrato de locações (Contratos  / Locações).

## Descrição geral dos lançamentos
Os lançamentos gerados por estre contrato são simples. Basicamente, é gerado um lançamento contábil para cada parcela do contrato.
E o lançamento pode ser gerado de duas formas, dependendo do tipo do contrato, que pode ser de "Locador" e de "Locatário".

### Locador
 - Data:  Primeiro dia do mês de vencimento da parcela (Ex: Vencimento = 10/05 -> Lançametno será na data de 01/05)
 - Valor: Valor da parcela
 - Débito: Conta contábil vinculada no "Locatário" que foi colocado no contrato.
 - Crédito: Conta contábil de "receita" informada no cadastro do contrato.

### Locatário
 - Data:  Primeiro dia do mês de vencimento da parcela (Ex: Vencimento = 10/05 -> Lançametno será na data de 01/05)
 - Valor: Valor da parcela
 - Débito: Conta contábil de "despesa" informada no cadastro do contrato.
 - Crédito: Conta contábil vinculado ao "Locador" que foi colocado no cadastro.

## Integrações contábeis a serem feitas quando o contrato receber o "Aditivo"

Neste caso, o sistema deverá excluir todos os lançamentos contábeis referentes às parcelas que estão em ABERTO, e que tem data de vencimento POSTERIOR à data de emissão do ativido.

E então, deverão ser criados novos lançamentos contábeis que serão referentes aos novos títulos criados pelo aditivo, seguindo as mesmas regras informadas no tópico anterior.

## Integrações contábeis a serem feitas quando o contrato receber a "Rescisão"

Neste caso, o sistema deverá excluir todos os lançamentos contábeis referentes às parcelas que estão em ABERTO, e que tem data de vencimento POSTERIOR à data de emissão do ativido.

É a mesma coisa que é feita com o "Aditivo", com a diferença de que não serão criados novos lançamentos contábeis neste caso.
 
