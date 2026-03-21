# Informacion_De_Ventas

Se tiene el historial de ventas en varias plataformas, en donde se desea llevar el control/reigstro ordenado de cada lugar con los datos que porporciona la plataforma, numero de orden, quien lo compro, cuando lo compro, correo electronico, etc.

# Informacoin de la normlalizacoin

Originalmente, el esquema presentaba una limitación si un consumidor deseaba adquirir múltiples productos en una misma transacción. Para solucionar esto, se identificó una relación de "muchos a muchos" (N:M) entre las ventas y los productos. Siguiendo las reglas de normalización, se optó por implementar una tabla intermedia o puente denominada Detalle_Venta. Con esta reestructuración, se logró dividir la relación: ahora una entidad de Ventas puede asociarse a múltiples Productos a través del detalle, y un Producto puede figurar en múltiples transacciones. Esto garantiza la atomicidad de los datos (cumpliendo con la Primera Forma Normal) y evita el uso de campos multivaluados o columnas repetitivas.
