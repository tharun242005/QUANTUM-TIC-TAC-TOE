# Quantum Tic-Tac-Toe

Quantum Tic-Tac-Toe is an interactive educational web game that gamifies core principles of quantum mechanics. It transforms the classic Tic-Tac-Toe game into a learning playground for understanding **Superposition**, **Entanglement**, and **Wave Function Collapse** through hands-on gameplay, real-time quantum circuit visualization, and an AI-powered tutor.

The application visualizes quantum behavior using dynamic circuit diagrams and explains complex board states using Google's Gemini API, making abstract quantum concepts intuitive, engaging, and accessible for students, developers, and enthusiasts.

---

## Live App

### Local Deployment
Open the `QUANTUM_TIC_TAC_TOE.html` file directly in any modern web browser.

### Future Deployment
Planned deployment on **Firebase Hosting** for public access.

---

## Tech Stack

- **HTML5** – Semantic structure and layout  
- **CSS3 + Tailwind CSS (CDN)** – Utility-first responsive styling  
- **JavaScript (ES6+)** – Game logic, quantum simulation, DOM manipulation  
- **Google Gemini API** – AI-powered Quantum Tutor explanations  
- **Font Awesome / Heroicons** – SVG iconography  

---

## Features

### Core Gameplay

- **Superposition Moves** – Place moves that exist simultaneously in two squares, represented by the Hadamard (H) gate  
- **Entanglement (Cycles)** – Create dependencies between moves using closed loops, visualized with CNOT gates  
- **Measurement (Collapse)** – Resolve entangled cycles into classical states using probabilistic measurement  
- **Simultaneous Wins** – Supports quantum outcomes where both players can win (Quantum Draw)  
- **Win Detection** – Robust detection for vertical, horizontal, and diagonal wins  

### UI / UX Features

- **Real-Time Circuit Visualizer** – Dynamic quantum circuit panel showing qubits and gates  
- **Interactive Animations** – Glow effects for entanglement, collapse flashes, animated win lines  
- **Guided Status Bar** – Context-aware gameplay instructions  
- **Responsive Design** – Fully playable on desktop and mobile  
- **Dark Mode Interface** – Neon-accented quantum-themed UI  

### AI Integration

- **Quantum Tutor** – Sends current game state to Gemini API for explanations  
- **Contextual Explanations** – Personalized insights on board states, cycles, and strategies  

---

## Getting Started

### Prerequisites

- Modern web browser (Chrome, Edge, Firefox, Safari)  
- Active internet connection (Tailwind CDN + Gemini API)  
- Google Gemini API Key (optional for AI Tutor)

---

### Installation & Usage

1. **Download the file**
   ```
   QUANTUM_TIC_TAC_TOE.html
   ```

2. **Run the game**
   Double-click the file to open it in your browser.  
   No server or build step is required.

3. **Enable AI Tutor (Optional)**
   - Click the **✨ Quantum Tutor** button  
   - Enter your Gemini API Key  
   - The key is stored temporarily for the session only  

---

## Project Structure

```
Quantum Tic-Tac-Toe/
├── QUANTUM_TIC_TAC_TOE.html   # HTML, CSS, JS, game logic
└── README.md                 # Documentation
```

### Internal Code Architecture

**<head>**
- Tailwind CDN imports  
- Custom animations  

**<body>**
- Board UI generation  
- Circuit visualization  
- Modals for help and AI tutor  

**<script>**
- `initGame()` – State initialization  
- `handleBoardClick()` – Input handling  
- `addQuantumMove()` – Superposition logic  
- `findCycle()` – BFS entanglement detection  
- `collapseCycle()` – Deterministic collapse  
- `render()` – UI updates  
- `callGeminiAPI()` – AI integration  

---

## Key Concepts Deep Dive

### Superposition (H Gate)
Moves exist in two squares simultaneously with equal probability.

### Entanglement (CNOT Gate)
Closed loops create linked outcomes forming Bell or GHZ states.

### Collapse (Measurement Gate)
Measurement forces deterministic resolution of all entangled moves.

---

## Browser Compatibility

- Chrome / Edge – Full support  
- Firefox – Full support  
- Safari – Full support  
- Mobile Browsers – Responsive support  

---

## Contributing

1. Fork the repository  
2. Create a feature branch  
3. Submit a PR with clear changes  
4. Maintain single-file structure  

---

## License

Open-source for educational use.

---

## Acknowledgments

- **Google Gemini** – AI Tutor  
- **Tailwind CSS** – Styling  
- **Qiskit** – Quantum circuit inspiration  

**Built by [THARUN P](https://www.linkedin.com/in/tharun-p-4146b4318/) from (https://github.com/tharun242005)** 

© 2025 QUANTUM TIC TAC TOE . All rights reserved.
