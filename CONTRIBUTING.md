# Участие в gate4.ai

Спасибо, что помогаете. Перед pull request:

1. **Тесты.** `go vet ./... && go test ./...` (в ядре — `./scripts/ci.sh`). Решает код, а не LLM: у политик и правил безопасности — тесты на каждое правило.
2. **Секреты** не попадают в код, журнал, вывод и тесты: в тестах — фейковые сервисы.
3. **SPDX-заголовок** в каждом исходнике (`// SPDX-License-Identifier: …`), лицензия — по каталогу (в gate4ai проверяет `scripts/spdx.sh`).

## Лицензии и права на вклад

| Репозиторий / каталог | Лицензия |
|---|---|
| gate4ai (ядро, relay, `connectors/`, `e2e/`) | AGPL-3.0-only |
| gate4ai, каталог `sdk-go/` | Apache-2.0 |
| registry | CC0 |

Вклад во все репозитории принимается с **CLA** (подписывается один раз через CLA Assistant в первом pull request: лицензиар сохраняет право выпускать версии и под другой лицензией) и **DCO** (`git commit -s` — `Signed-off-by` в каждом коммите).

## Новый коннектор

Свой репозиторий `gate4ai-<сервис>` на [sdk-go](https://github.com/gate4ai/gate4ai/tree/main/sdk-go) (`require github.com/gate4ai/gate4ai`; заготовка — `gate4ai connectors new`): манифест с минимальными возможностями (`capabilities`), тесты на тестовом хосте, релиз по тегу — workflow из [CONTRIBUTING registry](https://github.com/gate4ai/registry/blob/main/CONTRIBUTING.md). Для магазина — pull request в [registry](https://github.com/gate4ai/registry). Действия класса `money` проверяются другим коннектором (выписка), а не самим собой.
