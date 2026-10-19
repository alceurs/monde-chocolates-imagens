# CDN de imagens de produtos

Biblioteca temporária de imagens otimizadas para importação em ERPs e e-commerce.
As imagens são servidas pelo jsDelivr a partir deste repositório público:

    https://cdn.jsdelivr.net/gh/alceurs/monde-chocolates-imagens@main/<cliente>/<arquivo>

## Estrutura

- Uma pasta por cliente (ex.: `monde-chocolates/`).
- Nome do arquivo: `<SKU>-<ordem>-<titulo-do-produto>-<marca>.jpg` (ex.: `841-01-alfajor-...-70g-monde-chocolates.jpg`). A ordem 01 é sempre a capa do produto. O nome descritivo ajuda na indexação da imagem por buscadores e IAs.
- Padrão: JPG, quadrado, 72 DPI, otimizado para web.

## Ciclo de vida

As imagens ficam aqui apenas até serem incorporadas pelo sistema de destino e salvas no diretório do cliente.
Ao trocar uma imagem já publicada, use um nome novo (ex.: acrescentando `-v2` ao final): o jsDelivr mantém cópia em cache.
