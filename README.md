Quantum Tic-Tac-Toe

Quantum Tic-Tac-Toe is an interactive educational web game that gamifies core concepts of quantum mechanics. It transforms the classic grid game into a playground for understanding Superposition, Entanglement, and Wave Function Collapse. The application features a real-time quantum circuit visualizer and an integrated AI Tutor powered by Google's Gemini API to explain complex board states.

Live App

Local Deployment: Open the quantum_tic_tac_toe.html file in any modern web browser.

Future Deployment: Planned for Firebase Hosting.

Tech Stack

HTML5 (Semantic structure)

CSS3 + Tailwind CSS (Utility-first styling via CDN)

JavaScript (ES6+) (Game logic, quantum simulation, and DOM manipulation)

Google Gemini API (AI-powered "Quantum Tutor" feature)

Font Awesome / Heroicons (SVG Icons)

Features

Core Gameplay

Superposition Moves – Place moves that exist in two squares simultaneously (represented by the Hadamard H gate).

Entanglement (Cycles) – Create dependencies between moves by forming closed loops (represented by CNOT gates).

Measurement (Collapse) – Force a "collapse" of entangled cycles into classical states (represented by the Measure M gate).

Simultaneous Wins – Logic to handle distinct quantum outcomes where both players might achieve 3-in-a-row (Quantum Draw).

Win Detection – Robust algorithm to detect vertical, horizontal, and diagonal wins on the classical board.

UI/UX Features

Real-Time Circuit Visualizer – A dynamic panel that draws the actual quantum circuit diagram (qubits and gates) as you play.

Interactive Animations – Glowing pulses for entangled moves, flash animations for collapses, and drawing animations for win lines.

Guided Status Bar – Context-aware instructions guiding the player through each phase (Selection, Entanglement, Measurement).

Responsive Design – Fully playable on desktop and mobile devices.

Dark Mode Interface – Professional dark theme with neon accents for a "quantum" aesthetic.

AI Integration

Quantum Tutor – A "✨ Quantum Tutor" button that captures the current game state and sends it to the Gemini API.

Contextual Explanations – Receives personalized, easy-to-understand explanations of the specific board layout, cycles, and strategic options.

Getting Started

Prerequisites

A modern web browser (Chrome, Edge, Firefox, Safari).

An active internet connection (for loading Tailwind CSS and calling the Gemini API).

Google Gemini API Key (Required only for the "Quantum Tutor" feature).

Installation & Usage

Download the file:
Save the quantum_tic_tac_toe.html file to your computer.

Run the Game:
Double-click quantum_tic_tac_toe.html to open it in your default web browser. No server or build step is required.

Set up the AI Tutor (Optional):

Click the "✨ Quantum Tutor" button in the game.

A modal will appear asking for your API Key.

Enter your Gemini API key (get one at Google AI Studio).

The key is saved temporarily for your session to enable the AI features.

Project Structure

This project utilizes a Single File Architecture for maximum portability and ease of use.

Quantum Tic-Tac-Toe/
├── quantum_tic_tac_toe.html      # Contains all HTML, CSS, and Game Logic
└── README.md                     # This file


Internal Code Structure (inside HTML):

<head>: Tailwind CDN imports, Custom CSS animations (glows, spinners).

<body>:

Board UI: Dynamic grid generation.

Circuit UI: Dynamic gate rendering.

Modals: "How to Play" and "Quantum Tutor" overlays.

<script>:

initGame(): State initialization.

handleBoardClick() / handleCircuitClick(): User input handling.

addQuantumMove(): Logic for superposition.

findCycle(): BFS algorithm for entanglement detection.

collapseCycle(): Deterministic chain reaction logic.

render(): Updates Board and Circuit UIs.

callGeminiAPI(): Integration with Google Gemini.

Key Concepts Deep Dive

Superposition (The H Gate)

Instead of placing an 'X' in one square, a player places a "spooky" move (e.g., $x_1$) in two squares. In the circuit, this applies a Hadamard Gate, putting the qubit into a 50/50 probability state ($|0\rangle + |1\rangle$).

Entanglement (The CNOT Gate)

When a move connects two existing moves into a loop (e.g., A→B, B→C, C→A), a "Cycle" is formed. The fates of these moves become linked. In the circuit, this is visualized as Controlled-NOT (CNOT) gates connecting the qubit wires. The state becomes a Bell State or GHZ State.

Collapse (The M Gate)

To resolve a cycle, a player "measures" one move. This random decision (50/50) forces the chosen move into a specific square. Because of entanglement, this triggers a deterministic chain reaction, forcing all other moves in the cycle to collapse into their only remaining valid positions.

Browser Compatibility

Chrome/Edge (recommended) – Full support

Firefox – Full support

Safari – Full support

Mobile Browsers – Responsive layout adapts to touch screens

Contributing

Contributions are welcome! Since this is a single-file project, please ensure any Pull Requests maintain the contained structure.

Fork the repository.

Create a feature branch.

Submit a PR with a clear description of your changes (e.g., "Improved cycle detection algorithm" or "Added sound effects").

License

This project is open-source and available for educational use.

Acknowledgments

Google Gemini – For powering the AI Tutor.

Tailwind CSS – For the rapid styling system.

Qiskit – For the inspiration behind the quantum circuit logic.
