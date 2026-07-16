---
type: "query"
date: "2026-07-16T20:17:34.542835+00:00"
question: "Як виправлено cooldown, guild tab та білі офлайн-моделі GearScore?"
contributor: "graphify"
source_nodes: ["GearScore_RequestServerItemData(),GearScore_PumpServerItemRequests(),GearScore_ShouldWaitForServerRecord(),GearScore_BuildDatabase(),GearScore_SetCharacterModel()"]
---

# Q: Як виправлено cooldown, guild tab та білі офлайн-моделі GearScore?

## Answer

Клієнтська черга GearScore_PumpServerItemRequests узгоджена з глобальним серверним throttle: максимум один запит на 2 секунди, запит під час cooldown не губиться, а профіль показує Завантаження до відповіді. Guild tab тепер бере членство лише з актуального guild roster, case-insensitive, і оновлює кешовану назву гільдії. Білі моделі були спричинені raw player display ID без CreatureDisplayInfoExtra; cache-only creature templates переведені на текстуровані NPC display ID тієї самої race/sex.

## Source Nodes

- GearScore_RequestServerItemData(),GearScore_PumpServerItemRequests(),GearScore_ShouldWaitForServerRecord(),GearScore_BuildDatabase(),GearScore_SetCharacterModel()