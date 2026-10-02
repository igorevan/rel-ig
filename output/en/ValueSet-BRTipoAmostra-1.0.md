# Tipo de Amostra de Exame - Guia de Implementação do Resultado de Exame Laboratorial (REL) da RNDS v1.0.0-release

## ValueSet: Tipo de Amostra de Exame 

 
Tipo da amostra de um exame ou teste. 

 **References** 

* [Amostra Biológica](StructureDefinition-BRAmostraBiologica-1.0.md)

### Logical Definition (CLD)

 

### Expansion

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BRTipoAmostra-1.0",
  "language" : "en",
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
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRTipoAmostra-1.0",
  "version" : "1.0.0-release",
  "name" : "BRTipoAmostra",
  "title" : "Tipo de Amostra de Exame",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-06-30T18:56:47.6561959+00:00",
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
  "description" : "Tipo da amostra de um exame ou teste.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/v2-0487",
      "concept" : [{
        "code" : "FRS",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Fluido Respiratório"
        }]
      },
      {
        "code" : "LAVG",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Lavado Brônquico"
        }]
      },
      {
        "code" : "NSECR",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Secreção Nasal"
        }]
      },
      {
        "code" : "PLAS",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Plasma"
        }]
      },
      {
        "code" : "SPT",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Escarro"
        }]
      },
      {
        "code" : "TASP",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Aspirado Traqueal"
        }]
      },
      {
        "code" : "WB",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Sangue Total"
        }]
      },
      {
        "code" : "SER",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Soro"
        }]
      },
      {
        "code" : "SECRE",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Secreção Não Especificada"
        }]
      },
      {
        "code" : "ASP",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Aspirado Não Especificado"
        }]
      },
      {
        "code" : "SPUTIN",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Escarro induzido"
        }]
      },
      {
        "code" : "WASH",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Lavado"
        }]
      },
      {
        "code" : "CSF",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Líquor"
        }]
      },
      {
        "code" : "SAL",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Saliva"
        }]
      },
      {
        "code" : "UR",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Urina"
        }]
      }]
    },
    {
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoAmostraGAL"
    }]
  }
}

```
