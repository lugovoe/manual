# Mermaid Test ёёё

```mermaid
graph LR
  m1[Сервис и настройки] --> m2[О программе...]:::contextmenu;
  m2 --> C[fa:fa-ban forbidden];
  m2 --> D(fa:fa-spinner);
  classDef default fill:#fbed9e,stroke:#a0a0a0,stroke-width:1px;
  classDef contextmenu fill:#facc1f;
```

```mermaid
graph TB
    c1-->a2
    subgraph one
    a1-->a2
    end
    subgraph two
    b1-->b2
    end
    subgraph three
    c1-->c2
    end
```

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

```mermaid
classDiagram
classA <|-- classB
classC *-- classD
classE o-- classF
classG <-- classH
classI -- classJ
classK <.. classL
classM <|.. classN
classO .. classP
```

```mermaid
erDiagram
    CUSTOMER ||--o{ ORDER : places
    ORDER ||--|{ LINE-ITEM : contains
    CUSTOMER }|..|{ DELIVERY-ADDRESS : uses
```
