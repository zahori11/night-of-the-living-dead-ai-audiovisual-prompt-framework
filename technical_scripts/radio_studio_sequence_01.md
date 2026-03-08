# 🎬 Technical Script: Sequence 01 - Radio Studio

**Production Details:**
* **Engine:** LTX-2 (via ComfyUI)
**Rendering Resolution (Native):** 768x512 (Base resolution used to optimize the model’s VRAM memory usage).
* **Final Resolution (Export):** Upscaled in post-production using the *Upscale Image* (or *ImageScaleBy*) node.  
  > *Director’s Note: The final scaling must be performed strictly using the `nearest-exact` method. This allows the video to be exported at higher resolutions (e.g., 1536x1024) by multiplying pixels as solid Lego-like blocks, avoiding bicubic smoothing and preserving the extreme sharpness of the 1-bit style.*
* **Speed (Force Rate):** 40 FPS
* **Visual Style:** 1-bit Pixel Art (Monochrome: Black and White)

---

## 🎞️ Shot 1: The Head Turn
* **Time:** 0.00s - 2.00s
* **Frames:** 000 - 080
* **Main Action:** The announcer begins with his gaze directed downward and to the right. Slowly, he raises his eyes and turns his head to the left until making visual contact with the camera lens.
* **Technical Notes:** 
  * Start image anchored to the original frame at 00:00.
  * `frame_load_cap`: 81
  * `skip_first_frames`: 0

## 🎞️ Shot 2: The Broadcast
* **Time:** 2.00s - 4.00s
* **Frames:** 080 - 160
* **Main Action:** The announcer maintains eye contact with the camera and begins speaking with a serious expression. In the background, the technician on the right makes small adjustments on the sound console.
* **Technical Notes:** 
  * Frame 080 (end of Shot 1) is used as the starting anchor (Inplace) to ensure an invisible cut.
  * Audio `start_index`: 2.00 / `duration`: 2.00
  * `frame_load_cap`: 81
  * `skip_first_frames`: 80
