# 📊 Dashboard de Relatórios Instagram

Dashboard centralizado para gerenciar relatórios de performance no Instagram para múltiplos clientes.

## 📁 Estrutura

```
github-pages-dashboard/
├── index.html                 # Dashboard principal (lista clientes)
├── sara-paiva/
│   ├── index.html             # Lista de relatórios da Sara
│   ├── julho-2026.html        # Relatório de julho
│   └── junho-2026.html        # Relatório de junho
├── outro-cliente/             # Para adicionar novos clientes
│   ├── index.html
│   └── julho-2026.html
└── terceiro-cliente/          # Para adicionar mais clientes
    └── index.html
```

## 🚀 Como subir para GitHub Pages

### 1️⃣ Crie uma conta no GitHub (se não tiver)
- Acesse: https://github.com/signup

### 2️⃣ Crie um novo repositório
- Nome: **seu-usuario.github.io** (substitua pelo seu usuário do GitHub)
- Deixe público
- Não inicialize com README

### 3️⃣ Coloque os arquivos no repositório
```bash
# Clone o repositório vazio
git clone https://github.com/seu-usuario/seu-usuario.github.io.git
cd seu-usuario.github.io

# Copie todos os arquivos da pasta github-pages-dashboard para aqui
# (Ou use: cp -r /tmp/github-pages-dashboard/* .)

# Adicione tudo ao Git
git add .

# Faça o primeiro commit
git commit -m "Add relatórios dashboard"

# Suba para o GitHub
git push -u origin main
```

### 4️⃣ Pronto! Acesse em:
**https://seu-usuario.github.io/**

---

## 📝 Como adicionar novos clientes

### 1. Crie uma pasta para o cliente:
```bash
mkdir seu-usuario.github.io/novo-cliente
```

### 2. Crie um `index.html` dentro da pasta:
```html
<!-- Copie o conteúdo de sara-paiva/index.html e adapte -->
```

### 3. Atualize o `index.html` principal:
Adicione o novo cliente no array `clients`:

```javascript
const clients = [
  {
    name: "Sara de Paiva",
    handle: "@saradpaiva",
    icon: "👩‍💼",
    folder: "sara-paiva",
    reports: [
      { month: "Julho", year: 2026, file: "julho-2026.html" }
    ]
  },
  {
    name: "Novo Cliente",
    handle: "@novo",
    icon: "📱",
    folder: "novo-cliente",
    reports: [
      { month: "Julho", year: 2026, file: "julho-2026.html" }
    ]
  }
];
```

### 4. Faça upload dos relatórios na pasta do cliente

### 5. Commit e push:
```bash
git add .
git commit -m "Add novo cliente"
git push
```

---

## 🎨 Personalizações

### Mudar cores do dashboard:
- Abra `index.html`
- Procure por `background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);`
- Mude os códigos de cor hexadecimais

### Adicionar mais relatórios por cliente:
- Coloque o HTML na pasta do cliente
- Adicione no array `reports` dentro de `sara-paiva/index.html`

---

## 🔗 URLs de exemplo

```
Dashboard principal:
https://seu-usuario.github.io/

Relatórios da Sara:
https://seu-usuario.github.io/sara-paiva/

Relatório de julho da Sara:
https://seu-usuario.github.io/sara-paiva/julho-2026.html

Novo cliente (quando adicionar):
https://seu-usuario.github.io/novo-cliente/
```

---

## ✨ Vantagens

✅ Totalmente gratuito  
✅ Sem limite de banda  
✅ URL customizável (seu nome)  
✅ Fácil de atualizar  
✅ Escalável para múltiplos clientes  
✅ Acesso público ou privado (conforme desejar)  

---

## 💡 Dica

Se quiser um domínio próprio (tipo `relatorios.com.br`), é bem fácil:
1. Compre um domínio (ex: Hostinger, GoDaddy - ~R$ 20/ano)
2. Configure o DNS para apontar pro GitHub Pages
3. Ativa HTTPS automático

Quer fazer isso depois, é simples!

