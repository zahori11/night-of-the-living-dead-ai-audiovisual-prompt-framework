## 🖼️ Art Notebook: Stylization and Graphic Assets

This document details the **preproduction workflow** used to generate the **key frames and scenographic elements** (such as the arcade console), combining external tools before entering the **animation and compositing phase**.

---

## 🎞️ 1. Frame Stylization (Freepik + Seedream)

To ensure **maximum fidelity to the performance of the original clip**, the pixel art stylization was **not performed using text-to-image generation (txt2img) or local engines**.

Instead, an **AI rotoscoping workflow frame-by-frame** was used:

* A **custom style was trained in Freepik** *(Game Boy Noir 1-bit aesthetic)*.
* The **frames from the original video were processed through Seedream**, using the trained style as the base reference.

### 🔄 Transformation Prompt (Seedream)

The exact instruction sent to the AI to **clone the original composition while applying the pixel art filter** was:

```
Clone @img([original_frame_reference])
```

*(Director’s note: This method locks the structure of the original image, allowing the Seedream engine to focus exclusively on reinterpretation of pixels, lighting, and dithering.)*

---

## 📺 2. Scene Asset Generation (CRT Television)

To frame the final **news broadcast footage**, a graphic asset was generated in the form of an **arcade machine / CRT monitor**.

In post-production, the **screen area is emptied (alpha channel / transparency)** so the **pixel-art video can be composited behind it**.
