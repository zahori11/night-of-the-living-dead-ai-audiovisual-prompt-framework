#  Comunity_Cut
# 🎬 Marco Audiovisual con IA: La Noche de los Muertos Vivientes

¡Bienvenido al set de rodaje! Este repositorio organiza indicaciones, flujos de trabajo y recursos audiovisuales de IA para usar **LTX-2** y reanimar escenas clásicas con el estilo que prefieras. 

Fotorrealista, abstracto, surrealista, pintado a mano o, nuestro enfoque principal: **Pixel Art de 1-bit retro (estilo Game Boy Noir)**. Tú decides la interpretación. 

Usa [ComfyUI](https://github.com/comfyanonymous/ComfyUI), el modelo de código abierto LTX-2, o la API de LTX Studio. ¡Siempre que funcione con LTX-2, estás dentro!

---

## 📁 Estructura del Estudio (Repositorio)

Para mantener la producción ordenada, el proyecto se divide en los siguientes departamentos:

* **`📁 guiones_tecnicos/`**: Desgloses de producción. Aquí encontrarás documentos detallados fotograma a fotograma (tiempos, acciones, recortes) para replicar la sincronización exacta de cada toma.
* **`📁 flujos_comfyui/`**: El cerebro de la operación. Archivos `.json` listos para arrastrar y soltar en ComfyUI, incluyendo flujos avanzados de multi-prompting y anclaje de imágenes guía (`LTXVAddGuide`).
* **`📁 prompts_y_textos/`**: El departamento de guion. Colección de *prompts* positivos y nuestros escudos de *prompts* negativos (diseñados específicamente para bloquear el suavizado y proteger la estética de 1-bit).
* **`📁 recursos_visuales/`**: La sala de montaje. Contiene los fotogramas extraídos de las generaciones (`pixelart_clip_frames`) listos para ser ensamblados, además de recursos gráficos adicionales como marcos de máquinas arcade.

---

## 🚀 Cómo Empezar a Rodar

1. **Clona o descarga** este repositorio en tu ordenador.
2. Abre **ComfyUI** y arrastra el archivo maestro desde `02_flujos_comfyui/` a tu espacio de trabajo.
3. Carga el video original y ajusta el `frame_load_cap` y el `skip_first_frames` según las instrucciones detalladas en los `01_guiones_tecnicos/`.
4. Copia los Prompts (Positivo y Negativo) desde la carpeta `03_prompts_y_textos/` para asegurar la máxima nitidez.
5. ¡Grita "Acción" (Queue Prompt)!

## 🛠️ Requisitos del Sistema (Custom Nodes)

Para que los flujos de la carpeta `02_flujos_comfyui/` funcionen sin errores (nodos rojos), debes tener instalados los siguientes paquetes desde el **ComfyUI-Manager**:

| Nodo / Paquete | Uso en este Proyecto |
| :--- | :--- |
| **ComfyUI-VideoHelperSuite** | Carga de video original, control de FPS (`force_rate`) y guardado de resultados. |
| **ComfyUI-LTXTricks** | Implementación de LTX-2, nodos de guía (`LTXVAddGuide`) y decodificación tiled. |
| **ComfyUI-Essentials** | Operaciones de imagen como el escalado `nearest-exact` y recorte `center`. |
| **ComfyUI-Audio** | Recorte y sincronización precisa del audio de la escena (Toma 1 y Toma 2). |
| **ComfyUI-Custom-Scripts** | Mejoras de interfaz y organización de los nodos KSampler. |

> **Nota del Director:** Si al cargar el flujo te faltan nodos, usa la opción "Install Missing Custom Nodes" en tu Manager y busca los nombres de la tabla anterior.
