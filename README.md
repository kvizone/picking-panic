<p align="center">
  <img src="assets/logo-800.png" alt="Picking Panic" width="600">
</p>

# Picking Panic 📦⏱️

Jogo 2D de vista aérea, no estilo do GTA 1, ambientado num galpão de logística.
Você é um operador correndo contra o relógio: pedidos caem no balcão do WMS, você separa, embala e expede antes do caminhão sair. E ainda tem empilhadeira, coletor perdido e Black Friday.

## Como jogar

Abra o `index.html` no navegador ou jogue pelo GitHub Pages. As 6 fases são jogadas em sequência: terminou uma, vai para a próxima, até zerar o jogo. No final aparece o tempo total da campanha.

| Tecla | Ação |
|---|---|
| Setas | Andar (ou dirigir, nas fases de empilhadeira) |
| Shift | Correr |
| E | Interagir / abrir o balcão WMS / segurar para coletar ou erguer o garfo |
| C | Pegar ou soltar o carrinho de picking |
| Q | Ver a etiqueta (empilhadeira: ordem de serviço) |
| H | Buzina (dirigindo) |
| R / M | Liga/desliga a rádio 89 FM / som |
| Esc | Pausar |

Não precisa decorar: as dicas aparecem na hora certa, na primeira vez que cada coisa surge.

**Carrinho de picking:** fica perto do balcão nas fases a pé. Com ele você anda mais rápido e corre mesmo carregado, mas ele é mais largo e também leva batida de empilhadeira.

### No celular

Funciona em pé ou deitado: o mapa se ajusta ao formato da tela. Não tem joystick fixo:

- **Deslize o dedo** em qualquer lugar da tela: o operador anda na direção do deslize. Deslizando mais longe, ele corre. Um círculo mostra onde o dedo encostou.
- **Botão amarelo:** aparece só quando tem algo para fazer ali. Segure para coletar.
- **Empilhadeira:** deslize para onde ela deve ir. Deslizando para trás dela, ela dá ré. O botão azul é a buzina.
- **Toque no tempo** para pausar e **no objetivo** para ver a etiqueta.
- **Embalagem:** deslize o dedo na direção de cada seta e toque para o E, ou use os botões.
- **Garfo:** segure em qualquer lugar da tela (ou no botão) e solte na faixa verde.
- **Tempo:** no celular, as estrelas e a bateria do coletor têm 35% a mais de tempo, e o recorde fica separado do recorde do computador.

## Balcão WMS: como os pedidos chegam

Nas fases de picking, o turno começa com você colado no balcão do WMS. Os pedidos **caem no balcão** com um "plim", o contador 📥 no HUD e papéis empilhando no balcão. Quanto mais você demora, mais pedidos se acumulam, e cada um tem um prazo que conta desde que caiu.

1. Enquanto tiver pedido esperando, um marcador amarelo pulsa na frente do balcão e um aviso fixo diz o que fazer: chegar no balcão e apertar **E** (no celular, o botão **PEGAR PEDIDO**).
2. O cupom do pedido mais urgente sai impresso na hora, numa janela só. Com mais de um na fila, **◀ ▶** troca de pedido; **Esc** deixa para depois.
3. Separe, embale e deposite no pallet da doca do pedido.
4. O caminhão sai e abre a janela de **pedido concluído** (estrelas, tempo, prazo, penalidades). Depois, volta pro galpão.
5. Pedido entregue fora do prazo custa +5s. Quando o último pedido sai, aparece o relatório da fase.

As dicas de controle aparecem uma vez, como legenda curta no rodapé (no celular, logo abaixo do topo), sem cobrir o jogador.

## Fase 1: Pedido #1042

Pegue o pedido no balcão, separe 4 volumes em 3 endereços (R01-P04, R03-P07 e R04-P13) na ordem que quiser, embale na bancada e coloque a caixa lacrada no pallet da DOCA 2. Três empilhadeiras circulam pelo galpão, e encostar em qualquer uma custa +5s.

## Fase 2: Pallet no Alto

