# Modelo Computacional - Guia de Implementação do Resultado de Exame Laboratorial (REL) da RNDS v1.0.0-release

## Modelo Computacional

### Modelo Computacional

 Para a modelagem do modelo computacional do Resultado de Exame Laboratorial (REL) foram mapeados os campos do Modelo de Informação (MI) aos recursos internacionais [FHIR R4](https://hl7.org/fhir/R4/). Assim, foi realizada a modelagem fechada do perfil de modo a atender o contexto nacional. 

Foi criado um [Projeto Rede Nacional de Dados em Saúde](https://simplifier.net/redenacionaldedadosemsaude/), na plataforma [SIMPLIFIER.NET](https://simplifier.net/), para a publicação e distribuição dos perfis relacionados aos documentos computacionais em produção na rede.

### Bundle de Envio do REL

O diagrama abaixo apresenta o pacote *Bundle* no qual é condensado o Resultado de Exame Laboratorial (REL), referenciando todos os dados relevantes para caracterizar esse registro.

 **Figura 1 - Diagrama do *Bundle* do REL** 

### Recursos FHIR

 O modelo computacional do REL é definido pelo perfil ***BRResultadoExameLaboratorial-3.2.1*** [`Composition`].

| | |
| :--- | :--- |
| *Composition* | ` [BRResultadoExameLaboratorial-3.2.1](StructureDefinition-BRResultadoExameLaboratorial-3.2.1.md) ` |
| *Condition* | ` [BRCondicaoSaude](StructureDefinition-BRCondicaoSaude.md) ` |
| *Observation* | ` [BRDiagnosticoLaboratorioClinico-3.2.1](StructureDefinition-BRDiagnosticoLaboratorioClinico-3.2.1.md) ` |
| *Specimen* | ` [BRAmostraBiologica-1.0](StructureDefinition-BRAmostraBiologica-1.0.md) ` |

### ValueSets e CodeSystems utilizados no REL

 O Modelo Computacional do Resultado de Exame Laboratorial (REL) utiliza recursos terminológicos, como *ValueSets* e *CodeSystems*, para padronizar as informações compartilhadas na RNDS. Os perfis FHIR possuem vínculos (*bindings*) com *ValueSets*, que estabelecem os conjuntos de códigos admitidos, enquanto os *CodeSystems* definem os códigos e seus respectivos conceitos. 

 No JSON, `coding.system` identifica o *CodeSystem* utilizado e `coding.code` informa o código correspondente. 

 Considerando que esses recursos podem passar por atualizações e versionamentos, recomenda-se consultar as especificações vigentes e os artefatos publicados neste Guia de Implementação. 

Segue abaixo uma listagem de todos os *ValueSets* utilizados no REL e seus respectivos *CodeSystems*:

| | |
| :--- | :--- |
| [BRCategoriaExame](ValueSet-BRCategoriaExame-1.0.md) | [BRSubgrupoTabelaSUS](CodeSystem-BRSubgrupoTabelaSUS.md) |
| [BREstadoDocumento](ValueSet-BREstadoDocumento-1.0.md) | [CompositionStatus](https://hl7.org/fhir/R4/codesystem-composition-status.html) |
| [BREstadoObservacao](ValueSet-BREstadoObservacao-1.0.md) | [ObservationStatus](https://hl7.org/fhir/R4/codesystem-observation-status.html) |
| [BRNomeExame](ValueSet-BRNomeExame-2.0.md) | [BRNomeExameLOINC](CodeSystem-BRNomeExameLOINC.md)[BRNomeExameGAL](CodeSystem-BRNomeExameGAL.md) |
| [BRResultadoQualitativoExame](ValueSet-BRResultadoQualitativoExame-1.0.md) | [BRResultadoQualitativoExame](CodeSystem-BRResultadoQualitativoExame.md) |
| [BRResultadoQualitativoExame](ValueSet-BRResultadoQualitativoExame-2.0.md) | [BRResultadoQualitativoExame](CodeSystem-BRResultadoQualitativoExame.md)[BRTipoResultadoAVIDEZ](CodeSystem-BRTipoResultadoAVIDEZ.md)[BRTipoResultadoDTNT](CodeSystem-BRTipoResultadoDTNT.md)[BRTipoResultadoHISPT](CodeSystem-BRTipoResultadoHISPT.md)[BRTipoResultadoPRAU](CodeSystem-BRTipoResultadoPRAU.md)[BRTipoResultadoPSNG](CodeSystem-BRTipoResultadoPSNG.md)[BRTipoResultadoRGNR](CodeSystem-BRTipoResultadoRGNR.md)[BRTipoResultadoRSBAC](CodeSystem-BRTipoResultadoRSBAC.md)[BRTipoResultadoRSCUL](CodeSystem-BRTipoResultadoRSCUL.md) |
| [BRTerminologiaPatogeno](ValueSet-BRTerminologiaPatogeno.md) | [BRTerminologiaPatogeno](CodeSystem-BRTerminologiaPatogeno.md) |
| [BRTerminologiaSuspeitaDiagnostica](ValueSet-BRTerminologiaSuspeitaDiagnostica.md) | [BRCID10](CodeSystem-BRCID10.md) |
| [BRTipoAmostra](ValueSet-BRTipoAmostra-1.0.md) | [SpecimenType](https://terminology.hl7.org/CodeSystem-v2-0487.html)[BRTipoAmostraGAL](CodeSystem-BRTipoAmostraGAL.md) |
| [BRTipoDocumento](ValueSet-BRTipoDocumento-1.0.md) | [BRTipoDocumento](CodeSystem-BRTipoDocumento.md) |

