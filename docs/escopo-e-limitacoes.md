# Escopo e limitações

## Dentro do escopo

- ingestão de fontes textuais controladas;
- normalização e metadados;
- divisão do conteúdo;
- recuperação de contexto;
- geração de resposta apoiada nas fontes;
- referências para conferência;
- limites de consumo;
- registros operacionais e avaliação humana.

## Fora do escopo atual

- processamento direto de vídeo;
- transcrição automática de grandes bibliotecas de áudio;
- análise contínua de imagens e quadros;
- integração automática com o NotebookLM pessoal;
- substituição de uma base oficial de conhecimento;
- decisões autônomas em produção;
- coleta irrestrita de e-mails, conversas ou arquivos;
- publicação de dados internos no GitHub.

## Limitações conhecidas

### Qualidade da fonte

O sistema não corrige uma documentação desatualizada por conta própria. Se duas fontes discordarem, a resposta precisa indicar o conflito.

### Recuperação incompleta

O trecho correto pode não ser selecionado. Por isso, devem ser avaliados os resultados da busca antes de atribuir todo erro ao modelo.

### Resposta sem evidência

Modelos podem produzir uma explicação plausível mesmo com contexto insuficiente. A instrução para admitir ausência de informação reduz o risco, mas precisa ser testada.

### Custo variável

Fontes longas e perguntas amplas aumentam contexto e consumo. Limites técnicos e alertas precisam existir antes de liberar uso maior.

### Dependência externa

APIs, preços e limites mudam. A arquitetura reduz o acoplamento, mas não elimina a necessidade de manutenção.

## Critério de sucesso

O MVP é útil quando reduz o tempo para encontrar uma resposta sem esconder a fonte e sem criar um custo desproporcional. Velocidade sozinha não basta.

