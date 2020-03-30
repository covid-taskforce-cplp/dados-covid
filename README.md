# Dados para aplicações relacionadas a COVID-19 na CPLP, `dados-v1`
**Referências de APIs e conjuntos de dados para aplicações relacionadas ao
Coronavirus COVID-19. Foco na CPLP - Comunidade dos Países de Língua
Portuguesa:** Angola 🇦🇴, Brasil 🇧🇷, Cabo Verde 🇨🇻, Guiné Equatorial 🇬🇶,
Guiné-Bissau 🇬🇼, Macau 🇲🇴, Moçambique 🇲🇿, Portugal 🇵🇹, São Tomé e Príncipe
🇵🇹 e Timor-Leste 🇹🇱.

**Para pré-visualisar com DataPackage Viewer os dados criados especialmente
pelo [@covid-taskforce-cplp](https://github.com/covid-taskforce-cplp) acesse <https://data.okfn.org/tools/view?url=https%3A%2F%2Fgithub.com%2Fcovid-taskforce-cplp%2Fdados-v1>**

----

<!-- TOC depthFrom:2 depthTo:5 -->

- [APIs](#apis)
    - [Casos de COVID-19](#casos-de-covid-19)
        - [Global](#global)
            - [NovelCOVID/API](#novelcovidapi)
        - [Brasil](#brasil)
            - [brasil.io](#brasilio)
    - [Glossario (*)](#glossario-)
    - [População, por faixa de idade (*)](#população-por-faixa-de-idade-)
- [Fontes de informação, outros](#fontes-de-informação-outros)
    - [datasus.saude.gov.br](#datasussaudegovbr)
    - [Por documentar](#por-documentar)
- [Ferramentas de Apoio](#ferramentas-de-apoio)
    - [Para debugar APIs](#para-debugar-apis)
        - [postwoman.io](#postwomanio)
        - [postman](#postman)
        - [insomnia.rest](#insomniarest)
    - [Extensões para o VSCode](#extensões-para-o-vscode)
        - [RandomFractalsInc.vscode-data-preview](#randomfractalsincvscode-data-preview)
        - [khaeransori.json2csv](#khaeransorijson2csv)

<!-- /TOC -->

----
<!--
  ## TL;DR:
**Enquanto este repositório não está mais organizado recomendamos que para dados
a nível internacional use <https://covid-19-apis.postman.com/> e, para dados
específicos do Brasil, use <https://brasil.io/dataset/covid19/>.**
-->

## APIs

### Casos de COVID-19
> **Nossa recomendação padrão**: construa APIs usando uma opção que tenha dados
  a nível global, e então (casos exista) adicione mais detalhes com uma API
  que tenha detalhes do respectivo país.

#### Global

##### NovelCOVID/API
- **GitHub**: <https://github.com/NovelCOVID/API>
- **Painel**: Não aplicável
- **Documentação API**: <https://documenter.getpostman.com/view/8854915/SzS7R6uu?version=latest>
- **Funcionalidades**:
  - Casos confirmados de COVID-19
  - Mortes confirmadas de COVID-19
  - Histórico ao longo do tempo
  - Nível de detalhamento:
    - Nível de país
    - (Algumas regiões apenas) nível de província/estado/unidade federativa
      - Nenhum país da CPLP tem informações em nível mais detalhado do que de país

#### Brasil

> **Nossa recomendação padrão (2020-03-30)**: use a API do brasil.io e não perca
  tempo tentando minerar os dados do <https://covid.saude.gov.br/>.

##### brasil.io
- **Painel**: <https://brasil.io/api/dataset/covid19>
- **Documentação API**: <https://brasil.io/dataset/covid19/caso>
- **GitHub**: <https://github.com/turicas/covid19-br>

<!--
 ##### covid.saude.gov.br
- **GitHub**: Não aplicável
- **Painel**: <https://covid.saude.gov.br/>
-->

### Glossario (*)

> Potencialmente converter um ou mais dos seguintes recursos para .csv/.json e
> dar créditos às fontes:
> - <https://www.kff.org/glossary/covid-19-outbreak-glossary/>
> - <https://www.rochester.edu/coronavirus-update/terminology/>
> - <https://www.cbc.ca/news/health/covid19-glossary-1.5510230>
> - <https://www.google.com/search?q=covid+glossary>


### População, por faixa de idade (*)
> Não implementado

## Fontes de informação, outros

### datasus.saude.gov.br
- **Site**: <https://datasus.saude.gov.br/>

### Por documentar

- <https://datasus.saude.gov.br/>
- <https://ourworldindata.org/coronavirus>
- <http://data.un.org/Host.aspx?Content=API>
- <https://data.humdata.org/>
  - <https://hxlstandard.org/>
- <https://covid-19-apis.postman.com/>
- <https://github.com/dadosgovbr/catalogos-dados-brasil>

<!--
- https://github.com/github/covid19-dashboard
-->

## Ferramentas de Apoio
**AVISO: as ferramentas citadas aqui são uma sugestão baseada em opinião pessoal
de uso de ferramentas que podem ser úteis caso você já não tenha algun fluxo de
trabalho (usando ou não aplicativos) para certos tipos de ações**.

<!--
https://github.com/frictionlessdata/datapackage-js
-->

### Para debugar APIs
<!-- https://techbeacon.com/app-dev-testing/11-top-open-source-api-testing-tools-what-your-team-needs-know -->

#### postwoman.io
- Site: <https://postwoman.io/>

Alternativa ao Postman. Não precisa ser instalado. Pode ser acessado diretamente
do website https://postwoman.io/.

#### postman
- Site: <https://www.postman.com/>

Ferramenta popular para testar APIs. Requer instalação e criar conta.

#### insomnia.rest
- Site: <https://insomnia.rest/>

Alternativa ao Postman.

### Extensões para o VSCode

#### RandomFractalsInc.vscode-data-preview
- **GitHub**: <https://github.com/RandomFractals/vscode-data-preview>
- **Market Place**: <https://marketplace.visualstudio.com/items?itemName=RandomFractalsInc.vscode-data-preview>
- **Comando para instalar (Ctrl + P)**: `ext install RandomFractalsInc.vscode-data-preview`

#### khaeransori.json2csv
- **GitHub**: <https://github.com/khaeransori/vscode-json2csv>
- **Market Place**: <https://marketplace.visualstudio.com/items?itemName=khaeransori.json2csv>
- **Comando para instalar (Ctrl + P)**: `ext install khaeransori.json2csv`

Uso: 
- com um arquivo CSV aberto, aperte `F1` e escolha _Convert JSON to CSV_
- com um arquivo JSON aberto, aperte `F1` e escolha _Convert CSV to JSON_
 
<!--
  # TODO
- ~Implementar Data Package format <https://frictionlessdata.io/data-packages/>~
  - https://frictionlessdata.io/specs/data-package/
  - https://data.okfn.org/tools/view
-->
