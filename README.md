# OpenMoviePrompts (OMP) Standard v1.0
**The Open Standard for Text-Defined Cinema.**

OpenMoviePrompts (OMP) is a structured, version-controlled markdown framework designed to store entire cinematic projects as human-readable, machine-executable code. OMP enables AI video engines to generate high-consistency, ultra-realistic films by reading a standardized project directory rather than a single chaotic prompt.

## 🎞️ The Vision
In the OMP era, a movie is no longer a collection of pixels (MP4), but a collection of semantics (.md/.omp). This allows for:
* Zero-Loss Portability: Transfer entire 8K feature films in kilobytes.
* Identity Persistence: Ensure characters (@ID) maintain the same "Visual DNA" across every shot.
* Forkable Cinema: Clone a movie project, modify the prompt, and "re-render" a personalized version.

## 📂 Project Structure
A standard OMP project follows this directory architecture:
```text
/My_Epic_Movie
├── manifest.yaml          # Global physics, film stock, and engine specs
├── identity.omp           # Character & Prop "Visual DNA" definitions
├── environment.omp        # Location-specific lighting and asset data
├── audio.omp              # Procedural soundscape and BGM prompts
└── timeline/
    ├── scene_01.md        # Shot-by-shot cinematic instructions
    └── scene_02.md        # Logic-based branching narratives
```

## 🛠️ Component Specifications
1. `manifest.yaml` (The World Rulebook)
Defines the technical constraints of the render.
```yaml
Project: "Cyber Samurai"
Engine: "Cinema-Native-V1"
Specs:
  Aspect_Ratio: "2.35:1"
  Color_Science: "ACEScg"
  Physics: "Fluid_Rain_Simulation: On"
```

2. `identity.omp` (Semantic Character Consistency)
Solves the "AI Face-Swap" issue by pre-defining character parameters.
```markdown
## @Ronin_Alpha
- **Base_Mesh**: Male_Cybernetic_Humanoid
- **Texture**: Scratched_Titanium_Matte
- **Key_Feature**: Left_Shoulder_Scar, Hex_Glow_Visor(#FF0000)
```

3. `timeline/` (Cinematic Logic)
Uses a structured language to control the camera and action.
```markdown
### Shot_102 <@Action_Orbit_Camera>
- **Subject**: @Ronin_Alpha
- **Action**: Unsheathe_Katana(Speed: 0.8s)
- **VFX**: Cyan_Scan_Laser, Volumetric_Mist
- **Lighting**: Neon_Flicker(Frequency: 2Hz)
```

## 🚀 Getting Started

### For Directors
1. Initialize: omp init my_movie
2. Define Assets: Fill identity.omp with your character descriptions.
3. Write Shots: Use the OMP syntax in the timeline/ folder.
4. Render: Point your OMP-compliant AI engine to the project root.

### For Developers (AI Engines)
To support OMP, your engine must:
1. Parse @ID tags to maintain character/environment embeddings across shots.
2. Interpret manifest.yaml for global visual consistency.
3. Support "Seed-Linking" based on OMP shot sequences.

## 🤝 Contributing
OpenMoviePrompts is an open-source initiative. We welcome contributions to:
Lighting_Presets.omp: A library of classic cinematic lighting setups.
Camera_Library.omp: Standardized movement definitions (Dolly, Pan, Orbit).

## 📜 License
This project is licensed under the MIT License - see the LICENSE file for details.
"The era of text-defining movies starts here."
