# Próximos passos

## Base de avaliação

Criar um conjunto pequeno de perguntas com respostas conhecidas. Ele deve incluir perguntas fáceis, ambiguidades, conflitos entre fontes e casos em que a resposta não existe.

## Protótipo textual

Implementar o fluxo mínimo com poucas fontes neutras:

- coleta;
- normalização;
- divisão;
- recuperação;
- geração;
- referência;
- registro de custo e tempo.

## Comparação

Comparar busca por termos, busca semântica e uso combinado. Avaliar se os trechos recuperados contêm a resposta antes de comparar a redação do modelo.

## Segurança

Definir classificação das fontes, retenção, exclusão e mascaramento. Nenhuma credencial deve entrar no conteúdo indexado.

## Interface

Somente depois de validar o fluxo, criar uma interface simples para pergunta, resposta, fontes e feedback. A interface não deve esconder os limites do sistema.

## NotebookLM

Acompanhar a evolução das APIs do Gemini Notebook Enterprise e avaliar:

- maturidade fora de preview;
- licenciamento e custo;
- inclusão e atualização de fontes;
- consulta programática com referências;
- autenticação e isolamento dos dados;
- ganho real diante do fluxo próprio.

## Vídeo

Reavaliar vídeo apenas com um caso de uso definido. O primeiro teste deve usar poucos arquivos e separar:

- transcrição;
- marcadores de tempo;
- conteúdo visual importante;
- custo por minuto;
- qualidade em áudio ruim;
- revisão humana.

## Critérios antes de ampliar

- qualidade medida com perguntas conhecidas;
- respostas sem fonte rejeitadas;
- custo máximo por execução conhecido;
- atualização e remoção de fontes testadas;
- logs suficientes para investigar falhas;
- política de dados definida.

