# Categoria do Exame - Guia de Implementação do Resultado de Exame Laboratorial (REL) da RNDS v1.0.0

## ValueSet: Categoria do Exame 

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
  "id" : "BRCategoriaExame-1.0",
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRCategoriaExame-1.0",
  "version" : "1.0.0",
  "name" : "BRCategoriaExame",
  "title" : "Categoria do Exame",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-26T13:20:04.5290649+00:00",
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
  "description" : "Categoriza exames ou testes utilizando os subgrupos do grupo 02 - Procedimentos com finalidade diagnóstica da Tabela SUS.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRSubgrupoTabelaSUS"
    }]
  }
}

```
