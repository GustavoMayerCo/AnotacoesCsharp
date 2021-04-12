# House_p-_work
Coding tester


        Curso c# - Udemy 
* IDENTAÇÃO AUTOMÁTICA : CRTL + K + D 
(ajeitar a legibilidade do seu código, clean code) arquitetura 


- Restrições para nomes de variaveis : 
- nao pode começar com numero: use uma letra ou   '_'    =  int _5minutos
- nao pode usar acento 
-nao pode ter espaço em branco = int salario do funcionario ( ta errado )    			nesse caso, usar SalarioDoFuncionario ( certo)  
________________________________________________________________

- Convenções  (Clean Code/Organization) 
- Camel case : lastName
- Pascal case : LastName
- Padrão : _lastName  

______________________
Saida de dados: 
- exemplo double - 
( para controlar o numero de casas decimais, usar o seguinte comando) 

double = 10.3568; 

console.writeline(double.ToString("F2"));  
exibindo no console <> 10,35

// f2 para ter duas casas decimais após a virgula/ponto 


_____PLACEHOLDERS, CONCATENAÇÃO E INTERPOLAÇÃO______
Criando um exemplo: 

 int idade = 32;
 double saldo = 10.35784;
 string nome  = "Maria";

- PLACEHOLDER -> 
console.writeline(" {0} tem {1} anos e tem saldo igual a {2:F2} reais" , nome, idade, saldo); 

- INTERPOLAÇÃO -> 
console.writeline($" {nome} tem {idade} anos e tem saldo igual a {saldo:F2} reais ");

-CONCATENAÇÃO-> 
console.writeline( nome + "tem" + idade + "anos e tem saldo igual a " saldo.ToString("F2") + "reais"); 
__________________

Aula pratica, Usando Interpolação com opção de Concatenação: 

            string produto1 = "Computador";
             string produto2 = "Mesa de escritório";


             byte idade = 30;
              int codigo = 5290;
               char genero = 'M';

              double preço1 = 2100.0;
             double preço2 = 650.50;
            double medida = 53.234567;

            //CODIGO TODO COM INTERPOLAÇÃO 

             Console.WriteLine($"Produtos: " );
              Console.WriteLine($"{produto1}, cujo preço é ${preço1:F2}");
               Console.WriteLine($"{produto2}, cujo preço é ${preço2:F2}");
                Console.WriteLine();
                 Console.WriteLine($"Registro: {idade} anos de idade, código {codigo} e gênero: {genero}");
                  Console.WriteLine();
                 Console.WriteLine($"Medida com oito casas decimais: {medida:F8}");
                Console.WriteLine($"Arredondando (três casas decimais) : {medida:F3}" );
               Console.WriteLine($"Separador decimal invariant culture : {medida.ToString("F3", CultureInfo.InvariantCulture)}");
            //usando CONCATENAÇÃO e metodo ToString: Console.WriteLine("Separador decimal invariant culture:" + medida.ToString("F3", CultureInfo.InvariantCulture) );











