# Guía del estudiante – Tema 1
## SistemApp: inventario y trazabilidad para AgroVerde S.A.C.

**Estudiante:** Bryan Manuel Guerrero Guillén  
**Versión documental:** 1.0 – borrador para revisión  
**Fecha:** 18 de octubre de 2026

> Los casos de prueba se proponen como plan. No se declaran aprobados hasta ejecutar pruebas y adjuntar evidencia real.

## 1. Objetivo
Organizar la identificación y análisis de requisitos de SistemApp y mantener trazabilidad entre requisitos, modelos, criterios de aceptación y evidencias.

## 2. Contexto y alcance
AgroVerde S.A.C. requiere controlar el registro y movimiento de lotes, su ubicación y estado, stock y trazabilidad relacionada con pedidos de exportación. Se considera conectividad débil y distintos niveles de experiencia digital entre operadores.

**Incluido:** autenticación y roles; registro y actualización de lotes; historial; entradas, salidas y ajustes de almacén; consulta de stock; asociación a pedidos; alertas; reportes; auditoría; almacenamiento y sincronización offline.

**Fuera de alcance:** maquinaria/sensores, contabilidad, facturación, planillas, logística internacional completa e integraciones externas no confirmadas.

**Restricciones:** presupuesto máximo estimado S/ 80 000; conectividad limitada; aproximadamente 60 % de operadores con alfabetización digital básica; implementación incremental. Considerar la Ley peruana N.° 29733 de Protección de Datos Personales.

## 3. Procedimiento
1. Revisar contexto, actores y proceso crítico.
2. Organizar las necesidades recogidas en entrevistas y encuesta con sus identificadores.
3. Clasificar requisitos funcionales (RF) y no funcionales (RNF).
4. Definir criterios de aceptación verificables.
5. Relacionar requisitos con diagramas, matriz y casos de prueba.
6. Analizar consistencia, restricciones, riesgos y verificaciones pendientes.
7. Mantener cambios mediante commits descriptivos y versionado.

## 4. Requisitos y aceptación
| ID | Requisito | Criterio de aceptación |
|---|---|---|
| RF-01 | Autenticación | Credenciales válidas permiten ingresar; inválidas se rechazan. |
| RF-02 | Roles y permisos | Cada rol ejecuta solo acciones autorizadas. |
| RF-03 | Registro de lotes | Código único y validación de campos obligatorios. |
| RF-04 | Actualizar estado/ubicación | Cambio guarda fecha y usuario responsable. |
| RF-05 | Historial de trazabilidad | Se muestran eventos asociados al lote. |
| RF-06 | Movimientos de almacén | Entradas, salidas y ajustes actualizan existencias. |
| RF-07 | Consulta de stock | Muestra existencias por lote y ubicación. |
| RF-08 | Asociación a pedidos | Solo lotes disponibles y suficientes se asignan. |
| RF-09 | Alertas | Se alerta ante stock insuficiente o discrepancias definidas. |
| RF-10 | Reportes | Resultados coherentes con los registros. |
| RF-11 | Auditoría | Evento registra usuario, fecha y acción sensible. |
| RF-12 | Operación offline | Sincronización sin pérdida ni duplicación. |
| RNF-01 | Seguridad/privacidad | Roles y auditoría protegen datos y operaciones. |
| RNF-02 | Usabilidad | 4 de 5 operadores completan el registro sin ayuda. |
| RNF-03 | Rendimiento | 95 % de consultas en máximo 3 segundos. |
| RNF-04 | Sincronización | Dentro de 15 minutos tras reconexión, sin pérdida ni duplicación. |

## 5. Evidencias y trazabilidad
La matriz en requisitos/Matriz_Trazabilidad_AgroVerde.csv relaciona RF/RNF con criterios y evidencias sugeridas. El archivo pruebas/criterios_y_casos_de_prueba.md propone casos de prueba; deben ejecutarse y documentarse. evidencias/diagramas/ contiene fuentes DOT y diagramas SVG. requisitos/SRS_Breve_SistemApp_AgroVerde.md presenta la especificación resumida.

Para cada prueba registrar fecha, versión, datos de entrada, resultado esperado y observado, captura o archivo de evidencia e incidencias. Mantener los identificadores RF/RNF consistentes en todos los artefactos.

## 6. Análisis de resultados
La cobertura documental conecta el registro y actualización de lotes (RF-03/04), movimientos y consultas de stock (RF-06/07), trazabilidad y pedidos (RF-05/08), y funciones de control (RF-09/10/11). RF-12 y RNF-04 responden a la conectividad limitada.

**Brechas:** rendimiento, usabilidad y sincronización requieren pruebas prácticas; los diagramas de este repositorio deben contrastarse con los diagramas originales del expediente; entrevistas, encuesta y decisiones ponderadas deben adjuntarse si la guía los exige.

**Riesgos:** conflictos de cambios offline, duplicación de movimientos, permisos insuficientes, datos incompletos y baja adopción. **Mejoras:** identificadores únicos de operación, sincronización idempotente, bitácora de cambios, resolución explícita de conflictos y pruebas piloto con operadores.

## 7. Conclusiones
1. La especificación recoge las funciones centrales de inventario y trazabilidad y propone criterios iniciales verificables.
2. La matriz mejora la trazabilidad, pero no sustituye las pruebas reales de rendimiento, usabilidad y sincronización.
3. Antes de entregar, se deben contrastar los diagramas con el documento original, anexar evidencias de elicitación y publicar PDF/Word finales legibles.

## 8. Fuentes
- Documento de proyecto AgroVerde – Pasos 1, 2 y 3, proporcionado para el trabajo.
- Guía de estudiante del Tema 1, proporcionada para el trabajo.
- Perú, Ley N.° 29733, Ley de Protección de Datos Personales (consultar texto oficial vigente).

## 9. Lista de control previa a la entrega
- [ ] Exportar este informe revisado a PDF.
- [ ] Adjuntar Word editable y matriz Excel/CSV según la indicación docente.
- [ ] Verificar que los diagramas originales estén visibles y legibles en el PDF.
- [ ] Adjuntar registros de entrevistas/encuesta y pruebas realmente ejecutadas.
- [ ] Confirmar curso, sección y fecha con la ficha de la asignatura.
- [ ] Revisar ortografía, fuentes y consistencia de IDs.
- [ ] Etiquetar versión final solo después de revisar todos los archivos.