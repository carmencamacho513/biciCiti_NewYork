---
description: >-
  Se utiliza la variable tripduration para realizar las métricas
  correspondientes:
---

# 🚲 Número máximo, mínimo, promedio y desviación estándar en la duración de un viaje:

```sql
SELECT
  MAX(tripduration) AS max_trips,
  MIN(tripduration) AS min_trips,
  AVG(tripduration) AS AVG_trips,
  STDDEV(tripduration) AS STDDEV_trips
FROM
  `citi-bike-ny.bike_ny.view_totalTrips`;
```

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

```sql
SELECT
  MAX(tripduration/86400) AS max_trips,
  MIN(tripduration) AS min_trips,
  AVG(tripduration/60) AS AVG_trips,
  STDDEV(tripduration/3600) AS STDDEV_trips
FROM
  `citi-bike-ny.bike_ny.view_totalTrips`;
```

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

### Conclusiones

El máximo tiempo que dura un viaje en bicicleta es de 19.510.049 segundos que equivale a 226 días aproximadamente.

El mínimo tiempo que dura un viaje en bicicleta es de 60 segundos.

El promedio que dura un viaje en bicicleta es de 962.5 segundos que equivale a 16 minutos aproximadamente.

La desviación estándar de un viaje en bicicleta es de 13.546,010 segundos que equivale a 4 horas aproximadamente.
