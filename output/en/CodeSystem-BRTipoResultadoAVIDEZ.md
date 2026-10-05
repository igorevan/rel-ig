# Tipo de Resultado (AVIDEZ) - Guia de Implementação do Resultado de Exame Laboratorial (REL) da RNDS v1.0.0-release

## CodeSystem: Tipo de Resultado (AVIDEZ) 

This Code system is referenced in the definition of the following value sets:

* [Resultado Qualitativo do Exame 2.0 (ValueSet)](ValueSet-BRResultadoQualitativoExame-2.0.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRTipoResultadoAVIDEZ",
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
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoResultadoAVIDEZ",
  "version" : "1.0.0-release",
  "name" : "BRTipoResultadoAVIDEZ",
  "title" : "Tipo de Resultado (AVIDEZ)",
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
  "description" : "Code System utilizado para definir o valor atribuído ao resultado de um exame laboratorial realizado por método de análise qualitativo com o tipo de resultado AVIDEZ.",
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
    "display" : "Baixa Avidez"
  },
  {
    "code" : "2",
    "display" : "Alta Avidez"
  },
  {
    "code" : "3",
    "display" : "Indeterminado"
  }]
}

```
