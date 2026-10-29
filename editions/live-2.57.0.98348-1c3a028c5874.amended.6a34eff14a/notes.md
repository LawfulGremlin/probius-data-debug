# Live 2.57.0.98348 — Hotfix - 10/5/2026, amended by Probius

*from 2.57.0.98304*

> Blizzard's official notes with Probius additions. Green text marks changes found in the game data that the official notes do not mention. Green means additional, not a buff.
>
> Our next Heroes of the Storm patch is live! Read on for more information.
>
> NOTE: Orange text indicates a change between PTR and Live notes.
>
> Blizzard's original text colors are not available from the published page.

## Legend

- 🟢 **Probius addition — not in official notes**
- ⚠️ **Discrepancy — game data differs from the official notes**
- ❔ **Coverage uncertain — may be missing from the official notes**

13 additions · 0 discrepancies · 6 uncertain · 6 confirmed

## Hotfix - 10/5/2026

- Xal'atath Balance Updates  
  Abilities
- Shadow Mark (Q)
  - Void Orb speed slightly increased.
- Void Step (E)
  - Targeting range reduced from 5 to 2.
  - Distance between teleport points reduced from 7 to 6.5.
  - Now prevented and interrupted by Immobilize.
- Void Volley (D)
  - Base damage per missile reduced from 90 to 72.
  - Now generates 1 charge for every Basic Attack against enemy Heroes and every 2 Basic Attacks against non-Heroes.
  - ❔ **Coverage uncertain:** ~~After attacking enemies with her Basic Attacks 5 times~~ → Every basic attack against heroes, {+and every 2 basic attacks against non-heroes generate charge. Once fully charged+} Xal'atath can activate Void Volley to unleash a barrage of 6 Void Orbs at a target location, each dealing ~~90~~ → 72 (+4% per level) damage on impact.
- Void Eruption (R)
  - Uncharged damage reduced by 20%.
    - 🟢 **Probius addition — not in official notes:** Exact values: from 112 to 90
  - Fully charged damage reduced by 5%.
    - 🟢 **Probius addition — not in official notes:** Exact values: from 175 to 166
  - ❔ **Coverage uncertain:** Void Eruption: flight damage per second tier 2 reduced from 2000 to 1700 (game data)
  - ❔ **Coverage uncertain:** Void Eruption: flight damage per second tier 3 reduced from 2400 to 2160 (game data)

- Talents
- Level 1
  - Anchored Core
    - Radius bonus reduced from 50% to 25%.
- Level 4
  - Dark Barrier
    - Now only triggers when enemy Heroes are hit
    - ❔ **Coverage uncertain:** Each time {+the+} Dark Heart damages an enemy {+Hero+}, Xal'atath gains a Shield equal to 2% of her maximum Health, up to 10%.
- Level 7
  - Silence of the Lamb
    - Silence duration increased from 1 to 1.5 seconds.
- Level 13
  - Dark Heart's Protection
    - Detonating the Dark Heart on a target affected by Shadow Mark now Silences all enemies hit. Previously silenced on cast.
    - ❔ **Coverage uncertain:** ~~Casting~~ → Detonating the Dark Heart ~~Ritual~~ → now Silences enemies inside its radius for 1 second.
- Level 20
  - Rift Invasion
    - Portals now have non-lethal Health decay, stopping at 4 Health.
    - ❔ **Coverage uncertain:** Void Convergence's Void Portal {+self decay is+} no longer ~~has a life duration~~ → lethal, raises the active Void Portal limit to 2, and can spawn and sustain up to 4 Void Minions.

- Xal'atath Bug Fixes
- General
  - Orbiting orbs now pause during Time Stop and resume afterward.
  - Fixed issues that prevented orbiting orbs from correctly following the missile or continuing to orbit after a release queued during Time Stop.
  - Fixed an issue where Xal'atath was appearing brighter than intended in the game.
- Void Volley (D)
  - Fixed an issue that caused impact visual effects to appear at the cursor location instead of where missiles hit.
  - Fixed an issue that prevented the charge indicator from immediately displaying 1 charge upon reaching the second milestone.
- Void Eruption (R)
  - Can now be queued to cast or release during Time Stop.
  - Casting during Time Stop immediately enters targeting, with charging beginning when Time Stop ends.
  - Releasing during Time Stop queues the release for when Time Stop ends. The Ability button becomes greyed out while a release is queued.
  - Issuing another Ability, movement, or attack order during Time Stop cancels the pending cast or queued release.
  - Casting Void Eruption again during Time Stop clears earlier queued orders.
  - Fixed issues that could allow an additional charge to begin while already charging or during Void Step.
  - Orb growth and the flight damage timer now pause while Xal’atath is affected by Time Stop.
