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
| 🧹 Caixa derrubada | Alguém derrubou uma caixa numa das ruas. Vá até lá e segure a ação pra varrer (a bagunça some aos poucos) | 45s (turno sem fim) |
| 🖥️ Tela roxa no WMS | O sistema trava: abre a tela roxa "ERRO NO SISTEMA" e o balcão para de liberar pedido. Vá até a sala da TI (porta TI, ao lado do balcão) e chame o Vini na mesa dele. No turno sem fim são 2 minutos, sem apito. Ao chamar, o relógio para e o Vini sai pela porta da TI pra consertar. Quem já tem pedido na mão pode continuar | 40s / 35s |
| 😡 Briga no galpão | Dois colegas param e começam a brigar, numa de 5 discussões com roteiro (rádio, ar-condicionado, marmita, último café da garrafa e estilete sumido); a Gisele do RH responde sobre o assunto. Na briga da rádio, a música troca pra Casa dos Caipiras e volta pra 89 FM quando o RH resolve. Na do ar, um quer 16 °C e o outro está derretendo; o RH trava em 22 °C. No turno sem fim, o prazo é de 2 minutos, sem apito e sem modal: a seta aponta pra porta do RH. Vá até a sala do RH (porta lilás na parede de cima) e chame a Gisele na mesa dela. Ao chamar, o relógio para e ela sai pela porta do RH, acalma os dois e volta | 40s / 35s |
| 💥 Batida de empilhadeiras | Duas empilhadeiras levando carga pro caminhão batem de frente no corredor entre as bancadas e pega fogo. Apague com o extintor. A carga do último pedido entregue queima e volta pro balcão como "-R" pra refazer | 34s / 30s |

O extintor e a empilhadeira ficam sempre no mapa, mas só funcionam na urgência deles. Os pedidos não param: enquanto você resolve a urgência, o prazo deles continua correndo.

## Galpão vivo

Os colegas (Robson, Jéssica e Kauã) trabalham de verdade: pegam caixa na rua, embalam numa bancada livre (de frente pra ela, com a caixa no tampo e a fita sendo passada) e levam pro pallet da doca, em loop. Eles não usam a bancada em que você está e esperam o fogo apagar antes de passar. Eles saem das ruas pelo corredor de cima, pra deixar livre a área do pulmão onde a empilhadeira manobra.

O chefe sai da sala (porta "CHEFE" na parede de cima) de tempos em tempos, passeia por dois ou três pontos do galpão, para pra vigiar e volta. Se passar perto de você, solta um comentário.

O chefe também aparece no canto da tela reclamando: fila com 3 pedidos, pedido atrasado, cada urgência, esbarrão de empilhadeira e quando você fica parada com pedido esperando. Entre uma bronca e outra há pelo menos 18 segundos (fila cheia e urgências furam essa espera).

## Demandas e o Enzo

**🚛 Caminhão (demanda):** começa assim que você fecha a janela do pedido entregue. Abre uma janela explicando o passo a passo (subir na empilhadeira, pegar no recebimento, guardar no endereço da faixa azul, 3 vezes). Enquanto dura, os pedidos congelam: não cai pedido novo, o prazo de quem espera para, o balcão não libera pedido e o chip da fila fica azul com ❄.

**Empilhadeira livre:** dá pra subir e descer da empilhadeira a qualquer hora. Perto dela aparece o botão 🚜 (igual ao do carrinho), que fica amarelo enquanto você pilota e serve pra subir e descer; no teclado é a tecla F. No computador, os botões do carrinho e da empilhadeira também aparecem no canto de baixo e dá pra clicar. Na descarga, a ação também sobe (E). Precisa estar quase parada pra descer. O pallet fica no garfo e, ao subir de novo, você continua de onde parou.

**📋 Inventário rápido (demanda):** conte as caixas de 3 endereços (segure a ação em cada posição piscando em azul) e digite os números no WMS do balcão, com botões de + e −. Se algum número não bater, o WMS avisa qual conferir. Pedidos congelados enquanto isso.

**🎓 Treino do Enzo:** o Enzo te segue nos próximos 3 pedidos normais. Cada passo (pegar no balcão, coletar, embalar, entregar) só conta com ele do lado. Ele se distrai de vez em quando e some; é só chegar perto que ele volta. O treino corre em paralelo: os problemas continuam aparecendo no meio. Os 3 pedidos do treino não contam pro ciclo de demandas.

- No primeiro incêndio ou batida depois do primeiro treino, o Enzo vem ter aula de fogo: segue você enquanto apaga e comenta no fim.
- Depois do primeiro treino, ele aparece de vez em quando passeando pelo galpão e soltando comentários.
- Nos treinos seguintes ele volta "pra reaprender", com falas diferentes.

