# 📘 Aula 09 – Navbar com Colapso e Menu Mobile

## 🎯 Objetivos da Aula
- Compreender e aplicar o componente **Navbar** do Bootstrap.
- Criar menus de navegação responsivos com **colapso automático** em dispositivos móveis.
- Utilizar elementos como brand, links, dropdowns, ícones e botões na Navbar.
- Aplicar boas práticas de acessibilidade e design de navegação.

---

## 🧭 1. O que é a Navbar?

A **Navbar (barra de navegação)** é o elemento responsável por guiar o usuário pelas páginas e seções de um site. No Bootstrap, ela é:

- Responsiva automaticamente
- Flexível para incluir menus, logos, botões, ícones e até formulários
- Estilizada com cores, espaçamento e posição fixa se necessário

---

## 🧱 2. Estrutura básica da Navbar

```html
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container">
    <a class="navbar-brand" href="#">MeuSite</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
            data-bs-target="#menu" aria-controls="menu"
            aria-expanded="false" aria-label="Alternar navegação">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="menu">
      <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
        <li class="nav-item"><a class="nav-link active" href="#">Início</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Sobre</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Contato</a></li>
      </ul>
    </div>
  </div>
</nav>
```

---

## 🔍 3. Explicação do Código

- `navbar`: classe principal da barra
- `navbar-expand-lg`: expande o menu a partir do breakpoint `lg`
- `navbar-light` + `bg-light`: define cor de fundo clara e ícones escuros
- `navbar-brand`: logo ou nome do site
- `navbar-toggler`: botão de menu “hambúrguer”
- `collapse navbar-collapse`: define que o menu se esconde em telas menores
- `navbar-nav`: lista de itens de navegação
- `ms-auto`: alinha os itens à direita (margin-start automática)

---

## 🎨 4. Cores e estilos de Navbar

| Classe             | Estilo                  |
|--------------------|--------------------------|
| `navbar-light`     | Ícones escuros sobre fundo claro |
| `navbar-dark`      | Ícones claros sobre fundo escuro |
| `bg-primary`       | Fundo azul              |
| `bg-dark`          | Fundo escuro            |
| `bg-white`         | Fundo branco            |

---

## 📱 5. Comportamento responsivo

A combinação de `collapse` + `navbar-toggler` garante que a Navbar seja:

- **visível como menu completo** em telas grandes (`lg+`)
- **colapsada com botão de menu** em telas menores

> 🔁 O botão hamburguer ativa/desativa o menu escondido automaticamente.

---

## 🧠 6. Exemplo real com dropdown e botão

```html
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container">
    <a class="navbar-brand" href="#">TechPro</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
            data-bs-target="#navbarContent">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item"><a class="nav-link active" href="#">Início</a></li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown">
            Serviços
          </a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="#">Desenvolvimento</a></li>
            <li><a class="dropdown-item" href="#">Suporte</a></li>
          </ul>
        </li>
        <li class="nav-item"><a class="nav-link" href="#">Contato</a></li>
      </ul>
      <a href="#" class="btn btn-outline-light">Entrar</a>
    </div>
  </div>
</nav>
```

---

## 🔧 7. Fixando a Navbar no topo

Use `fixed-top` para que a Navbar **permaneça no topo da tela** ao rolar a página:

```html
<nav class="navbar fixed-top navbar-dark bg-dark"> ... </nav>
```

> 🧠 Combine com padding extra no `body` para evitar sobreposição de conteúdo:
```css
body {
  padding-top: 70px;
}
```

---

## 🧪 8. Desafio Prático

1. Crie uma navbar com:
   - Fundo `bg-primary` e texto claro
   - Um link ativo, dois comuns e um dropdown com dois itens
   - Um botão `Entrar` alinhado à direita
2. Aplique `navbar-expand-md` para que o colapso ocorra em tablets
3. Fixe a navbar no topo e ajuste o `body` com `padding-top`

---

## 🎓 9. Reflexões Técnicas

- Qual o impacto de uma navbar fixa na experiência do usuário?
- Como garantir que a navegação seja acessível por teclado e leitores de tela?
- Em que situações devemos ocultar ou modificar itens da navbar em dispositivos móveis?

---

## 📚 10. Referências Complementares

- [Navbar – Bootstrap Docs](https://getbootstrap.com/docs/5.3/components/navbar/)
- [Acessibilidade em Navegação – WAI](https://www.w3.org/WAI/tutorials/menus/)
- [Bootstrap Dropdowns](https://getbootstrap.com/docs/5.3/components/dropdowns/)

---

## ✅ Conclusão

A **Navbar** do Bootstrap é um componente essencial para qualquer site, oferecendo um menu de navegação elegante, **adaptável a qualquer dispositivo** e com suporte completo a recursos como colapso, dropdowns e botões.

> A próxima aula irá abordar **Modais e Collapse**, elementos-chave para interações contextuais no front-end.

---
