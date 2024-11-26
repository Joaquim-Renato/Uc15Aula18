# Função `calc()` no CSS  

A função `calc()` é uma ferramenta poderosa no CSS que permite realizar cálculos matemáticos diretamente no código para definir valores de propriedades.  

## Como Funciona  

- Com `calc()`, você pode somar, subtrair, multiplicar e dividir valores.
- Ela aceita combinações de unidades, como `px`, `%`, `em`, `rem`, entre outras.  

### Exemplo de Uso  

```css
.elemento {
  width: calc(100% - 50px); /* Define a largura como 100% da tela menos 50 pixels */
  margin-top: calc(2rem + 10px); /* Adiciona 10px ao valor de 2rem */
}
```
--- 
```html
<!-- Definição de um contêiner simples -->
<div class="container"></div>
```
```css
/* Estilo aplicado ao contêiner */
.container {
    background-color: grey; /* Define a cor de fundo como cinza */
    height: 100px; /* Define a altura fixa de 100 pixels */
    width: calc(100% - 100px); /* Define a largura como 100% da tela menos 100 pixels */
}
```


## Vantagens
Flexibilidade: Permite criar layouts dinâmicos e responsivos.
Legibilidade: Facilita a combinação de diferentes unidades sem a necessidade de cálculos manuais.
Manutenção: Ajustar valores se torna mais intuitivo em comparação a definir números estáticos.
Com `calc()`, o CSS ganha uma capacidade extra de adaptação, ideal para cenários onde valores dependem de proporções ou espaços dinâmicos.

----
# Exemplo de Uso de Estilização com CSS

Este exemplo demonstra como utilizar estilos CSS para criar um layout com um menu fixo e um banner ajustável usando a função `calc()`.

### Código CSS

```css
/* Define estilos globais para remover margens padrão */
* {
    margin: 0; /* Remove margens de todos os elementos */
}

/* Define o fundo da página */
body {
    background-color: antiquewhite; /* Cor de fundo da página */
}

/* Estiliza o menu */
.menu {
    background-color: aquamarine; /* Cor de fundo do menu */
    height: 100%; /* O menu ocupa toda a altura */
    color: black; /* Cor do texto */
    font-size: 5rem; /* Tamanho da fonte do texto no menu */
}

/* Estiliza o banner */
.banner {
    height: calc(100vh - 100%); /* Altura ajustada com calc() */
    background-color: blueviolet; /* Cor de fundo do banner */
}
```