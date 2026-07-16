---
type: "query"
date: "2026-07-16T19:59:00.248725+00:00"
question: "Is the offline GearScore implementation safe under server load?"
contributor: "graphify"
source_nodes: ["GearScore_RequestServerItemData()", "GearScore_HandleServerItemReply()"]
---

# Q: Is the offline GearScore implementation safe under server load?

## Answer

Normal use is safe and light: the client caches records, the server limits each requester, model data is direct-only, and stats save only on logout. Both character queries use indexes. The inventory query currently fetches all inventory rows for the GUID before C++ filters equipment, so adding bag=0 and slot<18 would reduce its result from roughly a full inventory to at most 18 rows. Coordinated malicious clients remain the main residual load risk because throttling is per requester, not global.

## Source Nodes

- GearScore_RequestServerItemData()
- GearScore_HandleServerItemReply()