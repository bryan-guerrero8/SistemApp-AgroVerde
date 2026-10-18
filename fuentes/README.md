# Fuentes editables

Los diagramas de este repositorio están en formato Graphviz DOT dentro de `evidencias/diagramas/`. Se pueden editar como texto y exportar a PNG o SVG con Graphviz instalado.

Ejemplo de exportación:

```bash
dot -Tpng evidencias/diagramas/contexto.dot -o evidencias/diagramas/contexto.png
dot -Tsvg evidencias/diagramas/contexto.dot -o evidencias/diagramas/contexto.svg
```

Estos archivos DOT son fuentes editables de los diagramas, no un archivo de proyecto nativo de Modelio.