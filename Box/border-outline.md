# Border (e outline)

- São as bordas da caixa

- value: <border-style> | <border-width> | <border-color>
    - style: solid | dotted | dashed | double | groove | ridge | inset | outset

    - width: <length>
    
    - color: <color>
    
```css
div {
    /* shorthand */
    border-top: solid 2px;
    /* style */
    border: solid;
    /* width <length> e style */
    border: 2px dotted;
    /* style e color */
    border: outset #f33;
    /* width, style e color */
    border: medium dashed green;
}
```
- seria mais vantajoso começar só com o border (para que todas as bordas sofram as alterações) e depois se alguma borda precisar de algo específico, colocar depois:

```css
div {
    border: 4px solid red;
    border-top: 2px solid black;
}
- posso também usar o box-sizing, tendo em vista o mesmo conceito que ocorre com o padding  

## Outline
- Não modifica o tamanho da caixa, pois não faz parte do Box Model
- Não permite ajustes individuais
- Mais usado pelo User Agent para acessibilidade