Suba na Empilhadeira 04, dirija até o pulmão PUL-02, alinhe os garfos de frente para o rack e erga até o nível 3. Depois leve o pallet até a área demarcada da DOCA 1. A direção é no estilo GTA 1, com inércia. Bater no rack custa +3s, passar rápido na faixa de pedestre dá multa de +2s e encostar em pedestre custa +5s.

## Fase 3: Cadê o Coletor?

O coletor sumiu, e sem ele não tem seta nem minimapa. Siga o bip, que fica mais alto e mais de um lado conforme você chega perto, ou acompanhe a barra de SINAL no HUD. Os colegas dão pistas com E, mas um deles mente. Se a bateria acabar, a fase recomeça. Achou o coletor? O WMS religa, a etiqueta imprime e ainda tem um pedido de 2 itens para fechar.

## Dois tipos de tarefa (fases 4 e 6)

**Pedidos** caem no balcão WMS a cada minuto: pega o cupom, separa, embala e expede. A fase fecha quando você entrega a meta.

**Urgências** estouram de tempos em tempos e param tudo, no estilo sabotagem do Among Us: alarme, borda vermelha e contagem regressiva. Se o tempo zerar, perde a fase.

| Urgência | O que fazer | Tempo (fase 4 / 6) |
|---|---|---|
| 🔥 Incêndio | Pegue o extintor no armário vermelho da parede e segure E perto do pallet até apagar | 30s / 26s |
| 📟 Coletor perdido | Sem coletor, sem WMS: siga o bip e a barra SINAL, pergunte aos colegas | 60s / 55s |
| 🚚 Descarga urgente | Suba na empilhadeira, pegue o pallet no recebimento e guarde na posição sorteada da rua (R0X-PYY), no nível pedido | 120s / 100s |
| 🪣 Pedido abandonado | Robson ou Jéssica chuta o balde e vai embora, e aparece no rádio (com rosto, igual ao chefe) contando o que largou. Logo depois o chefe reage. O pedido cai no topo do balcão, com o primeiro item já separado: termine e entregue | 150s / 130s |
| 🖥️ Tela roxa no WMS | O sistema trava: abre a tela roxa "ERRO NO SISTEMA" e o balcão para de liberar pedido. Vá ao balcão e chame a TI. Ao chamar, o relógio para e o técnico (colete azul) vem consertar. Quem já tem pedido na mão pode continuar | 40s / 35s |
| 😡 Briga no galpão | Dois colegas param e começam a brigar. Ligue pro RH no ramal da parede de cima (perto da placa EPI). Ao ligar, o relógio para e a moça do RH sai da sala, acalma os dois e volta | 40s / 35s |
| 💥 Batida de empilhadeiras | Duas empilhadeiras levando carga pro caminhão batem de frente no corredor entre as bancadas e pega fogo. Apague com o extintor. A carga do último pedido entregue queima e volta pro balcão como "-R" pra refazer | 34s / 30s |

O extintor e a empilhadeira ficam sempre no mapa, mas só funcionam na urgência deles. Os pedidos não param: enquanto você resolve a urgência, o prazo deles continua correndo.

## Galpão vivo

Os colegas (Robson, Jéssica e Kauã) trabalham de verdade: pegam caixa na rua, embalam numa bancada livre (de frente pra ela, com a caixa no tampo e a fita sendo passada) e levam pro pallet da doca, em loop. Eles não usam a bancada em que você está e esperam o fogo apagar antes de passar. Eles saem das ruas pelo corredor de cima, pra deixar livre a área do pulmão onde a empilhadeira manobra.

O chefe sai da sala (porta "CHEFE" na parede de cima) de tempos em tempos, passeia por dois ou três pontos do galpão, para pra vigiar e volta. Se passar perto de você, solta um comentário.

O chefe também aparece no canto da tela reclamando: fila com 3 pedidos, pedido atrasado, cada urgência, esbarrão de empilhadeira e quando você fica parada com pedido esperando. Entre uma bronca e outra há pelo menos 18 segundos (fila cheia e urgências furam essa espera).

