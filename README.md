<!-- MKBRAION-POLISH:START -->
<div align="center">

# Otimizador Midia

**Ferramenta web para processamento de imagens e vídeos com FFmpeg WebAssembly, OCR com Tesseract.js e integração com backend de mídia.**

[![Repositório](https://img.shields.io/badge/GitHub-Repositório-181717?logo=github)](https://github.com/mkbraion/otimizador-midia) [![Demo ao vivo](https://img.shields.io/badge/Demo-Abrir%20aplicação-2ea44f?logo=vercel)](https://otimizador-midia.vercel.app)

</div>

**Stack / tópicos:** ``css`` · ``ffmpeg`` · ``frontend`` · ``html`` · ``image-processing`` · ``javascript`` · ``media-tools`` · ``nodejs`` · ``ocr`` · ``tesseractjs`` · ``vercel`` · ``video-processing``

> Projeto mantido por [@mkbraion](https://github.com/mkbraion).
<!-- MKBRAION-POLISH:END -->

# Oficina de Mídia

Ferramenta web para processamento de imagem e vídeo, com operações locais no navegador e integração com um backend de download de mídia.

[Aplicação](https://otimizador-midia.vercel.app) · [Backend](https://github.com/mkbraion/otimizador-midia-yt-backend)

## Implementação

- HTML, CSS e JavaScript em `index.html`.
- FFmpeg/WebAssembly em `vendor/` para processamento de mídia.
- Tesseract.js para OCR e JSZip para arquivos ZIP, carregados por CDN.
- Backend Node.js separado para as rotas de consulta e download.
- Configuração de hospedagem e cabeçalhos em [vercel.json](vercel.json).

Algumas operações são locais; downloads remotos dependem do backend e dos sites de origem. A página também carrega fontes e scripts de publicidade externos. Consulte [privacidade.html](privacidade.html).

## Manutenção

Para desenvolvimento, sirva os arquivos por HTTP local. WebAssembly e recursos que dependem de cabeçalhos não devem ser avaliados apenas abrindo o arquivo por `file://`.

O backend tem instalação e configuração próprias, documentadas no respectivo repositório. Preserve os avisos de licença das bibliotecas ao atualizar os arquivos em `vendor/`.
