**Участники команды:**
Тупенко Евгений, Романович Владислав, Сазонов Сергей

---

## 1. Стиль кодирования
### a. Форматирование
- **Отступы:** 4 пробела (без табов)  
  Единый стандарт повышает читаемость и предотвращает конфликты в редакторах
- **Имена переменных:** camelCase (пример: `yetAnotherLet`)  
  Соответствует общепринятым практикам JavaScript/TypeScript
- **Классы/функции:** PascalCase (пример: `class UserService`)  
  Быстрое визуальное разделение конструкций от переменных
- **Типы/интерфейсы:** Префикс T для типов (`TButton`), I для интерфейсов (`IButton`)  
  Четкое различие между типами и обычными объектами
- **Пустые строки:** 1-2 строки между функциональными блоками  
  Улучшает визуальную навигацию по коду
- **Скобки:**
  ```
  if (condition) {
    // ...
  }
  ```
  Единый стиль снижает когнитивную нагрузку при ревью
- **Комментарии:** На русском языке  
  Все члены команды — носители русского языка

---

## 2. Инструменты форматирования
### b. Prettier
Конфигурация: `tabWidth=4, useTabs=false, printWidth=80`
Автоматическое применение правил форматирования экономит время

### e. ESLint
Базовый конфиг  
Стандартные правила для контроля качества кода

---

## 3. Работа с Git
### c. Ветки и коммиты
- **Именование веток:** `[действие]/[краткое-описание-задачи]` (пример: fix/modal-window)  
  Понятное назначение ветки без перегрузки названия
- **Коммиты:** По Conventional Commits (пример: feat: add login button)  
  Автоматизация генерации changelog и семантического версионирования

---

## 4. Процесс ревью
### d. Правила ревью
- 1 апрув (профильный разработчик) + успешные тесты/линтеры  
  Гарантирует качество и минимизирует риски багов

---

## 5. Инфраструктура
### e. Линтеры/форматтеры
Обязательное использование ESLint + Prettier  
Единый стиль кода и автоматическое исправление ошибок

---

## 6. Работа с багами и релизами
### f. Релизный цикл
- Фичи: Тестовый сервер → тестирование командой → прод
- Если бага на тестовом сервере то делаем фикс и теструем по новой
- Хотфиксы:  
  - Деплой в обход проверок  
- Не критические баги: Полный пайплайн  
Баланс между скоростью реакции на инциденты и стабильностью

### g. "Готовый" код
Протестирован, отревьювен, прошёл линтеры/тесты, не имеет известных багов, соответствует критериям по тз таски
Минимизация технического долга и ошибок в проде

---

## 7. Таск-менеджмент
### h. Организация задач (Notion)
- **Статусы:**  
  `Открыта → В работе → На ревью → Тестируется → Сделано`
- **Теги:**  
  - Приоритет: низкий, средний, высокий, критический  
  - Направления: frontend, backend, dev-ops, android, ios, testing  
Прозрачность приоритетов и распределения задач по специализациям
