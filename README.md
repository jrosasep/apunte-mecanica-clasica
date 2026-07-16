# Apunte de Mecánica Clásica

Este documento en desarrollo tiene la finalidad de recopilar los apuntes del Dr. **Juan Crisóstomo** de los cursos de **Mecánica Clásica 1** y **Mecánica Clásica 2**, con el afan de reorganizar el material y disponer de un archivo editable de este, capricho del autor.

## Contenido

El apunte se organiza en formato `book` y está separado por capítulos editables:

```text
apunte_mecanica_clasica.tex
preamble.tex
frontmatter.tex
chapters/
figures/
logo.png
```

La estructura actual considera:

```text
Parte I   Geometría, coordenadas y herramientas matemáticas
Parte II  Mecánica newtoniana y fuerzas centrales
Parte III Mecánica analítica
Parte IV  Material introductorio para Mecánica Clásica II
```

Algunos capítulos aún están en revisión, especialmente aquellos transcritos desde apuntes manuscritos o desde clases cuya fidelidad debe verificarse contra el material original.

## Compilación

En Overleaf, marcar como archivo principal:

```text
apunte_mecanica_clasica.tex
```

Compilación local recomendada:

```bash
pdflatex apunte_mecanica_clasica.tex
pdflatex apunte_mecanica_clasica.tex
```

También se puede usar `latexmk`:

```bash
latexmk -pdf apunte_mecanica_clasica.tex
```

## Organización de figuras

Las figuras se guardan por capítulo:

```text
figures/<numero_nombre_del_capitulo>/
```

Por ejemplo:

```text
figures/09_mecanica/
figures/10_fuerzas_centrales_binet_kepler/
figures/11_mecanica_racional/
```

Cada capítulo debe citar sus figuras mediante `\label{...}` y `Figura~\ref{...}`.

## Notas de edición

- Los capítulos están en `chapters/` y pueden editarse individualmente.
- El archivo `preamble.tex` contiene la configuración tipográfica y matemática.
- El archivo `frontmatter.tex` contiene portada, nota inicial y elementos preliminares.
- Se recomienda revisar manualmente la fidelidad de cada transcripción antes de considerar el capítulo como terminado.
- Las figuras recortadas pueden ser reemplazadas por versiones mejores manteniendo el mismo nombre de archivo.

## Agradecimientos

Agradezco al Dr. **Juan Crisóstomo** por las clases y por el material base a partir del cual se desarrolla este apunte.

La transcripción, reorganización y edición en LaTeX se ha realizado con asistencia de **ChatGPT** desde el primer semestre del 2025, usado como apoyo para estructurar el documento, convertir contenido a LaTeX, homogeneizar estilo y preparar versiones editables. La revisión final, corrección de errores y responsabilidad sobre el contenido corresponden al autor del repositorio.

## Autor

**José Ignacio Rosas Sepulveda**  
Licenciatura en Ciencias Físicas  
Universidad de Concepción
