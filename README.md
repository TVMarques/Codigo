# Codigo
Usando o C#
## 1°Resposta
using System;

class Program {

public static void Main (string[] args) {
  
      Console.WriteLine("Digite um número para verificar se ele pertence à sequência de Fibonacci:");
      int num = int.Parse(Console.ReadLine());
      bool pertence = VerificarFibonacci(num);
      
      if (pertence){
          Console.WriteLine($"O número {num} pertence à sequência de Fibonacci.");
      }
      else{
          Console.WriteLine($"O número {num} não pertence à sequência de Fibonacci.");
      }
  }
  
  static bool VerificarFibonacci(int num) {
  
      if (num < 0) return false; // Números negativos não pertencem à sequência
      int a = 0;
      int b = 1;
      
      // Checa os primeiros dois números da sequência
      if (num == a || num == b) return true;
      int c = a + b;
      
      // Verifica a sequência até encontrar ou ultrapassar o número
      while (c <= num){
          if (c == num) return true; // Se encontrar o número na sequência
          a = b;
          b = c;
          c = a + b;
      }
      return false; // Se o número não for encontrado na sequência
     }
  }


## 2° Resposta 

using System;

class Program { 

public static void Main (string[] args) {

  
      // String previamente definida no código
      string texto = "A raposa ágil salta sobre o cachorro preguiçoso."; 

      int contador = ContarOcorrenciasDeA(texto);
      Console.WriteLine($"A letra 'a' aparece {contador} vezes na string/palavra ou frase: {texto}.");
  }

  static int ContarOcorrenciasDeA(string texto){
      
      int contador = 0;
      foreach (char c in texto){
          if (c == 'a' || c == 'A'){   // Verifica maiúsculas e minúsculas
              contador++;
          }
      }

      return contador;
    }
}


## 3°Resposta

using System;

class Program {

      public static void Main (string[] args) {
    
       int INDICE = 12, SOMA = 0, K = 1;
    
     
       while (K < INDICE) {
            K = K + 1;
            SOMA = SOMA + K;
       }
       
          Console.WriteLine("A soma é: " + SOMA);
      
    }
   
}
