# Tarea en clase 

# 1. Crear una vista de la factura en donde aparezca el nombre del cliente
- sentencia
```
CREATE view invoice_view AS 
SELECT i.id, i.code, i.create_at, i.total, c.full_name
FROM invoice i JOIN client c
    ON c.id = i.client_id; 
```
- captura
<img src="captura/Captura de pantalla (155).png" alt="drawing" width="500"/>

# 2. Crear una vista de los detalles con la descripcion del producto
- sentencia 
```
CREATE view detail_view AS
SELECT d.quantity, p.description, d.price, d.price * d.quantity AS subtotal
FROM detail d JOIN product p
     ON d.product_id = p.id;
```
- captura
<img src="captura/Captura de pantalla (156).png" alt="drawing" width="500"/>