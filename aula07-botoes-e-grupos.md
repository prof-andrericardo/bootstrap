# 📘 Aula 07 – Botões e Grupos de Botões

## 🎯 Objetivos da Aula
- Aprender a utilizar os **botões padrão e avançados** do Bootstrap.
- Aplicar variações de **estilo, tamanho, estado e agrupamento** de botões.
- Compreender o uso de **ícones, acessibilidade e interatividade com botões**.
- Desenvolver seções com botões aplicáveis a formulários, navegação e ações.

---

## 🧠 1. A importância dos botões

Botões são os **elementos de ação mais importantes** em uma interface. Eles guiam o usuário a interagir com o sistema e realizam tarefas como:

- Enviar formulários
- Abrir modais
- Navegar entre seções
- Executar comandos (ex: "Salvar", "Excluir", "Voltar")

---

## 🧪 2. Estrutura de um botão no Bootstrap

```html
<button class="btn btn-primary">Clique aqui</button>
```

### ✳️ Explicação:
- `btn`: classe base obrigatória
- `btn-primary`: define a cor e estilo visual

> 🧠 Os botões podem ser usados tanto com `<button>` quanto com `<a>` ou `<input type="submit">`.

---

## 🎨 3. Variações de Estilo de Botões

| Classe            | Cor / Intenção        |
|------------------|------------------------|
| `btn-primary`     | Ação principal (azul)  |
| `btn-secondary`   | Ação secundária        |
| `btn-success`     | Sucesso (verde)        |
| `btn-danger`      | Erro ou perigo (vermelho) |
| `btn-warning`     | Aviso (amarelo)        |
| `btn-info`        | Informação (ciano)     |
| `btn-light`       | Claro (cinza claro)    |
| `btn-dark`        | Escuro (cinza escuro)  |
| `btn-link`        | Botão que parece um link |

```html
<a href="#" class="btn btn-success">Confirmar</a>
<input type="submit" class="btn btn-danger" value="Deletar">
```

---

## 🔍 4. Tamanhos e Larguras

| Classe           | Descrição                  |
|------------------|----------------------------|
| `btn-sm`         | Botão pequeno              |
| `btn-lg`         | Botão grande               |
| `w-100`          | Largura total da coluna    |

```html
<button class="btn btn-outline-dark btn-sm">Pequeno</button>
<button class="btn btn-primary btn-lg w-100 mt-2">Grande e largo</button>
```

---

## 🔄 5. Estados: Ativo, Desabilitado, Foco

```html
<!-- Botão ativo -->
<button class="btn btn-success active" aria-pressed="true">Ativo</button>

<!-- Botão desabilitado -->
<button class="btn btn-secondary" disabled>Desabilitado</button>
```

> ⚠️ Use `disabled` para `<button>` e `aria-disabled="true"` para `<a>` simulando um botão.

---

## 💡 6. Botões com Ícones

Você pode usar **Bootstrap Icons** para melhorar a compreensão visual.

```html
<button class="btn btn-outline-primary">
  <i class="bi bi-plus-circle"></i> Novo Item
</button>
```

> ✅ Sempre adicione `aria-label` se o botão não tiver texto visível.

---

## 🧱 7. Grupos de Botões

Botões podem ser agrupados horizontal ou verticalmente para representar **categorias, navegação ou filtros**.

```html
<div class="btn-group" role="group">
  <button class="btn btn-outline-primary">Dia</button>
  <button class="btn btn-outline-primary">Semana</button>
  <button class="btn btn-outline-primary">Mês</button>
</div>
```

📌 Você também pode empilhar botões:

```html
<div class="btn-group-vertical">
  <button class="btn btn-dark">Topo</button>
  <button class="btn btn-dark">Meio</button>
  <button class="btn btn-dark">Base</button>
</div>
```

---

## 🛠️ 8. Exemplo de uso em layout real

```html
<section class="container text-center py-5">
  <h2 class="mb-4">Escolha uma ação</h2>
  <div class="d-grid gap-2 d-sm-flex justify-content-sm-center">
    <button class="btn btn-primary btn-lg px-4">Salvar</button>
    <button class="btn btn-outline-secondary btn-lg px-4">Cancelar</button>
  </div>
</section>
```

---

## 🧪 9. Desafio Prático

1. Crie um grupo de botões com:
   - Três botões horizontais (`btn-outline-info`)
   - Um botão com ícone (`bi bi-arrow-right`)
   - Um botão desabilitado
2. Adicione uma nova linha abaixo com os mesmos botões em versão vertical (`btn-group-vertical`).
3. Estilize com `shadow`, `rounded` e `text-uppercase`.

---

## 🎓 10. Reflexões Técnicas

- Quando devo usar `btn-outline` ao invés de `btn` sólido?
- Como tornar botões mais acessíveis para leitores de tela?
- Qual a diferença entre `<button>`, `<a>` e `<input type="button">`?

---

## 📚 11. Referências e Leitura Recomendada

- [Documentação Bootstrap – Botões](https://getbootstrap.com/docs/5.3/components/buttons/)
- [Documentação Bootstrap – Grupos de Botões](https://getbootstrap.com/docs/5.3/components/button-group/)
- [Bootstrap Icons](https://icons.getbootstrap.com/)
- [WAI-ARIA Button Patterns](https://www.w3.org/WAI/ARIA/apg/patterns/button/)

---

## ✅ Conclusão

Botões são a base das interações em qualquer site moderno. Dominar suas variações, estilos e agrupamentos permite criar **interfaces poderosas, acessíveis e intuitivas**.

> Na próxima aula, aprenderemos a usar **Badges, Alertas e Cards** para enriquecer visualmente nossos layouts.

---
