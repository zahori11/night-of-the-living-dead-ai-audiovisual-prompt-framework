🎬 Technical Script: Sequence 01 - Radio Studio & Control Rooms

Production Details:
Engine: LTX-2 (via ComfyUI) 
Rendering Resolution (Native): 768x512 (Base resolution used to optimize the model’s VRAM memory usage).
Final Resolution (Export): Upscaled in post-production using the Upscale Image (or ImageScaleBy) node.
Director’s Note: The final scaling must be performed strictly using the nearest-exact method. This allows the video to be exported at higher resolutions (e.g., 1536x1024) by multiplying pixels as solid Lego-like blocks, avoiding bicubic smoothing and preserving the extreme sharpness of the 1-bit style.
Speed (Force Rate): 40 FPS
Visual Style: 1-bit Pixel Art (Monochrome: Black and White)

--------------------------------------------------

🎞️ Shot 1: The Head Turn
Time: 0.00s - 2.00s
Frames: 000 - 080
Main Action: The announcer begins with his gaze directed downward and to the right. Slowly, he raises his eyes and turns his head to the left until making visual contact with the camera lens. Background technician stands up.
Technical Notes:
* Start image anchored to the original frame at 00:00.
* frame_load_cap: 81
* skip_first_frames: 0
* Shield: Standard Shield

🎞️ Shot 2: The Broadcast
Time: 2.00s - 4.00s
Frames: 080 - 160
Main Action: The announcer maintains eye contact with the camera and begins speaking with a serious expression, displaying subtle rhythmic breathing. He eventually looks downward. In the background, the technician on the right makes small adjustments on the sound console.
Technical Notes:
* Anchor (Inplace): Frame 080 to ensure an invisible cut.
* Audio start_index: 2.00 / duration: 2.00
* frame_load_cap: 81
* skip_first_frames: 80
* Shield: Standard Shield

🎞️ Shot 3: Subtle Tension
Time: 4.00s - 6.00s
Frames: 160 - 240
Main Action: The technician looks toward the camera with restricted physical movement. He performs nuanced facial micro-expressions, including a subtle blink and tightening of the lips, maintaining a strict 1-bit style grid while the background continues to operate smoothly.
Technical Notes:
* Anchor (Inplace): Frame 160.
* frame_load_cap: 81
* skip_first_frames: 160
* Shield: Standard Shield

🎞️ Shot 4: Micro-Expressions
Time: 6.00s - 8.00s
Frames: 240 - 320
Main Action: Captured through the CRT bezel, the operator exhibits exceptionally subtle bodily micro-movements. He performs a rapid upward glance micro-expression and a brief softening around the mouth, moving away from his intense focus.
Technical Notes:
* Anchor (Inplace): Frame 240.
* frame_load_cap: 81
* skip_first_frames: 240
* Shield: Standard Shield

🎞️ Shot 5: Shift in Concentration
Time: 8.00s - 10.00s
Frames: 320 - 400
Main Action: A distinct localized facial micro-gesture occurs: his eyebrows furrow deeply in intense concentration. Towards the end of the shot, his face relaxes into a gentle, faint smile, releasing the built-up tension.
Technical Notes:
* Anchor (Inplace): Frame 320.
* frame_load_cap: 81
* skip_first_frames: 320
* Shield: Standard Shield

🎞️ Shot 6: Downward Gaze
Time: 10.00s - 12.00s
Frames: 400 - 480
Main Action: After his peaceful smile, the operator lowers his gaze (as if in a prolonged blink or looking at a lower console) and opens his mouth slightly, as if quietly speaking into his headset.
Technical Notes:
* Anchor (Inplace): Frame 400.
* frame_load_cap: 81
* skip_first_frames: 400
* Shield: Standard Shield

🎞️ Shot 7: The Lower Console
Time: 12.00s - 14.00s
Frames: 480 - 560
Main Action: The operator intensely looks downward, speaking or issuing an instruction toward the lower desk.
Technical Notes:
* Anchor (Inplace): Frame 480.
* frame_load_cap: 81
* skip_first_frames: 480
* Shield: Standard Shield

🎞️ Shot 8: Heavy Thoughts
Time: 14.00s - 16.00s
Frames: 560 - 640
Main Action: A frontal view of the announcer speaking into the mic. He stares intensely forward with deliberate finger movements on the buttons, then closes his eyes and directs his gaze downward with gentle torso breathing.
Technical Notes:
* Anchor (Inplace): Frame 560.
* frame_load_cap: 81
* skip_first_frames: 560
* Shield: Standard Shield

🎞️ Shot 9: Biomechanical Realism
Time: 16.00s - 18.00s
Frames: 640 - 720
Main Action: The operator sits at the control console moving with subtle biomechanical realism. His hands rest and move naturally across the soundboard. He looks forward with a serious, focused expression while three background technicians work smoothly.
Technical Notes:
* Anchor (Inplace): Frame 640.
* frame_load_cap: 81
* skip_first_frames: 640
* Shield: Standard Shield

🎞️ Shot 10: Authoritative Command
Time: 18.00s - 20.00s
Frames: 720 - 800
Main Action: Set in a bustling mission control room. The serious technician looks down at his console and then directly forward to deliver an authoritative command. Behind him, staff move rapidly (a standing man points abruptly, a woman types rhythmically).
Technical Notes:
* Anchor (Inplace): Frame 720.
* frame_load_cap: 81
* skip_first_frames: 720
* Shield: Standard Shield

🎞️ Shot 11
Time: 20.00s - 22.00s
Frames: 800 - 880
Main Action: The technician speaks slowly and precisely through his headset. He recites telemetry coordinates with a piercing gaze, authoritative tone while maintaining a calm exterior.
Technical Notes:
* Anchor (Inplace): Frame 800.
* frame_load_cap: 81
* skip_first_frames: 800
* Shield: Standard Shield

