
Quando este contrato ser� usado:
 - Sempre que o cliente tiver uma ap�lice de seguro, ele pode fazer o cadastro dela, com o objetivo de ter no New Job dados sobre os seguros de forma geral. Tirando relat�rios de bens que est�o com seguro vencido, ou bens que n�o tem seguro algum, vencimento de parcelas, ap�lices que est�o chegando no fim da vig�ncia etc.


Pr�-Requisitos:

 - Para fazer o cadastro de uma ap�lice, � necess�rio que o usu�rio insira um "bem" no contrato. Este "bem" � um cadastro feito em Ativos / Bens M�veis ou Bens Im�veis.

 - � necess�rio tamb�m, que os "subgrupos" tenham uma conta de despesa vinculada. Este cadastro de "subgrupo" ficam em Ativos / Bens M�veis ou Bens Im�veis / Subgrupos. Eu digo "bens m�veis ou bens im�veis", por que o contrato de seguro pode abranger estes dois cadastros.

 - Tamb�m � necess�rio fazer a parametriza��o do m�dulo de seguros (isto � feito em "Contratos / Seguros / Parametriza��es Gerais"). 
   As parametriza��es a serem feitas s�o: selecionar tipo de pagamento, conta caixa e centro de custo padr�o (isto pode variar de cliente para cliente), e informar tamb�m a conta cont�bil que ser� usada para o lan�amento de apropria��es, isto � informado no campo "Cta.Cont�bil Seguros a Apropriar"


Cadastrando o contrato:

 - O contrato � cadastrado em Contratos / Seguros / Cadastro do contrato
 

Dados a inserir no cadastro:

 Primeira p�gina:
  - N�mero de protoc�lo -> Este campo pode ser usado pelo usu�rio quando ele precisa fazer o pagamento adiantado � seguradora, por�m ainda n�o tem a ap�lice em m�os. Neste caso, o usu�rio pode cadastrar a ap�lice mesmo assim, preenchendo o n�mero de protoc�lo que ele tem em m�os neste campo "N�mero de proc�lo". E preencher o restante dos dados.
    *Neste caso, o usu�rio s� consegue fazer o cadastro do contrato caso ele tenha realmente os dados como os bens que est�o segurados, as coberturas, o valor das coberturas etc. Caso ele n�o tenha esses dados, ele precisar� lan�ar um "adiantamento" no financeiro para conseguir pagar a seguradora. E ent�o quando ele tiver a ap�lice em m�os, ele faz o cadastro no New Job.

 - N�mero da Ap�lice -> N�mero de identifica��o do contrato de seguro (ap�lice), normalmente na ap�lice impressa mesmo, o usu�rio n�o precisa "criar" um n�mero para isto.

  - Vr. Outros custos -> Neste campo o usu�rio dever� digitar a soma de encargos (com exce��o de IOF) que existem no contrato.

  - Vr. IOF -> O usu�rio vai digitar o valor de IOF.

 Segunda p�gina:
  - Descri�ao da cobertura: Aqui vai o nome da cobertura mesmo. *Em alguns clientes, eles podem acabar colocando uma descri��o "padr�o", e lan�ar a cobertura com o valor total de todas as coberturas do bem, e no campo de "observa��es" eles descrevem cada cobertura e o valor delas. Isto � feito por conta da grande quantidade de coberturas que existem no contrato, ent�o o pessoal acaba optando por lan�ar desta forma.

  - Tipo de Cobertura: Usar "valor" quando a seguradora j� combinou o valor m�ximo que ir� cobrir caso o cliente acione o seguro. E "percentual" deve ser usado quando o combinado � o percentual do valor do bem. (Ex: cobertura em caso de danos no bem, normalmente � combinado 100% do valor da tabela FIPE do bem por exemplo). *Serve apenas para consulta, este campo n�o � usado em nenhuma integra��o.

  - Vr. Premio: Este � o valor que o cliente est� pagando por esta cobertura.

  - Vr. Franquia: Este � o valor que o usu�rio dever� desembolsar caso ele precise acionar o seguro.

 Terceira p�gina:
  - Aqui s�o inseridas as parcelas que ser�o pagas, a inser��o � simples, pede somente valor e data de vencimento.

 Finalizando o contrato:
  - Ao finalizar o contrato, ser�o feitas as seguintes valida��es: Verificar se a soma das coberturas � igual ao valor da ap�lice, desconsiderando iof e outros custos. E Verificar se a soma das parcelas � igual ao Vr. da ap�lice (neste caso o iof e outros custos s�o considerados.

 Integra��es cont�beis:
  - Est�o descritas em um documento a parte na mesma pasta "Contratos/Seguros".
Endosso:
 - O contrato de seguro também pode ser "endossado" (o contrato é alterado por algum motivo)
 - O NewJob já tem duas funcionalidades prontas para atender este caso. Ambos estão descritos em um pdf na mesma pasta "Contratos/Seguros".
   
