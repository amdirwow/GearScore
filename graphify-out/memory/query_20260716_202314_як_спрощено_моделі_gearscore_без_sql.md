---
type: "query"
date: "2026-07-16T20:23:14.722793+00:00"
question: "Як спрощено моделі GearScore без SQL?"
contributor: "graphify"
source_nodes: ["GearScore_SetCharacterModel(),GearScore_DisplayUnit(),GearScore_HandleServerItemReply()"]
---

# Q: Як спрощено моделі GearScore без SQL?

## Answer

GearScore використовує стандартний PlayerModel:SetUnit лише коли персонаж має живий UnitToken. Для офлайн-запису модель приховується, але екіпірування, GearScore, раса, стать, гільдія та збережена статистика залишаються доступними. Сервер більше не надсилає model_entry, SQL cache-only creature templates видалено.

## Source Nodes

- GearScore_SetCharacterModel(),GearScore_DisplayUnit(),GearScore_HandleServerItemReply()