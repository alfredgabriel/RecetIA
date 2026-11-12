<p align="center">
  <img src="logo.png" alt="Logo de RecetIA" width="140">
</p>

# RecetIA

Mini asistente RAG de recetas en español con detección de alérgenos, búsqueda híbrida en **ChromaDB**, generación local con **Qwen3 (`qwen3:1.7b` vía Ollama)** y una interfaz web sencilla en **Flask**.

**Equipo:** Alfred, Ane y Naiara

## Contenido del repositorio
- `main2.ipynb` — Versión final limpia y comentada (20.012 recetas, búsqueda híbrida, reverificación condicional, métricas BLEU/fidelidad y web Flask).
- `main.ipynb` — Notebook inicial de pruebas.
- `RecetIA_presentacion_v2.pptx` — Presentación del proyecto (5 diapositivas).

## Cómo ejecutarlo en local
1. Instalar dependencias de Python (`datasets`, `pandas`, `sentence-transformers`, `chromadb`, `ollama`, `flask`).
2. Tener **Ollama** activo en local con el modelo `qwen3:1.7b` descargado (`ollama pull qwen3:1.7b`).
3. Ejecutar las celdas de `main2.ipynb` en orden (la primera ejecución crea la carpeta `chroma_recetas_20k/` en local).
4. Al ejecutar la celda de Flask, abrir `http://localhost:5000` en el navegador.

