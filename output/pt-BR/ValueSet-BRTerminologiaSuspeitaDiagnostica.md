# Suspeita Diagnóstica - Guia de Implementação do Resultado de Exame Laboratorial (REL) da RNDS v1.0.0-release

## ValueSet: Suspeita Diagnóstica 

 **References** 

* [Condição de Saúde](StructureDefinition-BRCondicaoSaude.md)

### Definição lógica (CLD)

 

### Expansão

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
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
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRTerminologiaSuspeitaDiagnostica",
  "version" : "1.0.0-release",
  "name" : "BRTerminologiaSuspeitaDiagnostica",
  "title" : "Suspeita Diagnóstica",
  "status" : "active",
  "experimental" : false,
  "date" : "2026-10-01T14:11:40.0457007+00:00",
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
  "description" : "Conjunto de terminologias para indicação da Suspeita Diagnóstica.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRCID10",
      "concept" : [{
        "code" : "B342",
        "display" : "Infecção por coronavírus de localização não especificada"
      },
      {
        "code" : "B04",
        "display" : "Varíola dos macacos [Monkeypox]"
      },
      {
        "code" : "A90",
        "display" : "Dengue [dengue clássico]"
      },
      {
        "code" : "A928",
        "display" : "Outras febres virais especificadas transmitidas por mosquitos"
      },
      {
        "code" : "A938",
        "display" : "Outras febres virais especificadas transmitidas por artrópodes"
      },
      {
        "code" : "A920",
        "display" : "Febre de Chikungunya"
      },
      {
        "code" : "A95",
        "display" : "Febre amarela"
      },
      {
        "code" : "A950",
        "display" : "Febre amarela silvestre"
      },
      {
        "code" : "A951",
        "display" : "Febre amarela urbana"
      },
      {
        "code" : "A959",
        "display" : "Febre amarela não especificada"
      },
      {
        "code" : "A930",
        "display" : "Febre de oropouche"
      },
      {
        "code" : "A938",
        "display" : "Outras febres virais especificadas transmitidas por artrópodes"
      },
      {
        "code" : "A923",
        "display" : "Infecção pelo vírus West Nile"
      },
      {
        "code" : "J10",
        "display" : "Influenza devida a outro vírus da influenza [gripe] identificado"
      },
      {
        "code" : "J11",
        "display" : "Influenza (gripe) devida a vírus não identificado"
      },
      {
        "code" : "B974",
        "display" : "Vírus sincicial respiratório, como causa de doenças classificadas em outros capítulos"
      },
      {
        "code" : "B05",
        "display" : "Sarampo"
      },
      {
        "code" : "B059",
        "display" : "Sarampo sem complicação"
      },
      {
        "code" : "B06",
        "display" : "Rubéola"
      },
      {
        "code" : "P350",
        "display" : "Síndrome da rubéola congênita"
      },
      {
        "code" : "B01",
        "display" : "Varicela"
      },
      {
        "code" : "B03",
        "display" : "Varíola"
      },
      {
        "code" : "A37",
        "display" : "Coqueluche"
      },
      {
        "code" : "A379",
        "display" : "Coqueluche não especificada"
      },
      {
        "code" : "A36",
        "display" : "Difteria"
      },
      {
        "code" : "A369",
        "display" : "Difteria não especificada"
      },
      {
        "code" : "A00",
        "display" : "Cólera"
      },
      {
        "code" : "A009",
        "display" : "Cólera não especificada"
      },
      {
        "code" : "B24",
        "display" : "Doença pelo vírus da imunodeficiência humana [HIV] não especificada"
      },
      {
        "code" : "B20",
        "display" : "Doença pelo HIV resultando em doenças infecciosas e parasitárias"
      },
      {
        "code" : "Z114",
        "display" : "Exame especial de rastreamento de vírus da imunodeficiência humana [HIV]"
      },
      {
        "code" : "B19",
        "display" : "Hepatite viral não especificada"
      },
      {
        "code" : "B15",
        "display" : "Hepatite aguda A"
      },
      {
        "code" : "B16",
        "display" : "Hepatite aguda B"
      },
      {
        "code" : "B171",
        "display" : "Hepatite aguda C"
      },
      {
        "code" : "B172",
        "display" : "Hepatite aguda E"
      }]
    }]
  }
}

```
