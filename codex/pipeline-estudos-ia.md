# Pipeline de estudos com IA

O fluxo separa a preparação do material da etapa de estudo:

1. Arquivos e links entram no Google Drive.
2. O Gemini faz a triagem e prepara fontes limpas, preservando o conteúdo e sinalizando dúvidas.
3. O GPT consome essas fontes para criar planos de estudo, flashcards e simulados.
4. Google Drive mantém os arquivos e uma estrutura simples ajuda a controlar o processamento.

O MVP foi aplicado no Google Cloud. A escolha foi manter a arquitetura simples e controlar o custo. O processamento de vídeos ficou fora do escopo por exigir mais armazenamento e processamento; o fluxo prioriza documentos e fontes textuais.

A integração direta com o NotebookLM depende de uma API pública adequada. Enquanto isso, o pipeline organiza as fontes para reduzir retrabalho quando essa integração estiver disponível.
