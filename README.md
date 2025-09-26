HTML

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>prova 08 - objeto literais</title>
    <link rel="stylesheet" href="./styles.css">
</head>
<body>
    
    <h1>prova 08 - objeto literais</h1>
    <h2>Explique o que são objetos literais em JavaScript?</h2>
    <br>
    <p>Objetos literais em JavaScript são estruturas de dados que
permitem armazenar pares de chave-valor.

Eles são uma maneira simples e direta de criar objetos, onde
as chaves (também chamadas de propriedades) são strings
que identificam os valores armazenados. Os valores podem ser de qualquer tipo, incluindo números,
strings, arrays, funções ou outros objetos.</p>


<script src="./script.js"></script>
</body>
</html>


CSS

/* Reset CSS por Eric Meyer */
html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details,
embed, figure, figcaption,
footer, header, hgroup,
menu, nav, output,
ruby, section,
summary {
   margin: 0;
   padding: 0;
   border: 0;
   font-size: 100%;
   font: inherit;
   vertical-align: baseline;
}
body {
   line-height: 1;
}
ol, ul {
   list-style: none;
}
blockquote {
   quotes: none;
}
table {
   border-collapse: collapse;
   border-spacing: 0;
}

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: rgb(74, 37, 83);
} 

h1 {
    background-color: rgb(20, 20, 20);
    color: white;
    padding: 20px;
    text-align: center;
}
h2 {
    color: white;
    margin: 20px 0 10px 0;
    padding: 0 20px;
    border-bottom: 2px solid white;
    padding-bottom: 5px;
    text-transform: uppercase;
    font-size: 1.5em;
    letter-spacing: 1px;
    
}   
p {
    color: rgb(228, 195, 195);
    margin: 10px 0;
    line-height: 1.6;
    padding: 0 20px;
}   

JAVASCRIPT

let aluno = {
    nome:"João",
    notas: [7, 8, 6, 9],

    calcularMedia: function() {
    let soma = 0;
    for(let i = 0; i < aluno.notas.length; i++) {
        soma += aluno.notas[i];
    }
    return soma / aluno.notas.length;
    
}
}

let {nome} = aluno
console.log(`nome do aluno:`, nome)

let nova_nota = [...aluno.notas, 6]
console.log ('notas do aluno:', aluno.notas)
console.log('nova nota do aluno:', nova_nota)

console.log(`média do aluno:`, aluno.calcularMedia())

