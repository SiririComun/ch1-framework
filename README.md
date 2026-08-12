# Capítulo 1: Marco de Trabajo (Framework)
**Tesis de Grado en Física — Universidad de Antioquia (UdeA)**

Este repositorio contiene las fuentes en LaTeX del Capítulo 1 (*Marco de Trabajo*), desarrollado de forma modular e independiente.

---

## 🛠️ Compilación Local

### **Requisitos Previos**
Asegúrese de tener instalado **TeX Live** con soporte para `spanish` y `biber`:

```bash
# En Tuxedo OS / Ubuntu / Debian
sudo apt update
sudo apt install -y texlive-latex-extra texlive-science texlive-lang-spanish biber latexmk
```

### **Comandos de Compilación**

Para compilar el capítulo de forma independiente:

```bash
# 1. Compilación limpia completa (pdflatex + biber)
latexmk -pdf ch1_framework.tex

# 2. Limpiar archivos auxiliares temporales
latexmk -C
```

El archivo compilado se generará localmente como **`ch1_framework.pdf`**.

---

## 📁 Estructura del Repositorio
* `ch1_framework.tex`: Código fuente del capítulo (compatible con `subfiles`).
* `standalone.tex`: Plantilla local para compilación independiente.
* `references.bib`: Base de datos de referencias bibliográficas.
* `figures/`: Diagramas e imágenes de bloques y resultados.