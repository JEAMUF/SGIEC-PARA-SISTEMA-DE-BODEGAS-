SIGEC · Sistema de Gestión Centralizada para Bodega
¿Qué es este proyecto?

SIGEC es un sistema web de punto de venta, inventario, control de caja y gestión de usuarios, pensado para una bodega, minimarket o tienda de barrio en Perú. Es una sola página web (HTML, CSS y JavaScript, sin instalación de servidor) con login por PIN y 5 roles distintos: Administrador, Supervisor, Cajero, Almacenero y Contador.

Es mi primer proyecto de este tipo, desarrollado por fases: alcance del negocio, diseño funcional de los módulos, flujos de operación, modelo de datos y finalmente el sistema funcionando.

¿Qué problema resuelve?

Una bodega típica suele vender "de memoria": no sabe con certeza cuánto stock tiene, pierde productos por vencimiento sin darse cuenta, no controla bien su caja al final del día y no sabe con claridad si está ganando o perdiendo dinero. SIGEC centraliza estos cuatro procesos para que:

Cada venta descuente el stock automáticamente, sin que nadie tenga que actualizar un cuaderno o Excel a mano.
Cada movimiento de dinero y de producto quede registrado con fecha, motivo y usuario responsable (nada se borra sin dejar rastro).
Al cerrar caja se compare lo que debería haber contra lo que realmente hay, y la diferencia quede documentada.
Cada persona (cajero, almacenero, supervisor, etc.) solo vea y pueda hacer lo que le corresponde a su rol.
¿Cómo lo instalo?

No necesita instalación ni base de datos externa: es un solo archivo index.html que corre directo en el navegador.

Para usarlo localmente:

Descarga el archivo index.html de este repositorio.
Ábrelo con doble clic (se abre en tu navegador: Chrome, Edge, Firefox, etc.).

¿Cómo lo uso?
Al abrir el sistema aparece una pantalla de login: elige tu usuario e ingresa tu PIN.
PIN de prueba para probar cada rol: Administrador 1234 · Supervisor 2345 · Cajero 1111 · Almacenero 2222 · Contador 3333.
Según el rol que uses, verás distintas pestañas:
Vender: busca un producto, agrégalo al carrito y confirma la venta (o guárdala como fiado).
Productos: da de alta productos con precio, costo y stock.
Caja: abre caja con un monto inicial, registra ingresos/egresos, y ciérrala comparando lo esperado contra lo contado.
Historial: revisa ventas pasadas, movimientos de stock (kardex) y cierres de caja anteriores.
Usuarios (solo Administrador): agrega o desactiva usuarios y define su rol.
Los datos quedan guardados en el navegador donde lo uses, así que si cierras la pestaña y vuelves a entrar, todo sigue ahí.
¿Quién lo hizo?

Jeampier Uscata Fernandez, estudiante de Ingeniería de Sistemas.

¿En qué estado está?

Funcional como prototipo / MVP, con las siguientes limitaciones conocidas y a propósito dejadas fuera por ahora:

No emite comprobantes electrónicos ante SUNAT (solo registro interno de ventas).
No soporta múltiples sucursales ni múltiples almacenes.
Cada dispositivo/navegador guarda sus propios datos de forma independiente (no hay un servidor central que sincronice varios dispositivos a la vez).
La autorización de un supervisor para anulaciones o ajustes aún no es un paso obligatorio dentro del flujo — cualquier usuario con el rol adecuado puede hacerlo directamente.

Próximos pasos posibles: backend con base de datos compartida para multi-dispositivo, flujo de autorización de supervisor, y facturación electrónica.