## Ritmo do turno sem fim

Cai um pedido a cada 35 segundos (no máximo 6 esperando). Com 5 ou mais pedidos parados no balcão, o próximo demora o dobro (70 segundos), pra dar tempo de recuperar.

As urgências são sorteadas com peso: tela roxa e briga aparecem mais (21% cada), coletor, descarga e abandono no meio (14% cada), e incêndio e batida menos (7% cada). O sorteio nunca repete a mesma urgência em seguida nem coloca dois fogos seguidos.

## Hidratação

No turno sem fim, embaixo do relógio tem uma gota com uma barra de água. Ela esvazia em cerca de 3 minutos andando (um pouco mais rápido correndo). Com 25% ela fica laranja e o rádio avisa. Zerou: a personagem desidrata e começa uma contagem de 20 segundos pra beber água no bebedouro (parede de cima, do lado da porta do Geraldo). A seta passa a apontar pra lá. Se não beber a tempo, o turno acaba com "VOCÊ DESIDRATOU".

## Personagens

Geraldo é o chefe (popup do rádio e ronda pelo galpão). Vini é o técnico da TI que conserta a tela roxa. Os balões de fala mostram o nome de quem está falando.

## Pedidos entregues

Por enquanto a marcação é o número de pedidos finalizados, no prazo ou atrasados. Aparece embaixo do relógio ("✔ 3 ENTREGUES"), no relatório do turno e no fim do turno sem fim. O total de todas as partidas fica salvo no navegador e aparece na tela inicial.

A etiqueta mostra os horários no relógio do turno: entrada do pedido, prazo e atraso (em vermelho quando passou).

## Progresso salvo

O navegador guarda em que fase da campanha você está (e os tempos das fases que já passou). Fechou o jogo no meio da fase 4? Na próxima vez a tela inicial mostra "CONTINUAR · FASE 4" e você volta no começo dela. "RECOMEÇAR DA FASE 1" apaga o progresso. Zerou a campanha, o progresso some. Fica salvo por navegador e aparelho (localStorage), sem login.

## Turno sem fim

É o jogo principal: a tela inicial tem um botão só, INICIAR, que abre o turno sem fim. As 6 fases da campanha continuam no código, mas sem entrada na tela inicial. Pedidos caem a cada 35 segundos e urgências a cada 45, sem meta. O turno acaba quando uma urgência dá errado, e a tela final mostra quantos pedidos você entregou e em quanto tempo.

## Fase 4: Fila no Balcão

Pedidos aleatórios a cada 40 segundos (itens, endereços, doca e cliente mudam a cada partida) e a primeira urgência aos 25 segundos, depois uma a cada 50. Fecha com 3 entregas.

## Fase 5: Chegou Carga

O caminhão do fornecedor encostou na DOCA 2. Suba na empilhadeira, encaixe o garfo em cada pallet do recebimento e guarde no pulmão (P1 no PUL-01 nível 2, P2 no PUL-03 nível 3).

## Fase 6: Black Friday

Começa com 2 pedidos na fila, um novo a cada 35 segundos e uma urgência a cada 45. Fecha com 5 entregas.

## Rádio

- **Rádio do galpão:** comenta o que acontece durante o turno. As falas ficam no objeto `TEXTOS`, no topo do script.
- **Rádio de fundo:** a 89 FM A Rádio Rock ao vivo. O [R] liga e desliga. As estações ficam na lista `RADIOS`, no começo do script; se tiver mais de uma, o [R] passa por elas antes de desligar. Se a emissora liberar, o som passa por um filtro de rádio AM; se não, toca sem filtro.

## Tecnologia

HTML, Canvas 2D e JavaScript puro, num único arquivo e sem dependências.
A missão e o mapa ficam como dados no topo do script, para facilitar a criação de novas fases.

## Status

🚧 Protótipo em desenvolvimento: versão 0.5 com 6 fases em sequência e pedidos caindo no balcão WMS. Próximas fases no [ROADMAP](ROADMAP.md).
