# font-variant

- Variações na apresentação da fonte;

- Ex: small-caps, normal;

# font-stretch

- Trabalha com o alargamento ou encolhimento da fonte
- Aceita palavras-chaves como: expanded, condensed, normal
- Aceita porcentagens de 50 a 200%
- Nem toda fonte irá aceitar o uso deste estilo

```css
p {
    font-stretch: expanded;
}
```

## letter-spacing

-  Confere espaço entre caracteres;

```css
p {
    letter-spacing: 4px;
}
```

## word-spacing

- Confere espaçamento entre palavras

```css
p {
    word-spacing: 4px;
}
```

## line-height

- Espaços entre linhas
- Pode ser com unidades ou sem unidades de medida
- Comuns: 1.5 ou 2

```css
p {
    line-height: 1.5;
}
```

## text-transform

- Transformação do texto

```css
p {
    text-transform: uppercase; /* capitalize | lowercase | none */
}
```

## text-decoration

- Aparênia decorativa de um texto
- line: underline | overline | line-trough
    *podemos aplicar +1 valor
- style: wavy | dotted | double | dashed | solid (estilo da linha)
- color: <color> values (cor da linha)

```css
p {
    text-decoration: underline; /*forma shorthand - pois poderia ser escrito tex-decoration-line, por ex.*/
}
```

## text-align

- Alinhamento de um texto

```css
p {
    text-align: center; /* left | right | center | justify */
}
```

## text-shadow

- Sombra aplicada a um texto
- Permite múltiplos valores

```css
p {
    text-shadow: 1px 1px 1px red,
                        2px 2px 1px green; /
}
```

- ordem dos valores: offset-x | offset-y | blur-radius | color 

# shorthand

- podemos aplicar todas as propriedades em uma única propriedade chamada font:

```css
p {
    /* -style, -variant, -weight, -stretch, -size/line-height, font-family */
    font: italic normal bold normal 3em/1.5 Helvetica, Arial, sans-serif;
```

