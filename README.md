# MIDI Synth

A web-based polyphonic synthesizer built with React and the Web Audio API. This application provides a rich interface for sound design, featuring multiple oscillators, filters, modulation envelopes, and full MIDI integration.

[🎹Try it here](https://www.xenoxxx.com/synth/)

## 🚀 Features

### 🎹 Sound Generation
- **Triple Oscillators:** Support for Sine, Square, Sawtooth, and Triangle waveforms with sub-oscillator options.
- **Noise Generator:** Dedicated noise source for adding texture and percussive elements.
- **ADSR Envelope:** Precise control over Attack, Decay, Sustain, and Release for amplitude shaping.
- **Filter Section:** Resonant low-pass filter with frequency and resonance (Q) controls.

### 🎛️ Control & Modulation
- **MIDI Support:** Connect external MIDI controllers to play notes and map hardware knobs/sliders to synth parameters.
- **MIDI Learn:** Intuitive "Learn" mode to quickly assign MIDI CC messages to UI controls.
- **Virtual Keyboard:** On-screen visualizer that highlights active notes and allows for mouse-based play.

### 💾 Presets & Workflow
- **User Presets:** Save and recall your favorite patches to local storage.
- **Batch MIDI Learn:** Special mode to quickly map a series of MIDI CCs to your preset slots.
- **Responsive Design:** Styled with Tailwind CSS for a modern, dark-themed aesthetic that works across different screen sizes.

## 🛠️ Tech Stack

- **Frontend:** React 19 (Functional Components & Hooks)
- **Audio Engine:** Web Audio API
- **Styling:** Tailwind CSS
- **Icons:** Lucide React
- **Animations:** Framer Motion
- **Language:** TypeScript

## 📂 Project Structure

```text
├── components/           # UI Components (Oscillators, Filters, ADSR, etc.)
├── hooks/                # Custom hooks (useSynthEngine for Web Audio logic)
├── constants.ts          # Default parameters and configuration
├── types.ts              # TypeScript interfaces and types
├── App.tsx               # Main application layout and state management
├── index.tsx             # Entry point
└── styles.css            # Global styles and Tailwind imports
```

## 🚦 Getting Started

### Prerequisites
- A modern web browser (Chrome, Edge, or Opera recommended for best MIDI support).
- (Optional) A MIDI controller connected via USB.

### Installation
1. Clone the repository.
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```

## 📖 How to Use

### Connecting MIDI
1. Plug in your MIDI device before opening the app.
2. Select your device from the dropdown menu at the top of the interface.
3. If prompted, allow the browser to access your MIDI devices.

### Using MIDI Learn
1. Click the **"MIDI Learn"** toggle in the header to show learn buttons on controls.
2. Click the **"L"** button next to any parameter (e.g., Filter Cutoff).
3. Move a knob or slider on your MIDI controller. The parameter is now mapped!

### Saving Presets
1. Dial in your desired sound.
2. Click the **"Save"** button on one of the preset slots.
3. Your patch is now stored in your browser's local storage.

## 📜 License
This project is open-source and available under the MIT License.
