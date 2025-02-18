# Contributing Guidelines

## Виды участия в роадмапе
- 💡 [Создавайте issue](https://github.com/tlbootcamp/tlroadmap/issues/new), если вы видите, что мы не хватили какую-то область ответственности тимлида, где-то ошиблись или у вас просто есть отличная идея для обсуждения.
- 🚫 [Присылайте Pull Request](https://github.com/tlbootcamp/tlroadmap/compare) с исправлением фактических ошибок.
- 📚 [Дорабатывайте базу знаний](https://github.com/tlbootcamp/tlroadmap/issues?q=is%3Aissue+is%3Aopen+label%3Aknowledge-base) – как новые ветки, так и отдельные секции в уже готовых (например, "Как прокачать", "Примеры поведения" или "Список литературы").
- 👨🏻‍💻 [Присылайте модели тимлидов своих компаний](https://github.com/tlbootcamp/tlroadmap/compare) – мы их добавим в раздел с примерами.

Если вы не знаете, чем конкретно хотите заняться, то можете пробежаться по нашим Issues – их очень много на любой вкус.

### Описание веток роадмапа
Если вы готовы взять в работу описание одной из веток, пройдитесь по нашему чек-листу:
1. Проверьте, что на [доске проекта](https://github.com/tlbootcamp/tlroadmap/projects/1) в колонке "In progress" эта задача отсутствует, иначе вы рсикуете проделать двойную работу.
2. Найдите соответствующий тикет [с лейблом `knowledge-base`](https://github.com/tlbootcamp/tlroadmap/issues?q=is%3Aissue+is%3Aopen+label%3Aknowledge-base) в Issues и заассайньте его на себя. На доске проекта передвиньте в статус "In progress".
3. Создайте новый файл описания в `/skills/role` с использованием [шаблона описания](https://github.com/tlbootcamp/tlroadmap/blob/master/skills/template.md).
4. Заполните столько секций, сколько вы готовы.
5. Добавьте ссылку на новое описание в файле `links.json`, который использует генератор.
6. [Пришлите PR](https://github.com/tlbootcamp/tlroadmap/compare).

## Процесс принятия изменений
*In progress*

## Технические детали
Для всех изменений структуры источником правды является файл `roadmap.mm`. Для того, чтобы обновить его структуру или содержание, выполните следующие шаги:
1. Внесите изменение в `roadmap.mm` с помощью [Freemind](https://sourceforge.net/projects/freemind/) и сохраните файл.
2. Экспортируйте `roadmap.mm` в `png` со 100% масштабом через Freemind.
3. Запустите скрипт `python3 tools/gen_roadmap_contents.py` для автоматического обновления базы знаний.