---
type: "query"
date: "2026-07-16T19:49:15.769365+00:00"
question: "How does offline gear response populate the GearScore model and stats?"
contributor: "graphify"
source_nodes: ["GearScore_HandleServerItemReply()", "GearScore_DisplayUnit()", "GearScore_SetCharacterModel()", "GearScore_SetDisplayStats()"]
---

# Q: How does offline gear response populate the GearScore model and stats?

## Answer

GearScore_HandleServerItemReply parses server metadata and STATS into the cached record. GearScore_DisplayUnit passes that record to GearScore_SetCharacterModel, while GearScore_SetDisplayStats reads Record.Stats. Therefore offline model and stats require those fields to be present in the server reply.

## Source Nodes

- GearScore_HandleServerItemReply()
- GearScore_DisplayUnit()
- GearScore_SetCharacterModel()
- GearScore_SetDisplayStats()