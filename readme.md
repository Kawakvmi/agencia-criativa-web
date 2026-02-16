# Otimizacao de Performance - Agencia Criativa Web

## Projeto
Site estatico (HTML + CSS) otimizado com base em metricas do Lighthouse no Chrome DevTools.

## Relatorios
Antes:
- reports/before/desktop.html
- reports/before/mobile.html
- reports/before/desktop.png
- reports/before/mobile.png

Depois:
- reports/after/desktop.html
- reports/after/mobile.html
- reports/after/desktop.png
- reports/after/mobile.png

## Gargalos encontrados (antes)
- Imagens pesadas em PNG/JPG
- Imagens fora da dobra sem lazy loading
- CSS com trechos nao utilizados
- HTML e CSS sem minificacao

## Melhorias aplicadas
- Conversao de imagens para WebP e uso das versoes otimizadas
- loading="lazy" e decoding="async" em imagens fora da dobra
- Remocao de CSS nao utilizado (DevTools Coverage)
- Minificacao do HTML e do CSS
