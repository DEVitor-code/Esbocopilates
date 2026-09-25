# Studio Alvora — Pilates e Saúde (esboço)

Site de página única **de demonstração** para clínicas de fisioterapia,
pilates, RPG e estética. Todas as informações — nome, endereço, telefone,
e-mail, convênios, avaliações e depoimentos — são **fictícias** e servem só
para apresentar o layout a clientes.

HTML, CSS e JavaScript puros — sem build, sem dependências. É só abrir o
`index.html` no navegador ou publicar a pasta em qualquer hospedagem estática
(GitHub Pages, Netlify, Vercel, Hostinger...).

## Estrutura

```
.
├── index.html                  Página completa
└── assets/
    ├── css/styles.css          Estilos (mobile first)
    ├── js/main.js              Menu, WhatsApp, animações
    ├── js/depoimentos.js       Conteúdo dos depoimentos
    └── img/                    Favicon e espaço para o logo/fotos
```

## Seções

1. **Hero** — chamada principal, nota, horário, endereço e telefone.
2. **Sobre** — história e diferenciais.
3. **Serviços** — Fisioterapia & Reabilitação, Pilates & Terapias Manuais e
   Estética & Bem-estar.
4. **Convênios** — lista de planos (nomes fictícios).
5. **Depoimentos** — nota média + cartões carregados de `depoimentos.js`.
6. **Onde estamos** — contato, horário e mapa incorporado.
7. **CTA de WhatsApp** — botão no menu, no topo, no meio, no final e um botão
   flutuante. Cada um abre a conversa com uma mensagem já escrita.

## Adaptar para um cliente real

Troque os dados fictícios nestes lugares:

| O quê | Onde |
|---|---|
| Nome (Studio Alvora / Pilates e Saúde) | `index.html` (cabeçalho, rodapé, `<title>`, metas, JSON-LD) |
| Endereço, telefone, e-mail, CNPJ | `index.html` (hero, "Onde estamos", rodapé, JSON-LD) |
| Número do WhatsApp e mensagem padrão | `assets/js/main.js`, objeto `CONFIG` no topo |
| Horário e selo "Aberto agora" | `index.html` + lista `horarios` do `CONFIG` |
| Nota e nº de avaliações | `index.html` (hero e seção de depoimentos) |
| Convênios | `index.html`, seção `#convenios` |
| Depoimentos | `assets/js/depoimentos.js` |
| Mapa e "Traçar rota" | `index.html`, `iframe` e link da seção `#localizacao` (hoje o mapa aponta para um local ilustrativo) |
| Instagram / Facebook / Google | links `href="#"` no rodapé e nos depoimentos |

## Identidade visual

- **Tipografia** — Montserrat nos títulos (Light nos títulos grandes, Bold no
  destaque); Inter no texto corrido.
- **Cores** — azul `#16698F` como cor principal e verde-água `#5CBDB3` como
  acento. Tokens em `:root` no `styles.css`.
- **Logo** — o símbolo do cabeçalho e o favicon são genéricos. Ver
  `assets/img/LEIA-ME.txt`.
