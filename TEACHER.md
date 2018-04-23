# Instructions

> Getting a clean list of POIs given an operator.

```sql
SELECT
  PoiName, ZoneCode, PoiDescription, PoiTypeId, UsageTypeId, PropertyTypeId, 
  PrimaryBrandId, PrimaryBrandKeyId, pm.OperatorMasterId, PoiStatusId, gm.Latitude, gm.Longitude
  FROM PoiMaster pm
  LEFT JOIN GisLinkage gl ON gl.PoiMasterId = pm.Id
  LEFT JOIN GisMaster gm on gm.Id = gl.GisMasterId
  WHERE pm.OperatorMasterId = 196
  AND pm.PoiDescription != ''
  AND gm.Latitude is not null
  LIMIT 20
```

> Getting an ugly list of POIs given an operator

```sql
SELECT
  PoiName, ZoneCode, PoiDescription, PoiTypeId, UsageTypeId, PropertyTypeId, 
  PrimaryBrandId, PrimaryBrandKeyId, pm.OperatorMasterId, PoiStatusId, gm.Latitude, gm.Longitude
  FROM PoiMaster pm
  LEFT JOIN GisLinkage gl ON gl.PoiMasterId = pm.Id
  LEFT JOIN GisMaster gm on gm.Id = gl.GisMasterId
  WHERE pm.OperatorMasterId = 3338001
  -- AND pm.PoiDescription != ''
  -- AND gm.Latitude is not null
  LIMIT 215
```