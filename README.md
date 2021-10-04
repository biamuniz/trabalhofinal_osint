# Trabalho final: A crise de oxigênio em Manaus através de tweets, posts, vídeos e notícias
_Repositório para documentar o trabalho final da disciplina Open Source Intelligence, do Master em Jornalismo de Dados, Automação e Data Storytelling do Insper_

**Grupo:** [Bianca Muniz](https://github.com/biamuniz), [Meyrele Torres](https://github.com/meyrele), Ricardo Grinbaum

## Objetivo
Recriar a cronologia dos acontecimentos que culminaram com a crise de oxigênio em Manaus usando técnicas de OSINT.

## Metodologia
Antes de começar, definimos algumas perguntas que gostaríamos de responder com este trabalho, como: Qual o primeiro tweet relatando falta de oxigênio ou pedindo ajuda? Quais as reações diante das medidas do governo, da chegada de oxigênio, da elevação de casos e mortes?

### Origem dos dados
* **Google**: com uso de operadores de busca avançada, pesquisamos as primeiras notícias que saíram a respeito da crise de oxigênio em Manaus e fatos relacionados à ela. Demos preferência a um jornal local do Amazonas ([A Crítica](https://www.acritica.com/)). Os resultados das buscas podem ser vistos [nesta pasta](https://github.com/biamuniz/trabalhofinal_osint/tree/main/dados_e_codigo);
* **Twitter**: por meio da ferramenta de pesquisa avançada, buscamos tweets relacionados a falta de oxigênio, reações aos decretos do governar do estado do Amazonas, pedidos de ajuda. A busca `oxigênio manaus until:2021-02-01 since:2021-01-01 -filter:replies` foi realizada inicialmente com a busca avançada do twitter e posteriormente com código em Python. A busca de tweets direcionados ao perfil do governador do Amazonas após os decretos de lockdown no dia 23/12 `(to:wilsonlimaam) until:2020-12-24 since:2020-12-23` também foi feita através da ferramenta de pesquisa do próprio twitter. O código utilizado, bem como os tweets coletados na primeira query podem ser vistos [nesta pasta](https://github.com/biamuniz/trabalhofinal_osint/tree/main/dados_e_codigo);
* **Facebook**: Usamos a ferramenta Crowdtangle para verificar qual foi a evolução das postagens e das interações no Facebook. Fizemos a pesquisa pelos termos `oxigênio AND Manaus`, de primeiro a 31 de janeiro de 2021. Mais informações, no [link](https://github.com/biamuniz/trabalhofinal_osint/blob/main/dados_e_codigo/facebook_analise.md).
* **Youtube**: Com o YouTube Datatools e YouTube Geofind, pesquisamos vídeos com a query `oxigênio manaus` e vídeos georreferenciados em um período específico. Mais detalhes, [aqui](https://github.com/biamuniz/trabalhofinal_osint/blob/main/dados_e_codigo/YouTube.md)

### Ferramentas e técnicas de OSINT utilizadas
* Captura de tela com a extensão [Awesome Screenshot & Screenrecorder](https://chrome.google.com/webstore/detail/awesome-screenshot-screen/nlipoenfbbikpbjkfpfillcgkoblgpmj?hl=pt-BR)
* CrowdTangle
* [Timeline, do KnightLab](https://timeline.knightlab.com/) para a visualização das informações
* [YouTube DataTools](https://tools.digitalmethods.net/netvizz/youtube/)
* [Youtube Geofinder](https://mattw.io/youtube-geofind/location)
* Verificação Geográfica: usada para conferir locais dos vídeos em Manaus;
* Verificação Cronológica: usada para verificar o momento em que os vídeos foram feitos (se foram realmente feitos no período da crise do oxigênio).

### Resultado

[Timeline com tweets, vídeos, notícias e posts](https://cdn.knightlab.com/libs/timeline3/latest/embed/index.html?source=1rSdCUTY3X_lSa7BlqKDsLKcJ1haucr5LO2nKXBtFhTM&font=Default&lang=pt-br&initial_zoom=2&height=650)

![Alt text](https://raw.githubusercontent.com/biamuniz/trabalhofinal_osint/main/media_timeline/TimelineJS-Embed.png)
