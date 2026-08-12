# Huilcapi_Evaluacion_UnidadIV

Prueba Práctica — Unidad IV — Ingeniería de Requerimientos (ISR-401)
Universidad Técnica Estatal de Quevedo

**Estudiante:** Huilcapi Leon Denisses Fabiola
**Docente:** Ing. Guerrero Ulloa Gleiston Ciceron

## Estructura del repositorio

```
├── figs/          # imágenes usadas por el documento (logo, capturas del SGA)
├── main.tex       # archivo principal LaTeX
├── Prueba.pdf     # PDF compilado
└── readme.md      # este archivo
```

## Archivo principal

- `main.tex`

## Compilador

- `pdflatex` (TeX Live 2023 o superior)

## Dependencias (paquetes LaTeX)

- `inputenc`
- `babel` (opción `spanish`, `es-noshorthands`)
- `fontenc` (T1)
- `times`
- `geometry`
- `tikz` (librerías: `shapes`, `arrows.meta`, `positioning`, `fit`, `backgrounds`, `shapes.multipart`, `calc`)
- `booktabs`
- `longtable`
- `array`
- `xcolor`
- `hyperref`
- `enumitem`
- `graphicx`

Todos estos paquetes están incluidos en una distribución TeX Live completa
(`texlive-full`) o en el esquema `texlive-latex-extra` +
`texlive-lang-spanish` (necesario para `babel-spanish`) +
`texlive-pictures` (necesario para `tikz`).

## Orden de compilación

Clonar el repositorio y, desde su raíz (donde están `main.tex` y la carpeta
`figs/`), ejecutar:

```bash
pdflatex -interaction=nonstopmode main.tex
```

El PDF resultante (`main.pdf`) se genera en el mismo directorio; el
entregado en el repositorio corresponde a `Prueba.pdf`.

## Instalación de dependencias (Ubuntu/Debian)

Si `pdflatex` no está instalado o falta el soporte de español:

```bash
sudo apt-get update
sudo apt-get install -y texlive-latex-extra texlive-lang-spanish texlive-pictures
```

