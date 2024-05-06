# my_mermaid
<p align="center">
<img src="https://raw.githubusercontent.com/mermaid-js/mermaid/develop/docs/public/favicon.svg" height="150">
</p>
Uma imagem vale mais que mil palavras. Agora você pode criar e editar rapidamente diagramas em markdown usando palavras com suporte Mermaid em seus arquivos Markdown.

<p><a href="https://github.com/mermaid-js/mermaid#readme"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Mermaid</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> é uma ferramenta de diagramação e gráficos baseada em JavaScript que usa definições de texto inspiradas em Markdown e cria diagramas dinamicamente no navegador. Mantido por </font></font><a href="https://github.com/knsv"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Knut Sveidqvist</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> , ele oferece suporte a vários tipos de diagramas comuns para projetos de software, incluindo fluxogramas, UML, gráficos Git, diagramas de jornada do usuário e até mesmo o temido gráfico de Gantt.</font></font></p>

## Como funciona
<p><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Quando encontramos blocos de código marcados como </font></font><code>mermaid</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">, geramos um iframe que pega a sintaxe bruta do Mermaid e a passa para Mermaid.js, transformando esse código em um diagrama em seu navegador local.</font></font></p>

### EXEMPLOS
#### DIAGRAMA DE SEQUÊNCIA

```mermaid
sequenceDiagram
Alice->>John: Hello John, how are you?
loop HealthCheck
    John->>John: Fight against hypochondria
end
Note right of John: Rational thoughts!
John-->>Alice: Great!
John->>Bob: How about you?
Bob-->>John: Jolly good!
```
#### SINTAXE MERMAID DO DIAGRAMA DE SEQUÊNCIA
       ```mermaid
       sequenceDiagram
       Alice->>John: Hello John, how are you?
       loop HealthCheck
           John->>John: Fight against hypochondria
       end
       Note right of John: Rational thoughts!
       John-->>Alice: Great!
       John->>Bob: How about you?
       Bob-->>John: Jolly good!
       ```

#### DIAGRAMA DE CLASSES

```mermaid
classDiagram
Class01 <|-- AveryLongClass : Cool
<<Interface>> Class01
Class09 --> C2 : Where am I?
Class09 --* C3
Class09 --|> Class07
Class07 : equals()
Class07 : Object[] elementData
Class01 : size()
Class01 : int chimp
Class01 : int gorilla
class Class10 {
  <<service>>
  int id
  size()
}
```
#### SINTAXE MERMAID DO DIAGRAMA DE CLASSES
       ```mermaid
       classDiagram
       Class01 <|-- AveryLongClass : Cool
       <<Interface>> Class01
       Class09 --> C2 : Where am I?
       Class09 --* C3
       Class09 --|> Class07
       Class07 : equals()
       Class07 : Object[] elementData
       Class01 : size()
       Class01 : int chimp
       Class01 : int gorilla
       class Class10 {
         <<service>>
         int id
         size()
       }
       ```

#### DIAGRAMA DE ESTADO

```mermaid
stateDiagram-v2
[*] --> Still
Still --> [*]
Still --> Moving
Moving --> Still
Moving --> Crash
Crash --> [*]
```
#### FLUXOGRAMA

```mermaid
flowchart LR

A[Hard] -->|Text| B(Round)
B --> C{Decision}
C -->|One| D[Result 1]
C -->|Two| E[Result 2]
```
