# Lab8-RAG

## Descripción

Este repositorio contiene un proyecto que implementa un sistema de Recuperación de Respuestas (RAG, por sus siglas en inglés) utilizando el framework `langchain`. El proyecto se enfoca en la integración de una solución que combina la búsqueda y la generación de respuestas, utilizando modelos preentrenados y fuentes externas como sitios web.

## Requisitos

Para ejecutar este proyecto, necesitas instalar las siguientes dependencias:

- `langchain`
- `langchain_community`
- `bs4`
- `requests`
- `openai`
- `IPython`

Puedes instalar las dependencias ejecutando:

```bash
pip install -r requirements.txt
```

## USOS

1. Cargar y dividir contenido: El proyecto carga contenido desde una página web específica, lo divide en fragmentos utilizando RecursiveCharacterTextSplitter, y los guarda en un almacén de vectores.

2. Definir el prompt para la respuesta: Se utiliza un prompt predefinido de hub para la generación de respuestas.

3. Estructura del estado: La aplicación define un tipo de estado que contiene la pregunta, el contexto y la respuesta generada.

4. Flujo de ejecución: Se define un flujo de pasos que incluye la recuperación de documentos relevantes y la generación de respuestas, todo controlado por un StateGraph.

Ejecución
Para ejecutar el flujo de trabajo, simplemente ejecuta el código en un entorno compatible con IPython y asegúrate de tener configurada correctamente tu clave de API de OpenAI para la generación de respuestas.

```bash
from IPython.display import Image, display

display(Image(graph.get_graph().draw_mermaid_png()))
```
