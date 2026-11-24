# Nome do Exame - Guia de Implementação do Resultado de Exame Laboratorial (REL) da RNDS v1.0.0

## ValueSet: Nome do Exame 

 **References** 

* [Diagnóstico em Laboratório Clínico](StructureDefinition-BRDiagnosticoLaboratorioClinico-3.2.1.md)

### Definição lógica (CLD)

 

### Expansão

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BRNomeExame-2.0",
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRNomeExame-2.0",
  "version" : "1.0.0",
  "name" : "BRNomeExame",
  "title" : "Nome do Exame",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-26T13:20:23.3537413+00:00",
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
  "description" : "Classifica o exame laboratorial realizado.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRNomeExameLOINC"
    },
    {
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRNomeExameGAL"
    }]
  }
}

```
