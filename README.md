# Péricles Tattoo e Piercing — Portfólio

Site institucional em página única (single page), desenvolvido em HTML, CSS e JavaScript puro, sem frameworks ou dependências de build. Serve como portfólio digital para tatuador e estúdio de piercing, com galeria de trabalhos filtrável por estilo.

## ✨ Funcionalidades

- **Galeria de trabalhos filtrável** por estilo (Traço Fino, Aquarela Marinha, Blackwork Suave, Old School Naval, Ornamental)
- **Lightbox** para visualização ampliada das fotos
- **Scroll reveal** — seções e cards surgem suavemente conforme o usuário rola a página
- **Totalmente responsivo** — menu adaptado para mobile, grid de fotos reflui automaticamente
- **Seção de Dúvidas Frequentes**
- **Bloco de contato** com links diretos para Instagram, WhatsApp e YouTube, além de endereço, horário de atendimento e formas de pagamento
- Respeita `prefers-reduced-motion` para usuários sensíveis a animação

## 🛠️ Tecnologias

- HTML5
- CSS3 (variáveis CSS, Grid, Flexbox, animações)
- JavaScript vanilla (sem dependências externas)
- Google Fonts (Fraunces, Jost, Space Mono)

## 📁 Estrutura de pastas

/
├── index.html # arquivo principal do site
└── imagens/ # fotos do portfólio e do artista
├── pericles.jpg
├── tattoo-01.png
├── tattoo-02.png
└── ...


> Crie a pasta `imagens/` na raiz do projeto e adicione os arquivos referenciados no HTML (ou ajuste os caminhos conforme sua organização).

## 🖼️ Como adicionar ou editar fotos do portfólio

A galeria é renderizada a partir de um array no final do arquivo HTML (`seedPhotos`). Para adicionar, remover ou editar uma peça, edite esse array:

```js
const seedPhotos = [
  { title: 'Tatuagem Leão', tag: 'Blackwork Suave · Braço', src: 'imagens/tattoo-01.png', cat: 'blackwork' },
  // adicione novos itens aqui
];
```

O campo `cat` precisa corresponder a um dos `data-filter` definidos nos botões de filtro (`fine-line`, `aquarela`, `blackwork`, `old-school`, `ornamental`). Para criar uma nova categoria, adicione também um novo botão em `.filters` no HTML.

## 🚀 Como rodar localmente

Por ser um projeto estático, basta abrir o `index.html` diretamente no navegador, ou servir a pasta com qualquer servidor local:

```bash
# usando Python
python3 -m http.server 8000

# ou usando Node (npx)
npx serve .
```

Depois acesse `http://localhost:8000`.

## 🌐 Deploy

Por não depender de backend, o projeto pode ser hospedado gratuitamente em qualquer serviço de hospedagem estática, como:

- GitHub Pages
- Netlify
- Vercel
- Cloudflare Pages

## 📬 Contato

Para dúvidas sobre o projeto, entre em contato com jcg5aquino@gmail.com.
