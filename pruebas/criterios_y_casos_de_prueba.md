# Criterios de aceptación y casos de prueba

**Estado:** plan de pruebas propuesto; las ejecuciones están pendientes.

| Caso | Requisitos | Pasos resumidos | Resultado esperado | Estado |
|---|---|---|---|---|
| CP-01 Inicio de sesión | RF-01 | Probar credenciales válidas e inválidas | Permite acceso válido y rechaza inválido | Pendiente |
| CP-02 Permisos | RF-02, RNF-01 | Intentar una acción con roles distintos | Solo el rol autorizado ejecuta la acción | Pendiente |
| CP-03 Alta de lote | RF-03 | Registrar lote con campos vacíos y código repetido | La validación impide datos incompletos/duplicados | Pendiente |
| CP-04 Actualización | RF-04 | Cambiar estado y ubicación | El cambio queda registrado con usuario y fecha | Pendiente |
| CP-05 Trazabilidad | RF-05 | Abrir historial de lote con eventos | Se muestran eventos ordenados y asociados | Pendiente |
| CP-06 Movimientos | RF-06, RF-07 | Registrar entrada, salida y ajuste | El stock resultante coincide con las operaciones | Pendiente |
| CP-07 Pedido de exportación | RF-08 | Asignar lote disponible y luego lote insuficiente | Se permite asignación válida y se rechaza la insuficiente | Pendiente |
| CP-08 Alertas y reportes | RF-09, RF-10 | Provocar discrepancia y generar reporte | Se genera la alerta y el reporte refleja los datos | Pendiente |
| CP-09 Auditoría | RF-11 | Realizar operación sensible | Se registra usuario, fecha y acción | Pendiente |
| CP-10 Sin conexión | RF-12, RNF-04 | Registrar offline, reconectar y repetir sincronización | Sin pérdida ni duplicación; sincroniza en 15 minutos | Pendiente |
| CP-11 Rendimiento | RNF-03 | Medir consultas representativas | 95 % completan en máximo 3 segundos | Pendiente |
| CP-12 Usabilidad | RNF-02 | Observar a cinco operadores al registrar un lote | Al menos cuatro completan sin ayuda | Pendiente |

## Evidencias de validación
Las evidencias de cada ejecución deben incluir fecha, versión evaluada, datos de prueba, resultado esperado y observado, incidencias y su resolución.