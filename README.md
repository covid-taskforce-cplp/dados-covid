# Fontes de dados sobre COVID-19 na CPLP, `dados-v1`
**Referências de APIs para aplicações relacionadas ao Coronavirus COVID-19. Foco
na CPLP - Comunidade dos Países de Língua Portuguesa:** Angola 🇦🇴, Brasil 🇧🇷,
Cabo Verde 🇨🇻, Guiné Equatorial 🇬🇶, Guiné-Bissau 🇬🇼, Macau 🇲🇴,
Moçambique 🇲🇿, Portugal 🇵🇹, São Tomé e Príncipe 🇵🇹 e Timor-Leste 🇹🇱.

Para ver apenas dados criados especialmente pelo
[@covid-taskforce-cplp](https://github.com/covid-taskforce-cplp) acesse a pasta
[/dados-v1/data/](data/).

----

<!-- TOC depthFrom:2 depthTo:5 -->

- [Fontes de dados, por tema](#fontes-de-dados-por-tema)
    - [Casos de COVID-19](#casos-de-covid-19)
        - [Global](#global)
            - [NovelCOVID/API](#novelcovidapi)
        - [Brasil](#brasil)
            - [brasil.io](#brasilio)
            - [covid.saude.gov.br](#covidsaudegovbr)
    - [Hospitais](#hospitais)
    - [TODO: Fontes de dados a serem documentadas](#todo-fontes-de-dados-a-serem-documentadas)
- [Ferramentas de Apoio](#ferramentas-de-apoio)
    - [Para debugar APIs](#para-debugar-apis)
        - [postwoman.io](#postwomanio)
        - [postman](#postman)
        - [insomnia.rest](#insomniarest)

<!-- /TOC -->

----
<!--
  ## TL;DR:
**Enquanto este repositório não está mais organizado recomendamos que para dados
a nível internacional use <https://covid-19-apis.postman.com/> e, para dados
específicos do Brasil, use <https://brasil.io/dataset/covid19/>.**
-->

## Fontes de dados, por tema

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
  tempo tentando minerar os dados do covid.saude.gov.br.

##### brasil.io
- **Painel**: <https://brasil.io/api/dataset/covid19>
- **Documentação API**: <https://brasil.io/dataset/covid19/caso>
- **GitHub**: <https://github.com/turicas/covid19-br>

##### covid.saude.gov.br
- **GitHub**: Não aplicável
- **Painel**: <https://covid.saude.gov.br/>

### Hospitais

(...)

### TODO: Fontes de dados a serem documentadas

- <https://datasus.saude.gov.br/>
- <https://brasil.io/dataset/covid19/caso>
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
