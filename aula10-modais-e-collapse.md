# 📘 Aula 10 – Modais e Collapse (FAQ Interativo e Popups Responsivos)

## 🎯 Objetivos da Aula
- Compreender e aplicar os componentes **Modal** e **Collapse** do Bootstrap.
- Criar **janelas flutuantes (pop-ups)** e **seções expansíveis** com interatividade.
- Integrar modais e collapses em fluxos reais como **FAQ, formulários, confirmações e navegação oculta**.
- Aplicar boas práticas de acessibilidade e responsividade nestes elementos.

---

## 🧩 1. O que é um Modal?

Um **Modal** é uma janela sobreposta à interface principal que exige a atenção do usuário. Ele pode conter:

- Mensagens
- Confirmações
- Formulários
- Conteúdo extra ou interativo

> ✅ Ideal para interações pontuais e não permanentes.

---

## 📦 2. Estrutura básica do Modal

```html
<!-- Botão que aciona o modal -->
<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#meuModal">
  Abrir Modal
</button>

<!-- Estrutura do Modal -->
<div class="modal fade" id="meuModal" tabindex="-1" aria-labelledby="tituloModal" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="tituloModal">Título do Modal</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Fechar"></button>
      </div>
      <div class="modal-body">
        Conteúdo interno do modal.
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Fechar</button>
        <button type="button" class="btn btn-primary">Salvar</button>
      </div>
    </div>
  </div>
</div>
```

---

## 🔍 3. Explicações importantes

- `data-bs-toggle="modal"`: ativa o modal ao clicar
- `fade`: efeito de transição
- `aria-*`: atributos de acessibilidade
- `btn-close`: botão com ícone de “X”
- `modal-dialog`: controla o tamanho (`modal-lg`, `modal-sm`, `modal-fullscreen`)

---

## 🧠 4. Modal em ação – Formulário de contato

```html
<div class="modal fade" id="contatoModal" tabindex="-1">
  <div class="modal-dialog modal-lg">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title">Fale Conosco</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
      </div>
      <div class="modal-body">
        <form>
          <div class="mb-3">
            <label for="nome" class="form-label">Nome</label>
            <input type="text" class="form-control" id="nome" placeholder="Seu nome completo">
          </div>
          <div class="mb-3">
            <label for="mensagem" class="form-label">Mensagem</label>
            <textarea class="form-control" id="mensagem" rows="3"></textarea>
          </div>
          <button type="submit" class="btn btn-primary">Enviar</button>
        </form>
      </div>
    </div>
  </div>
</div>
```

---

## 📚 5. O que é Collapse?

O **Collapse** permite **mostrar ou esconder conteúdo** ao clicar em botões ou links, sem sair da página.

> 🔁 Ideal para FAQ, menus ocultos, blocos de ajuda, etc.

---

## 🧱 6. Estrutura básica do Collapse

```html
<p>
  <a class="btn btn-outline-info" data-bs-toggle="collapse" href="#resposta1" role="button">
    O que é o Bootstrap?
  </a>
</p>
<div class="collapse" id="resposta1">
  <div class="card card-body">
    Bootstrap é um framework front-end que facilita o desenvolvimento de sites responsivos.
  </div>
</div>
```

### 🧠 Com vários botões:

```html
<button class="btn btn-outline-primary" type="button" data-bs-toggle="collapse" data-bs-target="#faq2">
  Como funciona o Grid System?
</button>
<div class="collapse mt-2" id="faq2">
  <div class="card card-body">
    O sistema de grid divide o layout em 12 colunas flexíveis e responsivas.
  </div>
</div>
```

---

## 💬 7. Collapse em FAQ (Multi-itens com Accordions)

```html
<div class="accordion" id="faqAccordion">
  <div class="accordion-item">
    <h2 class="accordion-header" id="pergunta1">
      <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#resposta1">
        Como me inscrevo no curso?
      </button>
    </h2>
    <div id="resposta1" class="accordion-collapse collapse show" data-bs-parent="#faqAccordion">
      <div class="accordion-body">
        Você pode se inscrever clicando em “Participar” no menu principal.
      </div>
    </div>
  </div>
  <!-- Repetir para mais perguntas -->
</div>
```

> 🔁 Somente um item permanece aberto de cada vez com `data-bs-parent`.

---

## 🧪 8. Desafio da Aula

1. Crie um botão `Abrir Modal` que mostre um **formulário de feedback**.
2. Crie um componente **accordion de FAQ** com pelo menos 3 perguntas e respostas.
3. Inclua um botão `Ajuda` que revela uma `div` com `collapse` e conteúdo explicativo.

---

## 🎓 9. Reflexões Técnicas

- Quando usar Modal ao invés de redirecionamento para uma nova página?
- O Collapse afeta a acessibilidade de leitores de tela? Como melhorar isso?
- Como criar Modais dinâmicos que se ajustem ao conteúdo carregado?

---

## 📚 10. Referências Oficiais

- [Bootstrap Modal – Documentação](https://getbootstrap.com/docs/5.3/components/modal/)
- [Bootstrap Collapse – Documentação](https://getbootstrap.com/docs/5.3/components/collapse/)
- [Bootstrap Accordion](https://getbootstrap.com/docs/5.3/components/accordion/)
- [Boas práticas de Acessibilidade – WAI](https://www.w3.org/WAI/tutorials/)

---

## ✅ Conclusão

**Modais e Collapse** são essenciais para criar **experiências ricas e interativas** sem recarregar páginas ou interromper o fluxo do usuário.  
Com eles, é possível implementar FAQs, formulários pop-up, notificações e conteúdos ocultos com **acessibilidade, leveza e elegância**.

> Com esta aula encerramos o **Módulo 3 – Componentes Essenciais**.

---
