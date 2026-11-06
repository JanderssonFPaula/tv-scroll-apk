# 📺 TV SCROLL: executável

Este repositório guarda o **executável do TV SCROLL** e o arquivo de controle de versão. O código-fonte está em [TV-SCROLL](https://github.com/JanderssonFPaula/TV-SCROLL).

## Para que serve o TV SCROLL

Transforma uma TV ligada a um PC Windows em um **painel que passa sozinho**: relatórios do Power BI, sistemas com login, imagens, vídeos, PowerPoint, PDF e páginas HTML, em rodízio contínuo, sem ninguém por perto.

Você monta a sequência arrastando caixas numa tela no navegador. O programa abre o Chrome em tela cheia na TV, entra nos sistemas, aplica filtros, rola a página e passa para o próximo item. Se o Chrome fechar ou travar, ele reabre sozinho.

O que dá para fazer:

- **Montar o rodízio visualmente**, ligando as caixas na ordem em que devem passar. Dá para editar, ativar, desativar e remover itens com o rodízio rodando.
- **Elementos prontos** para arrastar: página web (Power BI e outros), imagens, vídeos, PDF, PowerPoint, HTML, informativo com texto formatado e transição entre telas, com data, hora e previsão do tempo.
- **Modelos HTML** que enquadram a mídia, com ajuste de encaixe, zoom e alinhamento e uma prévia do resultado.
- **Login em sistemas** com usuário e senha guardados protegidos neste PC.
- **Antibloqueio:** evita que o PC bloqueie a tela ou desligue durante o rodízio.
- **Levar a configuração de um PC para outro**, com um arquivo que não leva usuários nem senhas.

## Como usar

1. Baixe o [`TV-SCROLL.exe`](https://github.com/JanderssonFPaula/tv-scroll-apk/raw/main/TV-SCROLL.exe).
2. Coloque-o numa pasta própria, por exemplo `C:\TV-SCROLL`. Os dados (configurações, modelos, login do Chrome) ficam **na mesma pasta** do `.exe`.
3. Execute. A interface abre no navegador em `http://127.0.0.1:8765`.
4. Precisa do Google Chrome instalado e de internet para a verificação de versão.

## Controle de versão

O programa **só roda na versão publicada aqui**.

- Ao abrir, e a cada 10 minutos, ele lê o [`versao.json`](versao.json) deste repositório.
- Se a versão publicada for **maior** que a do programa, ele para e mostra a tela para baixar a versão nova.
- Se o uso for desativado pelo autor, ele para em todos os PCs.
- Sem conseguir verificar (sem internet ou arquivo ausente), ele continua por até 24 horas desde a última verificação boa e depois bloqueia.
- O `versao.json` é **assinado digitalmente**. Só o autor consegue publicar um arquivo que o programa aceite.

Para atualizar um PC: baixe o `TV-SCROLL.exe` novo e substitua o antigo, mantendo a pasta `data`.

## Arquivos

| Arquivo | O que é |
| --- | --- |
| `TV-SCROLL.exe` | O programa, em um único executável |
| `versao.json` | Versão atual e estado de uso, assinados |

Desenvolvido por [Jandersson F. de Paula](https://www.linkedin.com/in/jandersson-ferreira-de-paula/).
