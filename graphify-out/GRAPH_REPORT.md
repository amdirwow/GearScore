# Graph Report - GearScore  (2026-07-16)

## Corpus Check
- 54 files · ~100,297 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 509 nodes · 865 edges · 56 communities (53 shown, 3 thin omitted)
- Extraction: 97% EXTRACTED · 3% INFERRED · 0% AMBIGUOUS · INFERRED: 28 edges (avg confidence: 0.81)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `feeedf21`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- [[_COMMUNITY_Community 0|Community 0]]
- [[_COMMUNITY_Community 1|Community 1]]
- [[_COMMUNITY_Community 2|Community 2]]
- [[_COMMUNITY_Community 3|Community 3]]
- [[_COMMUNITY_Community 4|Community 4]]
- [[_COMMUNITY_Community 5|Community 5]]
- [[_COMMUNITY_Community 6|Community 6]]
- [[_COMMUNITY_Community 7|Community 7]]
- [[_COMMUNITY_Community 9|Community 9]]
- [[_COMMUNITY_Community 10|Community 10]]
- [[_COMMUNITY_Community 11|Community 11]]
- [[_COMMUNITY_Community 12|Community 12]]
- [[_COMMUNITY_Community 13|Community 13]]
- [[_COMMUNITY_Community 14|Community 14]]
- [[_COMMUNITY_Community 17|Community 17]]
- [[_COMMUNITY_Community 18|Community 18]]
- [[_COMMUNITY_Community 19|Community 19]]
- [[_COMMUNITY_Community 20|Community 20]]
- [[_COMMUNITY_Community 21|Community 21]]
- [[_COMMUNITY_Community 22|Community 22]]
- [[_COMMUNITY_Community 23|Community 23]]
- [[_COMMUNITY_Community 24|Community 24]]
- [[_COMMUNITY_Community 25|Community 25]]
- [[_COMMUNITY_Community 26|Community 26]]
- [[_COMMUNITY_Community 27|Community 27]]
- [[_COMMUNITY_Community 28|Community 28]]
- [[_COMMUNITY_Community 29|Community 29]]
- [[_COMMUNITY_Community 30|Community 30]]
- [[_COMMUNITY_Community 31|Community 31]]
- [[_COMMUNITY_Community 32|Community 32]]

## God Nodes (most connected - your core abstractions)
1. `GearScore_DisplayUnit()` - 25 edges
2. `GearScore_TransmogSetDebug()` - 21 edges
3. `GearScore_OnEvent()` - 20 edges
4. `GearScore_FixRecordItemTooltip()` - 16 edges
5. `GearScore_DisplayDatabase()` - 16 edges
6. `GearScore_RequestServerItemData()` - 15 edges
7. `GearScore_HandleServerItemReply()` - 15 edges
8. `GearScore_PatchVisibleSocketBonus()` - 14 edges
9. `GearScore_GetQuality()` - 14 edges
10. `GearScore_GetTooltipFrame()` - 13 edges

## Surprising Connections (you probably didn't know these)
- `GearScore_OnEvent()` --calls--> `print()`  [INFERRED]
  GearScore/GearScore.lua → BonusScanner/libs/LibTipHooker-1.1/LibTipHooker-1.1.lua
- `GS_TmogSetDump()` --calls--> `print()`  [INFERRED]
  GearScore/GearScore.lua → BonusScanner/libs/LibTipHooker-1.1/LibTipHooker-1.1.lua
- `GS_BANSET()` --calls--> `print()`  [INFERRED]
  GearScore/GearScore.lua → BonusScanner/libs/LibTipHooker-1.1/LibTipHooker-1.1.lua
- `GS_MANSET()` --calls--> `print()`  [INFERRED]
  GearScore/GearScore.lua → BonusScanner/libs/LibTipHooker-1.1/LibTipHooker-1.1.lua
- `ClassicGearScoreCalculations()` --calls--> `print()`  [INFERRED]
  GearScore/weights.lua → BonusScanner/libs/LibTipHooker-1.1/LibTipHooker-1.1.lua

