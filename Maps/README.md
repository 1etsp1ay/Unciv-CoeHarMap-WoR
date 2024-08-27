> [!IMPORTANT]
> The CoeHarMod is designed for multiplayer so the map may not work 100%

# Map conversion

CoeHarMod uses a typed namespace to cluster the uniques

- {terrain} + **Landform** . {terrainFeature}
  - {terrain} = one of [_Desert_, _Graasslands_, _Plain_, __Snow_, _Tundra_]
  - {terrainFeature} = {terrainGeography} + {terrainHazard} + {terrainFeature}
  - {terrainGeography} = any of {_Hill_, _Forest_, _Jungle_, _Mountain_, _Swamp_}
  - {terrainHazard} = {_NuclearFallout_, _VolcanicSoil_, _Volano_} which inflict damage
  - but rules restraining _Forest_/_Jungle_ and irrigated tiles
- _Water_ may be treated differently [tba], CoeHarMod adds _Large River_
  - to implement constraints on ships movement cost of 2 for _Large River_ ignored by junk
  - considered like ice to be impassible for frigates, destroyers, battleships, carriers
  - at moment need to manually convert as no region

So we identify a number of uniques which are not within quotes (aka text) to insert **Landform.** for every terrainFeature.
