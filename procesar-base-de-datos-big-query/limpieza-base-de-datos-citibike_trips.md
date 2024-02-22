# 📥 Limpieza Base de Datos citibike\_trips

```sql
SELECT
  * EXCEPT(customer_plan, birth_year),
  CASE
    WHEN birth_year IS NULL THEN "Sin Datos"
    ELSE CAST(birth_year AS STRING)
  END AS year_birth,
  CASE    
    WHEN birth_year BETWEEN 1979 AND 2002 THEN 'Adulto 22 a 44 Años'
    WHEN birth_year BETWEEN 1965 AND 1978 THEN 'Adulto Medio 45 a 59 años'
    WHEN birth_year BETWEEN 1949 AND 1964 THEN 'Adulto Mayor 60 a 75 años'
    WHEN birth_year BETWEEN 1925 AND 1948 THEN 'Muy Mayor 76 a 99 años'
    ELSE 'Fuera de los Parámetros'
  END AS rango_edad
FROM
  `citi-bike-ny.bike_ny.view_citiBike`
WHERE
  tripduration IS NOT NULL
  AND starttime IS NOT NULL
  AND stoptime IS NOT NULL
  AND start_station_id IS NOT NULL
  AND start_station_name IS NOT NULL
  AND start_station_latitude IS NOT NULL
  AND start_station_longitude IS NOT NULL
  AND end_station_id IS NOT NULL
  AND end_station_name IS NOT NULL
  AND end_station_latitude IS NOT NULL
  AND end_station_longitude IS NOT NULL
  AND bikeid IS NOT NULL
  AND usertype IS NOT NULL
  AND gender IS NOT NULL;
```
