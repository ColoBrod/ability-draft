
# Инструкция

Файл `ability_draft.cfg` необходимо разместить в папке с конфигами Dota 2 (C:\Program Files (x86)\Steam\steamapps\common\dota 2 beta\game\dota\cfg).

Необходимо будет настроить скрипт. Выбрать героев, которых хотите видеть в пуле а также установить время, необходимое для размышления. 

*Примечание - Я тестировал в лобби на Локальном сервере. Рекомендую для начала делать также.*

Далее из клиента Dota 2 запускаем скрипт следующей командой:
~~~
exec ability_draft.cfg
~~~

## Настройки скрипта

Эта команда устанавливает время (здесь и далее - в секундах), которое будет у игрока в запасе чтобы подготовиться к Драфту:
~~~
dota_gamemode_ability_draft_pre_time 15
~~~
Время "на подумать" между раундами драфта (их 4):
~~~
dota_gamemode_ability_draft_pre_round_time 1;
~~~
Время, отведенное игроку, чтобы забрать способность:
~~~
dota_gamemode_ability_draft_per_player_time 1;
~~~
Вот так можно установить героя (Медузу) для сил света (Radiant):
~~~
dota_gamemode_ability_draft_set_draft_hero_and_team medusa radiant;
~~~
Устанавливаем героя для сил тьмы (Outworld Devourer):
~~~
dota_gamemode_ability_draft_set_draft_hero_and_team obsidian_destroyer dire;
~~~
А эта команда добавляет дополнительные способности в пул. Можно таких прописать 2. В нашем случае мы добавляем в пул все способности Dazzle:
~~~
dota_gamemode_ability_draft_set_draft_hero_and_team dazzle extra;
~~~
