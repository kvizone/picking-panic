<p align="center">
  <img src="assets/logo-800.png" alt="Picking Panic" width="600">
</p>

# Picking Panic 📦⏱️

Jogo 2D de vista aérea, no estilo do GTA 1, ambientado num galpão de logística.
Você é um operador correndo contra o relógio para separar, embalar e expedir um pedido antes do caminhão sair.

## Como jogar

Abra o `index.html` no navegador ou jogue pelo GitHub Pages. As 3 fases são jogadas em sequência: terminou uma, vai para a próxima, até zerar o jogo. No final aparece o tempo total da campanha.

| Tecla | Ação |
|---|---|
| WASD / Setas | Andar (ou dirigir, na fase 2) |
| Shift | Correr (não funciona carregando volume) |
| E | Interagir / segurar para coletar ou erguer o garfo |
| Q | Ver a etiqueta (fase 2: ordem de serviço) |
| H | Buzina (dirigindo) |
| R | Liga/desliga a rádio caipira |
| M | Som |
| Esc | Pausar |

### No celular

Funciona em pé ou deitado: o mapa se ajusta ao formato da tela. Não tem joystick fixo:

- **Deslize o dedo** em qualquer lugar da tela: o operador anda na direção do deslize. Deslizando mais longe, ele corre. Um círculo mostra onde o dedo encostou.
- **Botão amarelo:** aparece só quando tem algo para fazer ali. Segure para coletar.
- **Empilhadeira:** deslize para onde ela deve ir. Deslizando para trás dela, ela dá ré. O botão azul é a buzina.
- **Toque no tempo** para pausar e **no objetivo** para ver a etiqueta.
- **Embalagem:** deslize o dedo na direção de cada seta e toque para o E, ou use os botões.
- **Garfo:** segure em qualquer lugar da tela (ou no botão) e solte na faixa verde.
- **Tempo:** no celular, as estrelas e a bateria do coletor têm 35% a mais de tempo, e o recorde fica separado do recorde do computador.

## Fase 1: Pedido #1042

Imprima a etiqueta no terminal, separe 4 volumes em 3 endereços (R01-P04, R03-P07 e R04-P13) na ordem que quiser, embale na bancada e coloque a caixa lacrada no pallet da DOCA 2. Três empilhadeiras circulam pelo galpão, e encostar em qualquer uma custa +5s.

## Fase 2: Pallet no Alto

Suba na Empilhadeira 04, dirija até o pulmão PUL-02, alinhe os garfos de frente para o rack e erga até o nível 3. Depois leve o pallet até a área demarcada da DOCA 1. A direção é no estilo GTA 1, com inércia. Bater no rack custa +3s, passar rápido na faixa de pedestre dá multa de +2s e encostar em pedestre custa +5s.

## Fase 3: Cadê o Coletor?

O coletor sumiu, e sem ele não tem seta nem minimapa. Siga o bip, que fica mais alto e mais de um lado conforme você chega perto, ou acompanhe a barra de SINAL no HUD. Os colegas dão pistas com E, mas um deles mente. Se a bateria acabar, a fase recomeça. Achou o coletor? O WMS religa, a etiqueta imprime e ainda tem um pedido de 2 itens para fechar.

## Rádio

- **Rádio do galpão:** comenta o que acontece durante o turno. As falas ficam no objeto `TEXTOS`, no topo do script.
- **Rádio caipira:** música ao vivo de uma web rádio, com filtro de rádio AM. Se a emissora não liberar o efeito, ela toca sem filtro.

## Tecnologia

HTML, Canvas 2D e JavaScript puro, num único arquivo e sem dependências.
A missão e o mapa ficam como dados no topo do script, para facilitar a criação de novas fases.

## Status

🚧 Protótipo em desenvolvimento: versão 0.3 com 3 fases em sequência. Próximas fases no [ROADMAP](ROADMAP.md).
