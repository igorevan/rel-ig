# Condição de Saúde - Guia de Implementação do Resultado de Exame Laboratorial (REL) da RNDS v1.0.0-release

## Resource Profile: Condição de Saúde 

 
Contém os dados relacionados à condição de saúde ou condição alvo do paciente avaliado. 

**Usos:**

* Refere a este Perfil: [Resultado de Exame Laboratorial](StructureDefinition-BRResultadoExameLaboratorial-3.2.1.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/br.gov.saude.rel.fhir|current/StructureDefinition/StructureDefinition-BRCondicaoSaude.json)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-BRCondicaoSaude.csv), [Excel](../StructureDefinition-BRCondicaoSaude.xlsx), [Schematron](../StructureDefinition-BRCondicaoSaude.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "BRCondicaoSaude",
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
  "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRCondicaoSaude",
  "version" : "1.0.0-release",
  "name" : "BRCondicaoSaude",
  "title" : "Condição de Saúde",
  "status" : "active",
  "date" : "2022-09-16",
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
  "description" : "Contém os dados relacionados à condição de saúde ou condição alvo do paciente avaliado.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "fhirVersion" : "4.0.1",
  "mapping" : [{
    "identity" : "workflow",
    "uri" : "http://hl7.org/fhir/workflow",
    "name" : "Workflow Pattern"
  },
  {
    "identity" : "sct-concept",
    "uri" : "http://snomed.info/conceptdomain",
    "name" : "SNOMED CT Concept Domain Binding"
  },
  {
    "identity" : "v2",
    "uri" : "http://hl7.org/v2",
    "name" : "HL7 v2 Mapping"
  },
  {
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
    "identity" : "sct-attr",
    "uri" : "http://snomed.org/attributebinding",
    "name" : "SNOMED CT Attribute Binding"
  }],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Condition",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Condition",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "Condition",
      "path" : "Condition"
    },
    {
      "id" : "Condition.identifier",
      "path" : "Condition.identifier",
      "max" : "0"
    },
    {
      "id" : "Condition.clinicalStatus",
      "path" : "Condition.clinicalStatus",
      "max" : "0"
    },
    {
      "id" : "Condition.category",
      "path" : "Condition.category",
      "max" : "0"
    },
    {
      "id" : "Condition.severity",
      "path" : "Condition.severity",
      "max" : "0"
    },
    {
      "id" : "Condition.code",
      "path" : "Condition.code",
      "short" : "Suspeita Diagnóstica",
      "definition" : "Identifica a suspeita diagnóstica com relação à condição de saúde avaliado.",
      "min" : 1,
      "binding" : {
        "strength" : "required",
        "description" : "Terminologia de Suspeita Diagnósitca",
        "valueSet" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRTerminologiaSuspeitaDiagnostica"
      }
    },
    {
      "id" : "Condition.bodySite",
      "path" : "Condition.bodySite",
      "max" : "0"
    },
    {
      "id" : "Condition.subject",
      "path" : "Condition.subject",
      "short" : "Indivíduo com a Condição de Saúde avaliada",
      "definition" : "Referencia os dados sobre o indivíduo cuja a condição de saúde está sendo avaliada.",
      "type" : [{
        "code" : "Reference",
        "targetProfile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0"]
      }]
    },
    {
      "id" : "Condition.subject.identifier",
      "path" : "Condition.subject.identifier",
      "min" : 1
    },
    {
      "id" : "Condition.subject.identifier.system",
      "path" : "Condition.subject.identifier.system",
      "min" : 1
    },
    {
      "id" : "Condition.subject.identifier.value",
      "path" : "Condition.subject.identifier.value",
      "min" : 1
    },
    {
      "id" : "Condition.encounter",
      "path" : "Condition.encounter",
      "max" : "0"
    },
    {
      "id" : "Condition.onset[x]",
      "path" : "Condition.onset[x]",
      "max" : "0"
    },
    {
      "id" : "Condition.abatement[x]",
      "path" : "Condition.abatement[x]",
      "max" : "0"
    },
    {
      "id" : "Condition.recordedDate",
      "path" : "Condition.recordedDate",
      "max" : "0"
    },
    {
      "id" : "Condition.recorder",
      "path" : "Condition.recorder",
      "max" : "0"
    },
    {
      "id" : "Condition.asserter",
      "path" : "Condition.asserter",
      "max" : "0"
    },
    {
      "id" : "Condition.stage",
      "path" : "Condition.stage",
      "min" : 1
    },
    {
      "id" : "Condition.stage.assessment",
      "path" : "Condition.stage.assessment",
      "short" : "Diagnóstico de Laboratório Clínico",
      "definition" : "Referência aos dados de diagnóstico de laboratório clínico relacionados à suspeia diagnóstica.",
      "min" : 1,
      "type" : [{
        "code" : "Reference",
        "targetProfile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRDiagnosticoLaboratorioClinico-3.2.1"]
      }]
    },
    {
      "id" : "Condition.stage.assessment.reference",
      "path" : "Condition.stage.assessment.reference",
      "min" : 1
    },
    {
      "id" : "Condition.evidence",
      "path" : "Condition.evidence",
      "max" : "0"
    },
    {
      "id" : "Condition.note",
      "path" : "Condition.note",
      "max" : "0"
    }]
  }
}

```
