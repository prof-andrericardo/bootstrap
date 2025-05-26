# 📘 Aula 02 – Adicionando o Bootstrap via CDN

## 🎯 Objetivos da Aula
- Aprender como adicionar o Bootstrap em um projeto utilizando **CDN (Content Delivery Network)**.
- Compreender o papel de cada arquivo (CSS e JS) e sua ordem de inserção.
- Criar o primeiro layout funcional com Bootstrap sem instalar nada localmente.
- Garantir um ambiente preparado para as próximas aulas.

---

## 📖 1. O que é CDN?

Uma **CDN (Content Delivery Network)** é uma rede de servidores distribuídos globalmente que entrega conteúdo (como arquivos CSS, JS ou imagens) de forma mais rápida e segura.

### 🚀 Vantagens de usar CDN no Bootstrap:
- 💡 **Sem instalação local** – basta copiar o link.
- ⚡ **Desempenho** – arquivos hospedados em servidores otimizados.
- 🆓 **Gratuito e aberto** – não é necessário criar conta.
- 🔄 **Atualização automática** – sempre a última versão.

---

## 🧰 2. Estrutura mínima com Bootstrap via CDN

Aqui está o exemplo de um projeto mínimo utilizando Bootstrap 5 via CDN:

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Bootstrap via CDN</title>

  <!-- 🔗 CSS do Bootstrap -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">

</head>
<body>

  <div class="container text-center py-5">
    <h1 class="mb-4">Olá, Bootstrap!</h1>
    <button class="btn btn-primary btn-lg">Clique aqui</button>
  </div>

  <!-- 🔽 Script JS do Bootstrap -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

> 💬 A **ordem dos arquivos importa!**  
> O CSS vai dentro da `<head>`, e o JS (bundle) vai **no final do body** para evitar lentidão no carregamento da página.

---

## 🧠 3. Como funciona o Bundle JS?

O arquivo JS `bootstrap.bundle.min.js` contém dois elementos:
- O **JavaScript do Bootstrap** (para funcionalidades como modais, collapse, tooltips).
- O **Popper.js**, necessário para posicionamento de tooltips e dropdowns.

Assim, você não precisa importar dois arquivos separados.

---

## ⚙️ 4. Criando um Projeto Real com CDN

### Etapas:

1. Crie uma nova pasta chamada `aula02-bootstrap-cdn`.
2. Dentro dela, crie o arquivo `index.html`.
3. Copie o código acima para este arquivo.
4. Adicione uma imagem, um parágrafo e experimente mudar as cores dos botões usando classes como `btn-success`, `btn-danger`, `btn-warning`.

---

## 💻 5. Prática Guiada – Criando um mini site

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Mini site com Bootstrap</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-light">

  <div class="container py-5">
    <h1 class="text-center mb-4">Bem-vindo ao Curso de Bootstrap</h1>
    <p class="lead text-center">Estamos criando páginas modernas com agilidade e responsividade!</p>

    <div class="text-center">
      <button class="btn btn-outline-primary">Aprender Bootstrap</button>
    </div>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

> 💡 Experimente trocar `btn-outline-primary` por `btn-success`, `btn-dark`, `btn-warning` etc.

---

## 🧪 6. Desafio da Aula

Crie uma página simples com:
- Um título centralizado usando `text-center`
- Um botão de cada tipo: `btn-primary`, `btn-danger`, `btn-warning`, `btn-success`
- Um container com `bg-light` e `py-5`

Adicione também um segundo botão com a classe `btn-lg` e outro com `btn-sm`.

---

## 🧠 7. Perguntas para Reflexão

- Qual a vantagem de usar o Bootstrap por CDN em comparação com um download local?
- O que acontece se você esquecer de adicionar o script JS no final da página?
- Quais são as desvantagens do uso de CDN em ambientes sem internet?

---

## 📚 8. Referências e Leituras Complementares

- [Documentação Bootstrap – Getting Started](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- [JSDelivr – CDN oficial do Bootstrap](https://www.jsdelivr.com/package/npm/bootstrap)
- [MDN – Como funciona o carregamento de scripts JS](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/script)

---

## ✅ Conclusão

Agora você já consegue **usar Bootstrap em qualquer página web com apenas duas linhas de código**. A partir da próxima aula, exploraremos os **componentes estruturais do Bootstrap** e entenderemos a **anatomia das suas classes utilitárias**.

---
