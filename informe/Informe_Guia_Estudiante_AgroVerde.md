# Guía del estudiante – Tema 1
## SistemApp: inventario y trazabilidad para AgroVerde S.A.C.

**Estudiante:** Bryan Manuel Guerrero Guillén  
**Versión documental:** 1.0  
**Fecha:** 18 de octubre de 2026

## 1. Objetivo
Organizar la identificación y análisis de requisitos de SistemApp y establecer trazabilidad entre requisitos, modelos, criterios de aceptación y evidencias.

## 2. Contexto y alcance
AgroVerde S.A.C. requiere controlar el registro y movimiento de lotes, su ubicación y estado, las existencias y la trazabilidad relacionada con pedidos de exportación. El sistema considera conectividad débil y distintos niveles de experiencia digital entre operadores.

**Incluido:** autenticación y roles; registro y actualización de lotes; historial; entradas, salidas y ajustes de almacén; consulta de stock; asociación a pedidos; alertas; reportes; auditoría; almacenamiento y sincronización offline.

**Fuera de alcance:** maquinaria y sensores, contabilidad, facturación, planillas, logística internacional completa e integraciones externas no confirmadas.

**Restricciones:** presupuesto máximo estimado de S/ 80 000; conectividad limitada; aproximadamente 60 % de operadores con alfabetización digital básica; implementación incremental. Se considera la Ley peruana N.° 29733 de Protección de Datos Personales.

## 3. Procedimiento desarrollado
1. Identificación del contexto, los actores y el proceso crítico.
2. Organización de necesidades obtenidas mediante entrevistas y encuesta.
3. Clasificación de requisitos funcionales (RF) y no funcionales (RNF).
4. Definición de criterios de aceptación verificables.
5. Relación entre requisitos, diagramas, matriz de trazabilidad y casos de prueba.
6. Análisis de consistencia, restricciones, riesgos y verificaciones pendientes.
7. Organización de los artefactos mediante control de versiones.

## 4. Requisitos y criterios de aceptación
| ID | Requisito | Criterio de aceptación |
|---|---|---|
| RF-01 | Autenticación | Credenciales válidas permiten ingresar; inválidas se rechazan. |
| RF-02 | Roles y permisos | Cada rol ejecuta solo acciones autorizadas. |
| RF-03 | Registro de lotes | Código único y validación de campos obligatorios. |
| RF-04 | Actualizar estado y ubicación | El cambio guarda fecha y usuario responsable. |
| RF-05 | Historial de trazabilidad | Se muestran eventos asociados al lote. |
| RF-06 | Movimientos de almacén | Entradas, salidas y ajustes actualizan existencias. |
| RF-07 | Consulta de stock | Muestra existencias por lote y ubicación. |
| RF-08 | Asociación a pedidos | Solo lotes disponibles y suficientes se asignan. |
| RF-09 | Alertas | Se alerta ante stock insuficiente o discrepancias definidas. |
| RF-10 | Reportes | Los resultados son coherentes con los registros. |
| RF-11 | Auditoría | El evento registra usuario, fecha y acción sensible. |
| RF-12 | Operación offline | La sincronización ocurre sin pérdida ni duplicación. |
| RNF-01 | Seguridad y privacidad | Roles y auditoría protegen datos y operaciones. |
| RNF-02 | Usabilidad | 4 de 5 operadores completan el registro sin ayuda. |
| RNF-03 | Rendimiento | 95 % de consultas en máximo 3 segundos. |
| RNF-04 | Sincronización | Dentro de 15 minutos tras reconexión, sin pérdida ni duplicación. |

## 5. Evidencias y trazabilidad
La matriz de trazabilidad relaciona RF/RNF con criterios y evidencias. El archivo de criterios y casos de prueba describe las verificaciones previstas. La carpeta de diagramas contiene los modelos de contexto, procesos y proceso crítico offline, además de sus fuentes editables. La especificación breve SRS resume el propósito, alcance, requisitos y restricciones del sistema.

Los casos de prueba se encuentran pendientes de ejecución y documentación. Por ello, los criterios de rendimiento, usabilidad y sincronización no se consideran validados mediante pruebas prácticas.

## 6. Análisis de resultados
La cobertura documental conecta el registro y actualización de lotes (RF-03/RF-04), los movimientos y consultas de stock (RF-06/RF-07), la trazabilidad y los pedidos (RF-05/RF-08), y las funciones de control (RF-09/RF-10/RF-11). RF-12 y RNF-04 responden a las limitaciones de conectividad.

**Brechas identificadas:** rendimiento, usabilidad y sincronización requieren pruebas prácticas. Los diagramas publicados representan los procesos propuestos y deben interpretarse como artefactos de modelado, no como evidencia de software implementado. La validación de requisitos depende de contrastar las necesidades identificadas con las partes interesadas.

**Riesgos:** conflictos de cambios offline, duplicación de movimientos, permisos insuficientes, datos incompletos y baja adopción. Entre las oportunidades de mejora se encuentran el uso de identificadores únicos de operación, sincronización idempotente, bitácora de cambios, resolución explícita de conflictos y pruebas piloto con operadores.

## 7. Conclusiones
1. La especificación reúne las funciones principales de inventario y trazabilidad y define criterios iniciales de aceptación.
2. La matriz de trazabilidad facilita relacionar requisitos, modelos y verificaciones; sin embargo, no reemplaza las pruebas prácticas.
3. La operación offline constituye un aspecto crítico por la conectividad limitada y requiere validación en condiciones representativas.