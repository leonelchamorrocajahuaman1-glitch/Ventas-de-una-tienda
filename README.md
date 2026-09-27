# NovaCell — Ventas de una tienda

Sistema web de una tienda de celulares hecho con HTML, CSS y JavaScript.

## Funciones

- Catálogo y búsqueda de productos.
- Registro de ventas con varios detalles.
- Clientes y comprobante de venta.
- Inventario persistente y actualización automática del stock.
- Subtotal, descuento por cantidad, IGV configurable (18 %) y total.
- Validación atómica: primero valida todos los productos y stock; solo después descuenta inventario.
- Historial de ventas guardado en `localStorage`.

## Reglas implementadas

- Precios y cantidades positivos.
- Precio unitario histórico guardado en cada detalle.
- Descuento de 5 % cuando se venden 2 o más unidades del mismo producto, antes del IGV.
- Importes redondeados a dos decimales con redondeo convencional.

## Escenario de aceptación

El producto `P001` inicia con stock 3. Al vender 2 unidades queda en 1. Si se intenta vender 2 unidades nuevamente, la operación falla completa: no se descuenta stock ni se crea una venta parcial.

Abre `index.html` en el navegador para utilizarlo. Para publicarlo, sube los archivos a GitHub Pages.
