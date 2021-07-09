# Box-sizing

- Como será calculado o tamanho total da caixa?

EXEMPLO:
div {
    width: 100px;
    height: 100px;
    border: 1px solid red;
    padding: 0 20px;
}

- dessa forma acima, a largura de 100px não é mais respeitada, tendo uma caixa de 140px de largura - pois 'ao conteúdo de 100px' soma-se o padding dos dois lados. Para que o tamanho da caixa efetivamente seja calculado de uma borda a outra - ou seja, apesar de eu ter o padding, a caixa continuar tendo a largura realmente especificada - usamos o box-sizing

```css
div {
    width: 100px;
    height: 100px;
    border: 1px solid red;
    padding: 0 20px;

    box-sizing: border-box;
}
```
- assim realmente teremos uma caixa de 100px de largura com um preenchimento lateral de 20px;
- para evitar este problema, é comum fazer como abaixo: o * representa que para todos os conteúdos será adicionado a ideia de box-sizing, evitando o conflito com o padding

```css
* {
    box-sizing: border-box;
}
```

obs: o primeiro valor de padding é referente a top e bottom, e o segundo valor a left e right

obs2: quando o width nem o height é especificado, por padrão é pego a altura do conteúdo e a largura total do espaço


