# 🖼️ Cuaderno de Arte: Estilización y Assets Gráficos

Este documento detalla el flujo de trabajo de preproducción utilizado para generar los fotogramas clave y los elementos escenográficos (como la consola arcade), combinando herramientas externas antes de entrar a la fase de animación y empalme.

---

## 🎞️ 1. Estilización de Fotogramas (Freepik + Seedream)

Para garantizar la máxima fidelidad con la actuación del clip original, **la estilización del pixel art no se realizó mediante generación de texto a imagen (txt2img)** ni motores locales. 

Se utilizó un flujo de rotoscopia IA frame a frame:
1. Se entrenó un estilo propio en **Freepik** (Estética Game Boy Noir 1-bit).
2. Se procesaron los fotogramas del video original a través de **Seedream** usando como base el estilo entrenado.

### 🔄 Prompt de Transformación (Seedream)
La instrucción exacta enviada a la IA para clonar la composición original aplicando el filtro de pixel art fue:
> `Clon @img([referencia_del_fotograma_original])`

*(Nota del Director: Este método bloquea la estructura de la imagen original, permitiendo que el motor de Seedream se centre únicamente en reinterpretar los píxeles, la luz y el tramado).*

---

## 📺 2. Generación del Escenario (Televisor CRT)

Para enmarcar el metraje final del noticiero, generamos un activo gráfico (asset) en forma de maquina arcade (monitor CRT). Posteriormente, la pantalla se vacía (canal alfa/transparencia) en postproducción para incrustar el video de pixel art por detrás.
