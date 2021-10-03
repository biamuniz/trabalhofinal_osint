# trabalhofinal_osint
_Repositório para documentar o trabalho final da disciplina Open Source Intelligence, do Master em Jornalismo de Dados, Automação e Data Storytelling do Insper_

**Grupo:** [Bianca Muniz](https://github.com/biamuniz), [Meyrele Torres](https://github.com/meyrele), Ricardo Grinbaum

## Objetivo
Recriar a cronologia dos acontecimentos que culminaram na crise de oxigênio em Manaus usando técnicas de OSINT

## Metodologia
Antes de começar, definimos algumas perguntas que gostaríamos de responder com este trabalho, como: Qual o primeiro tweet relatando falta de oxigênio ou pedindo ajuda? Quais as reações diante das medidas do governo, da chegada de oxigênio, da elevação de casos e mortes?

### Origem dos dados
* **Google**: com uso de operadores de busca, pesquisamos as primeiras notícias que saíram a respeito da crise de oxigênio Manaus e fatos relacionados à crise. Demos preferência a um jornal local do Amazonas ([A Crítica](https://www.acritica.com/)). Os resultados das buscas podem ser vistos nesta pasta;
* **Twitter**: por meio da ferramenta de pesquisa avançada, buscamos tweets relacionados a falta de oxigênio, reações aos decretos do governar do estado do Amazonas, pedidos de ajuda. A busca `oxigênio manaus until:2021-02-01 since:2021-01-01 -filter:replies` foi realizada com código em Python. A busca de weets direcionados ao perfil do governador do Amazonas após os decretos de lockdown no dia 23/12 `(to:wilsonlimaam) until:2020-12-24 since:2020-12-23` foi feita através da ferramenta de pesquisa do próprio twitter. O código utilizado, bem como os tweets coletados na primeira query podem ser vistos [nesta pasta](https://github.com/biamuniz/trabalhofinal_osint/tree/main/dados_e_codigo);
* **Facebook**: Usamos a ferramenta Crowdtangle para verificar qual foi a evolução das postagens e das interações no Facebook. Fizemos a pesquisa pelos termos `oxigênio AND Manaus`, de primeiro a 31 de janeiro de 2021. Mais informações, no link.
* **Youtube**:

### Ferramentas e técnicas de OSINT utilizadas
* Captura de tela com a extensão [Awesome Screenshot & Screenrecorder](https://chrome.google.com/webstore/detail/awesome-screenshot-screen/nlipoenfbbikpbjkfpfillcgkoblgpmj?hl=pt-BR)
* Crowdtangle
* [Timeline, do KnightLab](https://timeline.knightlab.com/) para a visualização das informações
* [YouTube DataTools](https://tools.digitalmethods.net/netvizz/youtube/)
* Youtube Geofinder
* Verificação Geográfica: usada para conferir locais dos vídeos em Manaus;
* Verificação Cronológica: usada para verificar o momento em que os vídeos foram feitos (se foram realmente feitos no período da crise do oxigênio).


