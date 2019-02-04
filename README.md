# Aprendendo JAVA

###### Utilizar como material base: https://www.caelum.com.br/apostila-java-orientacao-objetos
###### Pré-requisitos:
- Os exercícios devem ser resolvidos na IDE IntelliJ, realizando um commit quando o projeto for configurado.
- O projeto criado deve utilizar o padrão de projeto Maven.
- Os exercícios devem ser resolvidados através de funções main.
- Para cada exercício será necessário um commit seguindo o padrão "[login][número do exercício] Descrição".

### Exercícios 
##### Variáveis primitivas e Controle de fluxo
1. Em uma empresa trabalham três funcionários que possuem "nome" (String), "idade" (int), "salário" (double) e "sexo" (String). 
Desejo que quando executar o programa ele exiba apenas os funcionários maiores que 18 anos e salário maiores que R$ 1000,50.
2. Desejo que quando executar o programa ele exiba apenas os números ímpares ou apenas o números pares de 1 a 100, o usuário informa o que quer exibir através de uma variável "true" ou "false".
3. Desejo que quando executar o programa ele exiba a seguinte pirâmide, o usúario informa a quantidade de linhas.
01  
02 02  
03 03 03  
04 04 04 04  
05 05 05 05 05  
06 06 06 06 06 06  
07 07 07 07 07 07 07  
08 08 08 08 08 08 08 08  
09 09 09 09 09 09 09 09 09  
10 10 10 10 10 10 10 10 10 10  
... 
4. Desejo que quando executar o programa ele exiba taboada do 1 ao 10.
1x1=1
1x2=2
1x3=3
1x4=4
1x5=5
1x6=6
1x7=7
1x8=8
1x9=9
1x10=10
2x1=2
2x2=4
...
5. Desejo que quando executar o programa ele exiba uma matriz 5 x 5 com valores aleatórios. Exemplo:
Matriz: 
4 5 3 2 4 
6 8 6 5 4 
1 2 4 5 6 
6 5 4 3 2 
5 3 1 8 6 

6. Desejo que quando executar o programa ele exiba uma matriz 5 x 5 com valores aleatórios sendo eles somente números pares. Exemplo:
Matriz: 
4 6 2 2 4 
6 8 6 2 4 
2 2 4 2 6 
6 4 4 2 2 
2 2 2 8 6 

7. Desejo que quando executar o programa ele exiba uma matriz 5 x 5 comos seus respectivos indices. Exemplo:
Matriz: 
00 01 02 03 04 
10 11 12 13 14 
20 21 22 23 24 
30 31 32 33 34 
40 41 42 43 44 

8. Uma escola deseja um sistema de avaliação de notas. Sendo que uma nota de 1 a 10 retorna "vermelho", de 11 a 20 retorna "azul", de 21 a 50 retorna "amarelo", qualquer outra retorna "branco".
Desejo que quando executar o programa ele exiba a cor correspondente da nota informada pelo usuário.

9. Dado que temos um array de notas, aplicar a mesma regra do exercício 8. 
Desejo que quando executar o programa ele exiba as cores correspondentes do array informado pelo usuário. Exemplo:
Array:
4 13 54 1000
Exibir:
vermelho azul branco branco

##### Orientação a objetos básica
10. Uma empresa que trabalha com vendas de passagens aéreas através de pontos de fidelidades deseja um sistema que possibilita usuários comprarem passagens com seus pontos. 
- A empresa possui a ação de compra que débita os pontos do cliente.
- Existem duas passagens cadastradas, a passagem de origem VCP e destino LAS que custa 3000 pontos e a passagem de origem ROM e destino LAS que custa 10000 pontos.
- Existem dois clientes cadastrados, o cliente Lucas que possui 20000 pontos e o cliente Osvaldo que possui 10000 pontos.
- As transações de quem vai comprar o que será informada pelo usuário do sistema. 
- Validar quando o cliente não têm saldo.
- Validar quando a passagem não existe.

Dica: https://alvinalexander.com/java/edu/pj/pj010005

Exemplo:
Qual é o identificador do cliente?
Resposta: Lucas

Qual a origem da passagem que deseja comprar?
Resposta: VCP

Qual o destino da passagem que deseja comprar?
Resposta: LAS

