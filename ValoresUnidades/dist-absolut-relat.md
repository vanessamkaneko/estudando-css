# Distâncias absolutas <length>

- São fixas e não alteram seu valor.

Unidade     Nome                            Equivalências
cm              centímetros                    1cm = 96px/2.54
in                inches (polegadas)         1in = 2.54cm = 96px
px               pixels                             1px = 1/96th (1/96 avos) of 1in

* o mais comum e mais utilizado é o px!
* não recomendado usar cm!

# Distâncias relativas

- São relativas a algum outro valor, pode ser o elemento pai, ou root, ou o tamanho da tela.

*Benefício: maior adaptação aos diferentes tipos de tela

Unidade           Relativo a
em                   tamanho da fonte do pai 
rem                  tamanho da fonte do elemento raíz (root/html)
vw                   1% da viewport width (largura)
vh                    1% da viewport height (altura)

*em: se o tamanho da fonte do pai for 16px, e eu atribuir 2em para a fonte do filho, então a fonte do filho terá tamanho 32 (o tamanho da fonte pai é multiplicada pelo do filho - pode-se usar valores decimais para o em)

*rem: pega como referência diretamente o elemento raíz/root, que é igual a 16px (tendo o mesmo esquema do em)

html {
    font-size: 14px       -> assim pode-se trocar o tamanho da raíz
}