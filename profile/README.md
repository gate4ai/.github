# gate4.ai

Шлюз действий для ИИ-агентов: агент работает с вашей почтой, файлами, браузером и сервисами только по вашим политикам — с подтверждениями, журналом с доказательствами и без доступа к секретам.

| Репозиторий | Что это | Лицензия |
|---|---|---|
| [gate4ai](https://github.com/gate4ai/gate4ai) | ядро: daemon, политики, подтверждения, журнал, Vault, MCP, Web UI, WASM-хост коннекторов, магазин; бинарник `gate4ai` | FSL-1.1-ALv2 |
| [sdk-go](https://github.com/gate4ai/sdk-go) | SDK коннекторов: манифест, ABI, функции хоста, тестовый хост | Apache-2.0 |
| [gate4ai-mail](https://github.com/gate4ai/gate4ai-mail), [gate4ai-files](https://github.com/gate4ai/gate4ai-files), [gate4ai-browser](https://github.com/gate4ai/gate4ai-browser), `gate4ai-*` | коннекторы (WASM-модули) | AGPL-3.0 + исключение для хоста |
| [relay](https://github.com/gate4ai/relay) | необязательный relay: публичный HTTPS-адрес устройства без своего домена | FSL-1.1-ALv2 |
| [tray](https://github.com/gate4ai/tray) | трей (Tauri) | FSL-1.1-ALv2 |
| [registry](https://github.com/gate4ai/registry) | индекс магазина коннекторов | CC0 |

FSL-1.1-ALv2: исходник открыт, запрещено только конкурирующее использование; каждая версия через два года становится Apache-2.0.
