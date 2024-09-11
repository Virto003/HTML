
# Estrutura Básica de HTML

## Tags em HTML

As tags são o que dá significado a um código HTML. Elas são os elementos com os quais podemos estruturar a página. As tags têm o seguinte formato:

```html
<tag> </tag>
```

Com abertura e fechamento. Algumas tags também podem não depender de um encerramento, como, por exemplo, as tags `<br>` e `<hr>`.

## Atributos

As tags podem possuir algumas informações adicionais que definem as propriedades e comportamentos. 

Exemplo: o atributo `href` dentro de uma tag `<a>` define o destino de um link.

Os atributos têm o seguinte formato dentro das tags:

```html
atributo="valor"
```

Eles são geralmente opcionais, mas alguns são essenciais para que o elemento funcione corretamente.

Exemplo:

```html
<a href="https://www.google.com">link para o Google</a>
```

## Tags Inline

As tags inline são aquelas que ocupam apenas o espaço necessário dentro da página e não quebram linhas nos textos. Como exemplos de tags inline temos:

- **`<span>`**: Usado para estilizar partes específicas do texto sem quebrar a linha.

  ```html
  <p>Texto normal, e <span style="color: red;">texto em vermelho</span>.</p>
  ```

- **`<a>`**: Define um link de hipertexto que fica na mesma linha do texto ao redor.

  ```html
  Clique <a href="#">aqui</a> para mais informações.
  ```

- **`<img>`**: Insere uma imagem no texto, mantendo o fluxo do conteúdo.

  ```html
  Aqui está uma imagem: <img src="imagem.png" alt="Descrição da imagem">
  ```

- **`<strong>`** e **`<em>`**: Para negrito e itálico, respectivamente, sem quebrar o fluxo do texto.

  ```html
  Este é um texto <strong>negrito</strong> e <em>itálico</em>.
  ```

Aqui está o texto sobre as tags de bloco, complementado conforme o seu estilo direto:

```markdown
## Tags de Bloco

Diferente das tags inline, as tags de bloco ocupam todo o espaço da página e sempre começam em uma nova linha. Exemplos:

- **`<div>`**: Usada para agrupar elementos em blocos.
  
  ```html
  <div>Este é um bloco de conteúdo.</div>
  ```

- **`<p>`**: Define um parágrafo de texto.

  ```html
  <p>Este é um parágrafo de texto.</p>
  ```

- **`<header>`**: Define o cabeçalho de uma seção ou página.

  ```html
  <header>Este é o cabeçalho da página.</header>
  ```

- **`<section>`**: Usada para definir seções dentro de um documento.

  ```html
  <section>Esta é uma seção de conteúdo.</section>
  ```

- **`<footer>`**: Define o rodapé de uma seção ou página.

  ```html
  <footer>Este é o rodapé da página.</footer>
  ```

## Tags de Cabeçalho

## Tabelas

No HTML, as tabelas são compostas por linhas e células que organizam os dados em um formato tabular. Para criar uma tabela, é necessário usar a tag **`<table>`**.

### Estrutura Básica de uma Tabela

Dentro da tag `<table>`, podemos usar as seguintes tags para agrupar e organizar o conteúdo:

- **`<thead>`**: Define o cabeçalho da tabela.
- **`<tbody>`**: Define o corpo da tabela.
- **`<tfoot>`**: Define o rodapé da tabela.

Dentro de cada grupo, podemos usar as tags **`<tr>`** para definir as linhas. Dentro das linhas, usamos:

- **`<th>`**: Define as células de cabeçalho. Essas células são geralmente usadas para descrever o conteúdo das colunas.
- **`<td>`**: Define as células de dados padrão.

### Exemplo de Tabela

```html
<table>
    <thead>
        <tr>
            <th>Nome</th>
            <th>Idade</th>
            <th>Cidade</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Victor</td>
            <td>19</td>
            <td>Itu</td>
        </tr>
        <tr>
            <td>Ana</td>
            <td>22</td>
            <td>São Paulo</td>
        </tr>
        <tr>
            <td>Lucas</td>
            <td>25</td>
            <td>Rio de Janeiro</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td colspan="3">Total de registros: 3</td>
        </tr>
    </tfoot>
