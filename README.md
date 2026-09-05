# Bases de Datos — sitio Quarto

Primera versión del sitio de estudio para IIC2413, organizada por conceptos y no por clases.

## Requisitos

- [Quarto CLI](https://quarto.org/) instalado.

## Uso local

Desde la raíz del proyecto:

```bash
quarto preview
```

Para generar el sitio completo:

```bash
quarto render
```

El render se escribe en `_site/`, carpeta que está excluida del repositorio.

## Publicación

La publicación en GitHub Pages no se configura automáticamente en esta versión. Después de revisar el contenido y renderizarlo localmente, se puede decidir entre `quarto publish gh-pages` o un workflow de GitHub Actions.

## Estructura

- `fundamentos/`: modelo relacional y relaciones nombradas.
- `teoria-consultas/`: lógica de primer orden y álgebra relacional.
- `sql/`: DDL, DML, consultas, subconsultas y agregación.
- `nulos/`: `NULL`, información incompleta y outer joins.
- `diseno/`: dependencias funcionales, llaves, clausura y descomposiciones.
- `references.bib`: bibliografía central.
- `styles.css`: estilos responsivos del sitio.
