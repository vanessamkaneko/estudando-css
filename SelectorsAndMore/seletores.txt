# Seletores

Conecta um elemento HTML com o CSS a fim de alterar o elemento.

## Tipos

* Element selector
    - todos os elementos HTML

* ID Selector (#)
    - um elemento que tenha um atributo `id`
    - cada id deverá ser único

* Class Selector (.)
    - os elementos que contenham um atributo `class` (pode ter diferentes class em um só elemento: <h1 class="red big"/> red é uma classe e big é outra)
    - podemos ter uma ou mais classes

* Attribute selector
    - um elemento que tenha um atributo específico (por exemplo, o title)
    - no CSS, ficaria [title] {
        
    }

* Pseudo-class selector
    - elementos em um estado específico
    - por exemplo, o hover:
        diretamente no CSS: h1:hover {
            color: red;
        }

        - assim o título h1 ficaria vermelho ao passar o mouse em cima dele

        ### Múltiplos elementos
        
        Você poderá selecionar múltiplos elementos e aplicar alguma regra CSS para todos eles.

        Usamos uma separação por vírgula para isso:

        no CSS: h1, p, .red {
            color: red;
        }

        p:hover, h1:hover {
            color: red;
        }