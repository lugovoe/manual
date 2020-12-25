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
  b1(["1С:Предприятие (кнопка)"]);
  b1 -. Открыть .-> m1[Сервис и настройки];
  m1 --> m2[fa:fa-info-circle О программе...];
  classDef default fill:none,stroke:none;
  classDef button fill:#f9f9f9,stroke-width:2px;
  classDef mainmenu fill:#fbed9e;
  class b1 button;
  class m1 mainmenu;
```
![about](images/about.png)

1. Открыть `Конфигурацию` в режиме конфигуратора (слева откроется окно)
``` mermaid
flowchart LR
  b1(["Конфигуратор (кнопка)"]);
  b1 -. Открыть .-> m1(Конфигурафия);
  m1 --> m2(Открыть конфигурацию);
  classDef button fill:#f9f9f9,stroke-width:2px;
  classDef confmenu fill:#d6e9ff,stroke:#9eb6e9,color:#3d4e8f;
  class b1 button;
  class m1,m2 confmenu;
```
2. Проверить настройки Начальной страницы `Конфигурации`
``` mermaid
flowchart LR
  b1[ДокументооборотКОРП];
  b1 -- ПКМ --> m1(Открыть рабочую область начальной страницы);
  m1 -. Открыть .-> b0["#hellip;#middot;"];
  b3["Шаблон начальной страницы [поле]"];
  classDef button fill:#f9f9f9,stroke-width:2px;
  classDef confmenu fill:#d6e9ff,stroke:#9eb6e9,color:#3d4e8f;
  class b1,b2 button;
  class m1 confmenu;
```
3. 
