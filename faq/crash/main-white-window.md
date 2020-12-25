# После обновления пустой экран

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

|1C:Предприятие|8.03.17.1851
|:--- |:--- 
|Документооборот КОРП|2.01.10.2
|Расширение ДОАМ|1.06.03

``` danger
**2020-12-24**  
После обновления компонентов C++ на клиенте отображается только белый экран.
```

1. Первым делом необходимо проверить работу лицензионного ключа:
``` mermaid
flowchart LR
  b1([1С:Предприятие]);
  b1 -. Открыть .-> m1[Сервис и настройки];
  m1 --> m2[fa:fa-info-circle О программе...];
  classDef default fill:#facc1f,stroke:#a0a0a0,stroke-width:1px;
  classDef button fill:#f9f9f9,stroke:#a0a0a0,stroke-width:2px;
  classDef mainmenu fill:#fbed9e,stroke:#a0a0a0,stroke-width:1px;
  class b1 button;
  class m1 mainmenu;
```
