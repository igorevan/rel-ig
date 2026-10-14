# Modelo de Informação - Guia de Implementação do Resultado de Exame Laboratorial (REL) da RNDS v1.0.0-release

## Modelo de Informação

### Objetivo

O documento clínico **REL** (Resultado de Exame Laboratorial) destina-se a promover o compartilhamento de resultados de exames realizados pelos Laboratórios de Análises Clínicas, permitindo a visualização dos resultados pelo cidadão e pelos profissionais de saúde envolvidos na continuidade do cuidado.

### Marcos Legais

*  [Portaria GM/MS Nº 8.276, DE 29 DE setembro DE 2025](https://www.in.gov.br/en/web/dou/-/portaria-gm/ms-n-8.276-de-29-de-setembro-de-2025-659605663) 

### Modelo de Informação

 O modelo de informação é uma representação conceitual e canônica, onde os elementos referentes a um documento específico são modelados em seções e blocos de dados, com seus respectivos tipos de dados a serem informados. Também são apresentadas as referências para o uso de recursos terminológicos, da seguinte maneira: 

*  **Nível**: apresenta o nível do elemento no modelo de informação; 
* **Ocorrência**: descreve o número de vezes (cardinalidade) que o elemento deve/pode aparecer:
*  **Seção/Item**: nome do bloco ou da informação a ser enviada; 
*  **Tipo de dado**: descreve o tipo de dado a ser preenchido; 
*  **Conceito**: apresenta as definições do elemento; 
*  **Mapeamento Computacional - FHIR**: relaciona o atributo do Modelo Informacional com o Modelo Computacional em FHIR. 

### Modelo de Informação

 Segue abaixo o modelo de informação para o Resultado de Exame Laboratorial (REL): 

| | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 1..1 | Laboratório |  |  | `Composition``Observation` |
| 2 | [1..1] | Nome do laboratório | Texto | Nome do estabelecimento de saúde responsável pelo resultado do exame laboratorial. |  |
| 2 | [1..1] | CNES | Caracteres numéricos | Número do Cadastro Nacional do Estabelecimento de Saúde do laboratório responsável pelo resultado do exame laboratorial. | `Composition.author.identifier.system``Observation.performer.identifier.value` |
| 2 | [0..1] | CNPJ | Caracteres numéricos | CNPJ do estabelecimento de saúde responsável pelo resultado do exame laboratorial. | `Composition.author.identifier.system``Observation.performer.identifier.value` |
| 2 | [0..1] | Responsável técnico |  |  | `Observation.performer.identifier.value` |
| 3 | [1..1] | Nome completo do profissional | Texto | Nome completo do responsável técnico pelo laboratório. |  |
| 3 | [1..1] | Conselho de Classe Profissional |  |  |  |
| 4 | [1..1] | Tipo de conselho | Texto codificado:* CRM
* CRF
* CRBM
* CRBIO
* CRQ
 | Conselho de classe profissional do responsável técnico pelo laboratório. |  |
| 4 | [1..1] | Unidade Federativa | Texto Codificado | Unidade Federativa do conselho de classe profissional do responsável técnico pelo laboratório. |  |
| 4 | [1..1] | Número do registro | Texto | Número do registro no conselho de classe profissional do responsável técnico pelo laboratório. |  |
| 1 | [1..1] | Identificação do indivíduo |  |  | `Composition``Observation``Condition` |
| 2 | [1..1] | Nome completo | Texto | Nome completo do sujeito do exame. |  |
| 2 | [1..1] | CNS | Texto | Número do Cartão Nacional de Saúde válido. | `Composition.subject.identifier.value``Observation.subject.identifier.value``Condition.subject.identifier.value` |
| 1 | [1..1] | Condição Alvo |  |  | `Condition` |
| 2 | [1..1] | Suspeita Diagnóstica | Texto codificado:* COVID-19
* Mpox
* Dengue
* Zika
* Chikungunya
* Febre Amarela
* Oropouche
* Mayaro
* Febre do Nilo Ocidental
 | Nome da doença que está sendo investigada. Texto codificado por terminologia externa CID-10. | `Condition.code.coding.code` |
| 1 | [1..N] | Resultado de exame de laboratório |  |  | `Observation``Specimen` |
| 2 | [1..1] | Nome do exame | Texto codificado | Nome do exame a que foi submetida a amostra biológica. Terminologia externa LOINC. | `Observation.code.coding.code` |
| 3 | [1..1] | Categoria do exame | Texto codificado | Categoriza o exame ou teste. Repositório de Terminologia em Saúde RTS/Grupo/Subgrupo da Tabela SUS | `Observation.category.coding.code` |
| 3 | [0..1] | Patógeno | Texto codificado:* Orthopoxvirus (nome do gênero do vírus)
* Orthopoxvirus não-varíola
* Vírus Monkeypox
* Parapoxvirus (nome do gênero do vírus)
* Vírus Orf
* Vírus Pseudovaíola
* SARS-CoV-2
* Chikungunya Vírus
* Dengue Vírus
* Vírus da Febre Amarela
* Zika Vírus
* Vírus do Nilo Ocidental
* Vírus Oropouche
* Vírus Mayaro
 | Nome do patógeno que está sendo testado. | `Observation.extension.valueCodeableConcept.coding.code` |
| 3 | [1..1] | Data e hora da coleta | Data/Hora | Data e hora da coleta da amostra, conforme ISO 8601. | `Observation.effectiveDateTime` |
| 3 | [1..1] | Resultado do exame |  | Resultado do exame laboratorial. É obrigatório o envio de um dos resultados (quantitativo ou qualitativo). | `Observation` |
| 4 | [0..1] | Resultado qualitativo | Texto codificado:* Detectável
* Não detectável
* Reagente
* Não reagente
* Baixa avidez
* Alta avidez
* Compatível
* Incompatível
* Presença
* Ausência
* Positivo
* Negativo
* Foram visualizados
* Não foram visualizados
* Não houve crescimento
* Houve crescimento
* Indeterminado
* Inconclusivo
 | Valor atribuído ao analito de acordo com o método de análise, de forma qualitativa.**RN1**: Cada tipo de resultado qualitativo está condicionado ao tipo de diagnóstico laboratorial. | `Observation.valueCodeableConcept.coding.code` |
| 4 | [0..1] | Resultado quantitativo | Quantidade | Valor quantitativo do resultado do exame expresso com unidade de medida.**RN2**: É obrigatório o envio de “Interpretação” uma vez que o resultado do exame preenchido seja “Resultado quantitativo”. | `Observation.valueQuantity.value` |
| 3 | [0..1] | Interpretação | Texto codificado:* Detectável
* Não detectável
* Reagente
* Não reagente
* Baixa avidez
* Alta avidez
* Compatível
* Incompatível
* Presença
* Ausência
* Positivo
* Negativo
* Foram visualizados
* Não foram visualizados
* Não houve crescimento
* Houve crescimento
* Indeterminado
* Inconclusivo
 | Interpretação qualitativa de um resultado quantitativo.**RN3**: Cada tipo de interpretação está condicionado ao tipo de diagnóstico laboratorial. | `Observation.interpretation.coding.code` |
| 3 | [1..1] | Amostra | Texto codificado | Amostra biológica, preparada ou não, que foi submetida ao exame laboratorial. Ex: "soro", "plasma", "sangue". Terminologias externas FHIR v2-0487 e Tipo Amostra GAL. | `Specimen.type.coding.code` |
| 3 | [1..1] | Método de análise | Texto | Método analítico utilizado para determinação do resultado analítico. | `Observation.method.text` |
| 3 | [1..1] | Faixa de referência | Texto | Faixa de valores de resultado esperada para determinada população de indivíduos. | `Observation.referenceRange.text` |
| 3 | [1..1] | Data hora do resultado | Data/Hora | Data e hora do registro do exame laboratorial, conforme ISO 8601. | `Observation.issued` |
| 3 | [0..N] | Nota Narrativa adicional sobre o exame laboratorial | Texto |  | `Observation.note` |

