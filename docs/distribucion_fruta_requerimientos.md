# Análisis y requerimientos y propuesta de solucion tecnica
## Grupo tutifruti - distribución de fruta al por mayor 
## Contexto del negocio
Empresa dedicada a la distribución de fruta y verdura al por mayor. Actualmente, el registro de facturas y guías de despacho se llena de forma manual, combinando cuadernos fisicos y planillas excel.
Esta forma de trabajo ha generado  múltiples problemas operativos que afetan directamente la eficiecia y la toma de decisiones del negocio.
## Problemas identificados
- perdida frecuente de documentos fisicos( facturas y guias de despacho)
- dificultad para buscar ventas antiguas por falta de un registro centralizado.
- ausencia de control de stock, lo que provoca ventas de productos sin existencias.
- calculo manual de ganancias mensuales, proceso lento y propenso a errores.
- falta de informacion sobre clientes frecuentes y productos vendidos.
- errores de digitacion por parte de los trabajadores al registrar datos.
- inexistencia de respaldo de la informacion, con riesgo de perdida total de datos.

## Analisis de requerimientos 
### Requerimientos funcionales:
1. El sistema debe permitir registrar facturas de ventas con datos del cliente, productos, cantidades y precios.
2. El sistema debe permitir registrar guias de despacho asociadas a cada venta realizada.
3. El sistema debe permitir el ingreso y actualizacion de productos en stock ( fruta y verdura)
4. el sistema debe descontar automaticamente del stock los productos vendidos al emitir un factura.
5. el sistema debe impedir la vemta de productos sin stock disponible, mostrando una alerta.
6. el sitema debe permitir buscar y filtar ventas historicas por fecha, cliente o producto.
7. el sistema debe calcular automaticamente las ganancias mensuales en base a las ventas registras
8. el sistema debe generar un reporte del producto mas vendido en un periodo determinado
9. el sistema debe generar un reporte de los clientes con mayor volumen de compra.
10. el sistema debe permitir la gestion de ususios( trabajadores) con distintos niveles de acceso.
### Requerimientos no funcionales 
1.El sistema debe realizar copias de seguridad (backups) automáticas de la base de datos diariamente y en la nube, garantizando que en caso de fallo el tiempo de recuperación de información no supere las 2 horas.
2.La interfaz de usuario debe incluir validaciones de campo en tiempo real (mínimos, máximos, formatos de texto/número) e interfaces intuitivas para reducir los errores de digitación de los trabajadores en al menos un 90%.
3.Las búsquedas y filtrados de ventas históricas, así como la generación de reportes mensuales de ganancias o productos más vendidos, deben ejecutarse y desplegarse en pantalla en un tiempo menor a 3 segundos.
4.El sistema debe implementar un control de acceso basado en roles (RBAC) con autenticación segura (contraseñas encriptadas), asegurando que solo los usuarios autorizados puedan modificar stock o acceder a reportes financieros.
5.El sistema debe actualizar el inventario de frutas y verduras en tiempo real y manejar transacciones concurrentes para evitar discrepancias de stock entre múltiples usuarios registrados simultáneamente.




