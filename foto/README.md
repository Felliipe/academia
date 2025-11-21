# 📸 Imagens do Hero - Desktop e Mobile

## 📁 Estrutura de Arquivos

Para que o sistema de imagens responsivas funcione corretamente, organize suas imagens da seguinte forma:

### 🖥️ Imagens para Desktop
Coloque as imagens para telas grandes (desktop/tablet) com os seguintes nomes:
- `hero-1-desktop.png` (ou `.jpg`, `.webp`)
- `hero-2-desktop.png`
- `hero-3-desktop.png`

**Recomendações:**
- Resolução: 1920x1080px ou maior
- Formato: PNG, JPG ou WebP
- Peso: Otimize para web (máx. 500KB por imagem)

### 📱 Imagens para Mobile
Coloque as imagens para telas pequenas (mobile) com os seguintes nomes:
- `hero-1-mobile.png` (ou `.jpg`, `.webp`)
- `hero-2-mobile.png`
- `hero-3-mobile.png`

**Recomendações:**
- Resolução: 800x1200px ou similar (formato vertical funciona melhor)
- Formato: PNG, JPG ou WebP
- Peso: Otimize para web (máx. 300KB por imagem)
- Formato vertical é recomendado para melhor visualização em mobile

## 🔄 Como Funciona

O sistema detecta automaticamente o tamanho da tela:
- **Desktop/Tablet** (≥768px): Usa as imagens `-desktop`
- **Mobile** (<768px): Usa as imagens `-mobile`

As imagens alternam automaticamente a cada 5 segundos em um slideshow.

## ⚠️ Fallback

Se as imagens específicas (`-desktop` ou `-mobile`) não forem encontradas:
1. O sistema tenta usar imagens genéricas (`hero-1.png`, `hero-2.png`, `hero-3.png`) se existirem
2. Se ainda assim não encontrar, usa imagens de fallback do Unsplash automaticamente

## 🔧 Migração de Imagens Existentes

Se você já tem imagens como `hero-1.png`, você pode:
- **Opção 1:** Renomeá-las para `hero-1-desktop.png` e criar versões mobile
- **Opção 2:** Manter como estão - o sistema tentará usá-las como fallback

## 📝 Exemplo de Estrutura

```
public/
  foto/
    hero-1-desktop.png
    hero-2-desktop.png
    hero-3-desktop.png
    hero-1-mobile.png
    hero-2-mobile.png
    hero-3-mobile.png
```