## Communities (56 total, 3 thin omitted)

### Community 0 - "Community 0"
Cohesion: 0.07
Nodes (70): GearScore_AddRealSetBlock(), GearScore_AddVisibleSetRowsByServerSignature(), GearScore_CleanTooltipText(), GearScore_DecodeServerSetText(), GearScore_EquipCodesMatch(), GearScore_EquipCompare(), GearScore_FindServerSetRow(), GearScore_FindSocketInsertLine() (+62 more)

### Community 1 - "Community 1"
Cohesion: 0.06
Nodes (38): AcquireCell(), AcquireFrame(), AcquireTable(), AcquireTooltip(), checkFont(), checkJustification(), ClearFrameScripts(), CreateLine() (+30 more)

### Community 2 - "Community 2"
Cohesion: 0.06
Nodes (4): BonusScanner:GetGemSum(), BonusScanner:ScanUnitInventory(), ClassColorise(), ScanTooltipGem()

### Community 3 - "Community 3"
Cohesion: 0.1
Nodes (34): GearScoreLDB:Initialize(), GearScoreLDB:OnClick(), GearScore_AttachServerSetMembers(), GearScore_BuildRecordFromItemCodes(), GearScore_CalculateEquipScoreFromCodes(), GearScore_ComposeRecord(), GearScore_DisplayUnit(), GearScore_GetAge() (+26 more)

### Community 4 - "Community 4"
Cohesion: 0.08
Nodes (22): GearScore_ContinueExchange(), GearScore_Exchange(), GearScore_GetGroupScores(), GearScore_GetQuality(), GearScore_HookSetUnit(), GearScore_OnUpdate(), GearScore_SendReport(), GearScore_SetDetails() (+14 more)

### Community 5 - "Community 5"
Cohesion: 0.07
Nodes (7): AceAddon:DisableAddon(), AceAddon:EnableAddon(), AceAddon:InitializeAddon(), AceAddon:NewAddon(), Embed(), NewModule(), safecall()

### Community 6 - "Community 6"
Cohesion: 0.1
Nodes (18): addBits(), addCode(), cleanup(), decode(), encode(), escape_code(), escape_for_gsub(), getCode() (+10 more)

### Community 7 - "Community 7"
Cohesion: 0.18
Nodes (21): GearScore_BuildDatabase(), GearScore_DatabaseOnClick(), GearScore_DisplayDatabase(), GearScore_GetDate(), GearScore_GetRecordClassColors(), GearScore_GetRecordDisplayClass(), GearScore_GetRecordDisplayRace(), GearScore_GetRecordGuild() (+13 more)

### Community 9 - "Community 9"
Cohesion: 0.18
Nodes (5): AceTimer:ScheduleRepeatingTimer(), AceTimer:ScheduleTimer(), OnUpdate(), Reg(), safecall()

### Community 10 - "Community 10"
Cohesion: 0.18
Nodes (14): GearScore_ApplyStatsProfile(), GearScore_BuildStatsColumn(), GearScore_BuildStatsText(), GearScore_EnsureStatsRows(), GearScore_FormatStatValue(), GearScore_GetCombatStatColumn(), GearScore_GetDefaultStatsProfile(), GearScore_GetDisplayClass() (+6 more)

### Community 11 - "Community 11"
Cohesion: 0.17
Nodes (12): AceLocale-3.0, AceTimer-3.0, BonusScanner, BonusScanner Changelog, Combat Rating Conversion, BonusScanner Curse Gaming Page, CUSTOM_CLASS_COLORS, Equipped Itemlink Cache (+4 more)

### Community 12 - "Community 12"
Cohesion: 0.54
Nodes (3): LibStub:GetLibrary(), LibStub:IterateLibraries(), LibStub:NewLibrary()

### Community 13 - "Community 13"
Cohesion: 0.29
Nodes (8): Central Character Model Preview, Character Search and Database Controls, Equipment Slots Surrounding Character Model, GearScore and Item Level Summary, GearScore Character Viewer Window, Inspected Character Identity: Гномік, Level 80 Gnome Mage, Primary Attributes and Armor Panel, Equipment, Experience, and Options Navigation

