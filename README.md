# Shadowrocket RU — TOP config

| Трафик | Действие |
|--------|----------|
| Реклама / трекеры | `REJECT-DROP` |
| LAN / private | `DIRECT` |
| Заблокированное в РФ | `PROXY` |
| Российские сервисы / `.ru` / GeoIP RU | `DIRECT` |
| Остальное | `PROXY` |

Списки: [Master-Yoba](https://github.com/Master-Yoba/shadowrocket-rules) + ads из [sub-kek](https://github.com/sub-kek/shadowrocket-lists).

## Импорт (актуальная ссылка)

```
https://raw.githubusercontent.com/encipher88/shadowrocket-ru-rules/main/russia-top.conf
```

### Если на iPad «не обновляется»

1. Shadowrocket → **Конфигурация**
2. Свайп влево по старому конфигу → **Удалить** (или не используй его)
3. **+** → вставь ссылку выше / сканируй QR → Download
4. Тап по новому конфигу → **Использовать конфигурацию**
5. Дождись загрузки RULE-SET (Wi‑Fi), потом включи VPN на вкладке Home

Не жми только «обновить» у старого файла — часто остаётся кэш. Нужен **новый download**.

Репозиторий должен быть **публичным**.
