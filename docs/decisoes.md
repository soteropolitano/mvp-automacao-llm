# Decisões do projeto

Este arquivo registra as escolhas que mudaram o formato do MVP. A intenção é preservar o motivo, e não apenas o resultado.

## Começar por texto

**Decisão:** aceitar primeiro fontes textuais ou conteúdo previamente convertido e revisado.

**Motivo:** texto permite validar extração, divisão, recuperação, resposta e referências com custo e tempo menores.

**Consequência:** vídeo e áudio não entram diretamente. Uma transcrição pode ser usada quando houver origem e marcadores suficientes para conferência.

## Não processar vídeos no MVP

**Decisão:** retirar vídeos do processamento inicial.

**Motivo:** um vídeo não é apenas um arquivo maior. Ele pode exigir transcrição, separação de vozes, tratamento de ruído, leitura de telas, OCR e sincronização por tempo. Cada camada aumenta custo e dificulta descobrir por que uma resposta ficou errada.

**Condição para rever:** o fluxo textual precisa estar estável e deve existir um caso de uso que justifique o custo adicional.

## Manter o NotebookLM fora do núcleo

**Decisão:** usar o NotebookLM como referência e comparação manual, sem torná-lo dependência do MVP.

**Motivo:** a integração buscada não estava disponível de forma adequada no produto pessoal. A oferta Enterprise possui APIs documentadas em preview, mas exige estrutura e licenciamento que não combinam com o objetivo inicial de baixo custo.

**Consequência:** a solução mantém a própria camada de fontes e recuperação. Uma integração futura poderá ser adicionada como adaptador.

## Separar origem, processamento e saída

**Decisão:** não criar um fluxo único preso a uma fonte ou fornecedor.

**Motivo:** essa divisão permite testar, substituir e controlar cada parte. Também reduz o risco de perder o projeto quando um serviço muda.

## Priorizar respostas verificáveis

**Decisão:** uma resposta precisa apontar o material que a sustenta.

**Motivo:** em suporte e operação, uma resposta segura precisa ser conferida. Fluência não substitui evidência.

## Controlar consumo desde o início

**Decisão:** limitar volume por fonte, contexto enviado, chamadas e custo por execução.

**Motivo:** o controle posterior costuma ser mais difícil. O MVP deve mostrar quanto custa para operar antes de crescer.

## Não publicar conteúdo interno

**Decisão:** manter no repositório apenas arquitetura, decisões e exemplos neutros.

**Motivo:** documentos internos, credenciais e resultados contendo dados privados não são necessários para explicar o trabalho.

