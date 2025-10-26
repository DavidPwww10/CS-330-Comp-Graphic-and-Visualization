
# CS 330 – Portfolio Artifact (David Parks)

**Artifacts:** `3D-Scene.zip` and `CS-330-FinalProject-DesignDecisions.docx`
**Summary:** This project showcases my ability to build a small, fully realized 3D world in OpenGL/C++, including geometry, texturing, lighting, camera/navigation, and clean code organization.

## How I approach designing software

I start with the user experience and the rubric requirements, then sketch the scene and break it into primitives, materials, lights, and controls. I design for readability and iteration: separate setup from the render loop, isolate input/camera logic, and keep objects/data self-contained.

* **New design skills I developed:** turning a reference idea into a simple composition (mug + tiled plane), choosing primitives that minimize poly count, planning materials/UV tiling, and balancing a key light with a fill.
* **Process I followed:** milestone-driven iterations → plane and complex object → navigation → textures → lighting → polish.
* **Future reuse:** I’ll reuse the same scene graph mindset—modular managers for view, shader, and scene—when I design interactive visuals or gameplay prototypes.

## How I approach developing programs

I code in small steps, test constantly, and use clear interfaces. Classes like `SceneManager`, `ViewManager`, `ShaderManager`, and reusable primitive meshes kept the codebase predictable.

* **New development strategies:** swapping ad-hoc “directions” for real velocity vectors, adding proper reflections, and isolating collision/transform helpers made behavior physically consistent and easier to debug.
* **Iteration:** each feature landed as a safe layer; I didn’t move on until input, textures, or lighting were stable.
* **How my approach evolved:** I reduced magic numbers, centralized uniforms/materials, added comments where future-me would forget why a choice was made (e.g., UV scaling, slight mesh overlap to hide seams).

## How computer science helps me reach my goals

* **Educational pathway:** computational graphics strengthened my linear-algebra intuition (vectors, normals, transforms) and reinforced API discipline (GLSL, buffers, textures).
* **Professional pathway:** the ability to build real-time visuals translates to UI polish, data visualization, simulation demos, and performance-minded thinking—useful across software, IT, and security contexts.

## Repository contents

* `3D-Scene.zip` — Final project build and source folder (include the EXE in the build so it runs without compiling).
* `CS-330-FinalProject-DesignDecisions.docx` — My design write-up (objects, textures, lighting, camera, code structure).
* `README.md` — This reflection.

## Run notes

Unzip `3D-Scene.zip`, launch the included EXE, and use **WASD/QE + mouse** to navigate (perspective/ortho toggle if included). If building from source, use **Visual Studio 2022** and the provided solution.
