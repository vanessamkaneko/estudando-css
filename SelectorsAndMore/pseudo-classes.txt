# Pseudo-classes

É um tipo de seletor que irá selecionar um elemento que estiver em um estado específico.

Exemplo: É o primeiro elemento dentro de uma caixa, ou o elemento está com o ponteiro do mouse em cima dele.

Pseudo-classes começa com 2 pontos seguido do nome da pseudo class `:pseudo-class-name`

## Selecionando elementos com pseudo-classes

* :first-child

<ul>
    <li>Flores</li>
    <li>Frutas</li>
    <li>Pães</li>
</ul>

ul li:first-child {
    color: pink;
}

- desta maneira, apenas Flores ficaria rosa | o mesmo aconteceria se houvessem outras listas



* :nth-of-type()

<article>
    <h3>Gratidão</h3>
    <p>Olá</p>
    <p>Oi</p>
    <p>Hey</p>
</article>

article p:nth-of-type(2) {
    font-weight: bold;
    font-size: 18px;
}

- neste caso, o Oi é que sofreria a estilização - dentre os p's, ele é o segundo elemento



* :nth-child()

<article>
    <h3>Pensamentos</h3>
    <p>Seja grato pelo que tem!</p>
    <p>Para tudo há diferentes perspectivas</p>
    <p>Se apague as coisas boas</p>
</article>

article p:nth-child(2) {
    font-weight: bold;
    font-size: 18px;
}
- neste caso, são considerados todos os filhos do article - então quem sofreria a estilização seria o Seja grato pelo que tem!, pois o número 1 agora é o h3 - se ao invés de (2) estivesse (1), não iria acontecer nada, pois não há nenhum p na posição 1.



*nth-child even e odd
- even: números pares | odd: números ímpares

<ul>
    <li>Banana</li>
    <li>Maçã</li>
    <li>Limão</li>
    <li>Melão</li>
    <li>Uva</li>
    <li>Laranja</li>
</ul> 

ul li:nth-child(even) {
    color: black;
    background: white;
}
- Maçã, Melão e Laranja sofreriam a estilização

ul li:nth-child(odd) {
    color: white;
    background: black;
}
- Banana, Limão e Uva  sofreriam a estilização

### Ações do usuário

:hover - quando o usuário estiver com o mouse em cima de determinado elemento posso fazer mudar a cor, por exemplo

h1:hover {
    color: blue;
}

:focus

input:focus {
    border-color: red;
}

- quando o campo de texto fosse clicado (estando em foco), a borda ficaria vermelha

#### Atributos
- disabled e required

input:disabled {
    background-color: gray;
}

input:required {

    background-color: gray;

}
