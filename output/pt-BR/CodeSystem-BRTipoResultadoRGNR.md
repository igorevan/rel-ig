# Tipo de Resultado (RGNR) - Guia de Implementação do Resultado de Exame Laboratorial (REL) da RNDS v1.0.0

## CodeSystem: Tipo de Resultado (RGNR) 

Este sistema de códigos é referenciado na definição dos seguintes conjuntos de valores:

* [Resultado Qualitativo do Exame 2.0 (ValueSet)](ValueSet-BRResultadoQualitativoExame-2.0.md)

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRTipoResultadoRGNR",
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoResultadoRGNR",
  "version" : "1.0.0",
  "name" : "BRTipoResultadoRGNR",
  "title" : "Tipo de Resultado (RGNR)",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-26T13:16:09.8385573+00:00",
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
  "description" : "Code System utilizado para definir o valor atribuído ao resultado de um exame laboratorial realizado por método de análise qualitativo com o tipo de resultado RGNR.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "1",
    "display" : "Reagente"
  },
  {
    "code" : "2",
    "display" : "Não Reagente"
  },
  {
    "code" : "3",
    "display" : "Indeterminado"
  }]
}

```
