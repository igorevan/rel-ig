# Amostra Biológica - Guia de Implementação do Resultado de Exame Laboratorial (REL) da RNDS v1.0.0-release

## Resource Profile: Amostra Biológica 

 
Amostra de origem humana/animal usada em investigações biológicas/laboratoriais para fins diagnósticos. 

**Usos:**

* Refere a este Perfil: [Diagnóstico em Laboratório Clínico](StructureDefinition-BRDiagnosticoLaboratorioClinico-3.2.1.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/br.gov.saude.rel.fhir|current/StructureDefinition/StructureDefinition-BRAmostraBiologica-1.0.json)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-BRAmostraBiologica-1.0.csv), [Excel](../StructureDefinition-BRAmostraBiologica-1.0.xlsx), [Schematron](../StructureDefinition-BRAmostraBiologica-1.0.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "BRAmostraBiologica-1.0",
  "meta" : {
    "lastUpdated" : "2020-03-26T13:02:05.548+00:00"
  },
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
  "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRAmostraBiologica-1.0",
  "version" : "1.0.0-release",
  "name" : "BRAmostraBiologica",
  "title" : "Amostra Biológica",
  "status" : "active",
  "date" : "2020-03-26T13:02:02.6493634+00:00",
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
  "description" : "Amostra de origem humana/animal usada em investigações biológicas/laboratoriais para fins diagnósticos.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "fhirVersion" : "4.0.1",
  "mapping" : [{
    "identity" : "rim",
    "uri" : "http://hl7.org/v3",
    "name" : "RIM Mapping"
  },
  {
    "identity" : "w5",
    "uri" : "http://hl7.org/fhir/fivews",
    "name" : "FiveWs Pattern Mapping"
  },
  {
    "identity" : "v2",
    "uri" : "http://hl7.org/v2",
    "name" : "HL7 v2 Mapping"
  }],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Specimen",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Specimen",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "Specimen",
      "path" : "Specimen",
      "short" : "Amostra Biológica",
      "definition" : "Amostra de origem humana/animal usada em investigações biológicas/laboratoriais para fins diagnósticos.",
      "mustSupport" : true
    },
    {
      "id" : "Specimen.identifier",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.identifier",
      "max" : "0"
    },
    {
      "id" : "Specimen.identifier.use",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.identifier.use",
      "max" : "0"
    },
    {
      "id" : "Specimen.accessionIdentifier",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.accessionIdentifier",
      "max" : "0"
    },
    {
      "id" : "Specimen.status",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.status",
      "max" : "0"
    },
    {
      "id" : "Specimen.type",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.type",
      "short" : "Tipo da Amostra",
      "definition" : "Tipo do material da amostra.",
      "min" : 1,
      "mustSupport" : true,
      "binding" : {
        "strength" : "required",
        "description" : "Tipo da Amostra",
        "valueSet" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRTipoAmostra-1.0"
      }
    },
    {
      "id" : "Specimen.type.coding",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.type.coding",
      "min" : 1,
      "max" : "1"
    },
    {
      "id" : "Specimen.type.coding.system",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.type.coding.system",
      "min" : 1
    },
    {
      "id" : "Specimen.type.coding.code",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.type.coding.code",
      "min" : 1
    },
    {
      "id" : "Specimen.type.coding.display",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/elementdefinition-translatable",
        "valueBoolean" : true
      }],
      "path" : "Specimen.type.coding.display",
      "max" : "0"
    },
    {
      "id" : "Specimen.type.coding.userSelected",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.type.coding.userSelected",
      "max" : "0"
    },
    {
      "id" : "Specimen.type.text",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/elementdefinition-translatable",
        "valueBoolean" : true
      }],
      "path" : "Specimen.type.text",
      "max" : "0"
    },
    {
      "id" : "Specimen.subject",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.subject",
      "max" : "0"
    },
    {
      "id" : "Specimen.receivedTime",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.receivedTime",
      "max" : "0"
    },
    {
      "id" : "Specimen.parent",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.parent",
      "max" : "0"
    },
    {
      "id" : "Specimen.request",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.request",
      "max" : "0"
    },
    {
      "id" : "Specimen.collection",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.collection",
      "max" : "0"
    },
    {
      "id" : "Specimen.processing",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.processing",
      "max" : "0"
    },
    {
      "id" : "Specimen.container",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.container",
      "max" : "0"
    },
    {
      "id" : "Specimen.condition",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.condition",
      "max" : "0"
    },
    {
      "id" : "Specimen.note",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "Specimen.note",
      "max" : "0"
    }]
  }
}

```
