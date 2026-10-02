# trabalho-engenharia-software

Trabalho de engenharia de software do prof Henry em 2026-02



Este repositório é onde vou guardar meu trabalho da disciplina de engenharia de software.

## Diagrama UML 

```mermaid
flowchart TD
    %% atores
    cliente[" 🙋‍♂️cliente"]
    garçom[" 🧑‍💼garçom"]

    %% ações
    subgraph sistema
        comida["pedir comida"]
        vinho["pedir vinho"]
    end

    %% relacinamentos
    cliente -- "faz pedido" --- comida
    garçom -- "recebe pedido" --- comida

    vinho -. "estende" .-> comida
```
