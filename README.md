# 🎨 Photoshop Scripts by Maestr.o

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Photoshop](https://img.shields.io/badge/Photoshop-2023+-ff00ff)
![Status](https://img.shields.io/badge/status-active-success)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow)

> Мощная сборка JSX/ExtendScript скриптов для автоматизации Adobe Photoshop. Идеально для ретушеров, фотографов и дизайнеров.

[![Skills](https://skillicons.dev/icons?i=js,ps&theme=dark&perline=2)](https://skillicons.dev)

---

## 📚 Содержание

- [Особенности](#-особенности)
- [Скрипты](#-скрипты)
- [Установка](#-установка)
- [Использование](#-использование)
- [Примеры](#-примеры)
- [Требования](#-требования)
- [Лицензия](#-лицензия)
- [Контакты](#-контакты)

---

## ✨ Особенности

- 🚀 **Готовые к использованию** — просто скопируй и работай
- 🎯 **Профессиональные инструменты** — написаны для реальных задач
- 🛡️ **Безопасные операции** — не разрушают оригинальные данные
- ⚡ **Пакетная обработка** — обработай сотни файлов автоматически
- 📱 **Кроссплатформенные** — работают на Mac и Windows
- 🌐 **Поддержка многих версий** — совместимы с PS CC 2020+

---

## 📁 Скрипты

| Скрипт | Описание | Назначение | Версия PS |
|--------|---------|-----------|----------|
| **Smart_Path_Crop** | Пакетный кроп по clipping path к стандартным размерам | Подготовка товарных фото | CS6+ |
| **Layer_Cleanup** | Удаление пустых и невидимых слоёв | Очистка документа | CC 2020+ |
| **PathTransfer** | Перенос путей из TIF в JPG по названию файла | Batch-обработка путей | CS6+ |
| **DocInfo Engine** | Добавляет текстовый слой с техническими параметрами | Информация о документе | CC 2020+ |
| **Document Info Extractor v2** | Продвинутая версия с авто-масштабом | Профессиональная версия | CC 2022+ |
| **Stack in PSD** | Разворот слоёв + сохранение в PSD | Массовая переработка | CS6+ |

---

## 🚀 Установка

### На macOS

```bash
# Клонируй репо
git clone https://github.com/TheMaestr-o/Photoshop-Scripts.git

# Копируй скрипты в Photoshop
cp -r *.jsx ~/Library/Application\ Support/Adobe/Adobe\ Photoshop\ [VERSION]/Presets/Scripts/
```

**Путь для разных версий:**
- Photoshop 2025: `~/Library/Application Support/Adobe/Adobe Photoshop 2025/Presets/Scripts/`
- Photoshop 2024: `~/Library/Application Support/Adobe/Adobe Photoshop 2024/Presets/Scripts/`
- Photoshop 2023: `~/Library/Application Support/Adobe/Adobe Photoshop 2023/Presets/Scripts/`

### На Windows

```bash
# Клонируй репо
git clone https://github.com/TheMaestr-o/Photoshop-Scripts.git

# Копируй скрипты в Photoshop
copy *.jsx "C:\Program Files\Adobe\Adobe Photoshop [VERSION]\Presets\Scripts\"
```

**Пути для Windows:**
- Photoshop 2025: `C:\Program Files\Adobe\Adobe Photoshop 2025\Presets\Scripts\`
- Photoshop 2024: `C:\Program Files\Adobe\Adobe Photoshop 2024\Presets\Scripts\`

### Быстрая установка

1. **Скачай** файлы скриптов
2. **Открой** Adobe Photoshop
3. **Перейди** в `File → Scripts → Browse...`
4. **Выбери** скрипт
5. **Готово!** ✅

---

## 💻 Использование

### Способ 1: Через меню Photoshop (рекомендуется)

```
File → Scripts → Other Scripts → выбери скрипт
```

### Способ 2: Через панель Scripts

1. Открой панель **Scripts** (Window → Scripts)
2. Найди нужный скрипт
3. Двойной клик для запуска

### Способ 3: Через консоль ExtendScript

```javascript
#include "/path/to/Smart_Path_Crop.jsx"
main();
```

---

## 🎬 Примеры

### Smart_Path_Crop — Пакетный кроп

**Что делает:**
- 📸 Автоматически находит clipping path ("Path 1")
- ✂️ Кропит изображение по пути
- 📐 Добавляет отступ 100px (настраивается)
- 🎯 Расширяет canvas к стандартному размеру:
  - 1181×1181 px
  - 1417×1417 px
  - 2362×2362 px

**[🎥 Смотри GIF примера обработки]**

**Пример расчёта:**
```
Размер объекта: 1100px
+ Отступ: 200px (100px × 2)
= Требуется: 1300px

Результат → выбирает 1417×1417 px canvas
```

---

### Layer_Cleanup — Очистка слоёв

**Что делает:**
- 🗑️ Удаляет пустые слои
- 👁️ Удаляет невидимые слои
- 🔒 Безопасно работает с заблокированными слоями
- 📦 Удаляет пустые группы слоёв
- 💾 Опционально сохраняет Layer Compositions

**[🎥 Смотри GIF примера очистки]**

---

### DocInfo Engine — Информация о документе

**Что добавляет:**
- 📊 Размер (px, cm, inch)
- 📏 Разрешение (PPI, PPCM)
- 🎨 Цветовой профиль и режим
- 📈 Мегапиксели
- 📐 Соотношение сторон (дробь Фарея)

**Пример вывода:**
```
Document: photo.psd
Dimensions: 4000 × 3000 px (40 × 30 cm)
Resolution: 300 PPI
Color Mode: RGB, 16-bit
Megapixels: 12 MP
Aspect Ratio: 4:3
```

---

### PathTransfer — Перенос путей

**Что делает:**
- 🔄 Находит файлы TIF и JPG с одинаковыми названиями
- ✨ Копирует все пути из TIF в JPG
- 💾 Сохраняет JPG с путями
- ⚙️ Автоматическая пакетная обработка

**[🎥 Смотри GIF примера переноса путей]**

---

### Stack in PSD — Разворот слоёв

**Что делает:**
- 🔄 Разворачивает стек слоёв (снизу вверх)
- 💾 Сохраняет в PSD на Desktop
- 👁️ Показывает только нижний слой
- 🏷️ Называет файл по нижнему слою

---

## 📋 Требования

| Параметр | Значение |
|----------|----------|
| **ОС** | macOS 10.14+ / Windows 10+ |
| **Photoshop** | CC 2020+ (большинство работают с CS6+) |
| **Язык** | ExtendScript (встроен в Photoshop) |
| **Зависимости** | Нет — полностью standalone |

### Версионность скриптов

| Скрипт | CS6 | CC 2015 | CC 2020 | CC 2024 | CC 2025 |
|--------|-----|--------|--------|---------|---------|
| Smart_Path_Crop | ✅ | ✅ | ✅ | ✅ | ✅ |
| Layer_Cleanup | ✅ | ✅ | ✅ | ✅ | ✅ |
| PathTransfer | ✅ | ✅ | ✅ | ✅ | ✅ |
| DocInfo Engine | ❌ | ⚠️ | ✅ | ✅ | ✅ |
| Document Info v2 | ❌ | ❌ | ⚠️ | ✅ | ✅ |
| Stack in PSD | ✅ | ✅ | ✅ | ✅ | ✅ |

---

## 🤔 FAQ

**Q: Скрипт не появляется в меню Photoshop**
```
A: Проверь путь установки для своей версии PS (см. выше)
   Перезагрузи Photoshop
   Убедись что файл имеет расширение .jsx
```

**Q: "DocInfo Engine" не имеет расширения**
```
A: Переименуй в "DocInfo Engine.jsx" вручную
```

**Q: Как запустить скрипт на пакете файлов?**
```
A: Используй меню File → Automate → Batch
   или запусти скрипт вручную для каждого файла
```

**Q: Скрипт медленно работает**
```
A: Это нормально для пакетной обработки
   Оптимизируй размеры изображений перед обработкой
```

---

## 🔗 Полезные ссылки

- 📚 [Adobe ExtendScript Documentation](https://github.com/Adobe-CEP/CEP-Resources)
- 🛠️ [Photoshop Scripting Guide](https://www.adobe.io/apis/creativecloud/photoshop.html)
- 💡 [ExtendScript Toolkit](https://www.adobe.com/products/extendscript.html)
- 🌐 [Adobe Developers Forum](https://forums.adobe.com/community/en/groups/adobe-dev)

---

## 📝 Лицензия

MIT License — свободное использование в личных и коммерческих проектах

```
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND
```

Подробнее — см. файл [LICENSE](LICENSE)

---

## 👤 Контакты и поддержка

[![Email](https://custom-icon-badges.demolab.com/badge/Email-EA4335.svg?logo=gmail&logoColor=white)](mailto:gssdarm@gmail.com)
[![GitHub](https://custom-icon-badges.demolab.com/badge/GitHub-black.svg?logo=github&logoColor=white)](https://github.com/TheMaestr-o)
[![Telegram](https://custom-icon-badges.demolab.com/badge/Telegram-0088cc.svg?logo=telegram&logoColor=white)](https://t.me/ohnedan)
[![Website](https://custom-icon-badges.demolab.com/badge/Portfolio-6B00FF.svg?logo=globe&logoColor=white)](https://example.com)

**Email:** gssdarm@gmail.com  
**Telegram:** [@ohnedan](https://t.me/ohnedan)

---

## 🎯 Что дальше?

- ⭐ Поставь звезду если нравится репо
- 🔔 Следи за обновлениями
- 🐛 Найденные баги можешь репортить в [Issues](https://github.com/TheMaestr-o/Photoshop-Scripts/issues)
- 💬 Вопросы и идеи приветствуются

---

<div align="center">

**Made with ❤️ for Adobe Photoshop community**

Последнее обновление: июнь 2026

</div>
