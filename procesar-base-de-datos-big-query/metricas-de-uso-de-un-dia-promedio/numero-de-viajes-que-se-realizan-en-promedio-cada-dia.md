---
description: 'Se utiliza la variable startime para realizar el calculo correspondiente:'
---

# 🚴 Número de viajes que se realizan en promedio cada día

```sql
SELECT
  COUNT(starttime) AS cantidad
FROM
  `citi-bike-ny.bike_ny.view_totalTrips` 
LIMIT
  1;
```

<figure><img src="../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

### Conclusiones

Se realiza 53.108.721 viajes en bicicleta diarios en New York.
