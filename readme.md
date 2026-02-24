# Otimizacao de Performance - Agencia Criativa Web

## Projeto
Site estatico (HTML + CSS) com comparacao de performance via Lighthouse.

Este repo possui 2 entradas:
- index.dev.html (before): versao legivel, sem minificacao
- index.html (after): versao otimizada, com HTML minificado e CSS minificado

Obs: este projeto nao possui imagens, entao nao se aplica WebP ou lazy loading de imagens.

## Melhorias aplicadas
- Minificacao do HTML no index.html
- Minificacao do CSS gerando css/estilos.min.css (usado no index.html)
- Mantida a versao original css/estilos.css para comparacao no index.dev.html

## Relatorios Lighthouse (Chrome DevTools)

Antes (index.dev.html):
- reports/before/desktop.html
- reports/before/mobile.html
- reports/before/desktop.png
- reports/before/mobile.png

Depois (index.html):
- reports/after/desktop.html
- reports/after/mobile.html
- reports/after/desktop.png
- reports/after/mobile.png

## Como gerar os relatorios (padrao unico)
1. Rode um servidor local na raiz do projeto (exemplo):
   - python -m http.server 5500

2. Abra no Chrome:
   - http://localhost:5500/index.dev.html
   - DevTools > Lighthouse > Desktop > Analyze page
   - Exporte o report em HTML (Save as HTML) e salve em: reports/before/desktop.html
   - Tire um print do resumo e salve em: reports/before/desktop.png
   - Repita em Mobile e salve em: reports/before/mobile.html e reports/before/mobile.png

3. Repita o mesmo processo para:
   - http://localhost:5500/index.html
   Salvando em:
   - reports/after/desktop.html, reports/after/desktop.png
   - reports/after/mobile.html, reports/after/mobile.png