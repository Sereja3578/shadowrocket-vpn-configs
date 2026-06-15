# Shadowrocket VPN Configs

Публичные example-конфиги Shadowrocket, приближенные к общей routing-логике Clash/Stash.

## Что внутри

- `sr_nonru_basic.example.conf` - Abroad-профиль: российские сервисы идут через `RU-PROXY`, глобальные сервисы остаются `DIRECT` или используют отдельную foreign proxy-группу.
- `sr_ru_geo.example.conf` - Russia-профиль: российские сервисы идут `DIRECT`, иностранные ограниченные сервисы идут через `PROXY` / `LOW-RESTRICT-FOREIGN`.

## Как использовать

1. Скопируйте нужный `*.example.conf` в рабочий Shadowrocket config.
2. Подключите свою подписку/серверы в Shadowrocket.
3. Настройте proxy-группы под имена и фильтры своих нод.
4. Проверьте работу ключевых приложений через Shadowrocket logs.

## Безопасность

Реальные `.conf`, базы Shadowrocket и локальные server IDs не отслеживаются Git. В публичный репозиторий попадают только переносимые examples.
