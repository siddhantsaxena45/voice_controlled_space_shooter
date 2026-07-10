# 🌌 Voice Controlled Space Shooter Game

A classic 2D space shooter game built with **Python**, **Pygame**, and **Vosk**, where you can control your spaceship entirely using your voice! Navigate through challenging waves, collect power-ups, and defeat powerful bosses—all by speaking commands.

download link -> https://drive.google.com/file/d/1mobAIixeH6N7pKpXY3MvVsQ6eYE7vVNc/view?usp=drive_link
---

## ✨ Features

*   **🎙️ Voice Control Gameplay:** Use spoken commands to move, shoot, navigate menus, and select levels.
*   **🛸 Exciting 2D Space Combat:** Battle through multiple waves of enemies with progressively increasing difficulty.
*   **💥 Boss Fights:** Face off against unique and challenging boss ships at the end of higher levels (Levels 2-4).
*   **⚡ Power-ups:** Enhance your ship with health boosts, protective shields, and rapid-fire capabilities.
*   **🖱️ Traditional Controls Supported:** Prefer the classic way? Keyboard and mouse controls are fully supported.
*   **🧵 Threaded Audio Processing:** Voice recognition runs in the background for lag-free gaming performance.

---

## 🛠️ Technology Stack

*   **[Python 3.7+](https://www.python.org/):** Core programming language.
*   **[Pygame](https://www.pygame.org/):** For rendering graphics, game loop management, collision detection, and audio playback.
*   **[Vosk](https://alphacephei.com/vosk/):** Lightweight and offline speech-to-text engine for voice control.
*   **[Sounddevice](https://python-sounddevice.readthedocs.io/):** For capturing raw audio from the microphone.

---

## 🎮 How to Play

### Voice Commands

Ensure your microphone is connected and try the following voice commands to control the game:

*   **Menu Navigation:**
    *   `"start"`: Start the game from the main menu.
    *   `"quit"`: Exit the game.
    *   `"level one"`, `"level two"`, `"level three"`, `"level four"`: Select a specific level.
*   **Movement:**
    *   `"left"`: Move ship left.
    *   `"right"`: Move ship right.
    *   `"up"`: Move ship up.
    *   `"down"`: Move ship down.
    *   `"stop"`: Stop movement.
*   **Combat:**
    *   `"fire"`: Start shooting lasers.
    *   `"cease fire"` or `"stop fire"`: Stop shooting.

### Keyboard Controls (Fallback)

*   **Movement:** Arrow keys (`Up`, `Down`, `Left`, `Right`)
*   **Shoot:** `Spacebar`
*   **Menu:** Mouse clicks

---

## 🚀 Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/voice-controlled-space-shooter.git
    cd voice-controlled-space-shooter/code
    ```

2.  **Create a virtual environment (Recommended):**
    ```bash
    python -m venv venv
    # On Windows:
    venv\Scripts\activate
    # On Linux/Mac:
    source venv/bin/activate
    ```

3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Download the Vosk Voice Model:**
    *   Download the **English Small** model from the [Vosk Models page](https://alphacephei.com/vosk/models).
    *   Extract the downloaded folder into the `models/` directory. Ensure the extracted folder is named exactly `vosk-model-small-en-us-0.15`.

5.  **Run the game:**
    ```bash
    python main.py
    ```

---

## 📂 Project Structure

```text
code/
├── main.py               # Core game loop, rendering, and logic
├── voice_control.py      # Audio capturing and Vosk model processing
├── requirements.txt      # Python package dependencies
├── assets/               # Images and sprites (ships, lasers, power-ups, bosses)
├── sounds/               # Sound effects (lasers, explosions, game over)
└── models/               # Vosk speech recognition models directory
```

---

## 💡 Troubleshooting

*   **Voice controls are unresponsive or laggy:**
    *   Ensure you are in a quiet environment.
    *   Consider using a headset microphone to reduce background noise interference.
*   **Model Not Found Error:**
    *   Double-check that the Vosk model is downloaded, extracted, and placed exactly at `models/vosk-model-small-en-us-0.15/`.
*   **Audio Device Issues:**
    *   Check your default microphone settings in your OS to ensure Python has permission to access it.

---

![Screenshot 1](screenshots/s%20(1).png)
![Screenshot 2](screenshots/s%20(2).png)
![Screenshot 3](screenshots/s%20(3).png)
![Screenshot 4](screenshots/s%20(4).png)

## 📜 Credits

*   **Programming & Design:** [Siddhant Saxena]
*   **Speech Recognition Engine:** [Vosk](https://alphacephei.com/vosk/)
*   **Game Framework:** [Pygame](https://www.pygame.org/)