### Community 14 - "Community 14"
Cohesion: 0.29
Nodes (7): Data Object Attribute Change Callbacks, LibDataBroker Data Objects, Display Addons, Fortress, GitHub Wiki Documentation, StatBlockCore, LibDataBroker 1.1 v1.1.4 Changelog

### Community 17 - "Community 17"
Cohesion: 0.6
Nodes (3): CallbackHandler:New(), CreateDispatcher(), errorhandler()

### Community 19 - "Community 19"
Cohesion: 0.5
Nodes (3): Answer, Q: Як працює 2-секундне очікування повного екіпірування GearScore?, Source Nodes

### Community 20 - "Community 20"
Cohesion: 0.5
Nodes (3): Answer, Q: What exactly was changed and how will offline GearScore work?, Source Nodes

### Community 21 - "Community 21"
Cohesion: 0.5
Nodes (3): Answer, Q: Як виправлено cooldown, guild tab та білі офлайн-моделі GearScore?, Source Nodes

### Community 22 - "Community 22"
Cohesion: 0.5
Nodes (3): Answer, Q: Як GearScore позначає відсутню модель персонажа?, Source Nodes

### Community 23 - "Community 23"
Cohesion: 0.5
Nodes (3): Answer, Q: Коли GearScore може показати модель онлайн-персонажа без SQL?, Source Nodes

### Community 24 - "Community 24"
Cohesion: 0.5
Nodes (3): Answer, Q: Is the offline GearScore implementation safe under server load?, Source Nodes

### Community 25 - "Community 25"
Cohesion: 0.5
Nodes (3): Answer, Q: Як спрощено моделі GearScore без SQL?, Source Nodes

### Community 26 - "Community 26"
Cohesion: 0.5
Nodes (3): Answer, Q: How does offline gear response populate the GearScore model and stats?, Source Nodes

### Community 27 - "Community 27"
Cohesion: 0.5
Nodes (4): ScanEquipment, Gear Bonuses and Average Item Level, LibDataBroker Feed, LibDBIcon

### Community 28 - "Community 28"
Cohesion: 0.5
Nodes (4): LibQTipClick License, LibQTipClick AS-IS Warranty and Liability Disclaimer, LibQTipClick Redistribution and Use Conditions, LibQTipClick Stand-alone Redistribution Restriction

### Community 29 - "Community 29"
Cohesion: 0.5
Nodes (4): LibQTip License, LibQTip AS-IS Warranty and Liability Disclaimer, LibQTip Redistribution and Use Conditions, LibQTip Stand-alone Redistribution Restriction

### Community 30 - "Community 30"
Cohesion: 0.67
Nodes (3): LibCompress Changelog, LibCompress r40-release, World of Warcraft Patch 3.2 (TOC 30200)

## Knowledge Gaps
- **47 isolated node(s):** `GearScore`, `Answer`, `Source Nodes`, `Answer`, `Source Nodes` (+42 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **3 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `GearScore_GetQuality()` connect `Community 4` to `Community 0`, `Community 3`, `Community 7`?**
  _High betweenness centrality (0.012) - this node is a cross-community bridge._
- **Why does `print()` connect `Community 4` to `Community 0`, `Community 3`?**
  _High betweenness centrality (0.011) - this node is a cross-community bridge._
- **What connects `GearScore`, `Answer`, `Source Nodes` to the rest of the system?**
  _47 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Community 0` be split into smaller, more focused modules?**
  _Cohesion score 0.07 - nodes in this community are weakly interconnected._
- **Should `Community 1` be split into smaller, more focused modules?**
  _Cohesion score 0.06 - nodes in this community are weakly interconnected._
- **Should `Community 2` be split into smaller, more focused modules?**
  _Cohesion score 0.06 - nodes in this community are weakly interconnected._
- **Should `Community 3` be split into smaller, more focused modules?**
  _Cohesion score 0.1 - nodes in this community are weakly interconnected._