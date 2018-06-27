# Confirmação de cheques - Lançamentos contábeis

Aqui neste documento serão descritos todos os lançamentos contábeis que devem ser gerados quando a confirmação de um cheque for feita.

 - A confirmação de um cheque deve gerar um único lançamento contábil
 - Neste caso, não é necesário se preocupar se existe mútuo ou não, pois nunca haverá um caso de mútuo. Já que não tem como um cheque ser de uma conta corrente diferente.
- É importante lembrar que a confirmação do cheque pode ter que diferenciar o cheque que foi gerado a partir de uma baixa em lote, e o cheque que foi gerado a partir de baixa comum ou baixa parcial.
- Os atributos do lançamento contábil são os mesmos nos dois casos, porém irei deixar separado na tentiva de facilitar o entendimento.

## Confirmação de cheque gerado pela baixa em lote
Obs: Neste caso, o cheque está vinculado a um título em aberto no contas a pagar. Quando a confirmação é feita, este título é baixado.
Sendo assim, é importante ter certeza de que **NÃO** sejam gerados dois lançamentos. Pois a baixa de um título do contas a pagar, por padrão, já faz um lançamento contábil também.



As regras do lançamentos são as abaixo:

 - Débito: Conta contábil vinculada ao FORNECEDOR da conta corrente 
 - Crédito: Conta contábil vinculada à conta corrente.  
 - Valor: Valor do cheque
 - Empresa: Empresa da conta corrente
 - Data: Data de CONFIRMAÇÃO (informada ao confirmar o cheque)
 - Histórico: "Confirmação de cheque"

## Confirmação de cheque gerado por Baixa Comum ou Baixa Parcial
Obs: Esta confirmação não envolve nenhuma integração com um título aberto do contas a pagar. Pois o que gerou o cheque já foi a ação de fazer a baixa de um título.

As regras do lançamentos são as abaixo:

 - Débito: Conta contábil vinculada ao FORNECEDOR da conta corrente 
 - Crédito: Conta contábil vinculada à conta corrente.  
 - Valor: Valor do cheque
 - Empresa: Empresa da conta corrente
 - Data: Data de CONFIRMAÇÃO (informada ao confirmar o cheque)
 - Histórico: "Confirmação de cheque"

 
 

 