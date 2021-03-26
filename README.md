# Flexbox

## Introdução ao flexbox e fazendo o cabeçalho

### Como colocar os elementos filhos lado a lado?

```css
elementoPai {
    display: flex;
}
```

### Como alinhar os elementos filhos, verticalmente?

```css
elementoPai {
    display: flex;
    align-items: center;
}
```

### Como colocar um espaço entre os elementos filhos?

```css
elementoPai {
    display: flex;
    justify-content: space-between;
}
```
### Como colocar um espaço em volta dos elementos filhos?
```css
elementoPai {
    display: flex;
    justify-content: space-around;
}
```
### Como definir os elementos filhos em coluna?
```css
elementoPai {
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    height: 250px; 
}
```
Caso eu quiser distribuir os filhos na mesma linha posso definir um `flex-wrap: wrap; e um `height: 250px;`, como definido acima, e todos serão separados por colunas de `height: 250px;`.

### flex-flow
Com o flex-flow, posso colocar dois valores de duas propriedades diferentes em uma propriedade.  
Por exemplo:
```css
elementoPai {
    display: flex;
    flex-flow: column wrap;
}
```
Ou seja, `flex-direction:;` e `flex-wrap:;` em uma só propriedade!

### Um pouco mais sobre justify-content

Posso distribuir os elementos dentro do **pai** de diversas formas, podemos por exemplo:

Colocar todo espaço à esquerda, jogando o conteúdo para direita com `justify-content: flex-end`.

Colocar todo espaço à direita, jogando o conteúdo para esquerda com `justify-content: flex-start` (que é o padrão).

Colocar todo espaço à esquerda e à direita, jogando o conteúdo para o meio com `justify-content: center`.

Colocar todo espaço entre os elementos como vimos antes usando `justify-content: space-between`.

E uma possibilidade bem interessante também é colocar o espaço em volta dos elementos. Podemos usar o `justify-content: space-around` para isso.