## Ritmo do turno sem fim

Cai um pedido a cada 35 segundos (no máximo 6 esperando). Com 5 ou mais pedidos parados no balcão, o próximo demora o dobro (70 segundos), pra dar tempo de recuperar.

Problemas vêm por TEMPO e demandas pela quantidade de pedidos:

- **Problemas:** o primeiro é sempre a tela roxa, aos 25 segundos. Depois, um novo uns 45 segundos depois de resolver o anterior (com 6 segundos pra mais ou pra menos de imprevisto). O intervalo aperta 2 segundos por minuto de turno, até uns 28 segundos. Depois de uma demanda, 20 segundos de respiro.
- **Demandas:** a cada 3 pedidos entregues, alternando caminhão, treino do Enzo e inventário. Começam ao fechar a janela do pedido entregue. O treino corre em paralelo, então os problemas continuam caindo no meio dele.

Os problemas são sorteados com peso: incêndio, tela roxa e briga aparecem mais; cliente ao telefone, caixa derrubada, coletor, abandono e batida no meio; descarga urgente menos (o caminhão já usa a empilhadeira). O sorteio nunca repete o mesmo problema em seguida nem coloca dois fogos seguidos.

Pensando em sessões de 20 a 30 minutos:

- Entre os 5 primeiros problemas sempre vêm a tela roxa (a primeira), um incêndio e a briga da rádio caipira (a primeira briga do turno é sempre essa).
- As brigas não entram no sorteio: depois da primeira, vem uma a cada ~6 minutos, e o assunto só repete depois que os 5 saírem (em 30 min dá umas 5 brigas).
- Se até os 5 minutos não houve incêndio, o próximo problema é fogo; se até os 12 minutos não houve descarga urgente, ela é forçada.
- **🏢 Visita da diretoria:** uma vez por turno, entre 9 e 11 minutos. O Geraldo avisa nervoso e aparecem 3 bagunças pelo galpão. Limpe todas (segure a ação) antes do tempo acabar, senão "O DIRETOR VIU A BAGUNÇA". Limpou tudo: o diretor entra com o Geraldo colado atrás, passeia comentando e vai embora. O Geraldo não dá bronca enquanto acompanha o diretor.
- **📞 Cliente ao telefone:** só toca com um pedido em separação. Atenda no balcão: o cliente troca um item que você ainda não pegou ou pede mais uma unidade. A etiqueta é reimpressa com a mudança marcada em amarelo.

Numa simulação de 30 minutos vieram cerca de 42 eventos, com 4 ou 5 incêndios, 2 ou 3 descargas, 3 caminhões, 3 inventários e 1 visita.

**📻 Rádio Peão:** durante a briga, a discussão aparece num chat próprio (fundo escuro, borda tracejada laranja, "AO VIVO" e "só ouvindo"), com rosto e nome de quem fala: os dois colegas e depois o RH. No computador fica no canto de cima à direita; no celular, logo abaixo da faixa da urgência. Mostra as últimas 4 falas (3 no celular), avisa quando trocam a rádio pra Casa dos Caipiras e quando ela volta, e some sozinho uns segundos depois da paz.

Quem larga o emprego volta arrependido uns 2 minutos depois, pra não faltar gente pra brigar nem pra largar pedido.

## Hidratação

No turno sem fim, embaixo do relógio tem uma gota com uma barra de água. Ela esvazia em pouco mais de 4 minutos andando (um pouco mais rápido correndo). Com 25% ela fica laranja e o rádio avisa. Zerou: a personagem desidrata e começa uma contagem de 20 segundos pra beber água no bebedouro (parede de cima, do lado da porta do Geraldo). A seta passa a apontar pra lá. Se não beber a tempo, o turno acaba com "VOCÊ DESIDRATOU".

## Personagens

Geraldo é o chefe (popup do rádio e ronda pelo galpão). Vini é o técnico da TI que conserta a tela roxa: fala quando chega e quando termina, e a conversa dos colegas não atropela o balão dele. O diretor aparece na visita da diretoria. Os balões de fala mostram o nome de quem está falando.

## Pedidos entregues

Por enquanto a marcação é o número de pedidos finalizados, no prazo ou atrasados. Aparece embaixo do relógio ("✔ 3 ENTREGUES"), no relatório do turno e no fim do turno sem fim. O total de todas as partidas fica salvo no navegador e aparece na tela inicial.

