# 🕸️ Wikitolica Knowledge Graph

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19091542.svg)](https://doi.org/10.5281/zenodo.19091542)
[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)

Este repositorio gestiona los metadatos y la preservación digital del **Knowledge Graph** de la [Enciclopedia Católica Wikitólica](https://www.wikitolica.com/). Para garantizar la frescura de los datos, el dataset principal se sirve de forma dinámica desde nuestra infraestructura oficial.

## 📊 Acceso a los Datos
Los datos están disponibles en los siguientes puntos de enlace:

- **Dataset Principal (JSON-LD):** [https://www.wikitolica.com/knowledge-graph.jsonld](https://www.wikitolica.com/knowledge-graph.jsonld)
- **Portal de Datos Abiertos:** [https://www.wikitolica.com/d/datos-abiertos/](https://www.wikitolica.com/d/datos-abiertos/)

## 🚀 Cómo consumir los datos
Puedes integrar el grafo en tus proyectos utilizando librerías de Web Semántica como `rdflib` (Python) o `jsonld.js` (JavaScript):

```python
import rdflib

g = rdflib.Graph()
g.parse("[https://www.wikitolica.com/knowledge-graph.jsonld](https://www.wikitolica.com/knowledge-graph.jsonld)", format="json-ld")
print(f"Grafo cargado exitosamente con {len(g)} tripletas.")
```
## ©️ Licencia de Uso
Este conjunto de datos se distribuye bajo la licencia [Creative Commons Atribución-ShareAlike 4.0 Internacional (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/) Usted es libre de compartir y adaptar el material para cualquier propósito, incluso comercial, siempre que otorgue el crédito correspondiente a Wikitólica y sus correspondientes artículos.

## ⚠️ Exención de Responsabilidad
El contenido de este Grafo de Conocimiento se ofrece "tal cual", sin garantías de ningún tipo respecto a su exactitud, integridad o actualidad. Wikitolica es un proyecto independiente y los datos aquí presentados tienen carácter puramente informativo, histórico y cultural. El uso de estos datos para fines teológicos, académicos o comerciales es responsabilidad exclusiva del usuario. Wikitolica se reserva el derecho de modificar o retirar datos sin previo aviso. Al usarlos acepta explícitamente nuestro [aviso legal](https://www.wikitolica.com/a/aviso-legal/).