- General Bug Fixes
  - Fixed an issue where certain Maskless skins were not appearing in the game.

## Additional changes found by Probius

### Whitemane

- 🟢 **Probius addition — not in official notes:** Desperate Plea (Q): cost modification increased from 40 to 45 (game data)

### Xal'atath

- 🟢 **Probius addition — not in official notes:** Dark Heart Ritual (W): detonation range reduced from 4 to 3 (game data)
- 🟢 **Probius addition — not in official notes:** Dark Heart Ritual (W): duration increased from 0.125 seconds to 1.1 seconds (game data)
- 🟢 **Probius addition — not in official notes:** Harbinger's Consumption (Level 20): damage tier 1 reduced from 400 to 320 (game data)
- 🟢 **Probius addition — not in official notes:** Harbinger's Consumption (Level 20): damage tier 2 reduced from 500 to 425 (game data)
- 🟢 **Probius addition — not in official notes:** Harbinger's Consumption (Level 20): damage tier 3 reduced from 600 to 540 (game data)
- 🟢 **Probius addition — not in official notes:** Harbinger's Consumption (Level 20): damage tier 4 reduced from 700 to 665 (game data)
- 🟢 **Probius addition — not in official notes:** Harbinger's Consumption (Level 20): flight damage per second tier 1 reduced from 1800 to 1440 (game data)
- 🟢 **Probius addition — not in official notes:** Harbinger's Consumption (Level 20): flight damage per second tier 2 reduced from 2000 to 1700 (game data)
- 🟢 **Probius addition — not in official notes:** Harbinger's Consumption (Level 20): flight damage per second tier 3 reduced from 2400 to 2160 (game data)
- 🟢 **Probius addition — not in official notes:** Harbinger's Consumption (Level 20): flight damage per second tier 4 reduced from 2800 to 2660 (game data)

## Technical appendix

### Coverage of the official notes

25 game-data claims compared with the official section: covered 6, partly 2, uncertain 6, absent 11; 16 official bullets have no related claim.

### Source-level changes not interpreted

273 changes in 1 group could not be tied to a player-facing statement.

- Xal'atath (273)
  - Button/Tooltip/XalatathVoidConvergence (changed)
  - $XalatathAnchoredCoreLinkRangeIncrease: 1.5 → (none) (const removed)
  - Entry added: CBehaviorBuff#XalatathOrbitalEruptionOrbTimeStopBehaviorBuff
  - Entry added: CBehaviorBuff#XalatathVoidConvergenceCasterBehavior
  - Entry added: CBehaviorBuff#XalatathVoidConvergenceRiftInvasionPortalDecayBehavior
  - Entry added: CBehaviorBuff#XalatathVoidEruptionTimeStopEnterPendingBehaviorBuff
  - Entry added: CBehaviorBuff#XalatathVoidEruptionTimeStopEnterPendingOrderWatchBehaviorBuff
  - Entry added: CBehaviorBuff#XalatathVoidEruptionTimeStopReleaseQueuedBehaviorBuff
  - Entry added: CBehaviorBuff#XalatathVoidEruptionVisualGrowBehaviorBuff
  - Entry added: CBehaviorBuff#XalatathVoidEruptionVisualGrowControllerBehaviorBuff
  - Entry added: CBehaviorBuff#XalatathVoidVolleyNonHeroChargeMarker
  - Entry added: CEffectApplyBehavior#XalatathOrbitalEruptionOrbTimeStopApplyBehavior
  - Entry added: CEffectApplyBehavior#XalatathVoidConvergenceApplyCasterBehavior
  - Entry added: CEffectApplyBehavior#XalatathVoidEruptionTimeStopEnterPendingApplyBehavior
  - Entry added: CEffectApplyBehavior#XalatathVoidEruptionTimeStopEnterPendingOrderWatchApplyBehavior
  - Entry added: CEffectApplyBehavior#XalatathVoidEruptionTimeStopReleaseQueuedApplyBehavior
  - Entry added: CEffectApplyBehavior#XalatathVoidEruptionVisualGrowCasterApplyBehavior
  - Entry added: CEffectApplyBehavior#XalatathVoidEruptionVisualGrowControllerApplyBehavior
  - Entry added: CEffectApplyBehavior#XalatathVoidEruptionVisualGrowTargetApplyBehavior
  - Entry added: CEffectApplyBehavior#XalatathVoidVolleyApplyNonHeroChargeMarker
  - Entry added: CEffectCancelOrder#XalatathVoidEruptionQueuedReleaseCancelOrder
  - Entry added: CEffectCancelOrder#XalatathVoidEruptionTimeStopEnterCancelOrders
  - Entry added: CEffectCreatePersistent#XalatathVoidEruptionTimeStopDeferredReleaseCreatePersistent
  - Entry added: CEffectRemoveBehavior#XalatathVoidConvergenceRemoveCasterBehavior
  - Entry added: CEffectRemoveBehavior#XalatathVoidEruptionTimeStopEnterPendingRemoveBehavior
  - +248 more

