# 🚀 UP THERE — The Human Body in Space

> How far can a human go — and what happens to the human body along the way?

[![Live experience](https://img.shields.io/badge/Live%20experience-Explore%20UP%20THERE-2563eb)](https://dhakshathamylsamy.github.io/up-there/) ![HTML](https://img.shields.io/badge/HTML5-Frontend-E34F26?logo=html5&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-Interactive-F7DF1E?logo=javascript&logoColor=black) ![Focus](https://img.shields.io/badge/Focus-Bioastronautics-455a64)

**[Launch the interactive experience →](https://dhakshathamylsamy.github.io/up-there/)**

*Scroll from Earth's surface into orbit, spend months in microgravity, and discover what it takes for the human body to return home.*

## About the project

UP THERE is an interactive science communication project exploring the intersection of **biomedical engineering, human physiology and aerospace**. It brings the physics of spaceflight and the physiological responses of an astronaut together in a single continuous, illustrated scroll experience.

Rather than treating the spacecraft and its human passenger as separate subjects, the website presents their changing conditions side by side. As the rocket ascends, the environment changes, and the visitor discovers how the body responds. Once in orbit, the journey shifts from altitude to mission duration, before returning to Earth and exploring recovery.

## Why I built this

As an undergraduate Biomedical Engineering student, I wanted to explore the role of biomedical science beyond conventional healthcare applications — particularly in human spaceflight.

The challenges astronauts face during long-duration missions and their readaptation to Earth inspired me to investigate how the cardiovascular, respiratory, musculoskeletal and nervous systems respond to unfamiliar environments. This project is my way of turning that curiosity into an accessible learning experience.

The central question is not just how we get humans into space, but how we keep them healthy there and help them return safely.

## The experience

| Mission phase | What you explore |
| --- | --- |
| Pre-launch and countdown | Baseline physiology, anticipation and sympathetic activation |
| Lift-off and ascent | Acceleration, apparent body weight, cardiovascular and respiratory demands |
| Max Q and stage separation | Aerodynamic loading, changes in acceleration and cabin protection |
| Orbital insertion | Orbital velocity, free fall and apparent weightlessness |
| First hour to first week | Fluid redistribution, vestibular adaptation, blood volume and sleep |
| One month to six months | Muscle unloading, bone remodeling, cardiovascular fitness and vision |
| One year and beyond | Radiation exposure, deconditioning and long-duration health risks |
| Return and recovery | Orthostatic intolerance, balance, physical rehabilitation and readaptation |

These milestones are narrative teaching points, not universal timelines of physiological change.

## Key features

- **Continuous scroll-driven storytelling:** one uninterrupted journey from Earth to orbit and back.
- **Synchronized visualizations:** spacecraft movement, atmospheric conditions and human physiological responses evolve together.
- **Illustrative flight parameters:** altitude, external atmospheric pressure, speed, apparent g-load and cabin context.
- **Human response panel:** qualitative descriptions of heart rate, blood pressure, respiration and oxygen context.
- **Biomedical perspective:** contextual explanations of how physiological changes can be studied and monitored.
- **Mission duration progression:** time advances in orbit without implying that the spacecraft travels farther from Earth.
- **Original SVG illustrations:** lightweight, schematic visuals with a changing atmospheric backdrop.
- **Interactive navigation:** scroll, mission slider, previous/next controls and restart.
- **Scientific transparency:** contextual source links and an expandable references and assumptions section.
- **Responsive, dependency-free frontend:** no backend, API keys or hardware required.

## The biomedical engineering connection

Spaceflight presents a unique challenge: the human body evolved under Earth's gravity, but must adapt to a substantially different mechanical and environmental setting during a mission.

| Physiological concern | Relevant biomedical assessment |
| --- | --- |
| Cardiovascular adaptation | ECG, blood pressure, ultrasound, orthostatic testing |
| Respiratory mechanics and oxygenation | Respiration monitoring, pulse oximetry, cabin gas monitoring |
| Fluid redistribution | Ultrasound and body fluid assessment |
| Muscle deconditioning | Strength testing, EMG and muscle imaging |
| Bone loss | DXA and other dedicated imaging techniques |
| Vestibular adaptation | Balance, gait and sensorimotor assessments |
| Neuro-ocular changes | Eye examinations and optical coherence tomography |
| Sleep and circadian disruption | Actigraphy and sleep assessment |
| Radiation exposure | Personal dosimetry |

These are examples of relevant assessment methods, not instruments implemented by the website. Routine vital signs alone cannot characterize every physiological adaptation.

## Technical implementation

Built using **HTML5, CSS3, vanilla JavaScript and SVG**, with GitHub Pages for hosting. Scroll progress drives the interpolation of illustrative flight keyframes, the visual environment and the selection of physiological narrative events. Scientific content is separated from the interaction logic.

```text
up-there/
├── index.html    # Layout, styling, SVG illustrations and credits
├── app.js        # Scroll progress, interpolation and interactive rendering
├── science.js    # Mission keyframes, physiology narratives and source links
└── README.md    # Project documentation
```

### Run locally

```bash
git clone https://github.com/DhakshathaMylsamy/up-there.git
cd up-there
python -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000) in a modern browser. Alternatively, open `index.html` directly. No npm installation or build step is necessary.

## Scientific sources and assumptions

The project draws on human spaceflight research and educational resources, including:

- [NASA — The Human Body in Space](https://www.nasa.gov/humans-in-space/the-human-body-in-space/)
- [NASA — Cardiovascular and Vision](https://www.nasa.gov/directorates/esdmd/hhp/cardiovascular-and-vision/)
- [NASA — Exercise Overview](https://www.nasa.gov/ochmo-tb-031-exercise-overview-2/)
- [NASA — Life After Microgravity: Astronauts Reflect on Post-Flight Recovery](https://www.nasa.gov/centers-and-facilities/johnson/life-after-microgravity-astronauts-reflect-on-post-flight-recovery/)
- [PubMed Central — Spaceflight physiology review (PMC2696527)](https://pmc.ncbi.nlm.nih.gov/articles/PMC2696527/)
- [NASA — Fundamentals of Human Health](https://www.nasa.gov/reference/fundamentals-of-human-health/)

<details>
<summary><strong>Model assumptions and limitations</strong></summary>

- The mission is illustrative, not a reconstruction of an actual launch or astronaut's flight. Scroll distance does not correspond to elapsed mission time.
- The representative low Earth orbit is approximately 400 km above Earth's surface, with an orbital speed of about 7.8 km/s. Gravitational acceleration there remains about 89% of its surface value; apparent weightlessness arises from orbital free fall.
- Standard sea-level pressure is approximately 101.3 kPa. Atmospheric pressure, speed and apparent load along the journey are simplified keyframes, not outputs of a validated flight dynamics model.
- Cabin pressure and oxygen are assumed to be maintained during flight. External atmospheric conditions are not the conditions experienced inside the spacecraft.
- Vital responses are qualitative, not measured or predicted clinical values. The oxygen indicator represents cabin context, not measured blood oxygen saturation.
- Physiological changes and recovery depend on individual characteristics, mission duration, exercise, nutrition and other factors. Illustrated milestones do not establish fixed onset times or rates of loss.
- No personal astronaut medical records or live biometric data are used. The illustrations are schematic.

</details>

**UP THERE is an educational science communication project, not a validated aerospace simulator, clinical model or diagnostic tool.**

## Future directions

- Refine anatomical animations of fluid redistribution, muscle unloading and bone remodeling.
- Incorporate research-supported quantitative ranges with mission context and uncertainty where evidence permits.
- Explore more detailed physiological countermeasures and postflight recovery.
- Improve accessibility, scientific source traceability and cross-browser testing.

## Inspiration and acknowledgements

The continuous scrolling interaction is inspired by [The Space Elevator by Neal.fun](https://neal.fun/space-elevator/). UP THERE uses its own narrative, implementation and illustrations, with a distinct focus on human physiology and biomedical engineering.

Developed through AI-assisted coding (vibe coding), combining biomedical curiosity, iterative interaction design and frontend development. Scientific interpretation remains an area for ongoing review and improvement.

## Author

**Dhakshatha M K**  
Undergraduate Biomedical Engineering student  
Exploring biomedical science, human physiology, bioastronautics and aerospace medicine.

[LinkedIn](https://www.linkedin.com/in/dhakshatha-m-k) · [GitHub](https://github.com/DhakshathaMylsamy)

Feedback, scientific corrections and suggestions are welcome through [GitHub Issues](https://github.com/DhakshathaMylsamy/up-there/issues).

---

*Getting humans into space is an engineering achievement. Keeping them healthy there — and helping them recover on Earth — is a biomedical challenge.*
