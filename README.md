<<<<<<< HEAD
﻿# Ficha 5 — Cartas novas

## API

A aplicação utiliza uma API desenvolvida com Node.js e Express para consultar e adicionar cartas.

| Método | URL | O que recebe | Resposta |
|---|---|---|---|
| GET | /api/cartas | Não recebe dados | 200 — Devolve todas as cartas em JSON. |
| POST | /api/cartas | JSON com name, type e attack | 201 — Devolve a carta criada. |
| POST | /api/cartas | Carta sem nome ou sem tipo | 400 — Devolve uma mensagem de erro. |

## Pergunta 3

O primeiro pedido é o OPTIONS, enviado automaticamente pelo browser para verificar se o servidor permite a comunicação entre origens diferentes. Isto acontece porque o POST utiliza JSON. Sem o pacote cors, o servidor não responde corretamente ao pedido OPTIONS e o browser bloqueia o POST. Por isso, a rota POST nunca chega a ser executada.

## Pergunta 4

Na primeira versão, a carta nova existia apenas no estado do React (setCards), sendo apagada ao atualizar a página com F5. Na segunda versão, a carta ficava guardada no array do servidor, mas desaparecia quando o servidor era reiniciado. Na terceira versão, a carta passou a ser guardada no ficheiro cartas.json, mantendo-se mesmo depois de reiniciar o servidor.
=======
# tarefa4
# tarefa4
>>>>>>> origin/main