A etiqueta mostra os horários no relógio do turno: entrada do pedido, prazo e atraso (em vermelho quando passou).



## Geraldo mais calmo

O Geraldo só reclama quando 5 pedidos atrasados ficam parados no balcão (e pra lembrar de beber água). Ele não comenta mais penalidade, briga, tela roxa nem pedido atrasado sozinho. No turno sem fim, pedidos novos entram a cada 95 segundos (era 35), mais a folga quando a fila está cheia.

## Primeiros 15 minutos (estreia)

Pra quem está conhecendo o jogo, o turno sem fim tem um roteiro fixo de demandas nos primeiros 15 minutos:

| Quando | Demanda |
|---|---|
| 2:30 | ☕ Café do Geraldo |
| 5:00 | 🎓 Enzo chega pro treino |
| 7:30 | 🚛 Caminhão (empilhadeira) |
| 10:00 a 11:00 | 🏢 Visita da diretoria |

Cada uma começa quando você está sem pedido na mão. Os problemas (tela roxa, incêndio, briga...) seguem normais. Depois dos 15 min, volta o rodízio: uma demanda a cada 3 pedidos entregues (caminhão, Enzo, relatório, inventário, café e bolo), o que dá mais ou menos uma a cada 5 ou 6 minutos com os pedidos a cada 95 s.

## Novas demandas: relatório e bolo surpresa

Entram no rodízio de demandas do turno sem fim (os pedidos congelam enquanto isso, igual ao café):

- **🖨️ Relatório do Geraldo:** vá até a impressora da sala da TI (ela funciona, ninguém sabe explicar). Abre a tela do PC: abrir o e-mail "URGENTE!!!! RELATORIO", baixar o `relatorio_final_v3_AGORAVAI (2).pdf`, ajustar (3 páginas, colorido) e imprimir. Depois dá pra espiar as 3 páginas: gráfico com a sexta "estimada com base no otimismo do gestor", pizza de tempo, "[inserir ponto de atenção aqui]" e as frases de IA no começo e no fim ("Claro! Posso te ajudar...", "Aqui está o seu relatório! 😊"). Leve as folhas até a mesa do Geraldo. +140 pontos.
- **🎂 Bolo surpresa:** a Gisele avisa que é aniversário de um colega. Pegue o bolo na geladeira da cozinha, segure a ação na mesa pra acender a vela e leve até o aniversariante no galpão (a seta segue a pessoa). O galpão canta parabéns. +160 pontos.

## Salas do RH e da TI

Todas as portas mostram o botão ENTRAR. Duas portas novas na parede de cima: **RH** (lilás, com coraçãozinho) e **TI** (azul-escura, ao lado do balcão). A porta pisca quando tem briga ou tela roxa esperando.

- **Sala do RH:** faixa "GRATIDÃO", mural de aniversariantes com balões, difusor soltando vapor, caixa de lenço e puff rosa. A Gisele trabalha lá. Dá pra conversar com ela e fuçar a caixa de sugestões anônimas, o mural dos aniversariantes (com a foto do Geraldo cantando Roupa Nova na festa junina) e o arquivo de ocorrências (com a autoavaliação nota 10 do Geraldo e as férias que ele mesmo aprovou).
- **Sala da TI:** rack com leds piscando, quadro branco rabiscado, pôster "SEM CHAMADO", latinhas e teclado colorido. Dá pra conversar com o Vini e fuçar o quadro (a rede passa por uma fita isolante), a fila de chamados (o Geraldo pediu pra aumentar a internet só no PC dele) e a caixa de cabos.
- Quando a pessoa sai pra atender, a mesa fica com a plaquinha "JÁ VOLTO" ou "ATENDENDO".

## Salas: cozinha e sala do chefe

Na parede de cima tem duas portas que dá pra entrar (ação perto da porta):

- **Cozinha** (porta à direita da placa PERIGO): pia, micro-ondas, cafeteira, geladeira com bilhete "NÃO MEXE" e mesa. A pia tem piadinha. Dá pra abrir (mesma pasta da sala do chefe, com a cara de cada lugar):
  - **Geladeira**: por dentro, com prateleiras de vidro e etiquetas de fita crepe escritas à mão: a marmita do Kauã (agora com nome), o bolo de pote "NÃO MEXE" da Jéssica, o pote de sorvete com feijão, a pizza da reunião com o nome do Geraldo, o suquinho do Enzo com letra de mãe, o iogurte de 2024, a garrafa de 2 litros do RH e 37 sachês de ketchup.
  - **Armário de canecas** (armários de cima, na frente do micro-ondas): uma caneca com o estilo de cada um: Geraldo (Roupa Nova 98), Jéssica (rosa com glitter, "não fale comigo antes do café"), Robson (térmica de 1 litro), Kauã (de banda, lascada), Enzo ("primeiro emprego!"), Vini ("já tentou desligar e ligar?"), RH ("gratidão") e a sua (brinde de fornecedor, alça torta).
