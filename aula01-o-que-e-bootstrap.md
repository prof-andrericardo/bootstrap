# 📘 **Aula 01 – O que é o Bootstrap?**  
## 🎯 **Objetivos da Aula**  
1. Entender o que é um **framework front-end** e como o Bootstrap acelera o desenvolvimento.  
2. Identificar **3 problemas comuns** que o Bootstrap resolve.  
3. Criar o **primeiro "Hello World"** com Bootstrap, comparando com CSS puro.  

---

## 🌍 **1. Introdução: Por que Bootstrap?**  
Imagine construir uma casa: você **poderia serrar madeira, fazer tijolos e misturar cimento manualmente**, ou **usar materiais prontos** para focar no design e funcionalidade. O Bootstrap é como um "kit de construção" para sites!  

### 📌 **Origem do Bootstrap**  
Criado em **2011** por desenvolvedores do Twitter, hoje é o **framework front-end mais popular do mundo**, usado por sites como Spotify, Netflix e Airbnb.  

### 🆚 **Bootstrap vs. CSS Puro**  
| Situação              | CSS Puro (Tradicional)  | Com Bootstrap                    |
| --------------------- | ----------------------- | -------------------------------- |
| Criar um botão azul   | 10+ linhas de código    | Apenas `class="btn btn-primary"` |
| Tornar um site mobile | Media queries complexas | Classes prontas como `col-md-6`  |
| Alinhar um texto      | `text-align: center;`   | `class="text-center"`            |

---

## 🧩 **2. Peças do Bootstrap: O que vem na caixa?**  
O Bootstrap é dividido em **3 partes principais**:  

1. **📦 Sistema de Grid (12 colunas)**  
   - Cria layouts responsivos automaticamente.  
   - Exemplo:  
     ```html  
     <div class="row">  
       <div class="col-md-6">Esquerda</div>  
       <div class="col-md-6">Direita</div>  
     </div>  
     ```

2. **🎨 Componentes Prontos**  
   - Botões, cards, navbars e mais – como peças de Lego.  
   ```html  
   <button class="btn btn-success">Salvar</button>  
   ```

3. **🔧 Utilitários CSS**  
   - Classes para margens, cores, flexbox e outros ajustes rápidos.  
   ```html  
   <p class="text-danger bg-light p-3">Alerta!</p>  
   ```

---

## 🛠 **3. Mão na Massa: Primeiro Código**  
### 🔄 **Comparação Prática**  
**Sem Bootstrap:**  
```html  
<button style="  
  padding: 10px 20px;  
  background-color: #0d6efd;  
  color: white;  
  border: none;  
  border-radius: 5px;  
">Clique aqui</button>  
```

**Com Bootstrap:**  
```html  
<button class="btn btn-primary">Clique aqui</button>  
```

### ✨ **Desafio Inicial**  
1. Abra o [CodePen](https://codepen.io/pen/) ou um arquivo `index.html`.  
2. Adicione o Bootstrap via CDN (código abaixo).  
3. Crie:  
   - Um título com classe `display-4`.  
   - Um botão verde (`btn-success`).  
   - Um parágrafo com fundo amarelo (`bg-warning`).  

```html  
<!DOCTYPE html>  
<html>  
<head>  
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">  
</head>  
<body>  
  <!-- Seu código aqui -->  
</body>  
</html>  
```

---

## 🤔 **4. Perguntas para Reflexão**  
1. Qual problema você acha que o Bootstrap resolve **mais rápido** no dia a dia?  
2. Por que classes como `btn-primary` são melhores que CSS inline?  

---

## 📚 **Recursos Extras**  
- [Documentação Oficial](https://getbootstrap.com/docs/5.3/getting-started/introduction/)  
- [Bootstrap Icons](https://icons.getbootstrap.com/)  

