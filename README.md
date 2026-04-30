# Vinheria Agnello

Site da **Vinheria Agnello**: loja especializada em vinhos que une atendimento consultivo (uvas, regiões, safras, harmonização) à experiência digital, com foco em armazenagem adequada e curadoria de rótulos nacionais e internacionais.

## Estrutura do projeto

Organização dos arquivos e função de cada página:

| Arquivo | Descrição |
|--------|-----------|
| `index.html` | Página inicial: proposta da vinheria, diferenciais e compromisso com qualidade. |
| `src/pages/historia.html` | Nossa história: origem da empresa, tradição no atendimento, visão de futuro e vídeo institucional. |
| `src/pages/produtos.html` | Catálogo por faixas (básicos, intermediários, premium), com imagens dos produtos. |
| `src/pages/harmonizacao.html` | Harmonização: guia de combinações entre vinhos e tipos de pratos (inclui tabela de referência). |
| `src/pages/contato.html` | Contato: canal para dúvidas e recomendações, com formulário (nome, e-mail, mensagem). |
| `src/css/style.css` | Estilos globais (classes e IDs). |
| `src/css/efeitos.css` | Efeitos globais (pseudo elementos, classes, transições e animações). |
| `src/assets/imgs/` | Imagens utilizadas nas páginas. |
| `src/assets/vids/` | Vídeo das instalações da vinheria. |

O menu de navegação aparece em todas as páginas, com links internos entre **Início**, **Nossa História**, **Produtos**, **Harmonização** e **Contato**.

```
cp1-Front-End-Design/
├── index.html
├── README.md
├── src/
│   ├── assets/
│   │   ├── imgs/
│   │   └── vids/
│   ├── css/
│   │   └── style.css
│   │   └── efeitos.css
│   └── pages/
│       ├── contato.html
│       ├── harmonizacao.html
│       ├── historia.html
│       └── produtos.html
```
## Efeitos visuais
O projeto utiliza recursos avançados de CSS para melhorar a experiência do usuário, incluindo pseudo-classes, pseudo-elementos e transformações com transições suaves.

## Pseudo-elementos
Foram utilizados pseudo-elementos para adicionar detalhes visuais sem alterar o HTML:

.selo::before {
    content: "🍷 ";
}

.selo::after {
    content: " 🍷";
}

.card h2::after {
    content: "";
    display: block;
    width: 3.2rem;
    height: 3px;
    background-color: #c69a4a;
}
Adiciona ícones decorativos automaticamente.
Cria uma linha estilizada abaixo dos títulos.

## Pseudo-classes
As pseudo-classes foram usadas para criar interatividade:

.menu a:not(.ativo):hover {
    transform: translateY(-2px);
}

.botao:focus-visible {
    outline: 2px solid #e6c995;
}
Links do menu se movimentam ao passar o mouse.
Destaque visual ao navegar com teclado.

## Animação


## Transformações e transições 
Foram aplicadas transformações CSS para criar animações suaves:

.card:hover {
    transform: scale(1.05) translateY(-5px);
}

figure img:hover {
    transform: rotate(3deg) scale(1.05);
}
Cards aumentam e sobem ao passar o mouse.
Imagens giram levemente.

as transições
.card {
  transition: transform 0.3s ease;
 } 
figure img {
 transition: transform 0.3s ease; 
}

## Integrantes

- Artur Brandi (RM570258)
- Victor Godoy  (RM571454)
- Victor Heineken (RM570782)

## Site publicado (GitHub Pages)

**[Case Vinheria Agnello](https://arturfbrandi.github.io/cp1-Front-End-Design/index.html)**
