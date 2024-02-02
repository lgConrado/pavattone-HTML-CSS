# HTML: Linguagem de formatação

<img src="image-2.png" alt="Alt text" width="500">

---

## Estrutura
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nome da Página</title>
</head>
<body>
</body>
</html>
```

<div style="display: flex; flex-direction: column; max-height: 240px; margin-bottom: 20px;max-width: 500px">
    <div style="align-items: center; background-color: #191919; display: flex; height: 100%; justify-content: center; padding-top: 10px;width: 100%">
        <p style="font-size: 24px; font-weight: 700">Head</p>
    </div>
    <div style="align-items: center; background-color: #225B66; display: flex; height: 100%; justify-content: center; padding-top: 10px; width: 100%">
        <p style="font-size: 24px; font-weight: 700">Main</p>
    </div>
    <div style="align-items: center; background-color: #D9D9D9; display: flex; height: 100%; justify-content: center; padding-top: 10px; width: 100%" >
        <p style="color: #000000; font-size: 24px; font-weight: 700">Footer</p>
    </div>
</div>

```
> <head></head>: contém o cabeçalho da página
Tags {
    <meta>: fornece metadados sobre o documento HTML.
    <title>: define o título da página.
    <link>: define a relação entre o documento atual e um recurso externo, como uma folha de estilo.
    <script>: define scripts incorporados no documento HTML.
}
```
```
> <main></main>: contém o conteúdo da página
```
```
> <footer></footer>: contém o rodapé da página
```
---

## Criando containers/blocos de código
```
> <article></article>: contém um conteúdo independente e autocontido, como um post de blog, um artigo de jornal
```
```
> <aside></aside>: contém conteúdo relacionado ou complementar ao conteúdo principal, muitas vezes colocado ao lado dele
```
```
> <div></div>: tag genérica para dividir o conteúdo em seções ou agrupar elementos
```
```
> <fieldset></fieldset>: agrupa elementos relacionados em um formulário, como campos de entrada, e pode ser usado com a tag <legend> para fornecer uma legenda descritiva
```
```
> <header></header>: contém elementos introdutórios ou de navegação para uma seção ou página
```
```
> <nav></nav>: contém links de navegação para outras páginas ou seções do site
```
```
> <p></p>: é usada para definir um parágrafo de texto
```
```
> <section></section>: representa uma parte temática ou funcional do conteúdo, como capítulos, abas de navegação
```
---
## Tipos de Títulos
```
<h1>Title</h1>
<h2>Sub Title</h2>
<h3>Sub Title</h3>
<h4>Sub Title</h4>
<h5>Sub Title</h5>
<h6>Sub Title</h6>
```
---


## Edição de texto
```
> Negrito:
    <strong>Text</strong>
    <b>Text</b>
```
```
> Itálico:
    <em>Text</em>
    <i>Text</i>
```
```
> Sublinhado:
    <u>Text</u>
```
```
> Tachado:
    <del>Text</del>
```

---
## Estilização `<style></style>`
```
<head>
    <style>
        body {
            background-color: blue;
        }
    </style>
</head>
```
---
## Estilização inline
```
<h1 style="text-align: center;">Text</h1>
<h1 style="text-align: right;">Text</h1>
<h1 style="text-align: left;">Text</h1>
<h1 style="text-align: justify;">Text</h1>
```
—

## Personalizando cores
```
> Hexadecimal #000000
Exemplo: background-color: #000000;
```
* 2 primeiros dígitos é a quantidade de vermelho;
* 2 segundo dígitos é a quantidade de verde;
* 2 últimos dígitos é a quantidade de azul;
```
> hsl (Matiz, saturação, luminosidade)
Exemplo: background-color: hsl(0,0%,0%);
```
* Matiz é um grau na roda de cores de 0 a 360. 0 é vermelho, 120 é verde e 240 é azul;
* A saturação é um valor percentual, 0% significa um tom de cinza e 100% é a cor completa;
* A luminosidade também é um valor percentual, 0% é preto e 100% é branco;
```
> hsla (0,0%,0%,0)
Exemplo: background-color: hsla(0,0%,0%,0);
```
* Matiz é um grau na roda de cores de 0 a 360. 0 é vermelho, 120 é verde e 240 é azul;
* A saturação é um valor percentual, 0% significa um tom de cinza e 100% é a cor completa;
* A luminosidade também é um valor percentual, 0% é preto e 100% é branco;
* Alfa pode ser 0, 1 ou um valor percentual onde, 1 corresponde a opacidade total 100%;
```
> rgb (Red, Green, Blue)
Exemplo: background-color: rgb(0, 0, 0);
```
```
> rgba (Red, Green, Blue, Alfa)
Exemplo: background-color: rgba(0, 0, 0, 1);
```
—

## Adicionando imagem
```
<img src="./src/img/image">
```
---
## Adicionando link
```
<a href="index.html">Home</a>
```
---
## Adicionando link com destino à uma nova aba

```
<a href="index.html" target="_blank">Home</a>
```
---
## Adicionando botão `<button></button>`
```
<button type="submit">Enviar</button>
```
---
## Menu de navegação `<nav></nav>`
```
> Unordered list <ul></ul>
```
```
> Ordered list <ol></ol>
```
```
> item no menu de navegação <li></li>
```
## Estrutura menu de navegação

```
<ol></ol>

    <nav>
        <ol type="1">
            <li>Text</li>
        </ol>
        <ol type="a">
            <li>Text</li>
        </ol>
        <ol type="A">
            <li>Text</li>
        </ol>
    </nav>

