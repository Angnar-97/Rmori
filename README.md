# Rmori

<p align="center">
  <img src="images/rmori2.png" alt="Rmori cover" width="900"/>
</p>

---

## Qué es Rmori

**Rmori** es una web construida en Quarto que actúa como repositorio estructurado de conocimiento en torno a:

- R
- Python
- Bases de datos
- Bioinformática
- Ciencia de datos aplicada

El proyecto nace de una necesidad concreta: disponer de un entorno donde los recursos no estén dispersos, sino organizados de forma coherente, navegable y útil en contextos reales de trabajo.

El nombre combina:

- **R**, como núcleo del ecosistema analítico  
- **Mori (森)**, “bosque” en japonés  

Esto no es solo un naming estético. Define la arquitectura conceptual del proyecto:

Rmori funciona como un bosque donde cada recurso es un nodo conectado con otros, permitiendo navegar el conocimiento de forma progresiva y contextual.

---

## Problema que resuelve

El ecosistema de data science y bioinformática tiene un problema recurrente:

- exceso de recursos sin jerarquía  
- listas sin contexto ni aplicación práctica  
- fragmentación entre tecnologías  
- dificultad para reutilizar conocimiento  

Rmori aborda este problema mediante:

- estructuración por dominio funcional  
- curaduría basada en uso real  
- organización transversal entre tecnologías  
- acceso rápido a herramientas relevantes  

El objetivo no es recopilar todo, sino **seleccionar lo que realmente importa**.

---

## Arquitectura del contenido

El contenido de Rmori no está organizado de forma arbitraria, sino siguiendo una lógica de uso en proyectos reales.

### R

El bloque de R se centra en el análisis, modelización y visualización, con especial atención a entornos científicos y biomédicos.

Incluye:

- **Bioconductor**  
  Librerías para análisis ómico (RNA-seq, metagenómica, etc.), con herramientas como DESeq2, edgeR o phyloseq.  
  Orientado a flujos de análisis reproducibles en biología computacional.

- **Visualización**  
  Paquetes para representación avanzada de datos, desde ggplot2 hasta librerías especializadas para gráficos estadísticos y biomédicos.

- **Estadística y modelización**  
  Métodos clásicos y modernos aplicados a datos reales, incluyendo regresión, modelos mixtos y análisis multivariante.

- **Shiny**  
  Desarrollo de aplicaciones interactivas para visualización y explotación de datos.

- **Quarto**  
  Generación de informes reproducibles, presentaciones y sitios web.

- **Mapas e imágenes**  
  Herramientas para análisis espacial y procesamiento de imágenes.

Este bloque está orientado a convertir datos en conocimiento interpretable.

---

### Python

El bloque de Python complementa a R en áreas donde su ecosistema es especialmente fuerte.

Incluye:

- **Análisis exploratorio**  
  Uso de pandas, numpy y librerías asociadas para manipulación de datos.

- **Series temporales**  
  Modelos y herramientas para análisis longitudinal.

- **SQL integrado**  
  Uso de Python como capa de acceso a bases de datos.

- **Validación de datos**  
  Frameworks para asegurar consistencia y calidad de datos.

- **Calidad de código**  
  Herramientas de linting, testing y buenas prácticas.

- **Documentación**  
  Generación de documentación técnica estructurada.

- **Integración R + Python**  
  Interoperabilidad entre ambos lenguajes en pipelines analíticos.

Este bloque posiciona Python como herramienta de ingeniería y soporte analítico.

---

### Bases de datos

Uno de los bloques más diferenciales de Rmori.

No se limita a listar datasets, sino que los organiza por dominio científico y aplicabilidad.

Incluye:

- **Socioeconómicas**  
  Datos poblacionales, económicos y demográficos.

- **Salud y demografía**  
  Fuentes clave para análisis epidemiológico y clínico.

- **Genómica**  
  Repositorios de secuencias y anotaciones genéticas.

- **Transcriptómica**  
  Expresión génica y datasets RNA-seq.

- **Proteómica y metabolómica**  
  Datos funcionales de sistemas biológicos.

- **Interacciones moleculares**  
  Redes proteína-proteína, pathways y sistemas complejos.

- **Organismos modelo**  
  Bases específicas para investigación experimental.

- **Variantes y cáncer**  
  Bases de datos clínicas y genómicas aplicadas a oncología.

Este bloque convierte Rmori en un punto de entrada real a datos científicos.

---

### Recursos adicionales

Este bloque amplía el alcance del proyecto más allá de herramientas puramente técnicas.

Incluye:

- **Herramientas de inteligencia artificial**  
  Plataformas y librerías relevantes para análisis avanzado.

- **Libros**  
  Referencias clave para formación estructurada.

- **Comunidades y competiciones**  
  Espacios donde aprender, compartir y validar conocimientos.

- **Referentes**  
  Personas y proyectos relevantes dentro del ecosistema.

Su función es aportar contexto, no solo herramientas.

---

## Stack tecnológico

Rmori está construido sobre un stack minimalista y reproducible:

- **Quarto** → generación del sitio web  
- **R** → entorno base  
- **renv** → gestión de dependencias  
- **SCSS / CSS** → personalización visual  

Este stack permite:

- reproducibilidad  
- portabilidad  
- mantenimiento sencillo  
- integración con workflows analíticos  

---

## Estructura del repositorio

```text
.
├── _quarto.yml           # Configuración global del sitio
├── index.qmd            # Página principal
├── about.qmd            # Información del proyecto
├── styles.css           # Estilos personalizados
├── theme-dark.scss      # Tema visual
├── r_pages/             # Contenido relacionado con R
├── python_pages/        # Contenido relacionado con Python
├── bd_pages/            # Bases de datos
├── recursos_pages/      # Recursos adicionales
├── images/              # Imágenes del sitio
├── renv/                # Entorno reproducible
├── renv.lock            # Snapshot de dependencias
└── _site/               # Sitio renderizado