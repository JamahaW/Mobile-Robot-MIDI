# Описание проекта: Mobile-Robot-MIDI

## Обзор

Проект **Mobile-Robot-MIDI** посвящен разработке мобильных роботов среднего размера (MIDI - от английского "Medium"), которые могут быть использованы в различных приложениях, включая образовательные и исследовательские. 
Этот проект объединяет 3D-моделирование, 3D-печать и лазерную резку для создания модульных роботов, которые легко адаптируются под различные задачи.

## Цели проекта

- Создание универсальной платформы для разработки мобильных роботов среднего размера, способных выполнять разнообразные функции.
- Обеспечение доступности и простоты в производстве компонентов роботов через 3D-печать и лазерную резку.
- Разработка модульной архитектуры, позволяющей легко адаптировать и расширять функциональность роботов.

## Репозиторий содержит

- **3D-модели**: Все необходимые модели для сборки роботов.
- **Файлы для печати**: GCODE, STP, STL и DFX файлы для 3D-печати и лазерной резки.
- ~~**Код, ПО, Скетчи**~~: В процессе разработки (WIP).

## Структура проекта

Проект организован в несколько ключевых разделов:

- **[Модели](./Модели)**: Содержит файлы моделей деталей и сборок, созданные в Компас 3D v23.
  - **[Комплектующие](./Модели/Комплектующие)**: Модели исходных деталей.
  - **[Модули](./Модели/Модули)**: Самодостаточные сборочные единицы, следуя [Правилам создания модулей](#правила-проектирования-модулей).
  - **[Шасси](./Модели/Шасси)**: Сборочные единицы шасси мобильной платформы.
  - **[Фрагменты и заготовки](./Модели/Фрагменты%20и%20Заготовки)**: Общие детали и фрагменты.
  - **`[WIP]` [Конструктор](./Модели/Конструктор)**: Детали конструктора.
  - **`[WIP]` [Сборки роботов](./Модели/Сборки%20роботов)**: Сборки роботов на основе шасси.
- **[Печать](./Печать)**: STP и STL файлы для нарезки.
- **[Печать/Нарезка](./Печать/Нарезка)**: Gcode файлы для 3D-печати.
- **[Резка](./Резка)**: DFX файлы для лазерной резки.
- **[Поля](./Поля)**: Фрагменты и готовые поля для заданий.
- **[Изображения](./Изображения)**: Иллюстрации и визуальные материалы.

---

## Правила проектирования модулей

1. Каждый модуль должен находиться в отдельном каталоге внутри директории [Модули](./Модели/Модули).
2. Наименование модуля, каталога и файла сборки должно совпадать, быть кратким и соответствовать ЕСКД.
3. Все файлы модуля размещаются в его каталоге.
4. Модуль представляет собой сборочную единицу формата `.a3d`, которая может ссылаться на другие модули или [Фрагменты и заготовки](./Модели/Фрагменты%20и%20Заготовки).
5. Детали модуля должны быть разработаны для простого изготовления (FFF 3D-печать, лазерная резка).
6. Рекомендуется проектировать модуль так, чтобы его можно было переиспользовать.

---

## Правила проектирования шасси

1. Шасси представляют собой сборочную единицу, включающую в себя [Модули](./Модели/Модули) или [Комплектующие](./Модели/Комплектующие) или другое [Шасси](./Модели/Шасси) (если это дополнение).
2. Каждое шасси имеет свою отдельную папку.
3. Детали для сборки шасси располагаются в его каталоге.
4. Детали шасси должны быть разработаны для простого изготовления (FFF 3D-печать, лазерная резка).
5. Наименование шасси, каталога и файла сборки должно совпадать, быть кратким и соответствовать ЕСКД.
6. Шасси должно обеспечивать надежное соединение с модулями и комплектующими
7. Рекомендуется проектировать шасси так, чтобы оно обеспечивало легкий доступ к внутренним компонентам для обслуживания и модификации.
8. Шасси должно быть спроектировано с учетом устойчивости и прочности, чтобы выдерживать нагрузки и воздействия в процессе эксплуатации.
9. При проектировании шасси следует учитывать возможность установки дополнительных модулей и аксессуаров, что позволит расширить функциональность робота в будущем.

---

## Заключение

Проект **Mobile-Robot-MIDI** предлагает уникальную возможность для разработчиков и энтузиастов в области робототехники. С помощью модульного подхода и доступных технологий 3D-печати и лазерной резки, пользователи смогут создавать свои собственные мобильные роботы среднего размера, которые могут выполнять разнообразные задачи в различных сферах.