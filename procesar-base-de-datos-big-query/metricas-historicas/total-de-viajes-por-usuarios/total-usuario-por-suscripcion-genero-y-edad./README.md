# 🚲 Total Usuario por Suscripción, Genero y Edad.

```sql
SELECT
  usertype,
  gender,
  rango_edad,
  COUNT(*) AS cantidad
FROM
  `citi-bike-ny.bike_ny.view_totalTrips`
GROUP BY
  usertype,
  gender,
  rango_edad
ORDER BY
  usertype,
  gender,
  rango_edad
```

###
