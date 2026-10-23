# Shadowrocket RU — TOP config

Маршрутизация для РФ:

| Трафик | Действие |
|--------|----------|
| Реклама / трекеры | `REJECT-DROP` |
| LAN / private | `DIRECT` |
| Заблокированное в РФ | `PROXY` |
| Российские сервисы / `.ru` / GeoIP RU | `DIRECT` |
| Остальное | `PROXY` |

**Источники списков (обновляются ежедневно у авторов):**
- [Master-Yoba/shadowrocket-rules](https://github.com/Master-Yoba/shadowrocket-rules) — ru-blocked, category-ru, geoip-ru
- [sub-kek/shadowrocket-lists](https://github.com/sub-kek/shadowrocket-lists) — category-ads-all

## Импорт в Shadowrocket

```
https://raw.githubusercontent.com/encipher88/shadowrocket-ru-rules/main/russia.conf
```

Config → `+` → URL → Download → Use Config → на Home выбери свой прокси.

Репозиторий должен быть **публичным**.
