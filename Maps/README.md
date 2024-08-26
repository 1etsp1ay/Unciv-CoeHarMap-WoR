> [!IMPORTANT]
> The CoeHarMod is designed for multiplayer so the map may not work 100%

# Map conversion

CoeHarMod uses a typed namespace to cluster the uniques

- {terrain} + **Landform** . {terrainFeature}
  - {terrain} = one of [_Desert_, _Graasslands_, _Plain_, __Snow_, _Tundra_]
  - {terrainFeature} = {terrainGeography} + {terrainVariation} + {terrainFeature}
  - {terrainGeography} = any of {_Hill_, _Forest_, _Jungle_, _Mountain_}
  - {terrainVariation} = {VolcanicSoil}
  - but rules restraining _Forest_/_Jungle_ and irrigated tiles
- _Sea_ may be treated differently [tba]

So we identify a number of uniques which are not within quotes (aka text) to insert **Landform.** for every terrainFeature.
