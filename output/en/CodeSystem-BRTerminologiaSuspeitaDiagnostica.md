# Suspeita Diagnóstica (CodeSystem) - Guia de Implementação do Resultado de Exame Laboratorial (REL) da RNDS v1.0.0-release

## CodeSystem: Suspeita Diagnóstica (CodeSystem) 

This Code system is referenced in the definition of the following value sets:

* Este CodeSystem não é utilizado aqui; pode ser utilizado noutro local (por exemplo, em especificações e/ou implementações que utilizem este conteúdo)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRTerminologiaSuspeitaDiagnostica",
  "language" : "pt-BR",
  "extension" : [{
    "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-wg",
    "valueCode" : "ehr"
  },
  {
    "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-fmm",
    "valueInteger" : 1,
    "_valueInteger" : {
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-conformance-derivedFrom",
        "valueCanonical" : "https://fhir.saude.gov.br/rel/ImplementationGuide/br.gov.saude.rel.fhir"
      }]
    }
  },
  {
    "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
    "valueCode" : "normative",
    "_valueCode" : {
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-conformance-derivedFrom",
        "valueCanonical" : "https://fhir.saude.gov.br/rel/ImplementationGuide/br.gov.saude.rel.fhir"
      }]
    }
  },
  {
    "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
    "valueCode" : "4.0.1"
  }],
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTerminologiaSuspeitaDiagnostica",
  "version" : "1.0.0-release",
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
