# O que foi aprendido
<li> Composição de entidades  </li>
<li> Composição de serviços </li>
<li> Interfaces </li>
<li> Inversão de controle / injeção de dependência </li>

# Enunciado do exercício 
Uma empresa deseja automatizar o processamento de seus contratos. O processamento de um contrato consiste em gerar as parcelas a serem pagas para aquele contrato, com base no número de meses desejado.

A empresa utiliza um serviço de pagamento online para realizar o pagamento das parcelas. Os serviços de pagamento online tipicamente cobram um juro mensal, bem como uma taxa por pagamento. Por enquanto, o serviço contratado pela empresa é o do Paypal, que aplica juros simples de 1% a cada parcela, mais uma taxa de pagamento de 2%.

Fazer um programa para ler os dados de um contrato (número do contrato, data do contrato, e valor total do contrato). Em seguida, o programa deve ler o número de meses para parcelamento do contrato, e daí gerar os registros de parcelas a serem pagas (data e valor), sendo a primeira parcela a ser paga um mês após a data do contrato, a segunda parcela dois meses após o contrato e assim por diante. Mostrar os dados das parcelas na tela.

# Exemplo
![example](https://user-images.githubusercontent.com/90002310/194433848-9c42fbc4-83cf-4678-be50-030373a1f6d7.png)


# Cálculos 

Parcela #1: 
200 + 1% * 1 = 202 
202 + 2% = 206.04

Parcela #2: 
200 + 1% * 2 = 204 
204 + 2% = 208.08

Parcela #3: 
200 + 1% * 3 = 206 
206 + 2% = 210.12

# Diagramas

**Entidades**

![entities](https://user-images.githubusercontent.com/90002310/194433602-3ac6f574-4f38-4756-9743-237c1ec11216.png)

**Serviços**
![services](https://user-images.githubusercontent.com/90002310/194433673-b275a516-c306-49dd-988a-2440a0bfe36d.png)

