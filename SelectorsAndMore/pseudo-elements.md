# Pseudo-elements

- Com pseudo-elements nós podemos adicionar elementos HTML pelo próprio CSS
`::pseudo-element-name`

## Exemplos

<li>Lista 1</li>
<li>Lista 2</li>
<li>Lista 3</li>
<li>Lista 4</li>

* ::before

li {
    position: relative;
}

li::before {
    content: "";
    width: 10px;
    height: 1px;
    background-color: blue;
    position: absolute;
    bottom: 0px;
}

* ::after

li::after {
    content:";"
}

- tanto no before quanto no after é obrigatório possuir o content, nem que seja pra deixar um conteúdo vazio (") - pois sem o content, no caso do before por exemplo, toda a estlização feita seria desconsiderada

*::first-line

<p>Escrevendo o primeiro parágrafo já dá para perceber que não é tão difícil. Entretanto, isso só  vem com o tempo. Os textos nessas linhas precisam ser grandes o suficiente para haver a quebra de linhas, pelo contrário, ficarão todas em uma única linha.</p>
<p> Não sei o que escrever agora, só estou testando um negocinho aqui. </p>

p::first-line {
    font-weight: bold;
}

- só as primeiras linhas ficariam em negrito

p:nth-of-type(2)::first-line {
    font-weight: bold;
}

- podemos agrupar pseudo-classes e pseudo elements - neste caso acima, somente o segundo <p> teria a primeira linha do texto em negrito