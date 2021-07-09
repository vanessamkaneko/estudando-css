# Trabalhando com fontes
- Diferentes tipografias transmitem diferentes mensagens

## Basic Font Properties
* font-family
* font-weight
* font-style
* font-size

## font-family
* Tipo de fonte de um elemento
* Lista as fontes em ordem de prioridade
* Inclui *fallback* font (caso não dê para usar uma fonte no caminho ideal, tem outra opção - seria um escape):

```css
p {
    font-family: "Times New Roman", Times, serif;
}
```
- o ideal seria a TNR, se não tiver ela, tenta usar a Times, se não tiver ela, utiliza uma fonte 'serifada';

- serif: são fontes que possuem um risquinho embaixo de letras como i, r, etc (como esta aqui mesmo);

- sans: contrário do serif - não tem esses risquinhos/dobrinhas, é mais reta

## font-weight

- Peso da fonte

```css
p {
    font-weight: bold;
}
```
- Dependendo da família da fonte, não conseguimos utilizar todos os pesos (não fazendo diferença se usar ou não)

## font-style

- Estilo da fonte, podendo ser normal | italic | oblique
- Assim como no font-weight, não são todas as famílias de fontes que aceitam todos os styles (as vezes aceitando apenas o normal mesmo)


```css
span {
    font-style: italic;
}
```

## font-size

- Tamanho da fonte
-  Utilizando-se de px, em ou rem, sendo os dois primeiros mais couns

## Web Fonts
- Fontes do sistema: fontes presentes no meu sistema, entretanto as vezes o que tem na minha máquina, não tem no de outra pessoa

- Fontes da web:
    - link: entra no site fonts, escolher a fonte desejada, copiar o link e na parte de html, colar o link no <head> | na parte de css, copiar a regra de css:

    ```css
    p {
        font-size: 12px;
        font-family: 'Yomogi', cursive;
    } 
    ```
    - @import
    - @font-face

fonts.google.com
