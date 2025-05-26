# 📘 Aula 08 – Alertas, Badges, Cards e Imagens no Bootstrap

## 🎯 Objetivos da Aula
- Compreender e aplicar componentes visuais do Bootstrap: **Alertas, Badges, Cards e Imagens**.
- Utilizar esses componentes para transmitir informações, notificações e apresentar conteúdo visual de forma eficiente.
- Aplicar boas práticas de acessibilidade e design informativo.
- Construir seções reais utilizando múltiplos componentes integrados.

---

## 🧩 1. Alertas – Informações e mensagens rápidas

Os **alertas** são componentes visuais para exibir mensagens informativas, de sucesso, erro ou aviso.

```html
<div class="alert alert-success" role="alert">
  ✔️ Ação realizada com sucesso!
</div>
```

### 🎨 Tipos de alertas

| Classe             | Finalidade                 |
|--------------------|----------------------------|
| `alert-primary`    | Informações gerais         |
| `alert-secondary`  | Informações neutras        |
| `alert-success`    | Sucesso                    |
| `alert-danger`     | Erro ou falha              |
| `alert-warning`    | Alerta ou aviso            |
| `alert-info`       | Informação leve            |
| `alert-light`      | Fundo claro                |
| `alert-dark`       | Fundo escuro               |

### ✅ Alertas com links

```html
<div class="alert alert-warning" role="alert">
  Atenção! <a href="#" class="alert-link">Clique aqui</a> para saber mais.
</div>
```

---

## 🏷️ 2. Badges – Indicadores rápidos

Os **badges** são pequenos elementos que servem como **etiquetas ou contadores**, geralmente usados em botões, menus ou títulos.

```html
<h4>Notificações <span class="badge bg-danger">4</span></h4>
```

### 🧠 Exemplo com botão:

```html
<button class="btn btn-primary">
  Mensagens <span class="badge bg-light text-dark">2</span>
</button>
```

### 🎨 Variações de cores: `bg-success`, `bg-warning`, `bg-info`, `bg-secondary`...

> 💡 Badges devem sempre manter **contraste adequado e legibilidade.**

---

## 📦 3. Cards – Componentes completos de apresentação

Um **card** é um container flexível para conteúdo visual e textual, geralmente com borda, sombra e layout modular.

### 🧱 Exemplo simples:

```html
<div class="card" style="width: 18rem;">
  <img src="https://via.placeholder.com/300x200" class="card-img-top" alt="Imagem de exemplo">
  <div class="card-body">
    <h5 class="card-title">Título do Card</h5>
    <p class="card-text">Descrição com conteúdo breve e contextual.</p>
    <a href="#" class="btn btn-outline-primary">Saiba mais</a>
  </div>
</div>
```

### 🔁 Variações:
- Adição de listas
- Cards com cabeçalhos e rodapés
- Cards com imagens, botões, textos e links

```html
<div class="card text-white bg-dark mb-3">
  <div class="card-header">Destaque</div>
  <div class="card-body">
    <h5 class="card-title">Card escuro</h5>
    <p class="card-text">Ideal para seções sobrepostas em imagens.</p>
  </div>
</div>
```

---

## 🖼️ 4. Imagens com Responsividade

No Bootstrap, imagens podem ser adaptadas com classes como:

| Classe         | Descrição                       |
|----------------|----------------------------------|
| `img-fluid`    | Escala automaticamente           |
| `rounded`      | Bordas arredondadas              |
| `rounded-circle` | Imagem circular                |
| `img-thumbnail`| Borda com padding e contorno     |

```html
<img src="foto.jpg" class="img-fluid rounded" alt="Exemplo de imagem">
```

> 📌 Sempre utilize `alt="descrição"` para acessibilidade e SEO.

---

## 🧠 5. Projeto Prático – Cards com badges e botões

```html
<div class="container py-5">
  <div class="row g-4">
    <div class="col-md-4">
      <div class="card h-100">
        <img src="https://via.placeholder.com/600x400" class="card-img-top" alt="Serviço">
        <div class="card-body">
          <h5 class="card-title">
            Web Design <span class="badge bg-info text-dark">Novo</span>
          </h5>
          <p class="card-text">Criamos layouts modernos, acessíveis e responsivos.</p>
          <a href="#" class="btn btn-primary">Solicitar orçamento</a>
        </div>
      </div>
    </div>
    <!-- Repetir colunas para mais cards -->
  </div>
</div>
```

---

## 🧪 6. Desafio da Aula

1. Crie uma seção de **destaques do site** com:
   - 3 cards lado a lado (`col-md-4`)
   - Cada card deve conter:
     - Uma imagem com `img-fluid`
     - Um título com `badge`
     - Um botão com `btn-outline-*`
2. Insira um **alerta personalizado** acima dos cards com `alert-success`.
3. Verifique a responsividade em telas pequenas.

---

## 🎓 7. Reflexões Técnicas

- Quando utilizar cards ao invés de apenas colunas e textos?
- Como tornar badges e alertas mais acessíveis (ex: leitores de tela)?
- Quais boas práticas visuais aplicam-se a cards com imagens?

---

## 📚 8. Referências Complementares

- [Bootstrap – Alertas](https://getbootstrap.com/docs/5.3/components/alerts/)
- [Bootstrap – Badges](https://getbootstrap.com/docs/5.3/components/badge/)
- [Bootstrap – Cards](https://getbootstrap.com/docs/5.3/components/card/)
- [Bootstrap – Imagens](https://getbootstrap.com/docs/5.3/content/images/)

---

## ✅ Conclusão

Com Alertas, Badges, Cards e Imagens, conseguimos construir **interfaces visuais completas e informativas**, mantendo uma identidade visual coesa e moderna.

> Na próxima aula, exploraremos a **Navbar e seus modos responsivos**, preparando a base de menus de navegação para nossos projetos.

---
