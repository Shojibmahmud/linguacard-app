# 🃏 LinguaCard Pro

![LinguaCard Pro Cover](https://via.placeholder.com/1200x400?text=LinguaCard+Pro+-+Advanced+Spaced+Repetition+Engine)

**LinguaCard Pro** is a high-performance, single-file web application engineered to accelerate language acquisition and vocabulary memorization. By combining a scientifically proven Spaced Repetition System (SRS) with an intuitive, gesture-driven user interface, LinguaCard Pro delivers a premium learning experience entirely within your web browser.

The entire application—including styles, application logic, and user interface—is contained within a single `linguacard_pro.html` file, requiring zero build steps, dependencies, or server-side infrastructure.

---

## ✨ Comprehensive Feature Set

### 🧠 Built-in Spaced Repetition System (SRS)
At the core of LinguaCard Pro is an automated Leitner Box algorithm designed to optimize your study time. 
*   **Adaptive Learning**: Cards are categorized into "Boxes" based on your recall confidence.
*   **Mastery Tracking**: Correctly recalling a card ("Know It!") promotes it to a higher box (up to Box 3), while marking it as "Hard" demotes it back to Box 1 for immediate reinforcement.
*   **Visual Progress**: Each deck displays a dynamic mastery progress bar calculating the percentage of cards that have reached maximum mastery.

### 🗣️ Native Text-to-Speech (TTS) Engine
Leveraging the browser's native `speechSynthesis` API, the application provides authentic pronunciation for your target vocabulary[cite: 1, 2].
*   **Smart Voice Matching**: The app automatically detects the target language of your deck (e.g., `es-ES`, `ja-JP`) and maps it to the appropriate system voice.
*   **Auto-Pronunciation**: Optionally toggle "Auto-Speak" to have words read aloud immediately upon viewing or flipping a card.
*   **Adjustable Rates**: Fine-tune the speaking speed (from 0.5x slow to 1.5x fast) using the built-in configuration modal.

### 📱 Gesture-Driven Interface
Designed with a mobile-first philosophy, the study workspace feels like a native mobile app.
*   **Tinder-Style Swiping**: Touch physics allow you to physically drag and swipe cards across the screen[cite: 1, 2].
*   **Swipe Right**: Mark a card as "Know It!"[cite: 1, 2].
*   **Swipe Left**: Mark a card as "Hard / Study"[cite: 1, 2].
*   **3D Animations**: Smooth, hardware-accelerated CSS 3D transforms (`perspective-1000`, `rotate-y-180`) power the card flipping and swiping animations.

### 💾 100% Client-Side Data Management
Privacy and speed are paramount. All user data is managed directly on your device[cite: 1, 2].
*   **LocalStorage Persistence**: Decks, custom cards, learning metrics, and settings are saved automatically to your browser's local storage[cite: 1, 2].
*   **JSON Import / Export**: Safely back up your database or share custom decks with friends by exporting your data as a `.json` file and importing it later[cite: 1, 2].
*   **Pre-loaded Decks**: First-time users are greeted with starter datasets, including "Spanish Essentials" and "Japanese Starter Pack"[cite: 1].

---

## 🚀 Technical Architecture & Stack

LinguaCard Pro achieves a rich feature set without relying on heavy frontend frameworks like React or Vue.

*   **HTML5**: Provides the semantic structure and accessibility foundations.
*   **Tailwind CSS (via CDN)**: Utility-first styling is used extensively to create a modern, clean, and responsive UI (featuring a custom `brand` color palette based on emerald/green tones)[cite: 1, 2].
*   **Vanilla JavaScript**: A centralized `state` object controls the application logic, managing deck selection, the active card index, daily streaks, and total reviews[cite: 1, 2].
*   **FontAwesome (v6.4.0)**: Delivers crisp, scalable vector icons for the user interface[cite: 1].
*   **Google Fonts**: Utilizes the highly legible `Inter` typeface for professional typography[cite: 1].

---

## 🛠️ Installation & Getting Started

Because the application is completely self-contained, getting started takes literally seconds.

1. **Acquire the File**: Clone the repository or simply download the `linguacard_pro.html` file.
   ```bash
   git clone [https://github.com/yourusername/linguacard-pro.git](https://github.com/yourusername/linguacard-pro.git)
Launch the App: Double-click linguacard_pro.html to open it in any modern, standard-compliant web browser (Google Chrome, Microsoft Edge, Apple Safari, or Mozilla Firefox).  No Build Step: There is no need to install Node.js, run npm install, or spin up a local development server.  

🧠 User Guide: How to Study
1. Deck Creation & ManagementNavigate to the sidebar and click + New Deck[cite: 1, 2].
Assign a title, a description, and strictly define the Target Language Tag (e.g., French, German, Mandarin) so the TTS engine functions correctly[cite: 1].
2. Creating FlashcardsOpen your newly created deck and click the black + Add Card button in the main workspace[cite: 1]. Provide the Front Word / Term (target language), the Back Translation, and an optional context sentence to help with real-world usage[cite: 1].
3. The Study LoopReveal: Click or tap the active flashcard to flip it over and reveal the translation and context sentence[cite: 1, 2].
 Grade Confidence: Click the green Know It! button (or swipe right) if you remembered the word easily[cite: 1].Click the red Hard / Study button (or swipe left) if you struggled[cite: 1]. Monitor Stats: Watch your daily streak (indicated by the fire icon) and your total review count climb in the sidebar metrics panel[cite: 1].
4. Application ConfigurationClick the sliders icon (fa-sliders) in the top navigation bar to open the Preferences & Synthesis modal[cite: 1]. Here, you can toggle the auto-speak functionality, adjust the voice reading speed, or perform a hard reset of the application database[cite: 1].

📁 File Structure Overview

Plaintext

📁 linguacard-pro/
 ├── 📄 linguacard_pro.html    # Core application (HTML Structure, Tailwind Config, CSS, Vanilla JS)
 └── 📄 README.md              # Project documentation and specifications

 
🤝 Contributing to LinguaCard ProContributions, bug reports, and feature requests are highly encouraged! If you have ideas to improve the SRS algorithm or add new UI themes, please get involved.  Fork the Project.  Create your Feature Branch: git checkout -b feature/AmazingFeature[cite: 2].Commit your Changes: git commit -m 'Add some AmazingFeature'[cite: 2].Push to the Branch: git push origin feature/AmazingFeature[cite: 2].Open a Pull Request[cite: 2].📜 LicenseThis project is distributed under the MIT License. See the LICENSE file for more information[cite: 2].

Built with ❤️ for language learners everywhere.
