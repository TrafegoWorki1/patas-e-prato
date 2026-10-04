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

---

## Versão de revisão (atual)

Esta é a versão **para revisão**, não para anunciar. Não há preço, prazo, produto,
métrica nem depoimento — tudo está marcado como pendente.

### Ligar o WhatsApp
Abra `index.html` e edite o script no final do arquivo:

```js
const WHATSAPP_NUMERO = '5585999999999';   // só dígitos, com DDI
const WHATSAPP_MENSAGEM = 'Olá! Vim pelo site e quero fazer um pedido de ração.';
```

Com o número vazio, os botões ficam desativados e aparece uma tarja avisando
que falta o número. Não há link morto.

### Preencher os campos
São 34 blocos `<span class="slot">[...]</span>`. Cada um é um ponto que precisa
de informação real: nome da loja, produtos, preços, prazo, região atendida,
diferenciais, perguntas, métricas e depoimentos.

### Publicar a versão final
1. Preencher `WHATSAPP_NUMERO`
2. Trocar cada `<span class="slot">[...]</span>` pelo texto real
3. Remover `class="modo-revisao"` do `<body>`

O aviso amarelo e a tarja do WhatsApp somem sozinhos.

## Regra de conteúdo
Não se escreve indicação por idade, porte ou benefício de saúde sem que o rótulo
do fabricante sustente a afirmação. Alegação de qualidade ("super premium",
"natural", "sem enchimento") exige lastro — CDC, art. 37.
