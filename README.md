# trabalho-engenharia-software

Trabalho de engenharia de software do prof Henry em 2026-02



Este repositório é onde vou guardar meu trabalho da disciplina de engenharia de software.

## Diagramas UML 
### Diagrama de casos de uso

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
###  Diagrama de classe 

```mermaid
classDiagram
   class Veterinario{
    -nomeVet: String
    +darNomeVet() String
    +atenderAnimal(animal: Animal) void
   }

    Veterinario -- Animal
   Animal -- Tutor
    
    class Animal{
        -nome: String
        -especie: String
        -done: Tutor
        +darNome() String
        +darEspecie() String
    }

    class Tutor{
        -nomeTutor: String
        -animais: Animal[]
        +darNomeTutor() String
    }
```
