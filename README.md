
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

## Tags de Cabeçalho

## Tags de Bloco


## Tabelas

## Tabelas em HTML

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
    <!-- Cabeçalho da Tabela -->
    <thead>
        <tr>
            <th>Nome</th>
            <th>Idade</th>
            <th>Cidade</th>
        </tr>
    </thead>

    <!-- Corpo da Tabela -->
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

    <!-- Rodapé da Tabela -->
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

