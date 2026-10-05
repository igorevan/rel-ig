# Patógeno (StructureDefinition) - Guia de Implementação do Resultado de Exame Laboratorial (REL) da RNDS v1.0.0-release

## Extension: Patógeno (StructureDefinition) 

**Context of Use**

**Usage info**

**Usos:**

* Usa este Extensão: [Diagnóstico em Laboratório Clínico](StructureDefinition-BRDiagnosticoLaboratorioClinico-3.2.1.md)
* Exemplos para este Extensão: [Bundle/example-bundle-rel-gal](Bundle-example-bundle-rel-gal.md) and [Bundle/example-bundle-rel-loinc](Bundle-example-bundle-rel-loinc.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/br.gov.saude.rel.fhir|current/StructureDefinition/StructureDefinition-BRPatogeno.json)

### Formal Views of Extension Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-BRPatogeno.csv), [Excel](../StructureDefinition-BRPatogeno.xlsx), [Schematron](../StructureDefinition-BRPatogeno.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "BRPatogeno",
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
  "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRPatogeno",
  "version" : "1.0.0-release",
  "name" : "BRPatogeno",
  "title" : "Patógeno (StructureDefinition)",
  "status" : "active",
  "date" : "2022-09-19",
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
  "description" : "Extensão para inserção dos termos relacionados ao Patógeno identificado.",
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
  }],
  "kind" : "complex-type",
  "abstract" : false,
  "context" : [{
    "type" : "element",
    "expression" : "Observation"
  }],
  "type" : "Extension",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Extension",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "Extension.url",
      "path" : "Extension.url",
      "fixedUri" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRPatogeno"
    },
    {
      "id" : "Extension.value[x]",
      "path" : "Extension.value[x]",
      "type" : [{
        "code" : "CodeableConcept"
      }],
      "binding" : {
        "strength" : "required",
        "description" : "terminologia Patogeno",
        "valueSet" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRTerminologiaPatogeno"
      }
    }]
  }
}

```
