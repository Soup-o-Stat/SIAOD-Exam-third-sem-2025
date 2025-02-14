# Файлы

## Файл как структура данных

**Файл** — это структура данных, предназначенная для долговременного хранения информации на носителе. 

### Основные характеристики файлов:
1. **Линейная организация данных** — данные записываются в последовательности.
2. **Формат хранения** — текстовый или двоичный.
3. **Доступ к данным**:
   - **Последовательный**: данные читаются или записываются в порядке их расположения.
   - **Прямой (произвольный)**: доступ к данным осуществляется по их индексу или смещению.

---

## Текстовый файл

**Текстовый файл** — это файл, содержащий данные в виде последовательности символов, понятных человеку и системе (ASCII, Unicode). 

### Особенности:
- Представляет данные в виде строк.
- Использует разделители строк (\n, \r\n).
- Размер файла больше, так как данные хранятся в текстовом виде.

### Пример использования:
- Хранение конфигураций, логов, скриптов и других данных, удобных для редактирования вручную.

---

## Двоичный файл

**Двоичный файл** — это файл, в котором данные хранятся в виде набора байтов (0 и 1). 

### Особенности:
- Хранит данные в сжатом формате, занимающем меньше места.
- Не читается человеком напрямую без специальных инструментов.
- Быстрее обрабатывается программами.

### Пример использования:
- Хранение изображений, видео, аудио, числовых данных, сериализованных объектов.

---

## Объем памяти под числовое значение 0 в двоичном файле

Объем памяти зависит от типа данных:
- **Целые числа (integer)**:
  - 1 байт: для типа `int8` (диапазон -128 до 127).
  - 4 байта: для типа `int32` (диапазон -2,147,483,648 до 2,147,483,647).
- **Числа с плавающей запятой (float, double)**:
  - 4 байта: для типа `float`.
  - 8 байт: для типа `double`.

---

## Структурированный протокол

**Структурированный протокол** — это способ организации данных в файле, обеспечивающий:
1. **Читаемость**: четко определённые поля и их структура.
2. **Обработку**: возможность извлекать, изменять или добавлять данные.

### Примеры структурированных протоколов:
- **JSON**: текстовый формат для передачи данных (читаем человеком).
- **XML**: текстовый формат с тегами для хранения данных.
- **Protocol Buffers (Protobuf)**: бинарный формат, оптимизированный для скорости и размера.
- **Avro** и **Thrift**: бинарные форматы для сериализации данных.

### Применение:
- Хранение данных в структурированном виде для передачи между приложениями или их долговременного хранения.
