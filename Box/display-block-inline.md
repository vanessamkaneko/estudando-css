# Display: block vs inline

- Refere-se ao comportamento das caixas em relação às outras caixas - comportamento externo das caixas (será que uma está ao lado da outra, ou embaixo da outra...?)
- Alguns conteúdos, por padrão, já tem um comportamento especificado:
    - <p>, <div>, <section>, todos os headings (<h1>, <h2>...)...: tem comportamento de block (na verdade a maioria tem este comportamento)
    - <a>, <strong>, <span>, <em>: tem comportamento inline

    Display block
    - Ocupa *toda a linha*, colocando o próximo elemento *abaixo* desse
    - Width e height *são respeitados - funcionam!*
    - Padding, margin, border irão funcionar *normalmente*

    Display inline
    - Elemento *ao lado* do outro
    - Width e height *não funcionam*
    - *Somente* valores *horizontais* de margin, padding e border - ou seja, o conteúdo só é empurrado para frente - não vai pra cima ou pra baixo

    - posso fazer com que uma div tenha um display inline e um span tenha um display block, por exemplo

```css
    div {
        height: 100px;
        border: 1px solid red;
        width: 10px;
        display: inline;
    }

    span: {
        width: 10px;
        height: 100px;
        border: 1px solid green;
        display: block;
}
```
