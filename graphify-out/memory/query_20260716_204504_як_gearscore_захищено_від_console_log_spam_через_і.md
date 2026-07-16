---
type: "query"
date: "2026-07-16T20:45:04.255332+00:00"
question: "Як GearScore захищено від console log-spam через ім'я з пробілом?"
contributor: "graphify"
source_nodes: ["GearScore_IsValidServerLookupName(),GearScore_RequestServerItemData(),GearScore_SetCharacterModel()"]
---

# Q: Як GearScore захищено від console log-spam через ім'я з пробілом?

## Answer

Клієнт GearScore_IsValidServerLookupName не надсилає GSTMOG-запити з whitespace. Сервер застосовує глобальний 2-секундний throttle до розбору будь-якого GSTMOG REQ, обрізає крайні пробіли та тихо відкидає внутрішній whitespace до normalizePlayerName, тому FAILED: name contains space більше не генерується цим мостом. Напис відсутньої моделі прив'язано до координат правої області GS_DisplayFrame.

## Source Nodes

- GearScore_IsValidServerLookupName(),GearScore_RequestServerItemData(),GearScore_SetCharacterModel()