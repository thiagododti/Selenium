### seletor geral( * )
Seleciona todos os elementos

### seletor de classe (.nome_da_classe)
Seleciona toda classe que tiver o nome definido apos o .

### seletor de id (#nome_do_id)
Seleciona toda id que tiver o nome definido apos o #

### combinadores (section section)
Pode ser combinado varios seletores para buscar algo especifico dentro de um outro elemento
Ex. section section eu vou selecionar somente as sections que estão dentro de outra section

### filho imediato (div > p)
Com o seletor > eu busco os elementos que são filhos de um outro elemento
Ex. div > p eu seleciono todos os elementos filhos p de uma div

### irmão ( ~ )
Com esse seletor eu busco elementos que tenha irmãos especificos
Ex. div ~ span eu seleciono todos os irmãos da div que sejam span

### irmão imediato ( + )
Com esse seletor eu ja busco o irmão imediato de um elemento
Ex. h2 + div eu vou selecionar a div que é irmã imediata de h2, assim mesmo que tenham outras divs irmãs do h2, somente a primeira div após o h2 vai ser selecionada pois ela é a irmã imediata dele.

### Seletor de atributo ( [nome] )
Com o colchetes eu busco qualquer tipo de atributo que tenha o nome especificado dentro de um elemento.
<div id="rating" class="rating" data-rating="4.5">
[data-rating] essa div seria selecionada pois dentro dela tem um atributo chamado data-rating

### Seletor de atributo com valor ([data-category="Bolos"])
Para essa seleção de elemento, eu especifico que o valor de um atributo deve ser exatamente igual ao que informei
Assim mesmo que tenha outros atributos em outros elementos, somente o atributo com o valor especificado vai ser selecionado

### Seletor de palavra ( [data-recipe~="de"] )
Com o ~= eu busco algum atributo que tenha a palavra especificada no valor dele.
Para essa situação a palavra é isolada, então mesmo que tenha algu valor com essa combinação de letra, ele nao vai ser selecionado caso essa combinação nao seja isolada.

### Seletor de combinação ( [data-recipe*="cc"] )
Diferente de ~= o *= vai buscar a combinação dentro de qualquer valor que ele exista.
Para o exemplo, se existir a combinação cc dentro de uma palavra o seletor irá selecionar esse elemento

### Seletor hifén ( [style|="font"] )
Esse seletor vai me selecionar qualquer elemento que tenha um valor selecionado seguido de hifén "font-"
Esse seletor é bastante usado para buscar propriedades do css

### Seletor de prefixo ( [class ^="r"] )
Como o proprio nome diz, ele vai buscar elementos que iniciam os valores com a busca especificada

### Seletor de sufixo ( [class $="r"] )
E aqui o seletor de sufixo vai buscar elementos que terminem os valores com a busca especificada
