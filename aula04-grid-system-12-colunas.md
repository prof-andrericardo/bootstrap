# 📘 Aula 04 – Introdução ao Grid System (Sistema de 12 Colunas)

## 🎯 Objetivos da Aula
- Entender como o Bootstrap organiza o layout com seu **Sistema de Grid Responsivo**.
- Compreender a lógica das **12 colunas flexíveis** e o comportamento em diferentes dispositivos.
- Aplicar o Grid na prática para criar **layouts reais e responsivos**.
- Estimular o raciocínio visual e lógico no design web com **exemplos práticos, comentados e escaláveis**.

## 🧭 1. Por que o Grid é tão importante?

Imagine que você precisa montar uma página com 3 colunas. Em CSS puro, isso exigiria várias regras, `media queries`, alinhamentos, flexbox, margens...  
Com o **Bootstrap**, essa estrutura já vem pronta, testada, responsiva e funcional.

> 💡 O Grid é como um “esqueleto invisível” que estrutura o layout da página.

---

## 🧱 2. Anatomia do Grid: `container > row > col`

O Grid do Bootstrap é baseado em 3 elementos fundamentais:

1. `container`: delimita a largura da área visível.
2. `row`: cria uma **linha** horizontal.
3. `col`: divide a linha em colunas (até 12 por linha).

### 🖼️ Visualmente:
```
<div class="container">
  <div class="row">
    <div class="col">Coluna 1</div>
    <div class="col">Coluna 2</div>
  </div>
</div>
```

---

## 🔢 3. Por que 12 colunas?

12 é um número **altamente divisível**:
- 2 colunas: `col-6 col-6`
- 3 colunas: `col-4 col-4 col-4`
- 4 colunas: `col-3 col-3 col-3 col-3`
- 6 colunas: `col-2 col-2 col-2 col-2 col-2 col-2`

Isso permite combinações extremamente flexíveis para qualquer tipo de layout.

---

## 💻 4. Exemplo básico – 3 colunas iguais

```html
<div class="container my-5">
  <div class="row">
    <div class="col text-center bg-primary text-white p-3">Coluna 1</div>
    <div class="col text-center bg-success text-white p-3">Coluna 2</div>
    <div class="col text-center bg-danger text-white p-3">Coluna 3</div>
  </div>
</div>
```

> 🎯 `col` sem número significa “divida igualmente o espaço restante”.

---

## ⚙️ 5. Exemplo com colunas de tamanhos diferentes

```html
<div class="container my-5">
  <div class="row">
    <div class="col-4 bg-dark text-white p-3">Sidebar (col-4)</div>
    <div class="col-8 bg-light p-3">Conteúdo principal (col-8)</div>
  </div>
</div>
```

> ✅ Sempre que somar os `col-n`, o total deve ser 12 por linha.

---

## 🔄 6. Tornando o layout responsivo com breakpoints

O Bootstrap permite definir **comportamentos diferentes para diferentes tamanhos de tela**.

### 📱 Exemplo com `col-sm`, `col-md`, `col-lg`:

```html
<div class="row">
  <div class="col-12 col-md-6 col-lg-4 p-3 bg-warning">1ª Coluna</div>
  <div class="col-12 col-md-6 col-lg-4 p-3 bg-info text-white">2ª Coluna</div>
  <div class="col-12 col-lg-4 p-3 bg-secondary text-white">3ª Coluna</div>
</div>
```

📌 Interpretação:
- Telas pequenas: todas ocupam `col-12` → empilhadas.
- Telas médias: ocupam `col-6` → 2 por linha.
- Telas grandes: ocupam `col-4` → 3 por linha.

---

## 🧠 7. Prática Guiada – Criando um layout de serviço

```html
<div class="container py-5">
  <h2 class="text-center mb-4">Nossos Serviços</h2>
  <div class="row text-center">
    <div class="col-sm-6 col-lg-4 mb-4">
      <div class="p-4 bg-light border rounded shadow-sm h-100">
        <i class="bi bi-laptop fs-1 text-primary mb-3"></i>
        <h5>Desenvolvimento Web</h5>
        <p>Criação de sites responsivos com tecnologias modernas.</p>
      </div>
    </div>
    <div class="col-sm-6 col-lg-4 mb-4">
      <div class="p-4 bg-light border rounded shadow-sm h-100">
        <i class="bi bi-phone fs-1 text-success mb-3"></i>
        <h5>Apps Mobile</h5>
        <p>Aplicativos híbridos com excelente desempenho.</p>
      </div>
    </div>
    <div class="col-sm-6 col-lg-4 mb-4">
      <div class="p-4 bg-light border rounded shadow-sm h-100">
        <i class="bi bi-shield-lock fs-1 text-danger mb-3"></i>
        <h5>Segurança</h5>
        <p>Consultoria em segurança digital e LGPD.</p>
      </div>
    </div>
  </div>
</div>
```

---

## 🧪 8. Desafios Interativos

1. Crie um layout com:
   - Uma `row` com 4 colunas iguais (`col-3`), coloridas.
   - Uma `row` com 2 colunas (`col-8` e `col-4`), simulando conteúdo e barra lateral.
   - Use `container-fluid` para um layout full-width.
   - Adicione ícones com Bootstrap Icons.

2. Teste o layout em diferentes larguras de tela e analise:
   - Os elementos colapsam corretamente?
   - A ordem dos elementos está clara?

---

## 🎓 9. Reflexões Técnicas

- O sistema de Grid do Bootstrap substitui o Flexbox? (Não. Ele é **baseado em Flexbox**.)
- Quais cuidados tomar ao usar `col` sem número?
- Como o uso incorreto do Grid pode afetar a acessibilidade?

---

## 📚 10. Referências e Leitura Avançada

- [Bootstrap Grid – Documentação Oficial](https://getbootstrap.com/docs/5.3/layout/grid/)
- [Flexbox Guide – CSS Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [Bootstrap Examples – Layouts reais](https://getbootstrap.com/docs/5.3/examples/)

---

## ✅ Conclusão

O **Sistema de Grid** é um dos pilares do Bootstrap e do desenvolvimento web moderno. Ele permite **pensar visualmente** o layout e montar estruturas com total controle da responsividade.

> A partir da próxima aula, vamos aprofundar nos **Containers, Rows e Cols com variações práticas**.

---
