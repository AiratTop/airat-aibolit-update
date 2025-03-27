# airat-aibolit-update
Скрипт для быстрой установки и/или обновления [ai-bolit](https://revisium.com/ai/) от Айрата Халитова

**ВАЖНО:** 
Сайт разработчиков ai-bolit https://revisium.com/ai теперь недоступен, поэтому официальных обновлений больше нет.
В архиве лежит последняя доступная версия.

Т.к. разработчики забросили этот скрипт, он не будет находить новые актуальные уязвимости, которые придумали после последнего обновления скрипта. (_Если только мы сами не начнем его обновлять и поддерживать_)

## Установка и запуск:
```bash
git clone https://github.com/AiratTop/airat-aibolit-update

cd airat-aibolit-update

cd ai-bolit

./run-aibolit.sh
```

**Примечания:** 
- Свои файлы для сканирования нужно копировать в папку `ai-bolit`, а уже потом запускать в ней скрипт `./run-aibolit.sh`
- Скрипт `./run-aibolit.sh` запускает по очереди два режима сканирования: обычный (`--mode=1`) и параноидальный (`--mode=2`)
- При сканировании файлы должны быть доступны для скрипта. Надежнее запускать с правами рута
- В параноидальном режиме возможны ложные срабатывания, т.к. он более чувствительный
- Инструкция по использованию описана в файле `readme.txt`, история изменений в файле `CHANGELOG.md`
