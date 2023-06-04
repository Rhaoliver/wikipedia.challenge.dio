#HTML II - Etapa mais avançada


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