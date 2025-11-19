cat > README.md << 'EOF'
# TFG: Análisis de AWS Marketplace

**Autora:** Julia  
**Director:** [Nombre del profesor]  
**Universidad:** Universidad Politécnica de Valencia  
**Curso:** 2024-2025

## Descripción

Este TFG analiza la estructura y tipología de la oferta en AWS Marketplace mediante un análisis descriptivo basado en datos públicos extraídos mediante web scraping y la API pública de AWS.

## Estructura del proyecto
```
thesis-AWS-marketplace/
├── data/
│   ├── raw/              # Datos sin procesar del scraping
│   └── processed/        # Datos limpios y procesados
├── scripts/              # Scripts de R para scraping y análisis
├── chapters/             # Capítulos del TFG en formato Quarto
├── figures/              # Gráficos y visualizaciones generadas
├── references.bib        # Bibliografía en formato BibTeX
├── _quarto.yml          # Configuración del libro Quarto
└── README.md            # Este archivo
```

## Requisitos

### R y paquetes necesarios
```r
install.packages(c(
  "tidyverse",   # Manipulación y visualización de datos
  "rvest",       # Web scraping
  "httr",        # Llamadas HTTP/API
  "jsonlite",    # Trabajar con JSON
  "RSelenium",   # Scraping dinámico (si es necesario)
  "tidytext",    # Análisis de texto
  "wordcloud2",  # Visualización de palabras
  "quarto"       # Generación del documento
))
```

## Uso

### Ejecutar scraping
```bash
Rscript scripts/01_scraping.R
```

### Compilar el TFG

En RStudio:
```r
quarto::quarto_render()
```

O desde terminal:
```bash
quarto render
```

## Log de actividades

- **2025-11-19**: Configuración inicial del repositorio y estructura del proyecto
- **2025-11-19**: Inicio exploración de AWS Marketplace

## Contacto

Para cualquier duda sobre este proyecto, contactar a [tu email]
EOF