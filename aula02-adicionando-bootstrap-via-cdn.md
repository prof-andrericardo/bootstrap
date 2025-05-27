# 📘 **Aula 02 – Adicionando o Bootstrap via CDN**  

## 🎯 **Objetivos da Aula**  

1. Entender o que é um **CDN** e como ele acelera seu projeto.  
2. Configurar o Bootstrap **sem instalar nada** no computador.  
3. Criar um **mini-site** com container, botões e cores.  

---

## 🌐 **1. CDN: A "Nuvem Mágica" do Bootstrap**  

### O que é?  

Um **CDN (Content Delivery Network)** é uma rede de servidores que armazena arquivos como o Bootstrap em locais estratégicos para **carregamento ultrarrápido**.  

### ⚡ **Vantagens**  

- 🚀 **Rápido**: Arquivos servidos pelo servidor mais próximo de você.  
- 💾 **Sem download**: Basta um link no HTML.  
- 🔄 **Sempre atualizado**: Versão mais recente automaticamente.  

---

## 🧩 **2. Estrutura Básica com CDN**  

### 🔗 **Ordem Importante!**  

1. **CSS no `<head>`**: Para estilizar a página antes de carregar o conteúdo.  
2. **JS no final do `<body>`**: Para não travar a renderização da página.  

```html  
<!DOCTYPE html>  
<html>  
<head>  
  <!-- Meta tags -->  
  <meta charset="UTF-8">  
  <meta name="viewport" content="width=device-width, initial-scale=1">  

  <!-- Bootstrap CSS -->  
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">  

  <title>Meu Site com Bootstrap</title>  
</head>  
<body>  

  <!-- Conteúdo -->  
  <div class="container">  
    <h1 class="text-center">Olá, Mundo!</h1>  
  </div>  

  <!-- Bootstrap JS + Popper -->  
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>  
</body>  
</html>  
```

---

## 🎨 **3. Prática: Criando um Mini-Site**  

### 🛠 **Componentes Usados**  

- **Container**: Limita o conteúdo e centraliza (`class="container"`).  
- **Botões**: Cores e tamanhos (`btn-primary`, `btn-lg`).  
- **Cores de Fundo**: `bg-light`, `bg-dark`, etc.  

```html  
<div class="container bg-light p-5 text-center">  
  <h1 class="text-primary">Bem-vindo ao Curso!</h1>  
  <p class="fs-5">Aprenda Bootstrap de forma simples.</p>  
  <button class="btn btn-success btn-lg">Começar</button>  
  <button class="btn btn-outline-danger">Cancelar</button>  
</div>  
```

### 🔍 **Experimente!**  

Substitua as classes e veja o resultado:  

- `btn-success` → `btn-warning`  
- `bg-light` → `bg-dark text-white`  

---

## 🏆 **Desafio da Aula**  

Crie uma página com:  

1. Um **container** com fundo claro (`bg-light`).  
2. Um **título centralizado** em vermelho (`text-danger`).  
3. Dois **botões lado a lado**:  
   - Um grande e azul (`btn-primary btn-lg`).  
   - Um pequeno e com borda (`btn-outline-secondary btn-sm`).  

---

## ❓ **Perguntas para Testar**  

1. O que acontece se você esquecer o **JS do Bootstrap**? *(Dica: modais e dropdowns não funcionam!)*  
2. Por que o CSS deve ficar no `<head>`?  

---

## 📚 **Recursos**  

- [JSDelivr (CDN Oficial)](https://www.jsdelivr.com/package/npm/bootstrap)  
- [Playground Bootstrap](https://playcode.io/bootstrap)  

