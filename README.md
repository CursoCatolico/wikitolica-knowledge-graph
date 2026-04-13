# 🕸️ Wikitolica Knowledge Graph

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19091541.svg)](https://doi.org/10.5281/zenodo.19091541)
[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)

Este repositorio gestiona los metadatos y la preservación digital del **Knowledge Graph** de la [Enciclopedia Católica Wikitólica](https://www.wikitolica.com/). Para garantizar la frescura de los datos, el dataset principal se sirve de forma dinámica desde nuestra infraestructura oficial.

## 📊 Acceso a los Datos
Los datos están disponibles en los siguientes puntos de enlace:

- **Dataset Principal (JSON-LD):** [https://www.wikitolica.com/knowledge-graph.jsonld](https://www.wikitolica.com/knowledge-graph.jsonld)
- **Portal de Datos Abiertos:** [https://www.wikitolica.com/d/datos-abiertos/](https://www.wikitolica.com/d/datos-abiertos/)
- **Visualizador Online:** [https://www.wikitolica.com/visualizador/](https://www.wikitolica.com/visualizador/)

## 🚀 Cómo consumir los datos
Puedes integrar el grafo en tus proyectos utilizando librerías de Web Semántica como `rdflib` (Python) o `jsonld.js` (JavaScript):

```python
# You need to open the console and install requests and pyld using:
# pip install requests
# pip install pyld

from pyld import jsonld
import requests

url = "https://www.wikitolica.com/knowledge-graph.jsonld"
doc = requests.get(url).json()

expanded = jsonld.expand(doc)
print(f"Documento expandido con {len(expanded)} nodos.")
```

## 🙏 Sobre el proyecto

La [Enciclopedia Católica Wikitólica](https://www.wikitolica.com/) Wikitólica busca acercar la riqueza de la tradición litúrgica de la Iglesia a la web moderna, manteniendo fidelidad, claridad y accesibilidad.

## ©️ Licencia de Uso
Este conjunto de datos se distribuye bajo la licencia [Creative Commons Atribución-ShareAlike 4.0 Internacional (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/) Usted es libre de compartir y adaptar el material para cualquier propósito, incluso comercial, siempre que otorgue el crédito correspondiente a Wikitólica y sus correspondientes artículos.

## ⚠️ Exención de Responsabilidad
El contenido de este Grafo de Conocimiento se ofrece "tal cual", sin garantías de ningún tipo respecto a su exactitud, integridad o actualidad. Wikitolica es un proyecto independiente y los datos aquí presentados tienen carácter puramente informativo, histórico y cultural. El uso de estos datos para fines teológicos, académicos o comerciales es responsabilidad exclusiva del usuario. Wikitolica se reserva el derecho de modificar o retirar datos sin previo aviso. Al usarlos acepta explícitamente nuestro [aviso legal](https://www.wikitolica.com/a/aviso-legal/).

<p align="center">
  Un proyecto de <a href="https://www.wikitolica.com"><strong>Wikitólica</strong></a> — La Enciclopedia Católica en español
</p>
