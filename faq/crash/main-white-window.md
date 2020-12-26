# После обновления пустой экран

1. Первым делом необходимо проверить работу лицензионного ключа:
``` mermaid
graph LR
  b1([fa:fa-external-link 1С:Предприятие]) -.-> |ЛКМ: Открыть| m1
  m1[fa:fa-caret-down Сервис и настройка] --> m2
  m2[fa:fa-info-circle О программе...]
  style b1 fill:#f9f9f9,stroke-width:2px
  style m1 fill:#fbed9e,stroke-width:1px
  style m2 fill:#facc1f,stroke-width:1px
  classDef default stroke:#a0a0a0
```
![about](images/about.png)

    ```mermaid
    graph TB
      classDef default fill:#facc1f,stroke:#a0a0a0,stroke-width:1px;
    ```


|1C:Предприятие|8.3.17.1851
|:--- |:--- 
|Документооборот КОРП|2.1.10.2
|Расширение ДОАМ|1.6.3

``` danger
**2020-12-24**  
После обновления компонентов C++ на клиенте отображается только белый экран.
```

## Разрешение конфликта

1. Открыть `Конфигурацию` в режиме конфигуратора (слева откроется окно)
``` mermaid
graph LR
  %% https://mermaid-js.github.io/mermaid-live-editor/
  %% https://fontawesome.ru/all-icons/
  b1([fa:fa-external-link Конфигуратор]) -.-> |ЛКМ: Открыть| m1
  m1(fa:fa-caret-down Конфигурация) --> m2
  m2(Открыть конфигурацию)
  style b1 fill:#f9f9f9,stroke:#a0a0a0,stroke-width:2px
  classDef confmenu fill:#d6e9ff,stroke:#9eb6e9,stroke-width:1px,color:#3d4e8f
  class m1,m2 confmenu
```

2. Проверить настройки Начальной страницы `Конфигурации` в поле `Шаблон 
начальной страницы`
``` mermaid
graph LR
  subgraph new[fa:fa-window-restore Рабочая область начальной страницы]
    i1[fa:fa-pencil-square-o Шаблон начальной страницы] -.-> e2 & e3 & e4
    e2[Одна колонка]
    e3[Две колонки одинаковой ширины]
    e4["Две колонки разной ширины (2:1)"]
  end
  subgraph main[" "]
    e1[fa:fa-plus-square-o ДокументооборотКОРП] -- ПКМ --> m1
    m1(Открыть рабочую область начальной страницы) -.-> e0
    e0[fa:fa-window-restore]
  end
  style i1 fill:#fff,stroke:#000,stroke-width:2px
  style m1 fill:#d6e9ff,stroke:#9eb6e9,stroke-width:1px,color:#3d4e8f
  style main fill:none,stroke:none
  classDef element fill:#fff,stroke:#a0a0a0,stroke-width:2px,stroke-dasharray:2 4
  class e0,e1,e2,e3,e4 element
```

3. 
