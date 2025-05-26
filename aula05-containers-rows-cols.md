# 📘 Aula 05 – Containers, Rows e Cols: Variações e Boas Práticas

## 🎯 Objetivos da Aula
- Explorar em profundidade os três pilares estruturais do Bootstrap: `container`, `row` e `col`.
- Entender as **variações avançadas** de containers e colunas com breakpoints.
- Aprender boas práticas de organização e escalabilidade de layout.
- Criar seções de página com responsividade real para múltiplos dispositivos.

---

## 🧱 1. Relembrando a base

No Bootstrap, a estrutura padrão de layout é sempre:

```html
<div class="container">
  <div class="row">
    <div class="col">Conteúdo</div>
  </div>
</div>
```

Mas o que acontece quando queremos um **layout full-width**, ou apenas com margens em resoluções maiores? E como garantir **legibilidade, fluidez e consistência visual**?

---

## 📦 2. Tipos de Containers

| Classe             | Descrição |
|--------------------|-----------|
| `container`        | Margens fixas com largura adaptativa |
| `container-fluid`  | 100% da largura da viewport em qualquer resolução |
| `container-{break}`| Ex: `container-md`: fixo a partir do breakpoint definido |

### 📌 Exemplo:

```html
<div class="container-fluid bg-dark text-white p-4">
  Este container ocupa toda a largura da tela.
</div>
```

### 💡 Prática:

Use `container` para o corpo do site e `container-fluid` para seções como banners, cabeçalhos ou rodapés.

---

## 📐 3. `row`: o organizador horizontal

A classe `row` utiliza `display: flex` para organizar o conteúdo horizontalmente.  
Ela também **remove automaticamente o padding lateral das colunas** com `margin-left` e `margin-right` negativo.

### ⚠️ Importante:
- A `row` deve estar **sempre** dentro de um `container`.
- As `col` devem estar **sempre** dentro de uma `row`.

---

## 🧩 4. `col`: a inteligência do layout

### 🧮 Variações:

| Classe            | Significado |
|------------------|-------------|
| `col`            | Divide igualmente o espaço restante |
| `col-6`          | Ocupa 6 das 12 colunas disponíveis |
| `col-md-4`       | Ocupa 4 colunas **a partir** do breakpoint `md` |
| `col-sm-12 col-md-6 col-lg-3` | Comportamento diferente em cada resolução |

### 📊 Tabela de breakpoints:

| Breakpoint | Classe prefixada | Resolução mínima |
|------------|------------------|------------------|
| Extra small | `col-`          | 0px              |
| Small       | `col-sm-`       | 576px            |
| Medium      | `col-md-`       | 768px            |
| Large       | `col-lg-`       | 992px            |
| X-Large     | `col-xl-`       | 1200px           |

---

## 🧪 5. Exemplo completo com responsividade total

```html
<div class="container my-5">
  <h2 class="mb-4 text-center">Galeria Responsiva</h2>
  <div class="row">
    <div class="col-sm-12 col-md-6 col-lg-3 mb-4">
      <div class="bg-primary text-white text-center p-5 rounded shadow-sm">
        Item 1
      </div>
    </div>
    <div class="col-sm-12 col-md-6 col-lg-3 mb-4">
      <div class="bg-success text-white text-center p-5 rounded shadow-sm">
        Item 2
      </div>
    </div>
    <div class="col-sm-12 col-md-6 col-lg-3 mb-4">
      <div class="bg-warning text-dark text-center p-5 rounded shadow-sm">
        Item 3
      </div>
    </div>
    <div class="col-sm-12 col-md-6 col-lg-3 mb-4">
      <div class="bg-danger text-white text-center p-5 rounded shadow-sm">
        Item 4
      </div>
    </div>
  </div>
</div>
```

> 🧩 Em telas pequenas: empilhado (`col-12`),  
> 🧩 Em tablets: 2 por linha (`col-md-6`),  
> 🧩 Em desktops: 4 por linha (`col-lg-3`).

---

## 🎨 6. Boas Práticas Visuais com Containers e Grid

### ✔️ Use:

- `container` para o conteúdo principal do site.
- `container-fluid` para banners, heros e seções 100% da tela.
- `row g-3` para adicionar espaçamento entre colunas.
- `col-auto` quando quiser que a coluna **se ajuste ao conteúdo**.
- `col-* offset-*` para centralizar ou criar margens laterais.

### ❌ Evite:

- Colocar `col` fora de uma `row`.
- Esquecer o `container`: o conteúdo ficará "colado" nas laterais.
- Usar `col-13` ou ultrapassar 12 unidades por linha.

---

## 🧱 7. Estrutura recomendada para seções

```html
<section class="container py-5">
  <div class="row align-items-center">
    <div class="col-md-6">
      <h2 class="fw-bold">Título de seção</h2>
      <p>Texto explicativo com margem e espaçamento controlado.</p>
    </div>
    <div class="col-md-6 text-center">
      <img src="imagem.jpg" alt="Descrição" class="img-fluid rounded">
    </div>
  </div>
</section>
```

---

## 🧪 8. Desafio Orientado

1. Crie uma estrutura `container-fluid` com uma `row` e 3 colunas (`col-md-4`).
2. Aplique `bg-light`, `p-5`, `rounded`, `text-center` e adicione ícones diferentes em cada uma.
3. Teste em **celular, tablet e desktop** (responsividade).
4. Adicione também uma nova `row` com 2 colunas e texto explicativo.

---

## 🧠 9. Reflexão Técnica

- Quando usar `col-auto` ao invés de `col-6`?
- Qual a diferença entre `container` e `container-md`?
- Como as boas práticas com grid evitam problemas de **legibilidade** e **acessibilidade**?

---

## 📚 10. Referências Técnicas e Didáticas

- [Bootstrap Grid System – Documentação](https://getbootstrap.com/docs/5.3/layout/grid/)
- [Bootstrap Layout Overview](https://getbootstrap.com/docs/5.3/layout/)
- [CSS Flexbox – MDN](https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_Flexible_Box_Layout)

---

## ✅ Conclusão

Nesta aula, aprofundamos a estrutura do Bootstrap com uso prático e consciente de containers, rows e cols.  
Agora você já consegue montar seções completas, organizadas e escaláveis, com **layouts reais e profissionais**.

> Na próxima aula, vamos estudar **breakpoints e responsividade em profundidade**, usando o Grid System adaptado a cada tela.

---