<ul></ul>

    <nav>
      <ul type="square">
        <li>Text</li>
      </ul>
      <ul type="circles">
        <li>Text</li>
      </ul>
      <ul type="disc">
        <li>Text</li>
      </ul>
    </nav>
```
---
## Formulário `<form></form>`
```
> Inserindo campo <input></input>
```
```
> Inserindo título ao campo <label></label>
```
```
> Tornando campo obrigatório com "required"
```
```
> Escrever texto no campo com "placeholder"
```
```
<form>
    <label for="telefone">Telefone</label>
        <input type="text" id="telefone" placeholder="(XX) XXXXX-XXXX" required>
</form>
```
---
## Menu de Seleção `<select></select>`
```
<h1>Text</h1>
<select>
    <option>Opção 1</option>
    <option>Opção 2</option>
    <option>Opção 3</option>
</select>
```
---
## Table `<table></table>`
```
> Cabeçalho <thead></thead>
```
- Título da tabela `<caption>`
- Linhas da tabela `<tr></tr>`
- Células da tabela `<th></th>`
```
> Corpo <tbody></tbody>
```
- Linhas da tabela `<tr></tr>`
- Célula da linha `<td></td>`
```
> Rodapé <tfoot></tfoot>
```
```
> rowspan: Mesclagem de células com linhas
```
- `<td rowspan="2">`
```
> colspan: Mesclagem de células com colunas
```
- `<td colspan="2">`
```
<table>
    <thead>
        <tr>
            <caption>Barbearia</caption>
                <th>Dia</th>
                <th>Horário</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Segunda</td>
            <td>8h ~ 20h</td>
        </tr>
        <tr>
            <td>Quarta</td>
            <td>8h ~ 20h</td>
        </tr>
        <tr>
            <td>Sexta</td>
            <td>8h ~ 20h</td>
        </tr>
    </tbody>
</table>
```
---
# CSS: Linguagem de estilização

## Propriedades de Layout

<img src="image-1.png" alt="Alt text" width="500" />

---
## Unidades de medida
```
> px: pixel
```
```
> em: relativo ao tamanho da fonte do elemento pai
```
```
> rem: relativo ao tamanho da fonte do elemento raiz
```
```
> %: porcentagem do tamanho do elemento pai
```
```
> vw: proporcional a largura da tela: 1vw é igual a 1% da largura
```
```
> vh: proporcional a altura da tela: 1vw é igual a 1% da altura
```
```
> vmin: O menor entre vw e vh
```
```
> vmax: O maior entre vw e vh
```
## Dimensões
```
> height: altura
Exemplo: height: 45px;
```
```
> width: largura
Exemplo: height: 100px;
```

---

## Espaçamento

```
> border: width style color (borda)
Exemplo: border: 1px solid #000000;

Exemplo {
    border-width: 1px;
    border-style: solid;
    border-color: #000000;
}
```

```
> margin: margem
Exemplo: margin: 20px;
//Será aplicado em todas as direções

Exemplo: margin: 20px 15px;
//Será aplicado 20px na vertical (em cima e em baixo), e 15px em na horizontal (esquerda e direita)

Exemplo: margin: 20px 15px 10px 5px;
//Será aplicado no sentido horário: 20px em cima, 15px à direita, 10px em baixo e 5px à esquerda

Exemplo {
    margin-top: 20px; //Será aplicado em cima
    margin-right: 15px; //Será aplicado à direita
    margin-bottom: 10px; //Será aplicado em baixo
    margin-left: 5px; //Será aplicado à esquerda
}
```

```
> padding: preenchimento
Exemplo: padding: 20px;
//Será aplicado em todas as direções

