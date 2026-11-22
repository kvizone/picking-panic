# Firebase do ranking

Projeto `picking-panic` (conta kvizone@gmail.com), plano Spark (grátis).

- **Realtime Database** `picking-panic-default-rtdb` (us-central1), com as regras de `regras.json` publicadas.
- **Authentication → Anônimo** ligado (sem limpeza automática, pra ninguém perder o nome depois de 30 dias).
- App web `picking-panic-web`, config em `config.js`.

## Como os dados ficam

| Caminho | Quem lê | Quem escreve |
|---|---|---|
| `ranking/{id}` | todo mundo | cria qualquer um logado (anônimo); só quem criou pode mudar ou apagar |
| `semanal/{AAAA-Wss}/{id}` | todo mundo | igual ao ranking, por semana |

Cada turno vira uma linha nova (o mesmo nome pode aparecer várias vezes). A linha guarda o `uid` de quem criou, pra pessoa poder trocar o nome do próprio resultado no relatório. Campos aceitos: nome, pontos, quando, pedidos, segundos, cargo, disp, versao e uid; qualquer outro é recusado.

Linhas antigas (antes de 22/11/2026) usam o nome como id e não têm uid; continuam aparecendo normalmente.

Pra apagar alguém do ranking (nome ofensivo, teste), apague a linha na aba Dados do console, em `ranking` e em `semanal/...`.
