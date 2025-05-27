
# 🚀 **Chirpy Starter + Obsidian Workflow**

[![GitHub license](https://img.shields.io/github/license/cotes2020/chirpy-starter.svg?color=blue)](LICENSE)

Template pronto para transformar suas anotações do **Obsidian** em um blog pessoal usando **GitHub Pages**, com o tema [Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy).

Uma solução elegante, leve e automatizada para quem deseja publicar notas, reflexões, estudos ou projetos diretamente do Obsidian para a web — sem complicações.

---

## 🎯 **Por que usar este template?**

Este repositório é baseado no [Chirpy Starter](https://github.com/cotes2020/chirpy-starter), adaptado para quem utiliza o **Obsidian como sistema de conhecimento pessoal (PKM)**. O objetivo é transformar seu repositório de notas em um blog profissional, com deploy automático e zero fricção.

### ✅ **Diferenciais do template:**

* 🔥 Deploy automático via **GitHub Actions**.
* 🔗 Organização de conteúdos seguindo a estrutura do **Obsidian**.
* ✍️ Templates flexíveis para **artigos longos, notas rápidas ou tutoriais**.
* 📄 Publicação de arquivos **Markdown → Blog**, sem processos manuais.
* 🎨 Design responsivo, limpo e focado na leitura.

---

## 🚀 **Começando em minutos**

### 1️⃣ **Crie seu repositório a partir do template**

1. Clique em **"Use this template"** no topo deste repositório.
2. Nomeie seu repositório no formato:

```
{seu-usuario}.github.io
```

Exemplo:

```
val.github.io
```

---

### 2️⃣ **Ative o GitHub Pages**

1. Acesse **Settings → Pages** no seu repositório.
2. Em **Build and deployment**, escolha:

```
Source: GitHub Actions
```

✅ Isso ativa a publicação automática sempre que você fizer push.

---

### 3️⃣ **Configure seu blog**

Edite o arquivo `_config.yml` com seus dados:

```yaml
title: Meu Blog de Notas
tagline: Reflexões, Estudos e Aprendizados
url: "https://{seu-usuario}.github.io"
author:
  name: Seu Nome
  bio: Explorador de ideias, aprendizados e soluções digitais
  email: seu@email.com
lang: pt-BR
```

Personalize também temas, cores, menus e outras opções se desejar.

---

### 4️⃣ **Clone o repositório localmente**

```bash
git clone https://github.com/{seu-usuario}/{seu-usuario}.github.io.git
```

---

### 5️⃣ **Conecte o Obsidian**

1. Abra o **Obsidian**.
2. Vá em **"Abrir Pasta como Vault"**.
3. Selecione a pasta `_posts` do seu repositório clonado.

A partir daqui, qualquer nota criada no Obsidian dentro da pasta `_posts` pode ser publicada no blog.

---

### 6️⃣ **Publique sua primeira nota**

1. Crie um arquivo seguindo o padrão:

```
YYYY-MM-DD-nome-da-nota.md
```

Exemplo:

```
2025-05-27-primeira-nota.md
```

2. Adicione este frontmatter no início da nota:

```yaml
---
title: "Título da Nota"
date: 2025-05-27 12:00:00 +0000
categories: [Notas]
tags: [obsidian, markdown, blog]
---
```

3. Após salvar, execute:

```bash
git add .
git commit -m "Publicando primeira nota"
git push
```

✨ Pronto! Sua nota será publicada automaticamente no blog.

---

## 🗂️ **Estrutura recomendada**

| Pasta      | Descrição                                      |
| ---------- | ---------------------------------------------- |
| `_posts`   | Suas notas públicas (markdown com frontmatter) |
| `_tabs`    | Páginas fixas (Sobre, Contato, Arquivo, etc.)  |
| `assets`   | Imagens, arquivos e mídias                     |
| `_plugins` | Funcionalidades adicionais                     |

---

## 📚 **Recursos e Documentação**

* 🐦 [Guia oficial do tema Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy/wiki)
* 🔧 [Documentação do Jekyll](https://jekyllrb.com/docs/)
* ✍️ [Guia Markdown no Obsidian](https://help.obsidian.md/)

---

## 🤝 **Contribuindo**

Este template é uma adaptação pensada para integrar o fluxo de trabalho do Obsidian com publicação web. Sugestões de melhorias, novas features e correções são sempre bem-vindas! Abra uma issue ou envie um pull request.

---

## 📜 **Licença**

Distribuído sob a licença [MIT](LICENSE).

