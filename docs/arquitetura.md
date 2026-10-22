# Arquitetura

## Visão geral

A arquitetura foi dividida para que cada etapa possa ser testada isoladamente. A fonte não conhece o modelo, e o modelo não precisa saber como o documento foi obtido.

## Entrada

As fontes entram por adaptadores. Nesta fase, a prioridade é conteúdo textual que possa ser identificado, revisado e atualizado. Cada item precisa manter pelo menos:

- origem;
- título ou identificação;
- data de coleta ou atualização;
- tipo de conteúdo;
- permissão de uso;
- referência para voltar ao material original.

## Preparação

O conteúdo é extraído e normalizado antes da busca. Cabeçalhos, espaços e caracteres precisam ser tratados sem apagar a estrutura que ajuda a interpretar o documento.

Depois, o texto é dividido em partes menores. Cada parte herda os metadados da fonte. O tamanho deve equilibrar contexto e precisão: partes grandes trazem ruído; partes pequenas podem separar uma explicação do trecho que dá sentido a ela.

## Recuperação

A pergunta não segue diretamente para o modelo. Primeiro, o sistema procura os trechos mais relevantes. Essa busca pode combinar termos exatos, filtros por metadados e similaridade semântica.

O resultado da recuperação precisa ser limitado. Enviar documentos inteiros em toda pergunta aumenta custo e pode piorar a resposta.

## Geração

O modelo recebe a pergunta, os trechos selecionados e regras claras:

- usar apenas o contexto fornecido;
- citar ou identificar as fontes;
- separar fato encontrado de interpretação;
- informar quando não houver material suficiente;
- evitar completar lacunas com suposições.

## Saída

A saída deve ser útil para quem está trabalhando. Dependendo da pergunta, pode assumir a forma de resumo, resposta técnica, sequência de verificação ou rascunho de documentação.

Além do texto, devem ser mantidos os trechos usados, as fontes, o horário, o modelo e os limites aplicados. Isso permite revisar a resposta e entender o custo.

## Observabilidade

Os registros necessários são operacionais e não devem guardar conteúdo sensível sem justificativa. As medidas mais úteis são:

- tempo por etapa;
- quantidade e tamanho das fontes;
- trechos recuperados;
- tokens ou unidade de consumo;
- custo estimado;
- erros por origem;
- perguntas sem resposta;
- avaliação humana da utilidade.

