# Tarea 
## 1. Productos sin pais de origen 
  - Sentencia:
  ```
  SELECT COUNT (*) - COUNT (country_of_origin) AS products_without_country
FROM product 
  ```
  - Captura:
<img src="./capturas/sentence01.png" alt="drawing" width="500"/>



## 2. Numero de cliente por cuidad 
  - Sentencia:
  ```
  SELECT DISTINCT  city, COUNT(city)
FROM client
GROUP BY (city)
  ```
  - Captura:
<img src="./capturas/sentence01.png" alt="drawing" width="500"/>


