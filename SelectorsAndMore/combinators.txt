# Combinators

Combinadores trabalha para buscar e combinar seletores a fim de aplicar uma estilização;

## Descendant combinator

* Identificado por um espaço entre os seletores
* Busca um elemento dentro de outro


```css
body article h2 {

}
```
- neste exemplo acima, todo o h2 que estivesse dentro de um article - dentro de um body- , receberia a estilização css
- porém, isto seria a mesma coisa que procurar um h2 dentro do body (body h2 {}) , ou simplesmente um h2 na página inteira (h2 {})

### Child combinator

* Identificado pelo sinal `>` entre dois seletores
* Seleciona somente o elemento que é filho direto do pai
* Elementos depois do filho direto serão desconsiderados

```css
body > ul > li {
    color: blue;
}
```
<body>
  <ul>
    <li>Flores</li>
    <li>Frutas</li>
    <li>Pães</li>
  
  <ul>
    <li>Flores</li>
    <li>Frutas</li>
    <li>Pães</li>
 </ul>
 </ul>
</body>
- neste caso, somente o primeiro grupo de li sofreria a estilização (pois está englobado pelo ul, que é o filho direto)
- supondo que o primeiro ul englobando o li estivessem dentro de uma div: o estilo seria aplicado ao que está fora da div
- agora caso ambos os ul estivessem na div, não seria aplicado nenhuma estilização - pois agora o primeiro filho seria a div

```css
ul > li {
    color: blue;
}
```
- neste caso, todos os li dentro de um ul sofreriam a estilização

#### Adjacent sibling combinator

* Identificado pelo sinal de `+` entre dois seletores
* Seleciona somente o elemento do lado direito que é irmão direto na hierarquia

```css
h1 + p 
```
- ou seja, se após o h1 houvessem dois p, somente o p que vem primeiro iria sofrer a estilização

- é muito usado neste exemplo: um button ao lado do outro; quero colocar um espaço entre eles
```css
button + button {
    margin-left: 20px;
}
```
- assim, seria adicionado um espaço no lado esquerdo do segundo button

##### General sibling combinator

* Identificado pelo sinal `~` entre dois seletores
* Seleciona todos os elementos irmãos

```css
h1 ~ p 
```
- desta maneira, TODAS os p's após o h1 sofrem a estilização, independente se tiver outro elemento no meio, como uma div

# Utilizando combinadores

```css
ul > li[class="red"] {
    color: pink;
}
```
- aqui seria aplicada a estilização em todos os li (dentro do ul) com a class=red | entretanto, este é um caso bem específico, o que pode dificultar o reuso das regras de estilização dos elementos, sendo muitas vezes mais eficiente um simples uso de classes (.red)