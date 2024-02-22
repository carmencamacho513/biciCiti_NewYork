---
description: >-
  Se utiliza la tabla en general y la variable starttime agrupando y ordenando
  por la misma para realizar el calculo correspondiente:
---

# 🚴♂ Crecimiento del número de viajes diarios a lo largo del tiempo.

```sql
SELECT
  DATE(starttime) AS fecha_dia,
  COUNT(*) AS viajes_diarios
FROM
  `citi-bike-ny.bike_ny.view_totalTrips`
GROUP BY
  fecha_dia
ORDER BY
  fecha_dia;
```

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
