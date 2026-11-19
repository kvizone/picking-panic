<p align="center">
  <img src="assets/logo-800.png" alt="Picking Panic" width="600">
</p>

# Picking Panic 📦⏱️

Jogo 2D de vista aérea, no estilo do GTA 1, ambientado num galpão de logística.
Você é um operador correndo contra o relógio para separar, embalar e expedir um pedido antes do caminhão sair.

## Como jogar

Abra o `index.html` no navegador ou jogue pelo GitHub Pages.

| Tecla | Ação |
|---|---|
| WASD / Setas | Andar |
| Shift | Correr (não funciona carregando volume) |
| E | Interagir / segurar para coletar |
| Q | Ver a etiqueta do pedido |
| Esc | Pausar |

## Missão 1: Pedido #1042

1. Imprimir a etiqueta no terminal WMS
2. Separar 4 volumes em 3 endereços diferentes (R01-P04, R03-P07 e R04-P13), na ordem que quiser
3. Levar tudo até uma bancada de embalagem
4. Embalar (minigame de teclas)
5. Colocar a caixa lacrada no pallet da DOCA 2
6. Ver o caminhão sair

Quanto mais rápido, mais estrelas: 3 estrelas até 40s e 2 até 55s. Três empilhadeiras circulam pelo galpão (corredor principal, corredor do fundo e faixa da expedição), e encostar em qualquer uma custa +5s.
Durante o turno, o rádio do galpão comenta o que acontece. Todas as falas ficam no objeto `TEXTOS`, no topo do script.

## Tecnologia

HTML, Canvas 2D e JavaScript puro, num único arquivo e sem dependências.
A missão e o mapa ficam como dados no topo do script, para facilitar a criação de novas fases.

## Status

🚧 Protótipo em desenvolvimento: versão 0.2 com uma missão. Próximas fases no [ROADMAP](ROADMAP.md).
