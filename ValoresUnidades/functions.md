# Funções

- Em programação, funções são reconhecidas por causar um reaproveitaento de código;
- Nome, abre e fecha parênteses e dentro dos parênteses vão valores (chamados argumentos)

rgb()
hsl()
url()
calc() - por exemplo, se quero que uma imagem tenha um tamanho, mas não sei exatamente o valor - usamos o calc para fazer este cálculo

EXEMPLO: supondo que há uma classe box dentro de uma <div>:

*o body não vem com um tamanho determinado, se for o caso, tem que reatribuir um valor a ele

body {
    height: 100vh;   //  - imagem pega a altura toda da viewport
    margin: 0;         //- por padrão, é deixado uma margem, desta forma, a margem é retirada
}

.box {
    height: calc(100% - 40px); // a imagem ocupando a tela toda, dela seria retirada um pedaço de 40px 
    width: 100%
}