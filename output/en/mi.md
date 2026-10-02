# Modelo de Informação - Guia de Implementação do Resultado de Exame Laboratorial (REL) da RNDS v1.0.0-release

## Modelo de Informação

### Objetivo

O documento clínico **REL** (Resultado de Exame Laboratorial) destina-se a promover o compartilhamento de resultados de exames realizados pelos Laboratórios de Análises Clínicas, permitindo a visualização dos resultados pelo cidadão e pelos profissionais de saúde envolvidos na continuidade do cuidado.

### Marcos Legais

*  [Portaria GM/MS Nº 8.276, DE 29 DE setembro DE 2025](https://www.in.gov.br/en/web/dou/-/portaria-gm/ms-n-8.276-de-29-de-setembro-de-2025-659605663) 

### Modelo de Informação

 O modelo de informação é uma representação conceitual e canônica, onde os elementos referentes a um documento específico são modelados em seções e blocos de dados, com seus respectivos tipos de dados a serem informados. Também são apresentadas as referências para o uso de recursos terminológicos, da seguinte maneira: 

*  **Coluna 1** - Nível: apresenta o nível do elemento no modelo de informação; 
* **Coluna 2** - Ocorrência: descreve o número de vezes (cardinalidade) que o elemento deve/pode aparecer:
*  **Coluna 3** - Seção/Item: nome do bloco ou da informação a ser enviada; 
*  **Coluna 4** - Tipo de dado: descreve o tipo de dado a ser preenchido; 
*  **Coluna 5** - Conceito: apresenta as definições do elemento; 
*  **Coluna 6** - Definição de uso do elemento: Observações e regras de negócio relacionadas ao elemento; 
*  **Coluna 7** - Conteúdo: apresenta, quando necessário, o grupo de códigos (*ValueSet*) a ser utilizado para preenchimento do elemento; 
*  **Coluna 8** - Recurso FHIR: relaciona o atributo do Modelo Informacional com o perfil do Modelo Computacional em FHIR. 

### Blocos do Modelo de Informação

 Segue abaixo o modelo de informação para o Resultado de Exame Laboratorial (REL): 

