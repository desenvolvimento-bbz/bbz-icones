# Ícones das ferramentas BBZ

Favicons das ferramentas internas da BBZ. Cada arquivo é um PNG de 64x64 com as
iniciais da ferramenta em branco sobre o azul da marca (`#0664e4`).

Este repositório é **público por necessidade técnica, não por conteúdo**. O
`setFaviconUrl` do Google Apps Script exige uma URL pública terminada em `.png`
ou `.ico` — SVG e URL sem extensão são recusados. Como o Google precisa buscar a
imagem sem credencial, ela tem de estar aberta.

Aqui não há dado de negócio: são três imagens de duas letras. Nenhum código,
nenhuma planilha, nenhum nome de cliente, nenhuma configuração.

## Por que existe

As ferramentas nasciam com o ícone genérico do Apps Script. Com várias abas
abertas, nenhuma se distingue da outra nem do resto do Google, e a pessoa passa a
caçar aba pelo título — que some quando há muitas. O ícone com as iniciais
devolve a identificação à aba.

O desenho é o mesmo que a vitrine de ferramentas usa nos cartões: Manrope 800,
branco sobre o azul. O ícone da aba e o do cartão têm de ser a mesma letra, senão
a pessoa aprende duas identidades para a mesma ferramenta.

## Como usar

Referencie o arquivo pela URL bruta:

    https://raw.githubusercontent.com/desenvolvimento-bbz/bbz-icones/main/icones/icone-<id>.png

Onde `<id>` é o id da ferramenta no índice.

## Como são gerados

Pelo `ferramentas/gerar-icones.js` do projeto das ferramentas, que rasteriza a
tipografia com o Chrome em modo headless. Este repositório guarda só o resultado.
