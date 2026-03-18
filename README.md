The-Community_Cut

# 🎬 AI Audiovisual Framework: Night of the Living Dead

Welcome to the film set! This repository organizes prompts, workflows, and AI audiovisual resources for using **LTX-2** to reanimate classic scenes in any visual style you prefer.

Photorealistic, abstract, surreal, hand-painted, or our main focus: **retro 1-bit Pixel Art (Game Boy Noir style)**. The interpretation is up to you.

Use **ComfyUI**, the **open-source LTX-2 model**, or the **LTX Studio API**. As long as it works with **LTX-2**, you’re in!

---

# 📁 Studio Structure (Repository)

To keep production organized, the project is divided into the following departments:

**📁 technical_scripts/**  
Production breakdowns. Here you’ll find detailed frame-by-frame documents (timings, actions, cuts) to replicate the exact timing of each shot.

**📁 comfyui_workflows/**  
The brain of the operation. `.json` files ready to drag and drop into ComfyUI, including advanced **multi-prompt workflows** and **guide image anchoring** (LTXVAddGuide).

**📁 prompts_and_texts/**  
The script department. A collection of **positive prompts** and our **negative prompt shields** (specifically designed to block smoothing and protect the 1-bit aesthetic).

**📁 visual_resources/**  
The editing room. Contains frames extracted from the generations (**pixelart_clip_frames**) ready to be assembled, along with additional graphic assets such as **arcade machine frames**.

---

# 🚀 How to Start Filming

1. Clone or download this repository to your computer.  
2. Open **ComfyUI** and drag the master file from `02_comfyui_workflows/` into your workspace.  
3. Load the original video and adjust **`frame_load_cap`** and **`skip_first_frames`** according to the detailed instructions in `01_technical_scripts/`.  
4. Copy the **Prompts (Positive and Negative)** from the `03_prompts_and_texts/` folder to ensure maximum sharpness.  
5. Shout **“Action!”** (Queue Prompt)!

---

# 🛠️ System Requirements (Custom Nodes)

For the workflows in `02_comfyui_workflows/` to run without errors (red nodes), you must install the following packages via **ComfyUI-Manager**:

Aquí tienes la **traducción al inglés en formato cuadrícula (tabla limpia para LinkedIn, Notion o GitHub):**

---

### ⚙️ ComfyUI Pipeline Breakdown

| Node / Component           | Function in This Project                                                                                 |
| -------------------------- | -------------------------------------------------------------------------------------------------------- |
| Load Image                 | Uploads static images (start, middle, end) from your computer into the program.                          |
| Load VHS Video             | Loads the original video file to read its frames or extract its audio track.                             |
| Load Audio                 | Loads a separate audio file to integrate into the final output.                                          |
| Image Scale / Scale By     | Adjusts the exact dimensions of the image (e.g. 768x512 pixels) so all assets share the same resolution. |
| Resizable Image Mask Node  | Adjusts the size of selection areas (masks) so they match the resized images.                            |
| Image to Mask              | Defines a specific area of the image, indicating what can be animated and what must remain static.       |
| Feather Mask               | Softens mask edges to avoid harsh cuts and create smooth pixel transitions.                              |
| UnetLoaderGGUF             | Loads the main video generation model (LTX-2), which computes and generates the animation.               |
| DualCLIPLoaderGGUF           | Loads the language model that converts text prompts into processable mathematical data.                  |
| VAELoader                  | Encodes and decodes between latent space and pixel space                  |
| CLIPTextEncode             | Receives text prompts defining what the model should generate (positive) or avoid (negative).            |
| KSampler                   | Executes diffusion steps and controls the sampler and scheduler                        |
| LTXVImgToVideoInplace      | Extends a static image and converts it into a continuous sequence of frames.                             |
| LTXVAddGuide         | Injects reference data to maintain visual and lighting consistency across frames.                        |
| VAEDecodeTiled / VAEDecode | Converts generated latent data back into visible pixel-based images.                                     |
| VHS_VideoCombine           | Combines all frames, syncs them with audio, and exports the final video file (.mp4).                     |

<img width="1704" height="905" alt="image" src="https://github.com/user-attachments/assets/91258e34-9eee-4e5e-89aa-4a4aa7d09d98" />

<img width="1628" height="879" alt="image" src="https://github.com/user-attachments/assets/363fb54f-bea8-45df-999b-4a84dc2cbd5b" />

<img width="1700" height="406" alt="image" src="https://github.com/user-attachments/assets/728e7dfe-b456-4014-a01d-e71bad7bed0b" />

<img width="1364" height="918" alt="image" src="https://github.com/user-attachments/assets/f1e51bac-8460-4db6-acb8-9b5176d65348" />


**Director’s Note:**  
If nodes are missing when loading the workflow, use **“Install Missing Custom Nodes”** in your Manager and search for the names listed in the table above.
