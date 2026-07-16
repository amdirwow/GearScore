---
type: "query"
date: "2026-07-16T19:55:15.817653+00:00"
question: "What exactly was changed and how will offline GearScore work?"
contributor: "graphify"
source_nodes: ["GearScore_HandleServerItemReply()", "GearScore_DisplayUnit()", "GearScore_SetCharacterModel()", "GearScore_SetDisplayStats()"]
---

# Q: What exactly was changed and how will offline GearScore work?

## Answer

The addon sends a GSTMOG request and the server returns real equipment, metadata, model_entry and saved stats. GearScore_HandleServerItemReply parses these fields into the cached record; GearScore_DisplayUnit uses SetCreature for the offline race/sex model, dresses it with the returned item links, and GearScore_SetDisplayStats renders Record.Stats. character_stats snapshots become available after the character is saved or logs out.

## Source Nodes

- GearScore_HandleServerItemReply()
- GearScore_DisplayUnit()
- GearScore_SetCharacterModel()
- GearScore_SetDisplayStats()