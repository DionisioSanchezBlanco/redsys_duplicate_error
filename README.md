# redsys_duplicate_error

Modificamos el fichero del plugin oficial de Redsys para no obtener el error de pedido duplicado en la pasarela de pago. Se ha hecho lo siguiente:
- Se añade un número aleatorio de 3 dígitos al principio del número de pedido para que cada vez que se acceda al pago este sea diferente.
- Se recupera el número de pedido original para que WooCommerce sea capaz de actualizar el estado del pedido una vez finalizada la transacción desde la pasarela.
