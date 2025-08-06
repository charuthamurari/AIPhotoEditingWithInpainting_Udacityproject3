# Udacity-GenAI-Phase2-Project3
AI Photo Editing with Inpainting

## Project Summary

In this project, we are going to build a simple web app that allows you to select a subject in an image and then either change its background or replace the subject itself.

The workflow is as follows:
1. **Upload an image.**
2. **Select the main object** by clicking on it.
3. The **Segment Anything Model (SAM)** generates multiple masks for the selected area.
4. The **best mask is chosen automatically**, but the user can refine it by adding more clicks for better segmentation.
5. Once the mask is finalized, the user enters a **text prompt (and optionally a negative prompt)** to describe the new background or subject.
6. An **inpainting diffusion model** is used to generate the new background or subject based on the prompt.
7. The final image is displayed.

Additionally, the user has the option to **invert the mask**:
- Keep the subject and change the background.
- OR keep the background and change the subject.

This app can be used for:
- Background swapping
- Subject replacement
- Object removal
- Creative image editing

The core functionality includes:
- Invoking the SAM model to generate masks.
- Processing and refining the segmentation.
- Using a Text-to-Image Diffusion model for inpainting based on user prompts.

---

### Example 1:
<!-- Image: trail1.png -->
<img width="1889" height="902" alt="image" src="https://github.com/user-attachments/assets/43ab1ef9-a504-41c7-a462-b38933fb095f" />


---

### Example 2:
<!-- Image: trail2.1.png -->
<img width="940" height="471" alt="image" src="https://github.com/user-attachments/assets/ca0f848b-8a96-419a-a33b-1326d5958f36" />


---

### Example 3:
<!-- Image: trail2.2.jpg -->
<img width="1707" height="822" alt="image" src="https://github.com/user-attachments/assets/eca1b3d3-8a13-45b5-868d-b2ff0e0d1a32" />


---

### Example 4:
<!-- Image: trail3.3.jpg -->
<img width="1711" height="832" alt="image" src="https://github.com/user-attachments/assets/461af551-4205-4edd-92e8-50935205536e" />

