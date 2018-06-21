## SEGUROS – LANÇAMENTOS CONTÁBEIS
Este documento tem como objetivo descrever quais são os lançamentos contábeis que o New Job precisa gerar quando for cadastrado um contrato de seguros (Contratos  / Seguros).

### Lançamentos referente a “apropriação do seguro”, para cada bem inserido no contrato
- Data:	Data de emissão do contrato
- Débito:	Conta parametrizada como “Cta.Contábil Seguros a Apropriar” (Contratos / Seguros / Parâmetros Gerais)
 - Crédito:	Conta contábil vinculada ao fornecedor usado no contrato de seguro
 - Valor:	Valor total dos prêmios do bem (lembrando, que é um lançamento para cada diferente bem inserido na apólice)
 

### Lançamentos de despesa do seguro:
Obs: Será gerado um lançamento contábil para cada bem dentro de cada mês de vigência do contrato. Isto é assim pois a despesa precisa ser “apropriada” conforme a vigência do contrato, e a conta contábil de despesa pode variar de acordo com o “subgrupo” do bem. Sendo assim, é sempre gerado um lançamento para cada bem inserido dentro de cada mês de vigência.
- Data:	Último dia do mês referente ao lançamento contábil. (Lembrando que é gerado um lançamento para cada mês de vigência do contrato, então a data vai ser o última deste mês)
 - Débito:	Conta parametrizada como “Despesa com seguros” no cadastro de “subgrupo” que está vinculado ao bem utilizado no cadastro do contrato de seguro.
 - Crédito:	Conta parametrizada como “Cta. Contábil Seguros a Apropriar” (Contratos / Seguros / Parâmetros Gerais).
- Valor:	Soma do total de prêmios inseridos para o bem em questão, dividido pela quantidade de meses de vigência do contrato.
 

### Lançamentos contábeis de “IOF” e “Outros custos”
Na primeira página do cadastro do contrato, o usuário tem a opção de informar um valor de custos com IOF ou “outros custos”. Estes dois valores precisam também chegar até a contabilidade, conforme os lançamentos abaixo.

 - Data:	Data de emissão do contrato
 - Débito:	Conta parametrizada como “Cta.Contábil Desp.IOF Empréstimos” ou “Cta.Contábil Desp.TAXAS Empréstimos” nas parametrizações do contrato de seguro.
 - Crédito:	Conta contábil vinculada ao fornecedor usado no contrato de seguro
 - Valor:	Valor de IOF ou Outros custos

#### Observações:
1. O lançamento contábil para iof e para outros custos é basicamente o mesmo, só muda a conta contábil que será usada como débito.
2. As contas que serão usadsa como "Débito" são as mesmas contas que o contrato de Empréstimo utiliza. Por isto o termo "empréstimo" está sendo mencionado no nome das contas acima.





