#HTML II - Etapa avançada


## Acessibilidade
- site adaptável para pessoas com algum tipo de deficiência = internet é para todos!
- definida pelo HTML e CSS, porém muito mais pelo HTML que é a parte estrural do site

utilizar o alt="" para descrever a imagem

### Árvore de acessibilidade (Acessibility Tree)
- ARIA = Accesssible Rich Internet Applications, que altera a árvore de acessibilidade da página


### <a href="#seo">Web Scraping</a>
- Crawler: programa utilizado que extrai informações de sites e usam
- GoogleBot: indexa páginas através de varreduras
- semântica do HTML se encaixa aqui, pois facilita a varredura de programas/robôs nas páginas e auxilia na indexação
- web scraping é o termo utilizado para pegar dados pré-definidos e utilizálos para um fim (dados públicos que podem ser consumidos)

## HTML 5
- tags que substituem as <divs>DIV</divs>

### header
-cabeçalho


### main
- tag principal, não podendo ser filha de outras tags (somente de body)
- aloca o conteúdo principal, podendo ser dividida em seções
- apenas uma por página e as outras tags podem ser filhas dela


### footer
- rodapé, apenas um por página


### aside
- pode ser colocado assuntos auxiliares que não são importantes (menos importante que section)


### section
- seções da main, podendo ter várias dentro da main


### nav
- navegação do html


### article
- comporta: h1, p
- para artigos: pubdate e datetime (atributos)


### blockquote
- citação de várias linhas


### Q
- citação pequena
- não quebra a linha como o blockquote
- cite (atributo)

### figure
- container, delimitando a área de uma imagem
- padrão: display block
- relaciona todas as informações dentro da tag, facilitando no caso de uma busca na internet e também na questão da acessibilidade
- tag que contém a tag img e figcaption


### figcaption
- legenda de figure


### picture
- dá para colocar múltiplas fontes para a imagem
- atributo midia="" no source (ex: source srcset="" midia="(min-width: 600px)" ->trocando a imagem apresentada conforme o largura da janela/resolução de tela do usuário


## SEO
- Search Engine Optimization (otimização para mecanismos de buscas)
- conjunto de técnicas que visam melhorar o posicionamento numa busca
- <h2 id="seo">.</h2>

### Como fazer?
- title: 50-60 caracteres, sendo uma descrição sucinta da página, para aparecer no mecanismo de busca "<title></title>"
- meta name: descrição sucinta também "<meta name="description" content="blá blá blá">"
- caprichar na semântica do HTML, utilizando tags e sections
- schema.org: comunidade que visa a melhoria dos mecanismos de buscas




## HTML Recursos Especiais

### Datalist
- options do combo box, sugerindo informações (sem obrigar a selecionar como a tag selected) a serem preenchidas

<input> 
<datalist>
    <options></options>
    <options></options>
    <options></options>
</datalist>


### Code
- tag indicando um código a ser usado
- tags voltadas para colocar comandos ou fontes na página HTML
- formatação pré-definida; fontes monoespaçadas

### Kbd
- keyboard, indicando um comando do teclado
- tags voltadas para colocar comandos ou fontes na página HTML
- formatação pré-definida; fontes monoespaçadas


### Pre
- tag que pode ser utilizada para agrupar vários códigos e serem indicados 
- tags voltadas para colocar comandos ou fontes na página HTML
- formatação pré-definida; fontes monoespaçadas


### Details
- detalhes, podendo colocar por exemplo, descriçoes

<details> // dessa forma, ao ser clicado, irá expandir para exibir o "p"
    <summary></summary>
    <p><code></code></p>
</details>

#### Summary
- já visto anteriormente, mas dentro da tag details, exibe um título sobre os dados que estão contidos

### Meter
- utilizado com a finalidade de medir (e não de progresso como o progress), com valores que podem aumentar ou diminuir

<meter id="progress" max="100" min="0" value="50"></meter>


### Progress
- utilizado para definir o progresso de uma ação: "carregando" por exemplo
- atributos "max" "min" e "value" 

ex: barra de progresso

<progress id="progress" max="100" min="0" value="0"></progress>

<script>
    var progress = document.getElementById('progress');
    const interval = setInterval(() => {
        progress.value += 10;
        if (progress.value >= 100) {
            alert('Carregamento realizado com sucesso')
            clearInterval(interval);
        }
    }, 1000);
</script>



### Mark
- já visto anteriormente


### Javascript
- manipula o HTML
- manipula o DOM (manipula dinâmicamente o HTML que já foi renderizado pelo browser)


#### Canvas
- utilizado na programação de jogos
- manipulação do javascript para a criação de animações e outras coisas do tipo (curso separado, bem extenso)


## HTML 5, novos atributos

### Autofocus
- atributo que coloca uma barrinha que fica piscando na tela nos campos de digitação, como por exemplo em formulários
- ex: <input type="" id="" name="" autofocus>


### Placeholder
- atributo que sugestiona um estilo de preenchimento
- ex: <input type="" id="" name="" placeholder="Ex: meuemail@gmail.com">

### Required
- atributo que define um campo como obrigatório
- aparece campo obrigatório ao tentar enviar
### Fieldset
- englobamento de um campo <form><fieldset><legend></legend></fieldset></form>
- desabilitar um campo
- ex: <fieldset disabled>


### Maxlength
- determina um máximo de caracteres para campos como o textarea


### Minlength
- determina um mínimo de caracteres para campos como o textarea


### tag form
- não precisa mais estar englobando tudo, podendo os campos do formulário serem referenciados pelo form="" nos atributos da tag


### content editable
<<<<<<< HEAD
- atributo que permite que, ao carregar a página, o conteúdo possa ser editado pelo usuário
=======
- atributo que permite que, ao carregar a página, o conteúdo possa ser editado pelo usuário
>>>>>>> 2b5430ac25f3e7ca091a1a1bc4fbfdf5b78c5020
