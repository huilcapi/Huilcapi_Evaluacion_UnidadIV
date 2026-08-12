# Prueba Práctica — Unidad IV — Ingeniería de Requisitos (ISR-401)

Repositorio con el desarrollo de las actividades prácticas P1–P7 del caso
"Sistema de Gestión de Pedidos".

## Archivo principal

- `prueba_isr401.tex`

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

Desde la raíz del repositorio, ejecutar:

```bash
pdflatex -interaction=nonstopmode prueba_isr401.tex
```

El PDF resultante (`prueba_isr401.pdf`) se genera en el mismo
directorio.

## Instalación de dependencias (Ubuntu/Debian)

Si `pdflatex` no está instalado o falta el soporte de español:

```bash
sudo apt-get update
sudo apt-get install -y texlive-latex-extra texlive-lang-spanish texlive-pictures
```

