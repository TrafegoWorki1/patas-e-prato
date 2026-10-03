# Patas & Prato — página de captura

Landing page para venda de ração para cachorros (assinatura mensal).

## Estrutura
- `index.html` — página única, sem build. CSS e JS embutidos.
- Sem dependências: abre direto no navegador ou sobe em qualquer host estático.

## Onde editar
- **Preço e cupom:** seção `#oferta`, bloco `.price-box`.
- **Depoimentos:** seção `.quotes` — os três cards estão com texto de placeholder.
- **Métricas:** `.stats` — atributos `data-c` aceitam o número; o contador anima até ele.
- **CTA:** os botões apontam para `#`. Trocar pelo link real do checkout/WhatsApp.
- **Cores:** variáveis `--brand` / `--brand2` no `:root`.

## Antes de anunciar
- [ ] Substituir o CTA `#` pelo destino real
- [ ] Preencher depoimentos com casos reais
- [ ] Confirmar preço, cupom e regra de frete
- [ ] Conferir alegações de qualidade — "sem enchimento" e similar precisam
      de respaldo no rótulo do produto