### Tooltip text corrections

- Xal'atath (2)
  - Void Summoner: Activating Void Step summons a single Void Minion in ~~Xalatath's~~ → Xal'atath's original postion. Void Minions are attracted to targets afflicted by Shadow Mark. Void Minions automatically choose a nearby lane to push. Void Minion Basi...
  - Void Summoner: Activating Void Step summons a single Void Minion in ~~Xalatath's~~ → Xal'atath's original postion.

### Collection and cosmetics

- Skin strings: 30 added; Maskless Peacekeeper Johanna, Maskless Gleaming Peacekeeper Johanna, Maskless Zealous Peacekeeper Johanna, Maskless Shadow Stalker Valla, Maskless Vibrant Shadow Stalker Valla, Maskless Alabaster Shadow Stalker Valla, Maskless Raynor 76, Maskless Enhanced Raynor 76, Maskless Elite Raynor 76
- crusaderowc20basedata.xml: 7 added; CSkin#CrusaderOWC20NoHelmetCommon
- crusaderowc20var3data.xml: 2 added; CRewardSkin#CrusaderOWC20Var3, CSkin#CrusaderOWC20Var3
- crusaderowc20var4data.xml: 4 added; CRewardSkin#CrusaderOWC20Var4, CSkin#CrusaderOWC20Var4
- crusaderowc20var5data.xml: 4 added; CRewardSkin#CrusaderOWC20Var5, CSkin#CrusaderOWC20Var5
- raynorowc20basedata.xml: 7 added; CSkin#RaynorOWC20NoMaskCommon
- raynorowc20var3data.xml: 2 added; CRewardSkin#RaynorOWC20Var3, CSkin#RaynorOWC20Var3
- raynorowc20var4data.xml: 4 added; CRewardSkin#RaynorOWC20Var4, CSkin#RaynorOWC20Var4
- raynorowc20var5data.xml: 4 added; CRewardSkin#RaynorOWC20Var5, CSkin#RaynorOWC20Var5
- demonhunterowc20basedata.xml: 7 added; CSkin#DemonHunterOWC20NoMaskCommon
- demonhunterowc20var3data.xml: 2 added; CRewardSkin#DemonHunterOWC20Var3, CSkin#DemonHunterOWC20Var3
- demonhunterowc20var4data.xml: 4 added; CRewardSkin#DemonHunterOWC20Var4, CSkin#DemonHunterOWC20Var4
- demonhunterowc20var5data.xml: 4 added; CRewardSkin#DemonHunterOWC20Var5, CSkin#DemonHunterOWC20Var5
- xalatathdata.xml: 1 added, 10 changed, 1 removed
- xalatathbasedata.xml: 4 changed
- xalatathvar1data.xml: 1 added, 2 changed; CSkin#XalatathVar1
- xalatathvar2data.xml: 1 added, 2 changed; CSkin#XalatathVar2
- xalatathvar3data.xml: 1 added, 2 changed; CSkin#XalatathVar3
- xalatathvar4data.xml: 1 added, 2 changed; CSkin#XalatathVar4
- xalatathvoidflamebasedata.xml: 1 changed
- xalatathvoidflamevar1data.xml: 1 changed
- xalatathvoidflamevar2data.xml: 1 changed
- xalatathvoidflamevar3data.xml: 1 changed
- xalatathvoidflamevar4data.xml: 1 changed
- xalatathvoideruptiondata.xml: 5 added, 7 changed
- xalatathvoidvolley2data.xml: 6 changed

### Assets

The asset index first appears in this build (200078 paths indexed).

