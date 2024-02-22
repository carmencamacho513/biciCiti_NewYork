# 🌤 Según Tipo de Subscripción

```sql
SELECT
usertype,
  COUNT(*) AS cantidad
FROM
  `citi-bike-ny.bike_ny.view_totalTrips`
GROUP BY
  usertype;
```

<figure><img src="../../../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

### Conclusiones

1. Hay  en total 46.917.572 tipo Subscriber que son miembros anuales.
2. Hay 6.191.149 Customer que son usuario de pase de 24 horas o pase de 3 días.
