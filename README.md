# 🎭 April Fools Prank Website

Este projeto é uma página web criada com o objetivo de realizar uma **pegadinha de Primeiro de Abril**, simulando a aparência de uma matéria de portal de notícias.

O foco do projeto foi combinar:
- Engenharia de front-end
- Comportamento de redes sociais (Open Graph)
- UX voltada para engajamento

---

## 🚀 Objetivo

Criar um link compartilhável (WhatsApp, Facebook, etc.) que:

1. Exiba um **preview convincente** (thumbnail + título + descrição)
2. Simule uma **página de notícia real**
3. Revele a pegadinha apenas após interação do usuário

---

## 🧠 Conceitos aplicados

### 1. Open Graph (OG Tags)

As meta tags Open Graph foram configuradas para controlar como o link aparece nas redes sociais:

```html
<meta property="og:title" content="..." />
<meta property="og:description" content="..." />
<meta property="og:image" content="https://.../og-image.jpg" />
```

🔑 Pontos importantes:
- A URL da imagem deve ser **absoluta** (https)
- Formato recomendado: **JPG ou PNG (não WEBP)**
- Tamanho ideal: **1200x630**

---

### 2. Compatibilidade com WhatsApp

O WhatsApp é mais restritivo que outros parsers.

Para garantir que a thumbnail apareça:

- `og:image` deve estar acessível publicamente
- Adicionados:
  - `og:image:width`
  - `og:image:height`
  - `og:image:type`
- Uso de `og:image:secure_url`

---

### 3. Estrutura de página estilo notícia

A página foi estruturada para parecer um portal real:

- Header com branding
- Breadcrumb (ex: / Dinheiro / Outro)
- Título + subtítulo
- Metadados (tempo, fonte)
- Imagem com legenda
- Texto em parágrafos

---

### 4. UX da pegadinha

A pegadinha NÃO acontece imediatamente.

Fluxo:

1. Usuário acessa a página
2. Vê conteúdo aparentemente legítimo
3. Interage com:
   - link "continuar lendo"
   - botão
4. Overlay aparece com:
   - GIF
   - mensagem "Primeiro de Abril"
   - áudio em loop

---

### 5. Autoplay de áudio (bypass)

Browsers modernos bloqueiam autoplay com som.

Solução implementada:

```javascript
// só toca após interação do usuário
button.addEventListener("click", () => {
  audio.play();
});
```

---

### 6. Overlay (efeito surpresa)

A pegadinha é exibida via overlay:

- `position: fixed`
- bloqueia scroll
- animação de entrada

Isso mantém o conteúdo inicial intacto e aumenta o impacto.

---

### 7. Thumbnail otimizado

A imagem de preview foi tratada para:

- proporção correta (1200x630)
- melhor legibilidade
- compatibilidade com redes sociais

---

## 📁 Estrutura do projeto

```
index.html
og-image.jpg
laughing-cat.gif
cat-laugh-meme-1.mp3
README.md
```

---

## 🌐 Deploy (GitHub Pages)

1. Criar repositório:
```
lucasbc92.github.io
```

2. Subir arquivos na raiz

3. Acessar:
```
https://lucasbc92.github.io/
```

---

## ⚠️ Cache de redes sociais

Plataformas como WhatsApp e Facebook fazem cache agressivo.

Para forçar atualização:

```
https://lucasbc92.github.io/?v=2
```

---

## 🛠️ Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript (vanilla)
- Open Graph Protocol

---

## 💡 Possíveis melhorias

- adicionar tracking de cliques
- múltiplas variações de pegadinha
- randomização de conteúdo
- suporte a múltiplos idiomas

---

## 🎯 Conclusão

Este projeto demonstra:

- domínio de comportamento de preview em redes sociais
- manipulação de UX para engajamento
- controle de mídia e interação no navegador

Além disso, é um exemplo prático de como detalhes técnicos (como Open Graph) impactam diretamente a percepção do usuário.

---

## 😈 Disclaimer

Use com responsabil