# The Elevator Challenge

## Critérios de aceite

### Painel e botões do elevador

1. Dado que cliquei no botão de qualquer andar no painel  
   O botão clicado deve ficar ativo até chegar no atual andar

2. Dado que estou indo para um andar superior ao atual  
   No painel deve aparecer a palavra "Subindo..."

3. Dado que estou indo para um andar Inferior ao atual  
   No painel deve aparecer a palavra "Descendo..."

4. Dado que, cliquei em qualquer andar  
   O painel deve exibir os andares conforme minha posição atual (exemplo, 1° Andar, 2° Andar, etc...)

### Elevador e Piso

1. Dado que esteja no andar térreo  
   O elevador só pode subir

2. Dado que esteja no últmo andar  
   O elevador só pode descer

3. Dado que o elevador esteja em movimento (subindo ou descendo)  
   A porta do elevador deve permancer fechada e abrir somente quando chegar no Andar

4. Dado que estou em algum piso cliquei no botão de qualquer outro piso  
   O texto do piso atual deve ser "Você está no {{número do andar}} Andar" ou Você está no Térreo para caso seja o Térreo  
   Exemplo: Estou no térreo e cliquei no 10. Quando chegar no Décimo Andar o texto deve alterar de "Você está no Térreo" para "Você está no 10° Andar"

5. Dado que eu cliquei em mais de um andar  
   O elevador deve parar nos respectivos andares por ordem crescente (em caso de subida) e descrescente (em caso de descida)  
   Exemplo 1) Estou no térreo e cliquei na seguinte ordem: 1, 6, 5 - O elevador seguir a ordem: 1, 5, 6;  
   Exemplo 2) Estou no 8° andar, cliquei na seguinte ordem: 5, 6, 2 - O Elevador deve seguir a ordem: 6, 5, 2;  
   Exemplo 3) Cliquei no 10 andar e depois, cliquei no 6 andar - o elevador deve ir primeiro ao 6 andar e depois subir para o 10 andar

6. Dado que cliquei em mais de um andar  
   O elevador deve permanecer no andar atual por no máximo 3 segundos e ir para o próximo andar

7. Dado que cliquei em andares distintos  
   O tempo de chegada do elevador ao próximo andar selecionado deve ser correspondente a diferença dos andares em segundos:  
   Exemplo 1): Estou no Térreo e vou para o 6° Andar. Deve levar 6 segundos para chegar até o 6° Andar.  
   Exemplo 2) Estou no 9° Andar e vou para o 5° Andar. Deve levar 4 segundos para chegar até o 5° Andar.
