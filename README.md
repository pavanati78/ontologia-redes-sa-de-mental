# Ontologia – Impacto das Redes Sociais na Saúde Mental

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC--BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

Este repositório disponibiliza uma ontologia OWL sobre o impacto das redes sociais na saúde mental. Ela foi desenvolvida para apoiar pesquisa, ensino e integração em cenários de Linked Data, especialmente envolvendo análise de fatores de risco, proteção e sintomas relacionados ao uso de mídias digitais.

## 📘 Visão Geral

A ontologia modela conceitos centrais do domínio, como tipos de usuários, sintomas de saúde mental (com subclasses), tipos de eventos (cyberbullying, campanhas de prevenção), fatores de risco (uso excessivo, cyberdependência), fatores protetivos (educação digital, grupos de apoio), tipos de interação, serviços de apoio e as principais redes sociais. Todas as definições são bilíngues (pt-br/en).

## 🌐 Estrutura

### Principais Classes e Subclasses
- **Usuário** (`Usuario`)
  - [`Adolescente`, `Adulto`, `AdultoJovem`]
- **Rede Social** (`RedeSocial`)
  - [`Facebook`,`Instagram`,`TikTok`,`WhatsApp`,`YouTube`]
- **Interação** (`Interacao`)
  - [`Curtir`,`Comentar`,`Compartilhar`,`Postar`]
- **Sintoma Mental** (`SintomaMental`)
  - [`Ansiedade`,`BaixaAutoestima`,`Depressao`,`Estresse`,`IsolamentoSocial`,`Nomofobia`]
- **Evento** (`Evento`)
  - [`Cyberbullying`,`ExposicaoNegativa`,`CampanhaSaudeMental`,`ParticipacaoGrupo`]
- **Fator de Risco** (`FatorRisco`)
  - [`UsoExcessivo`,`ConteudoNegativo`,`CyberDependencia`,`IsolamentoVirtual`,`ExperienciaNegativa`,`Fomo`]
- **Fator Protetivo** (`FatorProtetivo`)
  - [`LimiteUso`,`EducacaoDigital`,`GruposDeApoio`,`InteracaoSaudavel`]
- **Serviço de Apoio** (`ServicoApoio`)
  - [`CVV`,`TerapiaOnline`,`Caps`,`GrupoApoioOnline`]

### Propriedades Objetais
- `utiliza` (Usuário → Rede Social)
- `realiza` (Usuário → Interação)
- `apresenta` (Usuário → Sintoma Mental)
- `sofre` (Usuário → Evento)
- `busca` (Usuário → Serviço de Apoio)
- `temFatorProtetivo` (Usuário → Fator Protetivo)
- `temFatorRisco` (Usuário → Fator de Risco)

### Propriedades de Dados
- `idade`, `tempoDeUsoDiario` (Usuário)
- `dataEvento` (Evento)
- `frequenciaApoio` (Serviço de Apoio)
- `nivelGravidade` (Sintoma Mental)

### Indivíduos de Exemplo
- `usuariojoao` - adolescente que utiliza Instagram, apresenta Ansiedade, sofreu Cyberbullying, busca Terapia Online, pertence a Grupos de Apoio e tem como fator de risco Uso Excessivo.

## 📝 Anotações (Annotations)
Todas as classes principais têm rótulos (`rdfs:label`) e descrições (`dc:description`) em pt-br e inglês. Para cada conceito, são fornecidas referências em `rdfs:seeAlso` para normas (CID-10/DSM-V), materiais da APA, OMS, etc.

---

## 📦 Como usar

1. **Abra o arquivo .owl ou .ttl no Protégé ou WebProtégé.**
2. Explore a hierarquia e as anotações para cada classe, propriedade e indivíduo.
3. Utilize ou adapte a estrutura conforme sua necessidade acadêmica, de pesquisa ou integração Linked Data.

---

## 🛰️ Aplicações

- Pesquisas em ciências sociais e saúde digital.
- Ensino de ontologias, Semantic Web e Linked Data.
- Base para sistemas de apoio à decisão em saúde mental.
- Estruturar gráficos de conhecimento (knowledge graph) sobre usuários, sintomas e redes sociais.

#### Exemplo de visualização no WebVOWL:
[Visualize sua ontologia no WebVOWL](http://www.visualdataweb.de/webvowl/)

---

## 📜 Licença

Distribuída sob a licença [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

---

## 🖋️ Referências

- CID-10: https://icd.who.int/
- DSM-V: https://www.psychiatry.org/psychiatrists/practice/dsm
- APA: https://www.apa.org/

---

# Social Media Impact on Mental Health Ontology

This repository contains an OWL ontology about social networks' impact on mental health, modeled for research, education, and Linked Data scenarios.

**See above for structure, main classes, properties, and usage instructions. All concepts and descriptions are in both Portuguese and English.**

---

*Developed for academic purposes. Please cite this repository if you use or adapt the ontology.*

