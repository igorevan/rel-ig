# Patógeno (ValueSet) - Guia de Implementação do Resultado de Exame Laboratorial (REL) da RNDS v1.0.0

## ValueSet: Patógeno (ValueSet) 

 **References** 

* [Patógeno (StructureDefinition)](StructureDefinition-BRPatogeno.md)

### Definição lógica (CLD)

 

### Expansão

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BRTerminologiaPatogeno",
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRTerminologiaPatogeno",
  "version" : "1.0.0",
  "name" : "BRTerminologiaPatogeno",
  "title" : "Patógeno (ValueSet)",
  "status" : "active",
  "experimental" : false,
  "date" : "2022-09-16T14:11:40.0457007+00:00",
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
  "description" : "Conjunto de terminologias para indicação do Patógeno.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTerminologiaPatogeno"
    }]
  }
}

```