- **Sala do chefe** (porta CHEFE): o Geraldo atrás da mesa (se não estiver na ronda), quadro de "funcionário do mês" com a cara dele e gráfico de META. Falando com ele abre um chat com quatro pedidos: **aumento, férias, folga e sair mais cedo**. Ele sempre tem uma desculpa diferente. Dá pra **fuçar** três lugares (abre uma pasta de arquivo com papéis presos por clipe; o jogo pausa enquanto você lê):
  - **Gaveta da mesa** (lado esquerdo da mesa): o pedido de aumento do próprio Geraldo, carimbado APROVADO; um post-it pra ensaiar o "vou ver o que posso fazer"; um pente novinho (ele é careca).
  - **Arquivo** (gaveteiro da direita): a lista de desculpas pra não dar folga, com as já usadas riscadas; ingresso do show do Roupa Nova de 1998; carteirinha do fã-clube com foto de quando tinha cabelo.
  - **Mural de cortiça** (parede, à direita do gráfico de META): pôster do Roupa Nova, a setlist dele pro karaokê da firma, a escala de folgas de dezembro (só ele folga, carimbo CONFIDENCIAL) e o lembrete de dizer pro diretor que a ideia do café foi dele.
  - Se o Geraldo estiver na sala, metade das vezes ele pega você no flagra.

O relógio, os pedidos e os problemas continuam correndo enquanto você está numa sala (as salas ficam fora do mapa, então nada do galpão esbarra em você lá dentro). O carrinho fica do lado de fora, na porta. Se tem coisa pra fazer no galpão, a seta aponta pra SAÍDA.

**☕ Café do chefe (demanda nova, sem relógio):** o Geraldo pede café; os pedidos congelam. Entre na cozinha, segure a ação na cafeteira até encher a jarra e leve a garrafa até a mesa dele (+120 pontos). Entra na rotação das demandas junto com caminhão, treino do Enzo e inventário.

## Ritmo dos pedidos

- Um pedido novo a cada 35 s, mas com fila o próximo demora mais: 2 parados +30%, 3 parados +60%, 4 ou mais o dobro.
- Com 3 ou mais pedidos esperando, o próximo vem com **1 item só**; com 2 esperando, no máximo 2 itens e 1 unidade de cada.
- Enquanto um problema está na tela, o relógio do próximo pedido anda 40% mais devagar.
- Os problemas aceleram até ficar um a cada ~33 s (antes chegava a 28 s).
- O Geraldo ficou ~20% menos reclamão: intervalo entre broncas de 18 para 22,5 s, e 1 em cada 5 broncas urgentes ele deixa passar (o aviso da água sempre vem).

## Pontuação e ranking

No turno sem fim, o HUD mostra ★ pontos e o combo atual.

| O quê | Pontos |
|---|---|
| Pedido entregue | 100 + 10 por volume, +50 no prazo; atrasado perde 1 por segundo de atraso (mínimo 30) |
| Combo | cada pedido no prazo e sem trombada sobe o multiplicador em 0,1 (até x1,5); atraso ou trombada volta pra x1,0 |
| Problema resolvido | incêndio e descarga 150; batida e abandono 120; briga e cliente 100; tela roxa, coletor e caixa 80; + até 50 de rapidez |
| Demandas | caminhão 200, inventário 150, treino do Enzo 150, visita do diretor sem bagunça 300 |
| Trombadas e afins | -5 por segundo de penalidade |
| Tempo de turno | +10 por minuto |

No fim do turno sai o **relatório** com o total, o detalhamento e o cargo: Novato, Auxiliar (500), Separador (1.500), Conferente (3.000), Líder de Turno (5.000), Supervisor (8.000) e Lenda do Galpão (12.000).

**Ranking (Firebase, sem login):** todo fim de turno salva sozinho no ranking: quando a água acaba, quando um problema estoura, quando a pessoa sai pela pausa e até quando fecha a página no meio do turno. Cada turno é uma linha (pode repetir nome). Sem nome, entra como Visitante e dá pra trocar o nome ali no relatório. A tela inicial mostra o mural com o **Funcionário da semana** (1º da semana, troca toda segunda) e o top 10 da semana e geral, com o seu nome destacado. Detalhes do banco em `firebase/README.md`.

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
