# Orientações para Implantação do New Job
Depois de várias implantações realizadas, é sugerido que a implantação siga os passos abaixo para fazer uma implantação de forma mais organizada. E claro, sempre que seja entendido um passo abaixo como desnecessário, alterar ou incluir um novo, é interessante que este documento seja atualizado para que outras pessoas possam utilizar.


**Cadastro da base de dados do cliente**
 - O cadastro da base de dados é feito pela própria AdministreBem (Amarildo e Priscila)
 - Para prosseguir, entrar em contato com eles, e passa informações do cliente como Razão Social, CNPJ, Endereço etc. Estas informações são meramente para consulta, então pode ser colocado o nome do "grupo" do cliente por exemplo, como "Grupo FM Agrícola", "Grupo Sarto" etc. Quase sempre é feito desta forma pois o cliente possui várias empresas.

**Cadastro de empresas**

O NewJob é um sistema "multi-empresa", ou seja, ele pode ser utilizado com informações de mais de uma empresa. Para que isto funcione corretamente, deve-se seguir os passos abaixo:

- Este é o primeiro passo na implantação. É importante então reunir já levantar com o cliente quais são as empresas que devem ser cadastradas no New Job. 
- O cadastro de empresa pode ser feito pelo caminho: "Perfil do usuário" (menu superior) / Empresas do Grupo. Obs: "perfil do usuário" é um botão com um ícone laranja e o desenho de uma pessoa. ![Perfil do usuário](imgs/perfilusuario.PNG)
- Feito isto, clique no botão "Incluir" para preencher o formulário de cadastro.
- As informações a serem preenchidas, são de acordo com o que o cliente passar, e são usadas somente para fins de visualização da empresa.
- **Atenção:** As contas contábeis de mútuo são informadas nos dois últims campos. Após o plano de contas ser importado, é imprescendível que estas contas sejam informadas. O cliente não deve utilizar nenhuma funcionalidade caso estas contas não tenham sido informadas.
- As contas contábeis de mútuo são OBRIGATÓRIAS em todas as empresas.

**Cadastro de plano de contas**

O plano de contas consiste de todas as contas contábeis do cliente. Este plano de contas é único no sistema, e vale para todas as empresas.

Este deve cadastrado deve ser implantado já logo após o cadastro das empresas, pois é um requisito primordial para o funcionamento do New Job.

No geral, o cadastro da conta contábil é feito individualmente conforme o dia a dia pede. Porém, na implantação o ideal é fazer a importação das contas contábeis que serão necessárias por conta da quantidade.

 - Para fazer a importação do plano de contas, pode-se utilizar de um webservice que o NewJob fornece. Para mais informações, consultar o documento **newjobdocs/APIs para importações/Informações gerais**
 - O plano de contas deve ser antes definido pela equipe de contabilidade. É importante definir bem quais serão as contas contábeis utilizadas, pois uma vez cadastrada, não é possível excluí-la, somente desativá-la.
 - Para alguns nichos de empresas, podemos utilizar já alguns modelos prontos de plano de contas, que se aplicam neste nicho. Estes modelos estão já salvos para serem usados na pasta **newjobdocs/Implantação/1 - Primeiros passos/Modelos de Plano de contas** Obs: Este modelo precisa ser formatado em json para ser importado.





