# 🥳 Según Edad

```sql
SELECT
  usertype,
  rango_edad,
  COUNT(*) AS cantidad
FROM
  `citi-bike-ny.bike_ny.view_totalTrips`
GROUP BY
  usertype,
  rango_edad
ORDER BY
  usertype,
  rango_edad;
```

<figure><img src="../../../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

### Conclusiones

1. Hay 368.270 usuarios entre edades de 22 a 44 años y con un tipo de suscripción Customer (usuario de pase de 24 horas o pase de 3 días).
2. Hay 449.215 usuarios entre edades de 45 a 59 años y con un tipo de suscripción Customer (usuario de pase de 24 horas o pase de 3 días).
3. Hay 31.616 usuarios entre edades de 60 a 75 años y con un tipo de suscripción Customer (usuario de pase de 24 horas o pase de 3 días).
4. Hay 904 usuarios entre edades de 76 a 99 años y con un tipo de suscripción Customer (usuario de pase de 24 horas o pase de 3 días).
5. Hay 5.341.144 usuarios "Fuera de los Parámetros" son edades que pasan los 100 años  o no hay datos especificos; pero sus datos se hacen relevantes porque la suscripción ya que son Customer (usuario de pase de 24 horas o pase de 3 días).
6. Hay 25.350.555 usuarios entre edades de 22 a 44 años y con un tipo de suscripción Subscriber (miembro anual).
7. Hay 13.860.854 usuarios entre edades de 45 a 59 años y con un tipo de suscripción Subscriber (miembro anual).
8. Hay 6.951.517 usuarios entre edades de 60 a 75 años y con un tipo de suscripción Subscriber (miembro anual).
9. Hay 495.820 usuarios entre edades de 76 a 99 años y con un tipo de suscripción Subscriber (miembro anual).
10. Hay 258.826 usuarios "Fuera de los Parámetros" son edades que pasan los 100 años  o no hay datos especificos; pero sus datos se hacen relevantes porque la suscripción ya que son Subscriber (miembro anual).

