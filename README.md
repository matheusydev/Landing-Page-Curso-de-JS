<div align="center">

# 🚀 Landing Page - Curso de JS

### _Um projeto de estudo com HTML, CSS e JavaScript puro._

<br/>

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Responsive](https://img.shields.io/badge/Responsive-Design-6D28D9?style=for-the-badge&logo=googlechrome&logoColor=white)

🔗 **Link do Projeto:** [landing-page-curso-de-js.netlify.app](#)

<br/>

> Landing page desenvolvida durante um curso de JavaScript, com foco em estruturação semântica de HTML, estilização modular com CSS puro e um menu responsivo construído sem uso de bibliotecas externas.

</div>

---

## 📋 Índice

- [📖 Sobre o Projeto](#-sobre-o-projeto)
- [🚀 Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [✨ Funcionalidades](#-funcionalidades)
- [💡 Conceitos Aplicados](#-conceitos-aplicados)
- [📁 Estrutura de Pastas](#-estrutura-de-pastas)
- [⚙️ Como Executar o Projeto](#️-como-executar-o-projeto)
- [🧩 Seções da Página](#-seções-da-página)
- [🎓 Aprendizados Adquiridos](#-aprendizados-adquiridos)
- [🔮 Melhorias Futuras](#-melhorias-futuras)

---

## 📖 Sobre o Projeto

A **Landing Page - Curso de JS** é um projeto de estudo construído com **HTML5** e **CSS3** puros, sem o uso de frameworks. A página simula um site institucional completo, com menu lateral responsivo, seções de conteúdo em grid, galeria de imagens, tabela de preços e formulário de contato.

O projeto foi construído com foco em:

- ✅ Estruturação semântica de HTML (`section`, `article`, `aside`, `fieldset`, `footer`)
- ✅ Organização de estilos em múltiplos arquivos CSS por responsabilidade
- ✅ Menu responsivo utilizando a técnica *checkbox hack* (sem JavaScript)
- ✅ Uso de variáveis CSS (`custom properties`) para padronização visual
- ✅ Layout em grid para exibição de conteúdo e galeria de imagens
- ✅ Tabela responsiva para exibição de planos/preços

---

## 🚀 Tecnologias Utilizadas

| Tecnologia | Descrição |
|---|---|
| [HTML5](https://developer.mozilla.org/pt-BR/docs/Web/HTML) | Estruturação semântica do conteúdo da página |
| [CSS3](https://developer.mozilla.org/pt-BR/docs/Web/CSS) | Estilização e responsividade, organizada em múltiplos arquivos |
| [Google Fonts](https://fonts.google.com/) | Fontes `Montserrat` (títulos) e `Open Sans` (textos) |
| [Picsum Photos](https://picsum.photos/) | Serviço de imagens aleatórias utilizado na galeria |

---

## ✨ Funcionalidades

- 🍔 **Menu Lateral Responsivo** — Menu retrátil ativado via checkbox, sem dependência de JavaScript
- 🏠 **Seção de Introdução** — Apresentação inicial com texto e imagem
- 🧱 **Seções em Grid** — Blocos de conteúdo organizados em cards (`grid-one` e `grid-two`)
- 🖼️ **Galeria de Imagens** — Grid responsivo com imagens dinâmicas
- 💰 **Tabela de Preços** — Tabela responsiva com cabeçalho, corpo e rodapé
- 📬 **Formulário de Contato** — Campos de nome, sobrenome, e-mail e mensagem
- ⬆️ **Botão "Voltar ao Topo"** — Link de retorno rápido para o início da página

---

## 💡 Conceitos Aplicados

### 🍔 Menu Responsivo com *Checkbox Hack*

O menu lateral é controlado por um `<input type="checkbox">` oculto, combinado com um `<label>`. Isso permite abrir e fechar o menu utilizando apenas CSS, sem necessidade de JavaScript.

```html
<input id="close-menu" class="close-menu" type="checkbox" aria-label="Close menu" role="button">
<label class="close-menu-label" for="close-menu" title="close menu"></label>
```

O estado do checkbox (marcado/desmarcado) é usado nos seletores CSS para exibir ou ocultar o menu.

---

### 🎨 Organização de CSS por Responsabilidade

Os estilos são divididos em arquivos separados, cada um com uma responsabilidade específica:

```html
<link rel="stylesheet" href="assets/css/variables.css">
<link rel="stylesheet" href="assets/css/elements.css">
<link rel="stylesheet" href="assets/css/classes.css">
<link rel="stylesheet" href="assets/css/menu.css">
<link rel="stylesheet" href="assets/css/styles.css">
```

| Arquivo | Responsabilidade |
|---|---|
| `variables.css` | Variáveis CSS globais (cores, espaçamentos, fontes) |
| `elements.css` | Estilos base para elementos HTML nativos |
| `classes.css` | Classes utilitárias reutilizáveis |
| `menu.css` | Estilos específicos do menu lateral |
| `styles.css` | Estilos gerais das seções da página |

---

### 🧱 Layout em Grid

As seções `grid-one`, `gallery` e `grid-two` utilizam uma classe `.grid` para organizar o conteúdo (cards ou imagens) em colunas responsivas.

```html
<div class="grid">
  <article>
    <h3>Teste 1</h3>
    <p>Conteúdo do card...</p>
  </article>
  <!-- ... -->
</div>
```

---

### 📊 Tabela Responsiva

A tabela de preços é envolvida por um contêiner `.responsive-table`, permitindo rolagem horizontal em telas pequenas sem quebrar o layout.

```html
<div class="responsive-table">
  <table>
    <caption>Pricing table</caption>
    <thead>...</thead>
    <tbody>...</tbody>
    <tfoot>...</tfoot>
  </table>
</div>
```

---

## 📁 Estrutura de Pastas

```
Landing-Page-Curso-de-JS/
│
├── assets/
│   ├── css/
│   │   ├── variables.css       # Variáveis globais (cores, fontes, espaçamentos)
│   │   ├── elements.css        # Estilos base de elementos HTML
│   │   ├── classes.css         # Classes utilitárias
│   │   ├── menu.css            # Estilos do menu responsivo
│   │   └── styles.css          # Estilos gerais das seções
│   └── img/
│       └── javascript.svg      # Logo HTML/CSS/JS utilizada na página
│
├── index.html                  # Estrutura principal da landing page
└── README.md
```

---

## ⚙️ Como Executar o Projeto

### Pré-requisitos

- Um navegador web atualizado
- [Git](https://git-scm.com/) (opcional, para clonar o repositório)

### Clonando o Repositório

```bash
# Clone este repositório
git clone https://github.com/matheusydev/Landing-Page-Curso-de-JS.git

# Acesse a pasta do projeto
cd Landing-Page-Curso-de-JS
```

### Executando

Como é um projeto estático (HTML + CSS), basta abrir o arquivo `index.html` diretamente no navegador, ou utilizar uma extensão como o **Live Server** (VS Code) para melhor experiência de desenvolvimento com recarregamento automático.

---

## 🧩 Seções da Página

| Seção | ID | Descrição |
|---|---|---|
| Menu | `aside.menu` | Menu lateral retrátil com navegação por âncoras |
| Home/Intro | `#home` | Seção de abertura com texto de destaque e imagem |
| Sobre | `#intro` | Bloco de texto informativo |
| Grid One | `#grid-one` | Primeira seção de cards em grid |
| Galeria | `#gallery` | Galeria de imagens em grid |
| Grid Two | `#grid-two` | Segunda seção de cards em grid |
| Preços | `#pricing` | Tabela de planos/preços responsiva |
| Contato | `#contact` | Formulário de contato |
| Footer | `#footer` | Rodapé com créditos e link do GitHub |

---

## 🎓 Aprendizados Adquiridos

Ao desenvolver este projeto, os seguintes conhecimentos foram consolidados na prática:

- ✅ **Estruturação semântica** de HTML5 (`section`, `article`, `aside`, `fieldset`)
- ✅ **Menu responsivo sem JavaScript** utilizando a técnica *checkbox hack*
- ✅ **Organização de CSS em múltiplos arquivos** por responsabilidade
- ✅ **Variáveis CSS (custom properties)** para padronização de cores e espaçamentos
- ✅ **Layout em grid** para organização de conteúdo e imagens
- ✅ **Tabelas responsivas** com `thead`, `tbody` e `tfoot`
- ✅ **Formulários acessíveis** com `label`, `fieldset` e `legend`

---

## 🔮 Melhorias Futuras

O projeto está em constante evolução. As próximas melhorias planejadas incluem:

- [ ] 📱 **Menu Hambúrguer Animado** — Adicionar transições suaves de abertura/fechamento
- [ ] 🎯 **Scroll Suave** — Implementar `scroll-behavior: smooth` para navegação por âncoras
- [ ] 📬 **Validação de Formulário** — Adicionar validação client-side com JavaScript
- [ ] 🌗 **Tema Dark/Light** — Alternância entre modo claro e escuro
- [ ] 🖼️ **Lazy Loading de Imagens** — Otimizar carregamento da galeria
- [ ] ♿ **Melhorias de Acessibilidade** — Revisão de contraste, foco e navegação por teclado
- [ ] 🧪 **Integração com JavaScript** — Adicionar interatividade prevista pelo curso

---
