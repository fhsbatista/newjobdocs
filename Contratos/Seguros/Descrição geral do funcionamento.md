
Quando este contrato será usado:
 - Sempre que o cliente tiver uma apólice de seguro, ele pode fazer o cadastro dela, com o objetivo de ter no New Job dados sobre os seguros de forma geral. Tirando relatários de bens que estão com seguro vencido, ou bens que não tem seguro algum, vencimento de parcelas, apólices que estão chegando no fim da vigência etc.


Pré-Requisitos:

 - Para fazer o cadastro de uma apólice, é necessário que o usuário insira um "bem" no contrato. Este "bem" é um cadastro feito em Ativos / Bens Móveis ou Bens Imóveis.

 - É necessário também, que os "subgrupos" tenham uma conta de despesa vinculada. Este cadastro de "subgrupo" ficam em Ativos / Bens Móveis ou Bens Imóveis / Subgrupos. Eu digo "bens móveis ou bens imóveis", por que o contrato de seguro pode abranger estes dois cadastros.

 - Tambem é necessário fazer a parametrização do módulo de seguros (isto é feito em "Contratos / Seguros / Parametrizações Gerais"). 
   As parametrizações a serem feitas são: selecionar tipo de pagamento, conta caixa e centro de custo padrão (isto pode variar de cliente para cliente), e informar também a conta contábil que será usada para o lançamento de apropriações, isto é informado no campo "Cta.Contábil Seguros a Apropriar"


Cadastrando o contrato:

 - O contrato é cadastrado em Contratos / Seguros / Cadastro do contrato
 

Dados a inserir no cadastro:

 Primeira página:
  - Número de protocólo -> Este campo pode ser usado pelo usuário quando ele precisa fazer o pagamento adiantado à seguradora, porém ainda não tem a apólice em mãos. Neste caso, o usuário pode cadastrar a apólice mesmo assim, preenchendo o número de protocólo que ele tem em mãos neste campo "Número de protocólo". E preencher o restante dos dados.
    *Neste caso, o usuário só consegue fazer o cadastro do contrato caso ele tenha realmente os dados como os bens que estão segurados, as coberturas, o valor das coberturas etc. Caso ele não tenha esses dados, ele precisará lançar um "adiantamento" no financeiro para conseguir pagar a seguradora. E então quando ele tiver a apólice em mãos, ele faz o cadastro no New Job.

 - Número da apólice -> Número de identificação do contrato de seguro (apólice), normalmente na apólice impressa mesmo, o usuário não precisa "criar" um Número para isto.

  - Vr. Outros custos -> Neste campo o usuário deverá digitar a soma de encargos (com exceção de IOF) que existem no contrato.

  - Vr. IOF -> O usuário vai digitar o valor de IOF.

 Segunda página:
  - Descrição da cobertura: Aqui vai o nome da cobertura mesmo. *Em alguns clientes, eles podem acabar colocando uma descrição "padrão", e lançar a cobertura com o valor total de todas as coberturas do bem, e no campo de "observações" eles descrevem cada cobertura e o valor delas. Isto é feito por conta da grande quantidade de coberturas que existem no contrato, então o pessoal acaba optando por lançar desta forma.

  - Tipo de Cobertura: Usar "valor" quando a seguradora já combinou o valor máximo que irá cobrir caso o cliente acione o seguro. E "percentual" deve ser usado quando o combinado é o percentual do valor do bem. (Ex: cobertura em caso de danos no bem, normalmente é combinado 100% do valor da tabela FIPE do bem por exemplo). *Serve apenas para consulta, este campo não é usado em nenhuma integração.

  - Vr. Premio: Este é o valor que o cliente está pagando por esta cobertura.

  - Vr. Franquia: Este é o valor que o usuário deverá desembolsar caso ele precise acionar o seguro.

 Terceira página:
  - Aqui são inseridas as parcelas que serão pagas, a inserção é simples, pede somente valor e data de vencimento.

 Finalizando o contrato:
  - Ao finalizar o contrato, serão feitas as seguintes validações: Verificar se a soma das coberturas é igual ao valor da apólice, desconsiderando iof e outros custos. E Verificar se a soma das parcelas é igual ao Vr. da apólice (neste caso o iof e outros custos são considerados.

 Integrações contábeis:
  - Estão descritas em um documento a parte na mesma pasta "Contratos/Seguros".
Endosso:
 - O contrato de seguro também pode ser "endossado" (o contrato é alterado por algum motivo)
 - O NewJob já tem duas funcionalidades prontas para atender este caso. Ambos estão descritos em um pdf na mesma pasta "Contratos/Seguros".
   