Exemplo: padding: 20px 15px;
//Será aplicado 20px na vertical (em cima e em baixo), e 15px em na horizontal (esquerda e direita)

Exemplo: padding: 20px 15px 10px 5px;
//Será aplicado no sentido horário: 20px em cima, 15px à direita, 10px em baixo e 5px à esquerda

Exemplo {
    padding-top: 20px; - Será aplicado em cima
    padding-right: 15px; - Será aplicado à direita
    padding-bottom: 10px; - Será aplicado em baixo
    padding-left: 5px; - Será aplicado à esquerda
}
```

---

## Posicionamento
```
> align-items: alinha os elementos flexíveis
Exemplo :align-items: start; - Alinha os elementos no início do bloco

Exemplo :align-items: center; - Alinha os elementos no centro do bloco

Exemplo :align-items: end; - Alinha os elementos no fim do bloco
```
```
> align-content: define a distribuição dos elementos dentro do bloco
Exemplo :align-content: space-around; - Distribui os elementos com espaçamento no início, no fim e entre os mesmos dentro do bloco.

Exemplo :align-content: space-between; - Distribui os elementos com espaçamento entre os mesmos dentro do bloco.
```
```
> display: define a flexibilidade do componente
Exemplo: display: block; - Elementos de nível de bloco começam em uma nova linha e ocupam a largura total disponível

Exemplo: display: flex; - Estabelece um contêiner flexível, permitindo o uso de propriedades flexíveis para controlar o layout de seus filhos.l

Exemplo: display: grid; - Estabelece um contêiner de grade, permitindo o uso de propriedades de grade para arranjar seus filhos em linhas e colunas.

Exemplo: display: inline; - Elementos de nível de linha não começam em uma nova linha e ocupam apenas a largura necessária.

Exemplo: display: inline-block; - Cria um elemento de nível de linha que se comporta como um elemento de nível de bloco por dentro, permitindo definir largura, altura, margens e preenchimentos.

Exemplo: display: none; - Remove o elemento completamente do layout do documento; o elemento não será exibido.
```
```
> Grid
https://cssgridgarden.com
```
---

## Edição de texto
```
> uppercase: maiúscula
Exemplo: text-transform: uppercase;
```
```
> lowercase: minúscula
Exemplo: text-transform: lowercase;
```
```
> font-weight: intensidade da cor
Exemplo: font-weight: bold; //Negrito

Exemplo: font-weight: 100 | 200 | 300 | 400 | 500 | 600 | 700 | 800 | 900;
```
```
> text-decoration: formatação de linha
Exemplo: text-decoration: underline; //Sublinhado

Exemplo: text-decoration: overline; //Tachado
```
```
> text-size: tamanho
Exemplo: text-size: 1rem;
```
```
> text-shadow: h-shadow v-shadow blur-radius color (sombreamento)
Exemplo: text-shadow: 1px 1px 2px #000000;
```
- h-shadow: Sombra horizontal;
- v-shadow: Sombra vertical;
- blur-radius: Desfoque;
- color: cor;
—

## Estilização
```
> box-shadow: h-shadow v-shadow blur-radius spread-radius color (sombreamento)
Exemplo: box-shadow: 2px 2px 2px 1px #000000;
```
- h-shadow: Sombra horizontal;
- v-shadow: Sombra vertical;
- blur-radius: Desfoque;
- spread-radius: Expansão;
- color: cor;
```
> boder-radius: arredondar borda
Exemplo: border-radius: 10px;
```
—
## Arquitetura

## Metodologia BEM (Block, Element, Modifier)
https://www.alura.com.br/artigos/criando-componentes-css-com-padrao-bem

```
Fornece uma convenção para nomear classes em CSS, tornando seu código mais legível e compreensível.
```
```
> Block: É uma entidade independente e significativa por si só.
Exemplo: header, container, menu.
```
```
> Element: Partes de um bloco que têm significado em conjunto com esse bloco.
Exemplo: header, container, menu.
``````
> Modifier: Uma variação ou extensão de um bloco ou elemento.
Exemplo: menu--hidden, menu__item--active..
```
### Vantagens
```
> Legibilidade: Olhando para uma classe BEM, você pode facilmente entender a relação entre o CSS e o HTML, o que está acontecendo e onde.
> Independência: Os blocos são independentes e podem ser reutilizados, sem estar atrelados a outros elementos.
> Sem Cascata: Como o BEM evita a especificidade, os estilos não se sobrepõem, evitando efeitos colaterais indesejados.
```
