- Загрузка файла из документа формата Н.
- Редактирование введённого текста.
- Удаление комментариев и лишнего всего-всего.
- Количество и нумерация строк.
- Выделение и идентификация лексем. Запись в таблице классов лексем: класс класс класс класс класс.
- Формирование дескрипторного и псевдокода.
- Распознавание лексических ошибок: ошибки в константах, идентификаторах, **незакрытый комментарий** (пушто легко сделать, она советует), и т.д.

**Дополнительные требования:**
- Работа лексического анализатора должна моделироваться конечным автоматом.
- Построить КА распознающий классы лексем: 123456
- Построить регулярную грамматику, соответствующую конечному автомату.
- Построить КС грамматику по фрагменту варианта (Указать вариант)
- Построить порождение и дерево вывода

**Алгоритмы**

Откуда-то нам надо взять и указать. Она перечислила:
- Составить блок-схемы: общий алгоритм программы, все функции.
- Сложность алгоритма
- ...

**Этапы и стадии разработки по лабораторным работам:**

- Дополнительные функции лексического анализатора
- Распознавание  заданных  слов языка программирования
- Построение таблиц идентификаторов
- Построение дескрипторного кода. Построение регулярной грамматики.
- Обработка ошибок на этапе лексического анализа. Построение КС-грамматики.
- **ОФОРМИТЬ РПЗ ПО КУРСОВОЙ РАБОТЕ И СДАТЬ ПРЕПОДАВАТЕЛЮ!!!**

Первая звучит странно, наверное надо что-то иное написать, выписано на случай если она закроет и спрячет названия лаб.


```mermaid
graph TD
    A[Входные данные] --> B{ Условие}
    B -->|Да| C[Выполнить действие]
    B -->|Нет| D[Выполнить другое действие]
    C --> E[Выходные данные]
    D --> E

```

```mermaid
classDiagram

    class LightingDevice {
        # light_color: string
        # brightness: double
        # is_enabled: bool
        + setLightColor(string)
        + getLightColor() string
        + setBrightness(double)
        + getBrightness() double
        + setEnabled(bool)
        + getEnabled() bool
    }

    class ElectricalDevice {
        # energy_consumption: int
        + setEnergyConsumption(int)
        + getEnergyConsumption() int
    }

    class ManualDevice {
        # is_portable: bool
        + setPortable(bool)
        + isPortable() bool
    }

    class Lighter {
        # fuel: float
        + setFuel(float)
        + getFuel() float
    }

    class Flare {
        # burn_time: int
        # was_enabled: bool
        + setBurnTime(int)
        + getBurnTime() int
        + prime()
    }

    class Spotlight {
        # shape: string
        + setShape(string)
        + getShape() string
    }

    class Floodlight {
        # light_amount: int
        + setLightAmount(int)
        + getLightAmount() int
    }

    class PointSpotlight {
        # focal_point: double
        # angle: double
        + setFocalPoint(double)
        + getFocalPoint() double
        + setAngle(double)
        + getAngle() double
    }

    class Torchere {
        # leg_length: int
        # light_radius: int
        + setLegLength(int)
        + getLegLength() int
        + setLightRadius(int)
        + getLightRadius() int
        + pullString()
    }

    class AdjustableTorchere {
        # max_leg_length: int
        # min_leg_length: int
        + setMaxLegLength(int)
        + getMaxLegLength() int
        + setMinLegLength(int)
        + getMinLegLength() int
        + toggleLength() int
    }

    class DiscoTorchere {
        # colors: list<string>
        + setColors(list<string>)
        + getColors() list<string>
        + changeColor()
    }

LightingDevice <|-- ElectricalDevice
LightingDevice <|-- ManualDevice
ManualDevice <|-- Lighter
ManualDevice <|-- Flare
ElectricalDevice <|-- Spotlight
Spotlight <|-- Floodlight
Spotlight <|-- PointSpotlight
ElectricalDevice <|-- Torchere
Torchere <|-- AdjustableTorchere
Torchere <|-- DiscoTorchere
```
