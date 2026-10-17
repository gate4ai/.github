# gate4.ai

Шлюз действий для ИИ-агентов: агент работает с вашей почтой, файлами, браузером и сервисами только по вашим политикам — с подтверждениями, журналом с доказательствами и без доступа к секретам.

| Репозиторий | Что это | Лицензия |
|---|---|---|
| [gate4ai](https://github.com/gate4ai/gate4ai) | ядро: daemon, политики, подтверждения, журнал, Vault, MCP, Web UI, WASM-хост коннекторов, магазин; бинарники `gate4ai` и трей `gate4ai-tray` | AGPL-3.0 + исключение для коннекторов |
| [sdk-go](https://github.com/gate4ai/sdk-go) | SDK коннекторов: манифест, ABI, функции хоста, тестовый хост | Apache-2.0 |
| [gate4ai-mail](https://github.com/gate4ai/gate4ai-mail), [gate4ai-files](https://github.com/gate4ai/gate4ai-files), [gate4ai-browser](https://github.com/gate4ai/gate4ai-browser), `gate4ai-*` | коннекторы (WASM-модули) | AGPL-3.0 |
| [relay](https://github.com/gate4ai/relay) | необязательный relay: публичный HTTPS-адрес устройства без своего домена | AGPL-3.0 |
| [registry](https://github.com/gate4ai/registry) | индекс магазина коннекторов | CC0 |

AGPL-3.0: код открыт, доработки — тоже, в том числе когда изменённая версия работает как сервис. Исключение в ядре разрешает коннекторам и auth-модулям, работающим через ABI, любую лицензию.