</table>
```

## Listas

As listas em HTML podem ser ordenadas ou não.

### Exemplo de Lista Ordenada

```html
<ol>
  <li>Primeiro item</li>
  <li>Segundo item</li>
  <li>Terceiro item</li>
</ol>
```

Sendo `<ol>` a tag que define que a lista é ordenada e `<li>` a tag que define os itens da lista.

### Exemplo de Lista Desordenada

```html
<ul>
  <li>Primeiro item</li>
  <li>Segundo item</li>
  <li>Terceiro item</li>
</ul>
```

Sendo `<ul>` a tag que define que a lista é desordenada e `<li>` a tag que define os itens da lista.


## Links

Para criar links no HTML, usamos a tag **`<a>`** com o atributo `href`.

As tags `<a>` são tags inline, o que significa que elas podem ser inseridas no meio de um texto sem quebrar o fluxo.

Além de textos, dentro da tag `<a>`, podemos inserir outros elementos, como imagens.

### Exemplos:

- Link com texto:

  ```html
  <a href="https://www.exemplo.com">Clique aqui para visitar o site</a>
  ```

- Link com imagem:

  ```html
  <a href="https://www.exemplo.com">
      <img src="imagem.png" alt="Descrição da imagem">
  </a>
  ```
## Formulários

Os formulários em HTML permitem a coleta de dados do usuário por meio de diversos elementos de controle. Para criar um formulário, usamos a tag **`<form>`**.

### Estrutura Básica de um Formulário

```html
<form action="/enviar" method="post">
    <label for="nome">Nome:</label>
    <input type="text" id="nome" name="nome" placeholder="Digite seu nome">

    <label for="email">Email:</label>
    <input type="email" id="email" name="email" placeholder="Digite seu email">

    <input type="submit" value="Enviar">
</form>
```
### Atributos Comuns em Formulários

- **`action`**: Define o URL para onde os dados do formulário serão enviados.

  ```html
  <form action="/enviar" method="post">
  ```

- **`method`**: Define o método HTTP usado para enviar os dados (`get` ou `post`).

  ```html
  <form method="post">
  ```

- **`placeholder`**: Exibe um texto de dica dentro de um campo de entrada, até que o usuário digite algo.

  ```html
  <input type="text" placeholder="Digite seu nome">
  ```

- **`value`**: Define o valor inicial de um input ou o texto exibido em botões.

  ```html
  <input type="submit" value="Enviar">
  ```

- **`min` e `max`**: Definem o valor mínimo e máximo para campos numéricos, como números e datas.

  ```html
  <input type="number" min="1" max="10">
  ```

- **`required`**: Torna o campo obrigatório antes de enviar o formulário.

  ```html
  <input type="text" required>
  ```

- **`id` e `name`**: `id` é usado para identificação única do elemento na página, enquanto `name` é o nome do campo enviado no formulário.

  ```html
  <input type="text" id="nome" name="nome">
  ```

- **`type`**: Define o tipo de entrada, como `text`, `email`, `password`, `submit`, etc.

  ```html
  <input type="email" placeholder="Digite seu email">
  ```

- **`maxlength` e `minlength`**: Controlam o número máximo e mínimo de caracteres permitidos em um campo de texto.

  ```html
  <input type="text" maxlength="50" minlength="5">
  ```


### Elementos de Controle

- **`<input>`**: Usado para campos de entrada de texto, botões, caixas de seleção, etc.

  ```html
  <input type="text" placeholder="Digite aqui">
  ```

- **`<label>`**: Associado a um input, facilita o clique e a navegação.

  ```html
  <label for="email">Email:</label>
  <input type="email" id="email" name="email">
  ```

- **`<textarea>`**: Área de texto para entradas maiores.

  ```html
  <textarea rows="4" cols="50" placeholder="Digite seu comentário"></textarea>
  ```

- **`<select>`**: Menu suspenso para selecionar uma opção.

  ```html
  <select name="opcoes">
      <option value="1">Opção 1</option>
      <option value="2">Opção 2</option>
  </select>
  ```

- **`<button>`**: Botão para ações, como enviar o formulário.

  ```html
  <button type="submit">Enviar</button>
  ```
