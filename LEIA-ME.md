# Portfólio Ana Laura Carvalho Carnib

## Estrutura
- `index.html` – o site inteiro (textos, projetos e traduções ficam no `<script>` no fim do arquivo)
- `img/` – suas fotos
- `img/projetos/<projeto>/` – imagens de cada projeto
- `curriculo/Ana-Laura-Carnib-Curriculo.pdf` – currículo para download

## Como adicionar as imagens dos projetos
Em cada pasta de `img/projetos/` coloque:
- `capa.jpg` → aparece no card e no topo da página do projeto
- `01.jpg`, `02.jpg`, `03.jpg` … até `12.jpg` → galeria (pode ser .jpg, .png ou .webp)

Pastas: `ants`, `vovo-antonio`, `trufatella`, `soul-cabelos`, `reels`, `impressos`, `junior-carnib`.
Enquanto não houver imagem, o site mostra uma arte ilustrada no lugar.
Dica: exporte as imagens com até 1600px de largura para o site carregar rápido.

## Como editar textos
No `index.html`, procure por `const PROJETOS` (projetos), `const SERVICOS` (serviços) e `const I18N` (todos os outros textos, em pt/en/es).

## Publicar no GitHub Pages
1. Crie um repositório no GitHub (ex.: `portfolio`).
2. Envie todos os arquivos desta pasta (Add file > Upload files), mantendo as pastas.
3. Vá em Settings > Pages > Source: "Deploy from a branch", branch `main`, pasta `/ (root)` > Save.
4. Em 1–2 minutos o site fica em `https://SEU-USUARIO.github.io/portfolio/`.

## Capas dos projetos do Behance
O Behance bloqueia imagens usadas em outros sites, então a capa vinda de lá pode não aparecer.
Para garantir: abra cada projeto no Behance, salve a imagem de capa e as imagens do projeto, e coloque em:
- `img/projetos/ants/` (capa.jpg, 01.jpg, 02.jpg…)
- `img/projetos/vovo-antonio/`
- `img/projetos/trufatella/`

## Logos
Ficam em `img/logo/`. O cabeçalho usa `logo-horizontal-roxo.png`, o rodapé usa `logo-empilhado-creme.png` e o ícone da aba usa `monograma-ac.png`.

## Adicionar um novo impresso
1. Crie uma pasta em `img/projetos/` (ex.: `img/projetos/folder-cliente/`) com `capa.jpg`, `02.jpg`, `03.jpg`…
2. No `index.html`, dentro de `const PROJETOS`, copie um bloco de impresso (ex.: `calendario-h4log`) e troque `slug` (nome da pasta), `titulo` (tipo da peça) e `cliente`.
3. Em `imgs`, liste as imagens na ordem. Use `{src:'03',largo:true}` para uma imagem ocupar a largura toda.

## Reels
Ficam em `img/projetos/reels/`. Cada reel tem 3 arquivos:
- `reel-01.mp4`: vídeo completo, com som (abre ao clicar)
- `reel-01-prev.mp4`: prévia curta sem som, que roda no carrossel
- `reel-01.jpg`: imagem de capa do vídeo
Para adicionar um reel, crie os 3 arquivos com o próximo número e inclua `{n:'reel-12', cliente:'Nome do cliente'}` na lista `videos` do projeto `reels`. Sem `cliente`, o reel fica sem legenda.
