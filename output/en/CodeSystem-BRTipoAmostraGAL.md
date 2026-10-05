# Tipo de Amostra Biológica - Guia de Implementação do Resultado de Exame Laboratorial (REL) da RNDS v1.0.0-release

## CodeSystem: Tipo de Amostra Biológica 

This Code system is referenced in the definition of the following value sets:

* [Tipo de Amostra de Exame](ValueSet-BRTipoAmostra-1.0.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRTipoAmostraGAL",
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
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoAmostraGAL",
  "version" : "1.0.0-release",
  "name" : "BRTipoAmostraGAL",
  "title" : "Tipo de Amostra Biológica",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-06-09T14:39:37.7113823+00:00",
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
  "description" : "Classifica o tipo de amostra biológica utilizada em exames de acordo com a terminologia Gerenciador de Ambiente Laboratorial (GAL).",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "SECONF",
    "display" : "Secreção Orofaríngea e Nasofaríngea"
  },
  {
    "code" : "SNOF",
    "display" : "Swab Naso-Orofaríngeo"
  },
  {
    "code" : "SWNAFA",
    "display" : "Swab Nasofaríngeo"
  },
  {
    "code" : "SWAB",
    "display" : "Swab"
  },
  {
    "code" : "SECNAS",
    "display" : "Secreção Nasofaríngea"
  },
  {
    "code" : "ASNAFA",
    "display" : "Aspirado Nasofaríngeo"
  },
  {
    "code" : "SWORO",
    "display" : "Swab Orofaríngeo"
  },
  {
    "code" : "SWNAS",
    "display" : "Swab Nasal"
  },
  {
    "code" : "SECORF",
    "display" : "Secreção Orofaríngea"
  },
  {
    "code" : "LAVBRA",
    "display" : "Lavado Brônquico Alveolar"
  },
  {
    "code" : "LAVBRO",
    "display" : "Lavado Brônquico"
  },
  {
    "code" : "CORIZA",
    "display" : "Coriza"
  },
  {
    "code" : "EXSNAS",
    "display" : "Exsudato de Nasofaringe"
  },
  {
    "code" : "ASPBRO",
    "display" : "Aspirado Brônquico"
  },
  {
    "code" : "LAVTBR",
    "display" : "Lavado Traqueo-Brônquico"
  },
  {
    "code" : "SECTRA",
    "display" : "Secreção Traqueal"
  },
  {
    "code" : "EXSORO",
    "display" : "Exsudato de Orofaringe"
  },
  {
    "code" : "FGMP",
    "display" : "Fragmentos do pulmão"
  },
  {
    "code" : "FGMT",
    "display" : "Fragmento"
  },
  {
    "code" : "FLUORA",
    "display" : "Fluido oral"
  },
  {
    "code" : "FRAAMI",
    "display" : "Fragmentos de ampigdalas"
  },
  {
    "code" : "FRABAC",
    "display" : "Fragmentos de baço"
  },
  {
    "code" : "FRACOR",
    "display" : "Fragmentos de coração"
  },
  {
    "code" : "FRAFIG",
    "display" : "Fragmentos de fígado"
  },
  {
    "code" : "FRAGT",
    "display" : "Fragmento de tecido"
  },
  {
    "code" : "FRAMOR",
    "display" : "Fragmentos de múltiplos órgãos"
  },
  {
    "code" : "FRAPAN",
    "display" : "Fragmentos de pâncreas"
  },
  {
    "code" : "FRARIM",
    "display" : "Fragmentos de rim"
  },
  {
    "code" : "FRATRA",
    "display" : "Fragmentos de traquéia"
  },
  {
    "code" : "FRBRON",
    "display" : "Fragmentos de brônquio"
  },
  {
    "code" : "INFP",
    "display" : "Infiltrado pulmonar"
  },
  {
    "code" : "INODER",
    "display" : "Inoculação intradérmica"
  },
  {
    "code" : "LAVORO",
    "display" : "Lavado de orofaringe"
  },
  {
    "code" : "MTBIO",
    "display" : "Material Não Biológico"
  },
  {
    "code" : "SECBRO",
    "display" : "Secreção brônquica"
  },
  {
    "code" : "SECOC",
    "display" : "Secreção ocular"
  },
  {
    "code" : "SECPEN",
    "display" : "Secreção peniana"
  },
  {
    "code" : "SGEDT",
    "display" : "Sangue com EDTA"
  },
  {
    "code" : "SGHEM",
    "display" : "Sangue"
  },
  {
    "code" : "SNCCEB",
    "display" : "Fragmento do tecido do SNC - cérebro"
  },
  {
    "code" : "SWBAN",
    "display" : "Swab Anal"
  },
  {
    "code" : "SWOCU",
    "display" : "Swab Ocular"
  },
  {
    "code" : "SWRET",
    "display" : "Swab retal"
  },
  {
    "code" : "TECPM",
    "display" : "Tecido pós-mortem"
  },
  {
    "code" : "SWORA",
    "display" : "Swab Oral"
  },
  {
    "code" : "SWLES",
    "display" : "Swab de lesão"
  },
  {
    "code" : "SWLSP",
    "display" : "Swab de lesão de pele"
  },
  {
    "code" : "RASPEL",
    "display" : "Raspado de pele"
  },
  {
    "code" : "FRAPLA",
    "display" : "Fragmento de Placenta"
  },
  {
    "code" : "SGCUMB",
    "display" : "Sangue do Cordão Umbilical"
  },
  {
    "code" : "URIJ",
    "display" : "Urina 1º jato"
  }]
}

```
