## Margin

- Espaço entre os elementos
- margin-top | margin-right | margin-bottom | margin-left
- aceita values como: <lenght> | <percentage> | auto (só faz cálculos automáticos para as laterais)

```css
div {
    /* shorthand - agrupamento */
    margin: 12px 16px 10px 4px; /* top, right, bottom, left */
    margin: 12px 16px 0; /* top, left e right, bottom */
    margin: 8px 16px; /*top e bottom, left e right */
    margin: 8px; /* todos os lados */
}
```
- por padrão, o browser (chrome por exemplo) adiciona 8px de margin, por isso é comum retirar a margin de todos os elementos para assim se trabalhar melhor com as estilizações feitas:

* {
    margin: 0;
}

*Atenção ao margin collapsing*: para elementos em block - se de um a margin-bottom é um valor e de outro a margin-top é outro, considera-se o maior valor; se forem iguais, só considera um, não há a soma dos valores (diferente se estivere inline, em que há essa soma)