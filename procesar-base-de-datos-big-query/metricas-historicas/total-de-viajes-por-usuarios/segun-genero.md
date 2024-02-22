# 👫 Según Género

```sql
SELECT
  usertype,
  gender,
  COUNT(*) AS cantidad
FROM
  `citi-bike-ny.bike_ny.view_totalTrips`
GROUP BY
  usertype,
  gender
ORDER BY
  usertype,
  gender;
```

<figure><img src="../../../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

### Conclusiones

1. Hay 187.701 usuarios las cuales son género femenino y su tipo de inscripción es Customer (usuario de pase de 24 horas o pase de 3 días).
2. Hay 303.264 usuarios las cuales son género masculino y su tipo de inscripción es Customer (usuario de pase de 24 horas o pase de 3 días).
3. Hay 5.700.184 usuarios las cuales son género desconocido y su tipo de inscripción es Customer (usuario de pase de 24 horas o pase de 3 días).
4. Hay 11.188.711 usuarios las cuales son género femenino y su tipo de inscripción es Subscriber (miembro anual).
5. Hay 35.308.523 usuarios las cuales son género masculino y su tipo de inscripción es Subscriber (miembro anual).
6. Hay  420.338 usuarios las cuales son género desconocido y su tipo de inscripción es Subscriber (miembro anual).
