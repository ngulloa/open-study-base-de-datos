# Bases de Datos — sitio Quarto

Material académico autónomo de Bases de Datos, organizado por conceptos. Desarrolla el modelo relacional, lógica y álgebra de consultas, SQL, información incompleta y diseño relacional con ejemplos de un dominio universitario ficticio.

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

El render se escribe en `docs/`, según `_quarto.yml`. Esta carpeta forma parte del repositorio y debe actualizarse junto con las fuentes; incluye las páginas HTML, el índice de búsqueda y los recursos del sitio.

## Publicación

Para servir el resultado con GitHub Pages, configura la publicación desde la carpeta `docs/` de la rama elegida. La generación local mediante `quarto render` no publica cambios por sí sola.

## Estructura

- `fundamentos/`: modelo relacional y relaciones nombradas.
- `teoria-consultas/`: lógica de primer orden y álgebra relacional.
- `sql/`: DDL, DML, consultas, subconsultas y agregación.
- `nulos/`: `NULL`, información incompleta y outer joins.
- `diseno/`: dependencias funcionales, llaves, clausura y descomposiciones.
- `references.bib`: las cinco obras académicas de la bibliografía principal.
- `theme.scss`: paleta semántica, tipografía y variables compartidas de Bootstrap/Quarto.
- `styles/`: estilos globales organizados por base, layout, componentes, conceptos y comportamiento responsivo.

La interfaz aprovecha Bootstrap incluido en Quarto, sin dependencias adicionales ni fuentes externas. Conserva el menú colapsable de Quarto por debajo de 992 px, adapta los enlaces y recuadros a una columna en móvil y mantiene el desplazamiento de tablas y fórmulas dentro de sus contenedores. Respeta la preferencia de movimiento reducido y ofrece estados de foco para navegación con teclado.

## Edición y validación

Usa `$...$` para matemática inline y `$$` en líneas propias para bloques. Las fórmulas HTML se procesan con MathJax; revisa tanto la sintaxis como el resultado visual. La [documentación de Quarto sobre ecuaciones](https://quarto.org/docs/authoring/markdown-basics.html#equations) describe estos delimitadores.

Antes de entregar cambios, ejecuta `quarto render`, resuelve errores y advertencias relevantes, comprueba las citas y los enlaces internos, y verifica que `docs/` corresponda a las fuentes actuales. Mantén la exposición autocontenida y las convenciones explícitas; las citas deben respaldar el contenido sin atribuir a los libros decisiones editoriales propias.
