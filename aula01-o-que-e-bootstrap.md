# 📘 Aula 01 – O que é o Bootstrap?

## 🎯 Objetivos da Aula
- Compreender o conceito de **frameworks CSS** com foco em Bootstrap.
- Identificar os problemas que o Bootstrap resolve no desenvolvimento web.
- Diferenciar o uso de CSS puro e classes utilitárias.
- Preparar o ambiente de desenvolvimento para as próximas aulas.

---

## 📖 1. Introdução ao Bootstrap

Bootstrap é um **framework front-end open-source** criado para facilitar o desenvolvimento de interfaces web modernas. Ele oferece uma vasta biblioteca de **classes CSS pré-definidas**, componentes prontos (como botões, navbars, modais, etc.) e um **sistema de grid responsivo** baseado em 12 colunas.

> 📌 Bootstrap foi desenvolvido por Mark Otto e Jacob Thornton no Twitter em 2011.

---

## 🔎 2. Por que utilizar Bootstrap?

Ao trabalhar com projetos web sem frameworks, é comum escrever dezenas ou centenas de linhas de CSS para construir elementos comuns como botões, menus ou formulários. Bootstrap fornece soluções prontas e testadas para isso.

### 🛠 Problemas que o Bootstrap resolve:
- Inconsistência visual em navegadores diferentes.
- Repetição de código CSS.
- Dificuldade em aplicar responsividade manualmente.
- Falta de padrão visual em grandes projetos.

### ✅ Vantagens práticas:
| ✅ Vantagem | 💬 Descrição |
|------------|-------------|
| Rapidez | Criação de layouts com menos código |
| Mobile First | Padrão nativo: responsivo desde o início |
| Componentes prontos | Botões, menus, modais, formulários, etc. |
| Utilitários CSS | Classes como `mt-3`, `text-center`, `d-flex` |
| Integração com JS | Modais, tooltips e carrosséis com Bootstrap JS |

---

## 🧠 3. Como o Bootstrap funciona?

O Bootstrap funciona através da aplicação de **classes CSS** já preparadas, que você aplica diretamente nos seus elementos HTML. Não é necessário escrever seu próprio CSS para tudo.

### 🎯 Exemplo prático

#### 🔧 Sem Bootstrap
```html
<button style="padding: 10px 20px; background-color: blue; color: white; border-radius: 5px;">
  Enviar
</button>
```

#### ✅ Com Bootstrap
```html
<button class="btn btn-primary">
  Enviar
</button>
```

> 🔍 `btn` aplica o estilo base, `btn-primary` define cor azul com hover elegante e responsivo.

---

## ⚙️ 4. Distribuição e Instalação

### 🚀 Formas de usar o Bootstrap:

| Método | Quando usar |
|--------|-------------|
| CDN | Projetos didáticos, testes rápidos, protótipos |
| Download | Projetos offline ou internos |
| npm / yarn | Projetos com Node.js, Vite, Webpack |

Exemplo via **CDN**:

```html
<!-- Bootstrap CSS -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">

<!-- Bootstrap JS (com funcionalidades de Collapse, Modal, etc) -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
```

---

## 🏗️ 5. Estrutura típica de um projeto com Bootstrap

```plaintext
meu-projeto/
├── index.html
├── assets/
│   ├── css/style.css
│   └── js/main.js
└── imagens/
```

No `index.html`, você adicionará os links CDN no `<head>` para usar Bootstrap em qualquer elemento HTML.

---

## 💬 6. Curiosidades sobre o Bootstrap

- A primeira versão pública foi lançada em agosto de 2011.
- O nome original era “Twitter Blueprint”.
- Desde a versão 4, o Bootstrap adotou o padrão **mobile first** por padrão.
- Atualmente na versão 5.3, o framework deixou de usar jQuery como dependência obrigatória.

---

## 🧪 7. Atividade Prática

### Parte 1 – Pesquisa
- Acesse pelo menos **3 sites populares** que usam Bootstrap.
- Liste quais componentes do Bootstrap você identificou em cada um (navbar, botão, modal, etc).

### Parte 2 – Mão na massa
Crie um arquivo `index.html` com o seguinte conteúdo:

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Meu Primeiro Bootstrap</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="text-center py-5">

  <h1 class="mb-4">Meu primeiro site com Bootstrap</h1>
  <p class="lead">Estou aprendendo a usar um dos frameworks mais usados do mundo!</p>
  <button class="btn btn-success btn-lg">Clique aqui</button>

</body>
</html>
```

Salve, abra no navegador e explore.

---

## 🧠 8. Desafio Criativo

Crie uma **landing page simples** com os seguintes elementos:
- Um cabeçalho com título e subtítulo
- Um botão com estilo `btn-danger`
- Um parágrafo com `text-muted`
- Responsividade mínima (usar container e `text-center`)

---

## 📚 9. Referências e Leitura Complementar

- [Documentação Oficial do Bootstrap 5](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- [W3Schools - Bootstrap 5](https://www.w3schools.com/bootstrap5/)
- [MDN Web Docs – HTML e CSS](https://developer.mozilla.org/pt-BR/)
- [Bootstrap Expo – Sites criados com Bootstrap](https://expo.getbootstrap.com/)

---

## ✅ Conclusão

O Bootstrap é mais que um framework: é um **aliado poderoso na produtividade de desenvolvedores web**, promovendo acessibilidade, responsividade e visual moderno. Compreender sua estrutura será essencial para o restante do curso.

Na próxima aula, aprenderemos como **integrar o Bootstrap em nossos projetos via CDN** e configuraremos um ambiente profissional para nossos estudos.

---
