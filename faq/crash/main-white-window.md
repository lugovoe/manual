# После обновления пустой экран

    ```mermaid
    graph TB
      classDef default fill:#facc1f,stroke:#a0a0a0,stroke-width:1px;
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
  b1(["fa:fa-external-link 1С:Предприятие"]) -. fa:fa-spinner Открыть .-> m1;
  m1[fa:fa-caret-down Сервис и настройка] --> m2;
  m2[fa:fa-info-circle О программе...];
  classDef default fill:#facc1f,stroke:#a0a0a0,stroke-width:1px;
  classDef button fill:#f9f9f9,stroke-width:2px;
  classDef mainmenu fill:#fbed9e;
  class b1 button;
  class m1 mainmenu;
```
![about](images/about.png)

1. Открыть `Конфигурацию` в режиме конфигуратора (слева откроется окно)
``` mermaid
flowchart LR
  b1(["fa:fa-external-link Конфигуратор"]) -. fa:fa-spinner Открыть .-> m1;
  m1(Конфигурафия) --> m2;
  m2(Открыть конфигурацию);
  classDef default fill:#d6e9ff,stroke:#a0a0a0,stroke-width:1px;
  classDef button fill:#f9f9f9,stroke-width:2px;
  classDef cfgmenu stroke:#9eb6e9,color:#3d4e8f;
  class b1 button;
  class m1,m2 cfgmenu;
```
2. Проверить настройки Начальной страницы `Конфигурации`
``` mermaid
flowchart LR
  b1[fa:fa-circle-o ДокументооборотКОРП];
  b1 -- ПКМ --> m1(Открыть рабочую область начальной страницы);
  m1 -. fa:fa-spinner Открыть .-> b0;
  b0[fa:fa-window-restore];
  b2[fa-pencil-square-o Шаблон начальной страницы];
  classDef default fill:#d6e9ff,stroke:#a0a0a0,stroke-width:1px;

```
3. 
