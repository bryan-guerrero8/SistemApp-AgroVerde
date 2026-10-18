# SistemApp – AgroVerde S.A.C.

Repositorio académico para la documentación del sistema de inventario y trazabilidad de lotes de AgroVerde S.A.C.

## Documentación disponible
- [Informe de la guía del estudiante (Markdown)](informe/Informe_Guia_Estudiante_AgroVerde.md)
- [Especificación breve SRS](requisitos/SRS_Breve_SistemApp_AgroVerde.md)
- [Matriz de trazabilidad CSV](requisitos/Matriz_Trazabilidad_AgroVerde.csv)
- [Criterios y casos de prueba](pruebas/criterios_y_casos_de_prueba.md)
- [Control de versiones y pendientes](VERSIONES.md)

## Diagramas
- [Diagrama de contexto SVG](evidencias/diagramas/contexto.svg)
- [Mapa de procesos SVG](evidencias/diagramas/mapa_procesos.svg)
- [Proceso crítico offline SVG](evidencias/diagramas/proceso_critico_offline.svg)
- Fuentes editables Graphviz DOT en evidencias/diagramas/.

## Alcance resumido
Autenticación y roles, registro/actualización de lotes, historial de trazabilidad, movimientos de almacén, consulta de stock, asociación de lotes a pedidos de exportación, alertas, reportes, auditoría y sincronización offline.

## Estado antes de entregar
El informe Markdown, la SRS, la matriz y los diagramas SVG/DOT están publicados. **Aún faltan los archivos binarios finales PDF/DOCX/XLSX y las evidencias reales de pruebas/elicitación**; no se debe considerar la entrega cerrada hasta agregarlos y comprobar que el PDF final contenga los diagramas originales legibles. Los casos de prueba publicados son un plan, no resultados ejecutados.

## Trazabilidad
Mantener IDs RF/RNF consistentes entre SRS, matriz, diagramas y pruebas. Usar mensajes de commit descriptivos y crear la etiqueta final después de revisar todos los archivos.