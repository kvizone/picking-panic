# Firebase do ranking

Projeto `picking-panic` (conta kvizone@gmail.com), plano Spark (grátis).

- **Realtime Database** `picking-panic-default-rtdb` (us-central1), com as regras de `regras.json` publicadas.
- **Authentication → Anônimo** ligado (sem limpeza automática, pra ninguém perder o nome depois de 30 dias).
- App web `picking-panic-web`, config em `config.js`.

## Como os dados ficam

| Caminho | Quem lê | Quem escreve |
|---|---|---|
| `ranking/{nome}` | todo mundo | só o dono do nome, e só se a pontuação subir |
| `semanal/{AAAA-Wss}/{nome}` | todo mundo | igual ao ranking, por semana |
| `donos/{nome}` | todo mundo | quem pega o nome primeiro (ou quem tem o código) |
| `segredos/{nome}` | ninguém | o dono, uma vez, ao pegar o nome |
| `provas/{nome}/{uid}` | ninguém | qualquer um, pra provar o código e trocar de aparelho |

`{nome}` é o nome sem acento, espaço nem maiúscula (só a-z e 0-9). Os campos aceitos são nome, pontos, quando, pedidos, segundos, cargo, disp e versao; qualquer outro é recusado.

Pra apagar alguém do ranking (nome ofensivo, teste), apague na aba Dados do console: `ranking/{nome}`, `semanal/.../{nome}`, `donos/{nome}` e `segredos/{nome}`.
