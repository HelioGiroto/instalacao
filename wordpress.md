# Passo a passo para construção de sites em Wordpress

## Índice <a id='indice'></a>

[Instalar Wordpress desde cPanel](#instalar)

[Plugins](#plugins)

[Temas](#temas) 

[Elementor(s) PRO grátis](#elementorpro)

[Páginas](#paginas) 

[Configurações gerais de data/hora](#configurar)

[Criar blog](#blog)

[Escolher Fontes](#fontes)

[Escolher Cores](#cores)

[Favicon](#favicon)

[Customizar tema](#customizar)

[Criar Template para Elementor](#template)



As fontes consultadas foram:
 - https://www.youtube.com/watch?v=KlSbLS8hF8A
 - https://www.youtube.com/watch?v=7c2i4LF4mkc
 - https://www.youtube.com/watch?v=ZekMsDh7fec
 - https://www.youtube.com/watch?v=3vSDLPgTxZo
 - https://www.youtube.com/watch?v=vFaiytBdyH8
 - https://www.youtube.com/watch?v=Qw1lQC1H99E
 - https://www.w3schools.io/file/markdown-super-sub-script/
 - https://experienceleague.adobe.com/docs/contributor/contributor-guide/writing-essentials/markdown.html?lang=pt-BR

 ---

## Instalar Wordpress desde cPanel <a id='instalar'></a>

 - Ir a cPanel
 - FERRAMENTA
 - Wordpress Manager by Softaculous
 - Install
 - Escolha a URL de instalação = URL do site
 - Em: 'Conta do administrador' = mudar 'Senha do administrador'.
 - Desmarca todas as opções de plugins
 - Idioma = Português
 - Instalar

[Voltar ao índice](#indice)



## Plugins <a id='plugins'></a> 

### Para eliminar os plugins que vêm por padrão

 - Ir a: Plugins > Plugins Instalados = /wp-admin/plugins.php
 - Marque todos 
 - Ações por lote = Eliminar
 - Aplicar


### Para instalar plugins necessários

 - Ir a: Plugins > Instalar novo =  wp-admin/plugin-install.php
 - Instalar essenciais: 
    - Elementor Website Builder
    - Essential Addons for Elementor
    - Simple Custom CSS and JS
    - WPCode – Insert Headers and Footers
    - Loco Translate  (??)
 - Instalar e ativar todos.
  
[Voltar ao índice](#indice)



## Temas <a id='temas'></a>

 - Ir a Apresentação > /wp-admin/themes.php
 - Adicionar novo
 - Pesquisar...

[Voltar ao índice](#indice)



## Elementor(s) PRO grátis <a id='elementorpro'></a>

 - Baixar pasta zip em https://proelements.org/
 - Ir a Plugins > Adicionar novo (wp-admin/plugin-install.php)
 - Carregar Plugin
 - Sobe pasta zip
 - Ativa o plugin

Para atualizar este plugin: Desinstalar (PRO Elements), baixar nova versão em Elementos, reinstala e ativa.

[Voltar ao índice](#indice)


## Configurações necessárias do Elementor

 - wp-admin/admin.php?page=elementor#tab-experiments
 - wp-admin
 - Elementor
 - Configurações
 - Recursos
 - Contêiner Flexbox = ativo
 - Menu = ativo
 - Salvar alterações



## Páginas <a id='paginas'></a>

### Eliminar todas as páginas desnecessárias

 - Ir a: 'Páginas > Todas as páginas' = /wp-admin/edit.php?post_type=page
 - Marque todos 
 - Ações por lote = Eliminar
 - Aplicar


### Criar nova página Inicio (ou qquer outra)

 - Ir a Páginas > Nova página = /wp-admin/post-new.php?post_type=page
 - Criar nova página chamada inicio
 - Em 'Atributos da página' (coluna direita), escolher Modelo = Elementor Canvas [<sup>(1)<sup>](#modeloPagina)
 	- Talvez mudou para: wp-admin > páginas > edição rápida > modelo > Elementor Canvas *

 - Em Wp-admin > Configurações > Leitura > 'Opções > Leitura'
 - Mudar: 'A sua página inicial mostra = Uma página estática'
 - Em 'Página inicial = inicio'
 - Guardar alterações

<a id='modeloPagina'></a><sup>(1)</sup> * Caso não apareça esta opção, depois de criada a página, ir à Páginas > Todas as páginas > Edição rápida na página Inicio > Modelo = Tela do Elementor

[Voltar ao índice](#indice)



## Configurações gerais de data/hora <a id='configurar'></a>

### Mudar hora e data

 - Ir a: Opções/Configurações > Geral = /wp-admin/options-general.php
 - Altera as configurações necessárias
 	- SP = UTC-3
 - Guardar alterações


### Mudar opções de leitura
 - Ir a: Opções/Configurações > Leitura = /wp-admin/options-reading.php
 - Mudar para: 'A página inicial mostra: (x) Uma página estática'
 - Guardar alterações

 ### Opções de links
 - Ir a: Opções/Configurações > Ligações permanentes = /wp-admin/options-permalink.php
 - Mudar para: '
Estrutura das ligações permanentes = Nome do artigo'
 - Guardar alterações

### Mudar idioma
 - Ir a Configurações > Geral > Idioma do site = /wp-admin/options-general.php
 - Português do Brasil.
 
[Voltar ao índice](#indice)


## Criar blog <a id='blog'></a>

 - Cria uma página chamada **blog**: Em Páginas > Nova Página
 - Em 'Opções > Leitura'
 - Mudar: 'A sua página inicial mostra = Uma página estática'
 - Em 'Página de artigos = blog'
 - Guardar alterações


[Voltar ao índice](#indice)


## Escolher Fontes <a id='fontes'></a>

*Google fonts:*
	https://fonts.google.com/specimen/Jost?query=jost

Para editar: 
 - Edita uma página com Elementor
 - Menú hamburguer (Sup. esq.)
 - Site Settings
 - Tipografia
 - Muda fontes
 - Atualizar (Botão)

/wp-admin/post.php?post=11&action=elementor&active-document=5


*Subir arquivo ttf de fontes próprias:*
 - Instalar e ativar o plugin 
 	Custom Fonts de Brainstorm Force
 - Ir a Aparência > Custom Fonts (.../wp-admin/themes.php?page=bsf-custom-fonts)



[Voltar ao índice](#indice)


## Escolher Cores <a id='cores'></a>

Ver ideias em: 
	https://coolors.co/palettes/trending
	https://color.adobe.com/pt/trends

Para editar: 
 - Edita uma página com Elementor
 - Menú hamburguer (Sup. esq.)
 - Site Settings 	// Configurações do site
 - Global colors 	// Cors globais

[Voltar ao índice](#indice)

## Favicon <a id='favicon'></a>

Para editar: 
 - Edita uma página com Elementor
 - Menú hamburguer (Sup. esq.)
 - Site Settings
 - Site identity
 - Site Favicon
 - Sobe imagem 512 X 512 
 - Actualizar 

 [Voltar ao índice](#indice)



## Customizar tema <a id='customizar'></a>

 Ir a https://avivamentobatista.com/wp-admin/customize.php

 ...

[Voltar ao índice](#indice)


## Criar Template para Elementor <a id='template'></a>

Modo mais fácil:
 - Ao editar uma página
 - Seleciona uma seção 
 - Clica nos 6 pontinhos
 - Botão direito do mouse
 - "Guardar como modelo"
 - Define o nome

Ficará em:
 - Templates > Modelos Guardados

 - Ir a 'Templates' > Adicionar Novo = (/wp-admin/edit.php?post_type=elementor_library&tabs_group=library)
 - Escolher se é Header ou Footer, etc...
 - **Não** escolha instâncias
 ...

[Voltar ao índice](#indice)


## Adicionar permissões a pessoas

 - Ir a Utilizadores > Adicionar novo
(/wp-admin/user-new.php)

[Voltar ao índice](#indice)



# ELEMENTOR

## Criar div 100% de altura copm imagem de fundo
 - Editar página com Elementor
 - 6 pontinhos
 - Layout
 - Altura mínima = 100 vh
 - Estilo
 - Tipo de plano de fundo = pincel
 - Escolhe a imagem
	 - Posição = personalizado ? ou outras
 - Repetir - Não repetir


## Tirar a barra de rolagem (eixo X, horizontal):
 - Layout
 - conteiner
 - Largura do conteúdo = em caixa
 
 
 
 https://elementor.com/help/how-to-change-background-image/
 
 
 
 
