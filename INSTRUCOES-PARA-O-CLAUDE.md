# Instruções para o Claude – Portfólio Ana Carnib

Este zip é o site de portfólio da Ana Laura Carvalho Carnib. **Ela não sabe programar.** Toda alteração deve ser feita por você, e a entrega é sempre o **zip completo e atualizado**.

## Fluxo obrigatório em toda conversa
1. Descompacte o zip enviado e leia este arquivo e o `index.html` antes de mexer em qualquer coisa.
2. Faça as alterações pedidas mantendo exatamente a mesma estrutura de pastas e nomes.
3. Imagens novas:
   - converta para JPG com qualidade ~80;
   - largura máxima de 1200 px (slides, posts, stories) ou 1600 × 1200 px (capas `capa.jpg`, proporção 4:3);
   - salve em `img/projetos/<slug>/` com nomes simples, sem espaço nem acento.
4. Vídeos novos: no máximo 432 px de largura, H.264, `-crf 33`, AAC 64k, `+faststart`. Para reels, crie também a prévia `-prev.mp4` (7 s, sem som, 300 px) e a capa `.jpg`.
5. Todo texto novo precisa estar em **português, inglês e espanhol**.
6. Teste se o JavaScript não quebrou (por exemplo, `node --check` no conteúdo do `<script>`) e, se puder, veja a página renderizada.
7. Atualize a seção **Pendências** e o **Histórico** no fim deste arquivo.
8. Entregue o zip completo com o nome `portfolio-ana-carnib.zip`. O zip precisa ficar abaixo de ~28 MB, porque é ele que a Ana envia na próxima conversa. Se puder, entregue também uma prévia HTML autocontida para ela ver o resultado na conversa.
9. Na resposta, diga em linguagem simples o que mudou. Nunca peça para ela editar código ou mover arquivos.

## Identidade do site
- Fontes: Poppins (texto, títulos em bold) e Mrs Saint Delafield (destaques/script), via Google Fonts.
- Cores: roxo `#6A378D`, lilás `#E5BFFF`, verde `#6D8344`, verde claro `#AACA6E`, creme `#FCFADE`, neutro `#463A3A`.
- Vibe divertida e criativa: estrelas/explosões, sombras sólidas deslocadas, cantos arredondados.
- Logos em `img/logo/` (cabeçalho: horizontal roxo; rodapé: empilhado creme; favicon: monograma "ac").
- Rodapé em roxo (ela não quer marrom).

## Como o site funciona
- Um único `index.html`. Textos fixos ficam no objeto `I18N` (pt/en/es). Projetos ficam na lista `PROJETOS`. Serviços em `SERVICOS`.
- A navegação é feita por JavaScript (função `navegar`/`rota`), sem depender de trocar o endereço da página.
- Categorias (`CATS`): identidade, uiux, posts, reels, impressos.
- Tipos de projeto:
  - **Com seções** (ANT'S, J.Carnib, Vovô Antonio, Trufatella, Soul Cabelos, Sanluèr): ficha (cliente, ferramentas, entrega, projeto, equipe), resumo, desafio/processo/resultado e `secoes` com `texto`, `listas`, `grupos` de imagens (`sub`, `cols`, `imgs`; `{src:'x',largo:true}` ocupa a linha toda) e `botao`. `numerar:true` numera as seções; `destaque:true` faz o bloco lilás; `status:true` mostra a etiqueta "Em atualização".
  - **Impressos** (`galeria:true`): card com mockup + tipo da peça como título + cliente; a página mostra só a galeria (`imgs`).
  - **Reels** (`reels:true`): carrossel horizontal em movimento com prévias sem som; ao clicar, abre o player com som e setas. Lista em `videos` (`{n:'reel-01', cliente:'711 Comunicação'}`; sem `cliente` = sem legenda; os reels de salão não têm legenda).
- `capaPos` ajusta o enquadramento da capa no card (ex.: `'0% 50%'`).

## Contatos
- E-mails: anacarnibdesign@gmail.com (principal) e analauracarvalho18@gmail.com
- WhatsApp: (19) 98703-7170 – o botão "Pedir um orçamento" usa
  `https://wa.me/5519987037170?text=Ol%C3%A1%2C%20Ana!%20Gostaria%20de%20receber%20um%20or%C3%A7amento%20personalizado%20de%E2%80%A6`
- Instagram: @anacarnib.design · LinkedIn: https://www.linkedin.com/in/ana-laura-carvalho-carnib-a354a3191/
- Sem Behance no site.

## Pendências
- Sanluèr (design de posts, freela pela 711 Comunicação): falta 1 carrossel, as capas de reels e as ferramentas usadas.
- Soul Cabelos: confirmar ferramentas (hoje: "Photoshop, Illustrator, Canva").
- Novas capas dos cards em 1600 × 1200 px: ANT'S, Soul Cabelos e Sanluèr já atualizadas; faltam J.Carnib, Vovô Antonio, Trufatella, Reels e os impressos (Calendário H4LOG, Display, Catálogo e Folder Girotto).
- O currículo em PDF (`curriculo/`) ainda mostra o celular antigo (19) 98344-1312.
- O zip está no limite (~28 MB). Ao trocar as próximas capas, comprima bem (qualidade 65–75) ou recomprima vídeos antigos para liberar espaço.
- Publicar no GitHub Pages quando o site estiver completo (passo a passo no LEIA-ME).

## Histórico
- Estrutura completa do site, tradução PT/EN/ES, logos, rodapé roxo.
- Projetos: ANT'S, J.Carnib Imóveis, Vovô Antonio (com telas novas em atualização), Trufatella, Soul Cabelos (carrosséis, stories, posts), Sanluèr (4 carrosséis + stories), Edição de reels (11 vídeos), impressos (Calendário H4LOG, Display, Catálogo e Folder Girotto).
- WhatsApp adicionado no orçamento, contatos e rodapé.
- Vídeos e imagens comprimidos para o zip caber no envio.
- Capas novas (1600 × 1200 px) de ANT'S, Soul Cabelos e Sanluèr (JPG qualidade 62–70 para o zip caber).
