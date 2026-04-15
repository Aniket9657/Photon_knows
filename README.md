# Eye-Black-Hole Universe Simulator

A Streamlit thought-experiment app that turns a philosophical question into an interactive simulation:

**What if seeing was not passive, but gravitational?**

This project imagines a universe where eyes do not simply receive light. Instead, perception can behave like an active force — bending, collapsing, or shaping what is observed.

## Overview

The app blends ideas from:

- Vision and perception
- Black hole style gravitational attraction
- Quantum observer effects
- Consciousness and philosophy
- Generative reflection through a built-in pseudo-GenAI panel

It is not a physically accurate scientific model. It is a conceptual simulator designed to help explore your idea interactively.

## Features

- **Three simulation modes**
  - **Passive eye (our universe):** vision behaves like normal reception
  - **Gravitational eye:** the eye acts like an attractor that bends visual paths inward
  - **Conscious observer field:** observation shifts the system toward collapse

- **Interactive controls**
  - Number of photons / rays
  - Slit gap
  - Eye gravity factor
  - Consciousness weight
  - Observer active toggle
  - GenAI creativity level

- **Live metrics**
  - Rays fired
  - Left hits
  - Center hits
  - Right hits

- **Visualization**
  - Plotly-based scatter view of final hit regions
  - Vertical reference markers for the slit/threshold and eye/horizon
  - Dark themed simulation display

- **Interpretation panel**
  - Explains the current mode in plain language
  - Displays a curvature / collapse index

- **GenAI reflection panel**
  - Lets the user type a philosophical prompt
  - Produces a reflective response based on the selected simulation mode, observer state, consciousness weight, and creativity setting

## Project structure

```bash
eye_black_hole_sim/
├── app.py
└── README.md
```

## Requirements

Install the following Python packages:

```bash
pip install streamlit plotly numpy pandas
```

## Run locally

From the project folder, run:

```bash
streamlit run app.py
```

Then open the local Streamlit URL shown in your terminal.

## How the simulation works

The app uses a simplified model to generate a set of rays/photons and assign their final positions based on the selected mode.

### 1. Passive eye (our universe)
This mode uses sinusoidal patterns to mimic a more wave-like visual behavior, where the eye receives rather than actively pulls.

### 2. Gravitational eye
This mode applies an inward pull factor that increases around the “eye / horizon” region, bending paths toward the observer.

### 3. Conscious observer field
This mode uses a collapse-style parameter driven by consciousness weight and observer state, pushing the system from ambiguity toward more constrained outcomes.

### Observer effect
When the observer toggle is on, the simulation applies an additional collapse/compression effect to the final ray positions.

## GenAI note

The app currently uses a **local faux-GenAI generator** rather than calling an external language model API.

That means:

- No API key is required
- It works offline once dependencies are installed
- The reflection output is rule-based and state-aware, not produced by a real LLM

## Possible upgrades

You can extend this project by adding:

- Real Gemini, OpenAI, or Ollama integration
- Animated photon travel instead of final-hit visualization only
- Multi-step slit geometry
- Better wave/particle rendering
- Historical references to Euclid, Plato, and Ibn al-Haytham
- A stronger scientific disclaimer and a “philosophy vs physics” mode switch

## Disclaimer

This project is mainly a **creative and philosophical simulation**. It borrows language from physics, but it should not be treated as a rigorous model of optics, gravity, black holes, or quantum measurement.

## Why this project exists

This simulator was created to explore a provocative idea:

> If eyes pulled light like black holes, would perception become a form of physical intervention rather than passive observation?

The app gives that question a visual and interactive form.
