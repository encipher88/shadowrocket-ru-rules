# Shadowrocket RU rules

Полные списки правил для Shadowrocket: **РФ → DIRECT**, **заблокированное и зарубежное → PROXY**.

Все `.list` лежат в этом репозитории (`rules/`). Конфиг ссылается только на `raw.githubusercontent.com/encipher88/...`.

## Импорт в Shadowrocket

1. Открой ссылку:
   ```
   https://raw.githubusercontent.com/encipher88/shadowrocket-ru-rules/main/russia.conf
   ```
2. Shadowrocket → **Конфигурация** → **+** → вставь URL → Download
3. Выбери конфиг → **Использовать конфигурацию**
4. На вкладке **Домой** добавь свой прокси и включи VPN

Или скопируй содержимое `russia.conf` как текстовый конфиг.

## Состав

| Файл | Назначение |
|------|------------|
| `russia.conf` | Главный конфиг |
| `rules/geoip-private.list` | LAN / private → DIRECT |
| `rules/geosite-ru-blocked.list` | Заблокированные домены → PROXY |
| `rules/geoip-ru-blocked.list` | Заблокированные IP → PROXY |
| `rules/geosite-category-ru.list` | Российские сервисы → DIRECT |
| `rules/geoip-ru.list` | Российские IP → DIRECT |

Исходные данные сгенерированы из публичных GeoIP/GeoSite (runetfreedom → формат Shadowrocket). Здесь хранится **полный снимок**, без зависимости от чужих raw-URL в рантайме.

## Обновление списков

Перекачай актуальные `.list` в `rules/` и закоммить, либо обнови вручную нужные домены правилами выше `FINAL,PROXY`.
