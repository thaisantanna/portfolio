# Thaiana · Portfólio

Site de portfólio de Thaiana, storymaker e editora de vídeo.

## Arquivos

- `index.html`: o site inteiro (estilos e scripts já estão dentro dele)
- `img/`: pasta para a foto do perfil
- `.nojekyll`: diz ao GitHub Pages para publicar os arquivos como estão

## Como publicar no GitHub Pages

1. Entre em github.com e crie um repositório novo (botão **New**).
   - Para o endereço ficar `seuusuario.github.io`, dê ao repositório exatamente esse nome.
   - Com qualquer outro nome (por exemplo `portfolio`), o endereço fica `seuusuario.github.io/portfolio`.
   - Deixe o repositório como **Public**.
2. No repositório, clique em **Add file → Upload files** e arraste `index.html`, `README.md` e a pasta `img`.
   O arquivo `.nojekyll` fica oculto em alguns computadores; se não aparecer, tudo bem, o site funciona sem ele.
3. Clique em **Commit changes**.
4. Vá em **Settings → Pages**. Em **Branch**, escolha `main` e a pasta `/ (root)`, depois clique em **Save**.
5. Espere um ou dois minutos e recarregue a página de Settings → Pages. O link do site aparece no topo.

## Como colocar a foto do perfil

1. Salve a foto como `foto.jpg` dentro da pasta `img` (formato retrato, 4:5, por exemplo 800 × 1000 px).
2. Abra `index.html` e procure por `foto-vazia`.
3. Troque o bloco `<div class="foto-vazia" ...> ... </div>` por:

   ```html
   <img src="img/foto.jpg" alt="Thaiana">
   ```

## Como trocar ou adicionar vídeos

Cada vídeo é um bloco `<a class="video" ...>` dentro de `grade-longos` (vídeos longos) ou `grade-shorts` (shorts).
Para trocar, mude o código do vídeo em dois lugares: no link (`href`) e na capa (`i.ytimg.com/vi/CODIGO/hqdefault.jpg`).
O título fica dentro de `<h3>`.

Ao clicar num vídeo, ele toca numa janela sobre o próprio site (fecha com o X, com a tecla Esc ou clicando fora). Os shorts abrem no formato vertical. Se o dono do vídeo tiver desativado a incorporação no YouTube, o player mostra um aviso; nesse caso é preciso ativar "Permitir incorporação" nas configurações do vídeo no YouTube Studio.
