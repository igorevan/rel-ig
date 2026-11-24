# Suspeita Diagnóstica (CodeSystem) - Guia de Implementação do Resultado de Exame Laboratorial (REL) da RNDS v1.0.0

## CodeSystem: Suspeita Diagnóstica (CodeSystem) 

Este sistema de códigos é referenciado na definição dos seguintes conjuntos de valores:

* [Suspeita Diagnóstica](ValueSet-BRTerminologiaSuspeitaDiagnostica.md)

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRTerminologiaSuspeitaDiagnostica",
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTerminologiaSuspeitaDiagnostica",
  "version" : "1.0.0",
  "name" : "BRTerminologiaSuspeitaDiagnostica",
  "title" : "Suspeita Diagnóstica (CodeSystem)",
  "status" : "active",
  "experimental" : false,
  "date" : "2022-09-16T14:16:40.0457007+00:00",
  "publisher" : "Ministério da Saúde do Brasil",
  "contact" : [{
    "name" : "Ministério da Saúde do Brasil",
    "telecom" : [{
      "system" : "url",
      "value" : "http://www.saude.gov.br"
    },
    {
      "system" : "email",
      "value" : "cgiis.datasus@saude.gov.br"
    }]
  }],
  "description" : "Terminologia para indicação de uma Suspeita Diagnóstica.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "B04",
    "display" : "Varíola dos macacos [Monkeypox]"
  },
  {
    "code" : "B342",
    "display" : "Infecção por coronavírus de localização não especificada"
  }]
}

```
