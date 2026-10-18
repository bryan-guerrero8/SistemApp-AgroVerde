# Especificación breve de requisitos (SRS)

**Proyecto:** SistemApp – AgroVerde S.A.C.  
**Versión:** 1.0 (borrador académico)

## 1. Propósito
Documentar los requisitos principales del sistema de inventario y trazabilidad de lotes de AgroVerde S.A.C., para mejorar el control de existencias, la trazabilidad y la continuidad operativa ante conectividad limitada.

## 2. Alcance
Incluye autenticación y roles, registro y actualización de lotes, historial de trazabilidad, movimientos de almacén, consultas de stock, asociación de lotes disponibles a pedidos de exportación, alertas, reportes, auditoría y sincronización de operaciones realizadas sin conexión.

## 3. Requisitos funcionales
| ID | Requisito resumido | Criterio de aceptación resumido |
|---|---|---|
| RF-01 | Autenticar usuarios | Solo usuarios con credenciales válidas ingresan. |
| RF-02 | Administrar roles y permisos | Las operaciones se limitan según el rol asignado. |
| RF-03 | Registrar lotes | El código es único y los campos obligatorios se validan. |
| RF-04 | Actualizar estado y ubicación de lotes | Se guarda el cambio con fecha y usuario responsable. |
| RF-05 | Consultar trazabilidad histórica | Se visualizan los eventos asociados al lote. |
| RF-06 | Registrar movimientos de almacén | Entradas, salidas y ajustes actualizan el stock. |
| RF-07 | Consultar stock | La consulta devuelve existencias por lote/ubicación. |
| RF-08 | Asociar lotes a pedidos de exportación | Solo se asignan lotes disponibles y suficientes. |
| RF-09 | Alertar por stock insuficiente o discrepancias | Se genera una alerta ante las condiciones definidas. |
| RF-10 | Generar reportes operativos | Los reportes muestran datos coherentes con los registros. |
| RF-11 | Auditar accesos y cambios sensibles | Cada evento auditado identifica usuario, fecha y acción. |
| RF-12 | Guardar y sincronizar operaciones offline | Al reconectar, se sincronizan sin pérdida ni duplicación. |

## 4. Requisitos no funcionales
- **RNF-01 Seguridad y privacidad:** control por roles y auditoría, considerando la Ley peruana N.° 29733 de Protección de Datos Personales.
- **RNF-02 Usabilidad:** interfaz con lenguaje simple, botones visibles e iconos acompañados de texto; al menos 4 de cada 5 operadores completan el registro sin ayuda.
- **RNF-03 Rendimiento:** al menos el 95 % de las consultas se completan en un máximo de 3 segundos.
- **RNF-04 Sincronización:** sincronizar dentro de los 15 minutos posteriores a recuperar la conexión, sin pérdida ni duplicación de operaciones.

## 5. Restricciones y supuestos
- Presupuesto máximo estimado: S/ 80 000.
- Conectividad débil en algunas operaciones.
- Aproximadamente 60 % de los operadores tienen alfabetización digital básica.
- Implementación incremental.
- Fuera del alcance: maquinaria/sensores, contabilidad, facturación, planillas, logística internacional completa e integraciones externas aún no confirmadas.

## 6. Indicadores de éxito
- Al menos 95 % de lotes con trazabilidad completa en el piloto.
- Reducir al menos 50 % las discrepancias de inventario.
- 4 de cada 5 usuarios completan tareas objetivo sin ayuda.
- 100 % de accesos sensibles quedan auditados.

## 7. Trazabilidad y validación
Mantener los IDs RF/RNF en matrices, criterios de aceptación, casos de prueba y evidencias. RF-12 y RNF-03/RNF-04 requieren verificación práctica; la viabilidad de RF-12 y RNF-04 se considera parcial hasta realizar pruebas de sincronización en condiciones reales.

> Este archivo es una versión textual de apoyo. Para la entrega formal, contrastar el contenido con el informe Word/PDF final y anexar las evidencias de validación ejecutadas.