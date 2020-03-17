# Bitcoin-minning
 Gasirea valorii hash corespunzatoare unui bloc minat in Bitcoin care satisfice dificultatea ceruta.
 
 
2 cazuri:

  o Valoarea nonce se initializeaza de la 3 000 000 000, caz in care trebuie
sa gasiti o valoare nonce1 mai mica decat 3 100 000 000 pentru care se
satisfice dificultatea, i.e., se gaseste o valoare hash care incepe cu
numarul de zerouri cerut.

  o Valoarea nonce se initializeaza de la un numar aleator, dar mai mare
decat valoarea nonce1 gasita anterior. Atentie! Nu valoarea imediat mai
mare, i.e. nonce1 +1, ci un numar (pseudo-) aleator oarecare, cu conditia
sa fie mai mare decat valoarea nonce1 gasita mai sus. Verificati pentru
cel putin 100 000 000 de valori succesive pornind de la aceasta valoare,
sau pana cand ati gasit un nonce2 pentru care valoarea functiei hash
satisfice dificultatea.

Input:

Version: 0x20400000

Prev Block: 00000000000000000006a4a234288a44e715275f1775b77b2fddb6c02eb6b72f

Merkle Root: 2dc60c563da5368e0668b81bc4d8dd369639a1134f68e425a9a74e428801e5b8

Time: 0x5DB8AB5E

Bits: 0x17148EDF


Caz 1 

Nonce 1= 3060331852 

Hash1 = 0000000000000000000d7612d743325d8e47cb9e506d547694478f35f736188e 

Primele 5 valori 

  3000000000-'70ba305ff525556330ab7f3fc3f342f2e82acd8d896e52dee84c0fec07fd8881' 
  
  3000000001 -'e16392883f05773debd5be4f8e9b99d3445c3539b031cd857ac0dc48de85c3f4' 
  
  3000000002 - 'e7becb7c0bc3b14370dc33f289822e61b706febaae6f0ba7b9c96f4c0e31ffed' 
  
  3000000003 - '741fe37c2260738ceaeab90429b8adce1f1c1887a2a43855a79353cf35725e05' 
  
  3000000004 - 'be3336f846a487f00de37b1c7565e6dcf600b25fbb54025cc7776337b5d6ebc1' 

Caz 2  

Test1
  Nonce2 start: 3136568943 
  Numar testari: 100000000 
  Succes: Nu 
    Nonce2: -
    Hash2: -


Test2
  Nonce2 start: 3067194451 
  Numarul de testari 100000000
  Succes: Nu 

Test3
  Nonce2_start:  3144084796 
  Numarul de testari 100000000 
  Succes : Nu 
