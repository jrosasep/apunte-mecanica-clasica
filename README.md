# Apunte de Mecánica Clásica

Versión modular en formato `book` del apunte de **Mecánica Clásica**.

El proyecto fue reorganizado para que cada capítulo pueda editarse de forma independiente desde la carpeta `chapters/`, manteniendo `main.tex` como archivo principal de compilación.

## Estructura

```text
main.tex
preamble.tex
frontmatter.tex
logo.png
chapters/
figures/
LICENSE
main.pdf
```

## Capítulos

- `chapters/00_introduccion.tex` — Introducción
- `chapters/01_sistema_de_referencia.tex` — Sistema de Referencia
- `chapters/02_sistema_de_coordenadas.tex` — Sistema de Coordenadas
- `chapters/03_bases_coordenados.tex` — Bases Coordenados
- `chapters/04_metrica.tex` — Métrica
- `chapters/05_simbolos_de_christoffel.tex` — Símbolos de Christoffel
- `chapters/06_espacio_vectorial_dual.tex` — Espacio Vectorial Dual
- `chapters/07_operadores_diferenciales_clasicos.tex` — Operadores Diferenciales Clásicos
- `chapters/08_transformaciones_de_coordenadas.tex` — Transformaciones de Coordenadas
- `chapters/09_analisis_tensorial.tex` — Análisis Tensorial
- `chapters/10_mecanica.tex` — Mecánica
- `chapters/11_mecanica_racional.tex` — Mecánica Racional
- `chapters/12_formalismo_lagrangiano.tex` — Formalismo Lagrangiano
- `chapters/13_principio_de_hamilton.tex` — Principio de Hamilton
- `chapters/14_teoria_de_hamilton_jacobi.tex` — Teoría de Hamilton-Jacobi

## Figuras

Las imágenes fueron reorganizadas en una única carpeta:

```text
figures/<nombre_del_capitulo>/
```

Cada capítulo apunta a sus propias figuras mediante rutas del tipo:

```tex
\includegraphics{figures/00_introduccion/fig1.png}
```


## Ajustes visuales aplicados

Esta versión usa una plantilla sobria en blanco y negro. Se eliminaron los bloques de color; las definiciones, ejemplos, proposiciones y observaciones se presentan ahora mediante reglas finas y tipografía limpia.

También se mantuvieron ajustes de paginación para mejorar la lectura del PDF:

- menor separación vertical alrededor de figuras y captions;
- activación de `\raggedbottom` para reducir espacios blancos artificiales;
- ajustes puntuales en ecuaciones largas que producían desbordes horizontales;
- capítulos aún no transcritos marcados como `Capítulo en preparación`, en lugar de quedar visualmente vacíos.

## Compilación

En Overleaf o localmente, el archivo principal debe ser:

```text
main.tex
```

Compilación local:

```bash
pdflatex main.tex
pdflatex main.tex
```

Los capítulos usan `subfiles`, por lo que también pueden abrirse y editarse individualmente.
