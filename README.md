# The Elevator Challenge

## Critérios de aceite

### Painel e botões do elevador

Dado que cliquei no botão de qualquer andar no painel  
O botão clicado deve ficar ativo

Dado que estou indo para um andar superior ao atual  
No painel deve aparecer a palavra "Subindo..."

Dado que estou indo para um andar Inferior ao atual  
No painel deve aparecer a palavra "Descendo..."

Dado que, cliquei em qualquer andar  
O painel deve exibir os andares conforme minha posição atual (exemplo, 1° Andar, 2° Andar, etc...)

### Elevador

Dado que esteja no andar térreo  
O elevador só pode subir

Dado que esteja no últmo andar  
O elevador só pode descer

Dado que eu clique em mais de um andar  
O elevador deve parar nos respectivos andares por ordem de seleção (clique em cada botão do painel)  
Exemplo: cliquei na seguinte ordem: 1, 6, 5 - O elevador sobe até o 1° andar, depois para o 6° andar e por último volta até o 5° andar

Dado que cliquei em mais de um andar  
O elevador deve permanecer no andar atual por no máximo 3 segundos e ir para o próximo andar

Dado que estou no térreo, cliquei no 10 andar e depois, cliquei no 6 andar  
O elevador deve ir primeiro ao 10 andar e depois descer para o 6 andar

## Bindings

### Painel do Elevador

```html
  <div id="elevator-display" class="elevator-panel__display">
    <h2 data-display-floor="0">1° Andar<h2>
    <h3 data-elevator-state="up" class="active">Subindo...</h3>
    <h3 data-elevator-state="down" class="">Descendo...</h3>
  </div>
```

### Botões do Elevador

```html
<ul id="elevator-buttons" class="elevator-panel__buttons">
  <li><button class="elevator-button" data-elevator-button="10">10</button></li>
  /* [...] * /
  <li><button class="elevator-button" data-elevator-button="1">1</button></li>
  <li class="elevator-item-first">
    <button class="elevator-button active" data-elevator-button="0">T</button>
  </li>
</ul>
```

### Andares do Prédio

```html
<ul id="buiding-floors" class="building__floors">
  <li class="building-floor" data-floor="10">10° Andar</li>
  <li class="building-floor" data-floor="9">9° Andar</li>
  /* [...] * /
  <li class="building-floor" data-floor="1">1° Andar</li>
  <li class="building-floor" data-floor="0">Térreo</li>
</ul>
```

### Elevador

```html
<div id="elevator-car" class="elevator-car">
  <span class="door door-left"></span>
  <span class="door door-right"></span>
</div>
```
