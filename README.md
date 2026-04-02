# 🎭 April Fools Prank Website

![EN](https://img.shields.io/badge/lang-EN-blue) ![PT-BR](https://img.shields.io/badge/lang-PT--BR-green)

[EN](#en) | [PT-BR](#pt-br)

---

## 🇺🇸 English Version {#en}

This project is a web page designed to create an **April Fools prank**, simulating a real news article layout.

The goal was to combine:

* Front-end engineering
* Social media preview behavior (Open Graph)
* Engagement-focused UX

---

## 🚀 Goal

Create a shareable link (WhatsApp, Facebook, etc.) that:

1. Displays a **convincing preview** (thumbnail + title + description)
2. Mimics a **real news article**
3. Reveals the prank only after user interaction

---

## 🧠 Key Concepts

### 1. Open Graph (OG Tags)

```html
<meta property="og:title" content="..." />
<meta property="og:description" content="..." />
<meta property="og:image" content="https://.../og-image.jpg" />
```

Key points:

* Image must be **absolute URL (https)**
* Recommended format: **JPG or PNG (not WEBP)**
* Ideal size: **1200x630**

---

### 2. WhatsApp Compatibility

* Public `og:image`
* Include width/height/type
* Use secure_url

---

### 3. News-like Layout

* Header + branding
* Breadcrumb
* Title + subtitle
* Metadata
* Image + caption
* Article paragraphs

---

### 4. Prank UX Flow

1. User opens page
2. Sees legitimate content
3. Interacts
4. Overlay reveals prank

---

### 5. Audio Autoplay Strategy

Audio only starts after user interaction.

---

### 6. Overlay Effect

* Fixed positioning
* Scroll blocking
* Entrance animation

---

### 7. Optimized Thumbnail

* 1200x630 ratio
* Social media friendly

---

## 📁 Structure

```
index.html
og-image.jpg
laughing-cat.gif
cat-laugh-meme-1.mp3
README.md
```

---

## 🌐 Deployment

```
https://lucasbc92.github.io/
```

---

## ⚠️ Cache Busting

```
?v=2
```

---

## 🛠️ Tech Stack

* HTML5
* CSS3
* JavaScript
* Open Graph Protocol

---

## 🎯 Conclusion

This project demonstrates:

* Social preview control
* UX manipulation for engagement
* Browser media interaction handling

---

## 🇧🇷 Versão em Português {#pt-br}

Este projeto é uma página web criada com o objetivo de realizar uma **pegadinha de Primeiro de Abril**, simulando a aparência de uma matéria de portal de notícias.

O foco do projeto foi combinar:

* Engenharia de front-end
* Comportamento de redes sociais (Open Graph)
* UX voltada para engajamento

---

## 🚀 Objetivo

Criar um link compartilhável (WhatsApp, Facebook, etc.) que:

1. Exiba um **preview convincente** (thumbnail + título + descrição)
2. Simule uma **página de notícia real**
3. Revele a pegadinha apenas após interação do usuário

---

## 🧠 Conceitos aplicados

### 1. Open Graph (OG Tags)

```html
<meta property="og:title" content="..." />
<meta property="og:description" content="..." />
<meta property="og:image" content="https://.../og-image.jpg" />
```

Pontos importantes:

* URL da imagem deve ser **absoluta (https)**
* Formato recomendado: **JPG ou PNG (não WEBP)**
* Tamanho ideal: **1200x630**

---

### 2. Compatibilidade com WhatsApp

* `og:image` público
* `og:image:width`, `og:image:height`
* `og:image:type`
* `og:image:secure_url`

---

### 3. Estrutura estilo notícia

* Header + branding
* Breadcrumb
* Título + subtítulo
* Metadados
* Imagem + legenda
* Conteúdo em parágrafos

---

### 4. UX da pegadinha

Fluxo:

1. Usuário acessa
2. Vê conteúdo legítimo
3. Interage
4. Overlay revela a pegadinha

---

### 5. Autoplay de áudio

Som só inicia após interação do usuário.

---

### 6. Overlay

* `position: fixed`
* bloqueia scroll
* animação

---

### 7. Thumbnail otimizado

* proporção 1200x630
* compatível com redes sociais

---

## 📁 Estrutura

```
index.html
og-image.jpg
laughing-cat.gif
cat-laugh-meme-1.mp3
README.md
```

---

## 🌐 Deploy

```
lucasbc92.github.io
```

---

## ⚠️ Cache

```
?v=2
```

---

## 🛠️ Tecnologias

* HTML5
* CSS3
* JavaScript
* Open Graph

---

## 🎯 Conclusão

Projeto demonstra domínio de:

* preview social
* UX
* comportamento de browser

---

## 😈 Disclaimer

Use com responsabilidade 😄