Passagem comprada com sucesso, você possui agora 17000 pontos!

##### Exceções e controle de erros
11. Criar uma calculadora com as opções de multiplicação, divisão, subtração e soma, as informações são recebidas pelo usuário. Tratar que quando ocorrer um erro no cálculo, uma mensagem "Ocorreu um erro!" deve ser exibida.

Dica: https://www.w3schools.com/java/java_try_catch.asp
- Exemplo:
Digite: 1 + 1
Resposta: 2
- Exemplo de erro:
Digite: + + 1
Resposta: Ocorreu um erro!

##### Modificadores de acesso e atributos de classe
12. Crie uma classe denominada Elevador para armazenar as informações de um elevador dentro de um prédio.
A classe deve armazenar o andar atual (térreo = 0), total de andares no prédio (desconsiderando o térreo), capacidade do elevador e quantas pessoas estão presentes nele.
A classe deve também disponibilizar os seguintes métodos:

- Construtor: Deve receber como parâmetros a capacidade do elevador e o total de andares no prédio (os elevadores sempre começam no térreo e vazio);
- Entra: para acrescentar uma pessoa no elevador (só deve acrescentar se ainda houver espaço);
- Sai: para remover uma pessoa do elevador (só deve remover se houver alguém
dentro dele);
- Sobe: para subir um andar (não deve subir se já estiver no último andar);
- Desce : para descer um andar (não deve descer se já estiver no térreo);
Encapsular todos os atributos da classe (criar os métodos set e get).

##### Interfaces, Herança, reescrita e polimorfismo
13. Crie um sistema que controle os tipos de veiculos. O sistema vai abranger diversos tipos de carros, caminhões, motos ambos com suas funções.
   

- Implemente uma classe Proprietário 
Declare os seguintes atributos na classe: 
   - Nome
   - CPF
   - RG
   - Data de Nascimento
   - Rua
   - Bairro
   - Cidade
   - Estado 
   - Cep
   - Complemento
- Faça o encapsulamento dos atributos da classe Proprietário
Os atributos nome, cpf e rg são obrigatórios (crie um construtor com esses parâmetros)
- Implemente uma classe Carro
Declare os seguintes atributos na classe:
   - Modelo
   - Cor
   - Ano
   - Marca
   - Chassi
   - Proprietário
   - Velocidade máxima
   - Velocidade atual
   - Nr de portas
   - tem teto solar?
   - Nr Marchas
   - tem cambio automatico?
   - Volume de combustível
- Faça o encapsulamento da classe Carro e seus atributos
- Implemente o método acelera que aumenta a velocidade de 1 em 1 km/h
- Implemente o método freia que para o carro – Velocidade = 0 km/h
- Implemete o método troca marcha
- Implemente o método reduz a marcha;
- Altere a classe Proprietário para que o atributo Endereço vire uma classe;
- Encapsule os atributos da classe Endereço;
O endereço do proprietário não pode ser vazio (altere no construtor para receber o endereço);
- Todo veículo tem um proprietário obrigatoriamente (implemente um construtor de veículo passando o proprietário como parâmetro);
- A marcha ré nao pode ser engatada se o a velocidade for superior a 0 KM/h;
- Implemente um método que calcule a autonomia de viagem do veículo com base no consumo médio passado como parâmetro;
- Implemente um método para exibir o volume de combustível 
- Transforme o atributo Marca de um carro em uma classe Marca com nome, nrDeModelos, ano de lançamento e código identificador
- Crie a classe abstrata Veiculo que a classe Carro pode extender, extraindo os atributos que são comuns a todos os tipo de veiculos, podendo ter Caminhao, Moto e entre outros.
- Instancie um objeto de cada classe Veiculo criada e relacione todas as outras.
- Exiba todos os atributos do Veiculo instanciado.

##### APIs

14. Criar as seguintes APIs, utilizando como base de dados HashMap: 

Dica: https://start.spring.io/
- Cadastrar veiculo (POST).
- Listar veiculos (GET).
- Executar ações dos veiculos (POST), acelerar, freiar, troca marcha, reduz marcha.

##### Micro serviço

15. Criar um serviço que lista as informações da seguinte API: http://www.mocky.io/v2/5c583ae02f0000070f856d91
Considerar somente animais que nasceram depois de 2010.
