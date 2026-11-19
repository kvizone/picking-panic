# Roadmap do Picking Panic

## Visão geral

| Fase | Nome | Mecânica nova | Status |
|---|---|---|---|
| 1 | Pedido #1042 | Picking a pé, embalagem e consolidação | 🚧 Em ajustes |
| 2 | Pallet no Alto | Dirigir a empilhadeira | 💡 Planejada |
| 3 | Cadê o Coletor? | Exploração sem GPS, guiada pelo som | 💡 Planejada |

**Ordem de construção sugerida:** melhorias da fase 1 → reorganizar o código para suportar várias fases → fase 3 → fase 2.
A fase 3 reaproveita o personagem a pé e o áudio posicional que já existem. A fase 2 exige física de veículo, que é a parte mais trabalhosa. A ordem dentro do jogo continua 1, 2, 3.

---

## Fase 1: Pedido #1042 (melhorias)

### Pedido como etiqueta real
- O terminal "imprime" o pedido: a etiqueta sai da impressora linha a linha, com som de impressora térmica.
- Visual de etiqueta térmica: papel branco levemente amarelado, fonte monoespaçada, código de barras e QR desenhados em pixels, borda serrilhada de picote, número do pedido grande, logo do cliente fictício.
- Lista de itens com endereço, quantidade e uma caixinha `[ ]` que vira `[X]` ao coletar.
- A tecla Q mostra a etiqueta "na mão" do operador, meio amassada, com os itens já riscados.

### Coleta em endereços diferentes (multi-picking)
- O pedido tem de 3 a 4 itens em ruas diferentes, por exemplo:
  - `R01-P04`: 1x Fita adesiva industrial
  - `R03-P07`: 2x Caneca térmica
  - `R04-P12`: 1x Etiquetadora
- A ordem de coleta é livre. Escolher a melhor rota é a habilidade do speedrun.
- A seta-guia aponta para o item não coletado mais próximo. O minimapa marca todos.
- O HUD mostra o checklist resumido (`2/4`).
- Nas próximas versões, a estrutura do pedido pode virar sorteio: cada partida gera um pedido diferente com base numa lista de produtos e endereços.

### Storytelling com a voz da Karla
- Todas as falas do jogo saem do código e vão para um objeto `TEXTOS` no topo do arquivo, com várias variações por evento, sorteadas a cada vez, para não repetir.
- Tom: sarcástico e bem-humorado, sem zoar o trabalho em si (nada de piada com retrabalho ou com a equipe). O alvo da piada é a situação: a empilhadeira, o relógio, o cliente apressado, a fita que gruda no dedo.
- Eventos que precisam de texto: início do turno, pedido impresso, endereço errado, volume coletado, pedido completo, bancada, erro na embalagem, embalagem ok, batida na empilhadeira, esbarrão em NPC, perdeu estrela, pallet errado, caminhão saindo, vitória (1, 2 e 3 estrelas), novo recorde, pausa.
- Exemplos para calibrar o tom (Karla edita e escreve os definitivos):
  - Início: "Pedido prioritário. Todos são, mas esse é mais."
  - Endereço errado: "Isso é a P08. A P07 tá do outro lado. Confia."
  - Empilhadeira: "A empilhadeira tem preferência. Sempre teve."
  - Erro na embalagem: "A fita grudou no dedo. Clássico."
  - 1 estrela: "Saiu. O cliente achou que demorou, mas saiu."
  - 3 estrelas: "Isso foi um pedido ou um teletransporte?"

---

## Fase 2: Pallet no Alto (empilhadeira)

**Situação:** a posição de picking da R02 zerou e um pedido grande depende dela. O jogador precisa buscar um pallet cheio no nível alto (pulmão) da R04 e levá-lo até a doca.

### Fluxo da missão
1. Ir a pé até o carregador e entrar na empilhadeira (E).
2. Dirigir até `R04-P10 / Nível 3`.
3. Alinhar os garfos de frente para a baia.
4. Subir os garfos: minigame de segurar uma tecla até a barra parar na faixa verde do nível 3. Passar do ponto = pallet balança, solta caixa e +3s.
5. Retirar o pallet, dirigir de ré com cuidado e levar até a área de staging da DOCA 1.
6. Baixar e soltar o pallet dentro da demarcação laranja.

### Direção estilo GTA 1
- W acelera, S freia e dá ré, A e D giram. A empilhadeira tem inércia, então derrapa um pouco na curva.
- Com o pallet nos garfos, ela fica mais lenta e vira mais devagar.
- H buzina e faz os NPCs saírem da frente.
- O apito de ré (o som já existe) toca quando o jogador dá ré.
- A câmera se afasta um pouco enquanto o jogador dirige.

### Riscos e penalidades
- Bater em rack: caixas caem no chão (ficam como obstáculo) e +3s.
- Faixa azul de pedestre: limite de velocidade. Passar rápido = "multa" de +2s.
- Atropelar cone: o cone sai rolando e a penalidade é leve.
- Encostar em NPC: ele pula para o lado assustado e +5s.

### Código
- Transformar a empilhadeira numa classe `Veiculo` reaproveitável, que tanto o jogador quanto os NPCs podem usar.
- Hitbox retangular orientada, já pedida nos ajustes da fase 1.

---

## Fase 3: Cadê o Coletor?

**Situação:** o coletor de dados sumiu no meio do turno. Sem ele não tem WMS, ou seja, **sem seta-guia e sem minimapa**. O jogador precisa achar o aparelho antes que a bateria acabe.

### Mecânica central: guiado pelo som
- O coletor apita de tempos em tempos.
- O volume e o pan estéreo dependem da distância e da posição, como "quente ou frio" (reaproveita o áudio posicional da empilhadeira).
- A bateria vai caindo e os bipes ficam mais fracos e espaçados, o que cria a pressão de tempo.
- A posição muda a cada partida, sorteada entre vários esconderijos: atrás de um pallet, numa bancada, no meio de uma pilha de caixas vazias, dentro da cabine do caminhão.

### Pistas
- NPCs dão dicas ao apertar E perto deles, com falas sarcásticas:
  - "Vi alguém largando um troço preto perto das bancadas. Ou era um grampeador."
  - "Coletor? Achei que era o controle da TV."
- Algumas pistas são falsas, e o jogador aprende quais NPCs mentem.

### Recompensa
- Ao achar o coletor: animação de boot retrô (tela verde, "WMS v1.996 carregando...") e o HUD, a seta-guia e o minimapa "ligam" na tela.
- Para fechar a fase: um pedido rápido de 2 itens para provar que o coletor funciona.

### Acessibilidade
- Como a fase depende de som, ela precisa de um modo alternativo: um indicador visual de "sinal" (barrinhas de rádio) que funciona igual ao áudio.

---

## Estrutura técnica para várias fases
- Objeto `FASES` com a configuração de cada uma (mapa, objetivos, textos, tempos das estrelas). Cada fase vira dado, não código novo.
- Tela de seleção de fase depois do menu: cada fase mostra o melhor tempo e as estrelas. Para liberar a próxima, é preciso pelo menos 1 estrela na anterior.
- Recordes salvos por fase no localStorage.
- Quando o código passar de uns 4 mil linhas, separar em arquivos (`js/engine.js`, `js/sfx.js`, `js/juice.js`, `js/fases/*.js`, `js/textos.js`). Arquivos menores são mais fáceis para as IAs editarem sem quebrar o resto, e o GitHub Pages serve tudo normalmente.