🎞️ Shot 12: Flight Commands
Time: 22.00s - 24.00s
Frames: 880 - 960
Main Action: Operating the central console, the technician transmits, monotone voice. The flickering glow of the central computers bathes the room in high-contrast shadows.
Technical Notes:
* Anchor (Inplace): Frame 880.
* frame_load_cap: 81
* skip_first_frames: 880
* Shield: Standard Shield

🎞️ Shot 13: Operational Sequences
Time: 24.00s - 26.00s
Frames: 960 - 1040
Main Action: With absolute focus and calm, the technician reports instrument readings and dictates operational sequences. Background operators work actively under intense overhead lighting.
Technical Notes:
* Anchor (Inplace): Frame 960.
* frame_load_cap: 81
* skip_first_frames: 960
* Shield: Standard Shield

🎞️ Shot 14: Quiet Exhaustion
Time: 26.00s - 28.00s
Frames: 1040 - 1120
Main Action: The lean man stares directly into the lens with alert anticipation. He closes his eyes in deep concentration, conveying a heavy weight of responsibility and quiet exhaustion before a massive wall of blinking matrix computers.
Technical Notes:
* Anchor (Inplace): Frame 1040.
* frame_load_cap: 81
* skip_first_frames: 1040
* Shield: Standard Shield

🎞️ Shot 15: Youngstown Dispatch
Time: 28.00s - 30.00s
Frames: 1120 - 1200
Main Action: The setting shifts to a hospital dispatch center. A slow push-in focuses on the dispatcher's subtly clenched jaw. Pixelated text overlay "YOUNGSTOWN TOWNSHIP MUNICIPAL HOSPITAL" appears on the screen. Background staff work with methodical urgency.
Technical Notes:
* Anchor (Inplace): Frame 1120.
* frame_load_cap: 81
* skip_first_frames: 1120
* Shield: Banner Shield (Crucial for clear text generation)

🎞️ Shot 16: Stoic Resolve
Time: 30.00s - 32.00s
Frames: 1200 - 1280
Main Action: The dispatcher looks straight ahead with exhausted determination, then slightly downward. The hospital text banner remains rigidly overlaid at the bottom while subtle screen jitter is introduced.
Technical Notes:
* Anchor (Inplace): Frame 1200.
* frame_load_cap: 81
* skip_first_frames: 1200
* Shield: Banner Shield

🎞️ Shot 17: The Lockdown
Time: 32.00s - 34.00s
Frames: 1280 - 1360
Main Action: The dispatcher, initially looking at paperwork, abruptly raises his head. He looks directly into the lens with urgent realization. Background figures become frantic.
Technical Notes:
* Anchor (Inplace): Frame 1280.
* frame_load_cap: 81
* skip_first_frames: 1280
* Shield: Banner Shield

🎞️ Shot 18: Escalation
Time: 34.00s - 36.00s
Frames: 1360 - 1440
Main Action: The overhead lights flicker violently. The operator's expression shifts to wide-eyed alarm as he leans sharply into the mic. Background operators jump from their seats in a wave of panic.
Technical Notes:
* Anchor (Inplace): Frame 1360.
* frame_load_cap: 81
* skip_first_frames: 1360
* Shield: Banner Shield

🎞️ Shot 19: The Chaos
Time: 36.00s - 38.00s
Frames: 1440 - 1520
Main Action: Drastic change. The dispatcher is hunched forward in tense distress, speaking frantically. Background operators shout. The camera slowly pushes in on the dispatcher's eyes, then pulls back.
Technical Notes:
* Anchor (Inplace): Frame 1440.
* frame_load_cap: 81
* skip_first_frames: 1440
* Shield: Banner Shield

🎞️ Shot 20: Peak Distress
Time: 38.00s - 40.00s
Frames: 1520 - 1600
Main Action: The chaotic atmosphere continues. The primary operator types rapidly and lowers the mic. A colleague stands up pointing. Scanlines and screen jitter intensify heavily.
Technical Notes:
* Anchor (Inplace): Frame 1520.
* frame_load_cap: 81
* skip_first_frames: 1520
* Shield: Banner Shield

🎞️ Shot 21: Sharon Central Transition
Time: 40.00s - 42.00s
Frames: 1600 - 1680
Main Action: A transition shot. Harsh sunlight fades into deep shadows. The operator closes his eyes in a heavy sigh of exhaustion, then opens them wide in hyper-vigilant readiness. Text overlay changes to "SHARON CENTRAL FIRE DEPARTMENT".
Technical Notes:
* Anchor (Inplace): Frame 1600.
* frame_load_cap: 81
* skip_first_frames: 1600
* Shield: Banner Shield

🎞️ Shot 22: Clean Dispatch
Time: 42.00s - 44.00s
Frames: 1680 - 1760
Main Action: Scene rendered with extremely flat lighting to prevent structural distortion. Operator Sharon sits perfectly rigid to prevent pixel morphing, moving only his lips to articulate a multi-alarm warning, then looks down to review a printed log.
Technical Notes:
* Anchor (Inplace): Frame 1680.
* frame_load_cap: 81
* skip_first_frames: 1680
* Shield: Banner Shield

🎞️ Shot 23: Final Comms
Time: 44.00s - 46.00s
Frames: 1760 - 1840
Main Action: Operator Sharon looks directly into the camera stating, He immediately lowers his eyes toward the desk, subtly tucking his chin while the static fire department banner remains anchored.
Technical Notes:
* Anchor (Inplace): Frame 1760.
* frame_load_cap: 81
* skip_first_frames: 1760
* Shield: Banner Shield
