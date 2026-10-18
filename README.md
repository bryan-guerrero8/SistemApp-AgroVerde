# SistemApp – AgroVerde S.A.C.

Repositorio académico para la documentación del sistema de inventario y trazabilidad de lotes de AgroVerde S.A.C.

## Objetivo
Organizar los requisitos funcionales y no funcionales, la matriz de trazabilidad, los diagramas y las evidencias de verificación del proyecto.

## Estructura de entrega
- `informe/`: informe de la guía del estudiante en PDF y Word.
- `requisitos/`: especificación breve de requisitos (SRS) y matriz de trazabilidad.
- `evidencias/diagramas/`: diagramas de contexto y proceso exportados.
- `fuentes/`: archivos editables de diagramas/modelado.
- `pruebas/`: criterios de aceptación, casos de prueba y resultados.

## Alcance resumido
El sistema considera autenticación y roles, registro y actualización de lotes, historial de trazabilidad, movimientos de almacén, consulta de stock, asociación de lotes a pedidos de exportación, alertas, reportes, auditoría y sincronización de operaciones sin conexión.

## Requisitos no funcionales destacados
- Seguridad y privacidad mediante roles y auditoría.
- Usabilidad: al menos 4 de cada 5 operadores completan el registro sin ayuda.
- Rendimiento: 95 % de consultas en un máximo de 3 segundos.
- Sincronización: dentro de los 15 minutos posteriores a recuperar la conexión, sin pérdida ni duplicación.

## Estado
Este repositorio se está preparando para la entrega académica. Antes de presentarlo, incorporar los archivos binarios (PDF, DOCX, XLSX e imágenes) en las carpetas correspondientes y comprobar que el PDF final incluya los diagramas.

## Trazabilidad y control de versiones
Conservar los identificadores RF/RNF en los documentos, usar mensajes de commit descriptivos y crear una etiqueta de versión para la entrega revisada.
