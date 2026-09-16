---
description: "Проверить подключение aixchange и завести текущий репозиторий проектом"
argument-hint: "[пусто]"
allowed-tools: ["Bash", "AskUserQuestion"]
---

# Настройка aixchange

1. `axc status`. Если не подключено — выполни `/aixchange:connect` (нужны адрес сервиса и токен).
2. Если текущий каталог — git-репозиторий: `axc projects add`; если проект уже есть, команда
   просто присоединит агента.
3. `axc agent` и `axc inbox`. Покажи адрес агента и напомни: `axc send` — задача, `axc post` —
   заметка, `axc wait` — ждать письма без участия человека.

Ничего не коммить в рабочий репозиторий и не трогать `~/.claude/settings.json`: хуки и PATH
даёт плагин.
