# gate4.ai

Страж вашего компьютера для AI-агентов: любой агент (Claude.ai, ChatGPT, Claude Code, OpenClaw, Hermes) работает с вашим браузером, файлами и сайтами только по вашим политикам — с подтверждениями, журналом с доказательствами и без доступа к паролям.

- Сайт и установка: [gate4.ai](https://gate4.ai) · [gate4.ai/install](https://gate4.ai/install) — `curl -fsSL https://gate4.ai/install.sh | sh`
- Агенту, который ставит gate4ai для вас: [gate4.ai/install.md](https://gate4.ai/install.md)
- Безопасность и проверка релизов: [SECURITY.md](https://github.com/gate4ai/gate4ai/blob/main/SECURITY.md) · [OpenSSF Scorecard](https://scorecard.dev/viewer/?uri=github.com/gate4ai/gate4ai) · [OpenSSF Best Practices](https://www.bestpractices.dev/projects/15964)
- Спецификация продукта: [docs/specification.md](https://github.com/gate4ai/gate4ai/blob/main/docs/specification.md)

| Репозиторий | Что это | Лицензия |
|---|---|---|
| [gate4ai](https://github.com/gate4ai/gate4ai) | всё в одном репозитории и одном релизе: ядро (daemon, политики, подтверждения, журнал, Vault, MCP, Web UI, встроенные Браузер и Файлы, хост коннекторов, магазин; бинарники `gate4ai` и трей `gate4ai-tray`), [SDK коннекторов](https://github.com/gate4ai/gate4ai/tree/main/sdk-go), необязательный [relay](https://github.com/gate4ai/gate4ai/tree/main/relay) (публичный HTTPS-адрес устройства без своего домена), образ `ghcr.io/gate4ai/gate4ai` | AGPL-3.0; SDK — Apache-2.0 |
| [registry](https://github.com/gate4ai/registry) | индекс магазина коннекторов | CC0 |
| [www](https://github.com/gate4ai/www) | сайт gate4.ai и установщики | — (без лицензии) |

AGPL-3.0: код открыт, доработки — тоже, в том числе когда изменённая версия работает как сервис. SDK под Apache-2.0: коннектор на нём может иметь любую лицензию, совместимую с AGPL-3.0 (так его примет магазин). Внешний вклад — [CONTRIBUTING.md](https://github.com/gate4ai/.github/blob/main/CONTRIBUTING.md) (CLA и DCO).
