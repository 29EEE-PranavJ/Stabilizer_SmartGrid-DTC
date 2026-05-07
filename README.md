# Quantum-Inspired Nonlinear Feedback System for Smart Grid Signal Stabilization Using DTC Dynamics

A quantum-inspired nonlinear feedback framework for stabilizing noisy smart grid signals using concepts derived from Discrete-Time Crystal (DTC) dynamics.  
This project explores how nonlinear evolution, feedback loops, periodic driving, and memory-based dynamics can suppress disturbances and generate stable signal behaviour in modern power systems.

---

## 📌 Overview

Modern smart grids face severe instability due to:

- Renewable energy intermittency
- Nonlinear disturbances
- Frequency fluctuations
- Harmonic noise
- Dynamic load variations

Traditional filters such as low-pass filters and Kalman filters often struggle in highly nonlinear environments.

This project proposes a completely different approach:

> Instead of filtering the signal directly, the system dynamically evolves toward stability through nonlinear feedback interactions.

The framework is inspired by **Discrete-Time Crystal (DTC)** behaviour observed in physics, where systems maintain stable periodic patterns despite external disturbances.

---

## 🎯 Objective

The main objective of this project is to:

- Design a nonlinear feedback-driven signal stabilization system
- Implement the model in MATLAB Simulink
- Stabilize noisy smart grid signals
- Explore DTC-inspired dynamic behaviour
- Demonstrate emergent stability using nonlinear evolution

---

## 🚀 Key Features

- Quantum-inspired nonlinear dynamics
- Feedback-based stabilization
- DTC-inspired periodic driving
- Memory-based signal evolution
- Noise suppression without conventional filtering
- Adaptive behaviour under disturbances
- MATLAB Simulink implementation
- Smart grid focused architecture

---

## ⚙️ Working Principle

The system operates as a nonlinear dynamical framework.

### Signal Flow

```text
Sine Wave + Noise
        ↓
Input Coupling
        ↓
Nonlinear Processing
        ↓
Memory + Feedback
        ↓
Stabilized Output
```

### Core Mechanism

```math
x(n+1) = α · tanh [ cos( θ · ( x(n) + k·u(n) ) ) ]
```

Where:

- `x(n)` → Current system state
- `u(n)` → Noisy input signal
- `k` → Input coupling strength
- `θ` → Periodic driving parameter
- `α` → Damping factor

---

## 🧠 Core Concepts Used

### 1. Nonlinear Dynamics
The system uses nonlinear evolution instead of linear filtering.

### 2. Feedback Systems
Previous outputs are continuously fed back into the system.

### 3. Periodic Driving
A cosine-based forcing mechanism creates oscillatory structure similar to DTC behaviour.

### 4. Hyperbolic Tangent Stabilization
`tanh()` compresses extreme fluctuations and suppresses noise spikes.

### 5. Memory-Based Evolution
A Unit Delay block stores previous states, enabling adaptive temporal behaviour.

### 6. Emergent Stability
The system self-organizes into a stable waveform despite noisy inputs.

---

## 🖥️ Software Used

| Software | Purpose |
|---|---|
| MATLAB | Mathematical modelling |
| Simulink | System simulation and block implementation |
| Scope Analyzer | Time-domain waveform analysis |

---

## 🏗️ Simulink Architecture

### Main Components

- Sine Wave Block
- Random Noise Generator
- Gain Blocks
- Cosine Function
- Hyperbolic Tangent (`tanh`)
- Unit Delay (`1/z`)
- Feedback Loop
- Scope Visualization

### Architecture Flow

```text
Sine ─┐
      ├── Add → Gain(k) → Add → Gain(θ) → cos → tanh → Gain(α) → Unit Delay → Output
Noise ─┘                               ↑                                        |
                                       └──────── feedback ──────────────────────┘
```

---

## 📊 System Behaviour

### Input Signal
- Highly noisy
- Distorted waveform
- Unstable oscillations

### Output Signal
- Reduced noise
- Stable oscillatory behaviour
- Structured dynamic response
- Bounded nonlinear evolution

The output is **not an exact reconstruction** of the input.

Instead:

> The system generates a stabilized representation through nonlinear self-organization.

---

## 🔬 Observations

### Key Findings

- Noise fluctuations were significantly reduced
- The system remained stable under tuned parameters
- Feedback and damping prevented divergence
- Emergent waveform structures appeared naturally
- High-frequency disturbances were suppressed

### Important Insight

This model does **not behave like a conventional filter**.

It behaves like:

> A nonlinear adaptive stabilization engine.

---

## 📈 Results

| Feature | Input Signal | Output Signal |
|---|---|---|
| Noise Level | High | Reduced |
| Stability | Low | High |
| Waveform Structure | Irregular | Organized |
| Dynamic Behaviour | Chaotic | Controlled |

### Achievements

- Successful stabilization of noisy signals
- Dynamic suppression of fluctuations
- Demonstration of DTC-inspired behaviour
- Robust nonlinear operation under disturbances

---

## ⚡ Applications

### Smart Grid Signal Conditioning
Improves signal integrity before processing.

### Renewable Energy Systems
Stabilizes fluctuating solar/wind output signals.

### Frequency Stability Monitoring
Tracks and smooths frequency variations.

### Microgrid Control
Enhances resilience under dynamic loads.

### Fault Detection
Suppresses normal noise and exposes abnormal disturbances.

### Smart Metering
Improves measurement accuracy and signal quality.

### Adaptive Signal Processing
Acts as an alternative to traditional filters.

---

## 🔮 Future Scope

- FPGA implementation
- Embedded hardware realization
- Multi-state nonlinear systems
- AI-assisted adaptive parameter tuning
- Real smart-grid data testing
- Hybrid nonlinear + classical filtering systems
- Integration into IoT-enabled power infrastructure

---

## 🧪 Technical Highlights

- Nonlinear signal stabilization
- Feedback-controlled evolution
- Quantum-inspired engineering approach
- Emergent dynamic behaviour
- Physics-inspired smart grid application

---

## 🏛️ Institution

**School of Electrical Engineering (SELECT)**  
Vellore Institute of Technology, Chennai

---

## 📚 Research Domain

- Smart Grids
- Nonlinear Dynamics
- Signal Stabilization
- Quantum-Inspired Systems
- Renewable Energy Systems
- Adaptive Signal Processing
- Power System Stability

---

## ⭐ Final Note

This project explores a shift in engineering philosophy:

> From directly filtering signals  
> to allowing stability to emerge through nonlinear dynamics.

The idea is powerful because modern power systems are becoming too chaotic for purely linear assumptions.

This is where future grid intelligence will evolve:
- adaptive
- nonlinear
- feedback-driven
- self-organizing systems.
- ---

## 👨‍💻 Authors

- **Pranav J**
- **Karthikeyan D**
- **Tharun S**
- **Kavin M K**
- **Sri Sarvesh S**
- **Akash Sawhney**
- ---
