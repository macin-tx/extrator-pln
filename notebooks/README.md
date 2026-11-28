# Extração de palavras e de classes gramaticais
Este notebook contém uma ferramenta para extração e identificação de substantivos em arquivos PDF produzida para a primeira tarefa da minha IC pela Universidade federal de Sergipe.

O problema proposto foi:

> Ler arquivos PDF no Google Colab, localizar e extrair classes gramaticais específicas, como substantivos. Para tanto, fazer isso combinando bibliotecas de extração de texto com ferramentas de Processamento de Linguagem Natural (PLN) em Python. Os termos extraídos devem ser salvos em uma planilha (Excel/CSV), de forma que a execução seja feita sem trabalho manual.

Para usar a ferramenta, basta colocar os seus próprios PDFs na pasta de entrada do Google Drive. Veja [Como usar](#como-usar)

---
## O que a ferramenta faz
1. Leitura de PDF, com a biblioteca `pypdf` que converte o conteúdo visual em texto puro;
2. Análise gramatical em português com a biblioteca `spaCy`, fazendo uso da técnica Part-of-Speech (POS) Tagging - associar cada palavra a sua classe gramatical;
3. Busca e filtragem de substantivos. OBS: O código foi aprimorado para fazer a busca de outras classes gramaticais ou de termos (frequência).

## Como usar
1. Coloque o(s) pdf(s) na pasta `extractor/pdfs`. A pasta `extractor/resultados` é gerada automaticamente.
2. Preencha o formulário de busca.
3. Depois vá no menu superior, clique em Ambiente de execução > Executar tudo (ou apertar `Ctrl + F9`).
4. Resultado é exportado na tela e vai para a pasta `extractor/resultados` 



