# 📘 Aula 03 – Anatomia do Bootstrap

## 🎯 Objetivos da Aula
- Compreender a estrutura organizacional do Bootstrap.
- Identificar os principais elementos da "anatomia" de um projeto com Bootstrap.
- Aprender sobre containers, rows, cols e classes utilitárias.
- Criar uma estrutura básica reutilizável para os próximos projetos.

---

## 🧠 1. O que é a Anatomia do Bootstrap?

A **anatomia do Bootstrap** se refere à forma como o framework organiza os elementos na página, incluindo:

- **Containers**: delimitadores da largura do conteúdo.
- **Rows**: linhas onde os elementos são agrupados.
- **Columns**: colunas flexíveis que organizam o layout.
- **Classes Utilitárias**: pequenas classes CSS que adicionam espaçamento, cores, alinhamentos, etc.

Essa estrutura segue o modelo **flexbox**, altamente personalizável e responsivo.

---

## 🧱 2. Containers – A base de tudo

Containers são os **blocos principais de layout** do Bootstrap. Eles definem os limites laterais do conteúdo.

| Tipo de Container | Descrição |
|-------------------|-----------|
| `container` | Largura fixa em cada breakpoint |
| `container-fluid` | Ocupa 100% da largura da viewport |
| `container-{breakpoint}` | Ex: `container-md` – fixo a partir de determinado tamanho |

### 💡 Exemplo:
```html
<div class="container">
  <p>Este conteúdo possui margens laterais automáticas.</p>
</div>
```

---

## 🧩 3. Rows e Columns – Sistema de Grid 12 colunas

O Bootstrap divide cada linha (`row`) em **12 colunas virtuais**. Você pode combiná-las como desejar, respeitando o total de 12.

```html
<div class="container">
  <div class="row">
    <div class="col-4">1/3 da largura</div>
    <div class="col-8">2/3 da largura</div>
  </div>
</div>
```

### 🔢 Outras combinações válidas:
- `col-6` + `col-6`
- `col-3` + `col-3` + `col-6`
- `col-2` + `col-10`

> ✅ As colunas usam flexbox por padrão e se ajustam automaticamente.

---

## 🖌️ 4. Classes Utilitárias (Utility Classes)

O Bootstrap oferece centenas de classes para ajustes rápidos e sem escrever CSS.

### Exemplos úteis:

| Classe | Função |
|--------|--------|
| `mt-3`, `mb-4`, `py-2` | Margens/Paddings top/bottom |
| `text-center`, `text-end` | Alinhamento de texto |
| `bg-light`, `bg-dark`, `text-muted` | Cores de fundo e texto |
| `d-flex`, `justify-content-center` | Layout flexbox |
| `rounded`, `shadow`, `border` | Estilo visual |

### 💡 Exemplo:
```html
<p class="text-center text-muted mt-4">
  Este parágrafo está centralizado, com cor de texto suave e margem no topo.
</p>
```

---

## 🧪 5. Exemplo Completo de Estrutura Base

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Anatomia do Bootstrap</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <div class="container py-5">
    <h1 class="text-center mb-4">Anatomia do Bootstrap</h1>

    <div class="row">
      <div class="col-md-6 bg-light p-3">
        <p>Coluna 1 de 2</p>
      </div>
      <div class="col-md-6 bg-secondary text-white p-3">
        <p>Coluna 2 de 2</p>
      </div>
    </div>

    <div class="text-center mt-4">
      <button class="btn btn-outline-primary">Clique aqui</button>
    </div>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

---

## 🎯 6. Desafio Prático

1. Crie um layout com 3 colunas (`col-4`) em telas grandes e 1 coluna (`col-12`) em telas pequenas.
2. Utilize `container-fluid`, `bg-dark`, `text-white` e `text-center`.
3. Adicione um título e um subtítulo com espaçamento e estilização adequada usando utilitários.

---

## 🧠 7. Reflexões

- Por que o Bootstrap usa 12 colunas ao invés de 10 ou 16?
- Qual a vantagem de usar utilitários CSS ao invés de criar suas próprias regras no arquivo `.css`?
- Como o Flexbox influencia o comportamento das colunas?

---

## 📚 8. Referências Externas

- [Documentação oficial – Layout e Grid](https://getbootstrap.com/docs/5.3/layout/grid/)
- [Utility API Bootstrap](https://getbootstrap.com/docs/5.3/utilities/api/)
- [Flexbox MDN Web Docs](https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_Flexible_Box_Layout)

---

## ✅ Conclusão

A estrutura `container > row > col` é o **coração do layout do Bootstrap**. Compreendê-la é essencial para dominar qualquer projeto visual com o framework.

A partir da próxima aula, começaremos a trabalhar com **componentes prontos**, como **botões, cards e alertas**.

---