- core.stormmod/base.stormassets: 1080 added, 0 changed, 0 removed (dds 775, lvl0 202, m3 100, db 1, m3h 1)
- core.stormmod/base.stormdata: 15 added, 0 changed, 0 removed (bin 6, ttf 5, otf 2, (none) 1, triggerlib 1)
- core.stormmod/enus.stormassets: 1 added, 0 changed, 0 removed (db 1)
- gameplaymods/lootbox.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- gameplaymods/progression20.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heroes.stormmod/base.stormassets: 109550 added, 0 changed, 0 removed (dds 39131, wav 25264, lvl0 23146, m3 18370, ogg 2879)
- heroes.stormmod/base.stormmaps: 107 added, 0 changed, 0 removed ((none) 85, dds 11, tga 5, ogg 3, wav 2)
- heroes.stormmod/enus.stormassets: 88881 added, 0 changed, 0 removed (ogg 58927, fxe 28022, wav 1894, dds 18, lvl0 16)
- heroesbrawlmods/arenamodemods: 21 added, 0 changed, 0 removed ((none) 21)
- heroesbrawlmods/brawlmapmods: 119 added, 0 changed, 0 removed (dds 58, (none) 50, m3 10, png 1)
- heroesbrawlmods/heroesbrawl.stormmod: 3 added, 0 changed, 0 removed ((none) 3)
- heroesbrawlmods/heroselectionmods: 3 added, 0 changed, 0 removed ((none) 3)
- heroesdata.stormmod/base.stormdata: 5 added, 0 changed, 0 removed ((none) 4, tga 1)
- heroesmapmods/battlegroundmapmods: 106 added, 0 changed, 0 removed ((none) 89, lst 8, dds 6, m3 1, ogg 1)
- heromods/alarak.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/alexstrasza.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/amazon.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/ana.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/anduin.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/auriel.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/chogall.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/chromie.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/deathwing.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/deckard.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/dehaka.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/dva.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/fenix.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/firebat.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/garrosh.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/genji.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/guldan.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/hanzo.stormmod: 3 added, 0 changed, 0 removed ((none) 3)
- heromods/herointeractions.stormmod: 2 added, 0 changed, 0 removed ((none) 2)
- heromods/hogger.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/imperius.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/junkrat.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/kelthuzad.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/lucio.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/maiev.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/malganis.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/malthael.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/medivh.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/meiow.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/mephisto.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/nexushunter.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/orphea.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/probius.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/samuro.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/stukov.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/thefirelords.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/tracer.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/valeera.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/varian.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/whitemane.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/xalatath.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/yrel.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/zarya.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- heromods/zuljin.stormmod: 4 added, 0 changed, 0 removed ((none) 4)
- testmods/autopve.stormmod: 3 added, 0 changed, 0 removed ((none) 3)
- testmods/tilesettesting.stormmod: 3 added, 0 changed, 0 removed ((none) 3)

### Coverage

1133 changed paths; claims: 9 player-facing, 16 from game data, 273 not interpreted, 100 excluded or duplicate.

- asset-index: 832 paths, 831 with claims
- hero-structured: 1 path, 1 with claims
- layout-ui: 1 path, 0 with claims
- metadata: 264 paths, 0 with claims
- other: 1 path, 0 with claims
- strings: 2 paths, 2 with claims
- tooltip-derived: 2 paths, 0 with claims
- unit-structured: 2 paths, 0 with claims
- xml-catalog: 28 paths, 27 with claims

Changed paths without claims, by reason:

- tooltip-derived duplicate of hero JSON (2)
  - heroes-talents/.tooltip\_markup.json
  - heroes-talents/.tooltip\_simple.json
- version-renamed unit data, compared by content (2)
  - heroes-talents/unitdata\_2.57.0.98304.json
  - heroes-talents/unitdata\_2.57.0.98348.json
- asset index (1)
  - heroes-mods/.files/\_build.txt
- include list (1)
  - heroes-mods/heroesdata.stormmod/base.stormdata/gamedata.xml
- layout or interface file, not interpreted (1)
  - heroes-mods/heromods/xalatath.stormmod/base.stormdata/ui/layout/xalatath.stormlayout
- not interpreted (1)
  - heroes-mods/heromods/xalatath.stormmod/gamedata.version

## Sources

- [Blizzard: Heroes of the Storm Live Patch Notes - September 28, 2026, Hotfix - 10/5/2026](https://news.blizzard.com/en-us/article/24303007/heroes-of-the-storm-live-patch-notes-september-28-2026) (observed 2026-10-29T14:08:59Z)
- [LawfulGremlin/probius-data-debug@​1c3a028c (Live data commit)](https://github.com/LawfulGremlin/probius-data-debug/commit/1c3a028c5874930f60e72bd0df388c1038bb63c5) (observed 2026-10-05T17:17:31Z)
