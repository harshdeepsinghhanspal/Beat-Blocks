# Beat Blocks 🎵
### Interactive 16-Step Drum Machine & Music Sequencer

Beat Blocks is a browser-based drum machine that lets you create, customize, play, and export musical patterns directly from your browser.

Built using **HTML5, CSS3, JavaScript, and the Web Audio API**, it combines a classic 16-step sequencer with customizable instruments, genre-based sound kits, real-time audio visualization, and audio export functionality.

From Rock, Hip-hop, House, Trap, and Techno to traditional Indian percussion styles like Raga and Punjabi, Beat Blocks provides a simple yet powerful environment for experimenting with rhythm and sound.

## ✨ Features

### 1. 16-Step Sequencer
- 8 independent instrument tracks.
- 16 programmable steps per track.
- Interactive beat grid.
- Real-time playback highlighting.
- Individual step activation and deactivation.
- Visual representation of step volume and waveform.
- Clear all option to reset the pattern.

### 2. Multiple Music Genres

Choose from 9 built-in musical presets:

| Genre | Default BPM |
|---|---:|
| Rock | 110 |
| Hip-hop | 90 |
| House | 124 |
| Trap | 140 |
| Funk | 104 |
| Phonk | 130 |
| Techno | 132 |
| Raga | 108 |
| Punjabi | 104 |

Each genre automatically loads its corresponding rhythm pattern, instrument kit, and musical settings.

### 3. Instrument Library

Beat Blocks includes a collection of synthesized instruments.

**Electronic and Western instruments:**
- Kick
- 808 Kick
- Snare
- Rim
- Hi-hat
- Open Hi-hat
- Shaker
- Clap
- Cowbell
- Tom
- Bass
- 808 Bass
- Lead
- Synth Stab
- Pad
- Keys
- Bell

**Indian musical instruments:**
- Dhol
- Tabla
- Bayan
- Taali
- Sitar
- Harmonium
- Tanpura
- Tumbi

All instruments are generated programmatically using browser-based audio synthesis.

### 4. Indian Music Kits 🇮🇳

Beat Blocks includes dedicated Raga and Punjabi instrument configurations.

- **Raga:** Dhol, Tabla, Shaker, Taali, Bayan, Tanpura, Sitar, and Harmonium.
- **Punjabi:** Dhol, Tabla, Shaker, Taali, Bayan, Bass, Tumbi, and Harmonium.

These kits include predefined rhythmic patterns and melodic note arrangements.

### 5. Advanced Block Editor

Customize individual steps using the integrated block editor.

- Block Volume: Adjust the volume of an individual step.
- Pitch / Tune: Change pitch from -24 to +24 semitones.
- Damp / Sustain: Control the sound's decay and sustain characteristics.
- Waveform Selection: Choose between Sine, Square, Sawtooth, and Triangle.
- Apply Wave to Whole Row: Apply the selected waveform across an entire instrument track.
- Switch Block Off: Disable an individual step.

Melodic instruments also support a note-selection interface with octave shifting.

### 6. Playback & Audio Controls

- Adjustable tempo from 40 to 220 BPM.
- Manual BPM input.
- Master volume control.
- Swing control from 0% to 60%.
- Individual track volume.
- Track mute functionality.
- Keyboard shortcut: Press Space to play or stop.

### 7. Live Audio Visualizer

A real-time sound-wave visualizer displays the audio waveform during playback.

Powered by the Web Audio API's AnalyserNode, it provides a visual representation of the generated audio signal.

### 8. Audio Export

Export your generated musical patterns directly from the application.

Supported formats:
- MP3
- WAV

Additional options:
- Adjustable export duration from 5 to 120 seconds.
- Offline audio rendering.
- Stereo audio output.
- Automatic download of the generated audio file.

MP3 encoding uses the LAME.js library.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Application structure |
| CSS3 | Responsive interface and styling |
| JavaScript | Sequencer and application logic |
| Web Audio API | Real-time audio synthesis |
| AudioContext | Audio generation and playback |
| OfflineAudioContext | Offline audio rendering |
| AnalyserNode | Live audio visualization |
| Canvas API | Waveform rendering |
| LAME.js | MP3 encoding |
| WAV / PCM | Audio file generation |

## 🚀 Getting Started

### Prerequisites

- Modern web browser (Chrome, Firefox, Edge, or Safari).
- JavaScript enabled.
- Audio output device.
- Internet connection for loading the external LAME.js library.

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/YOUR_USERNAME/beat-blocks.git
```

**2. Navigate to the project directory**

```bash
cd beat-blocks
```

**3. Launch the application**

Open `Beat_Blocks___Drum_Machine.html` in your browser.

Alternatively, use the Live Server extension in Visual Studio Code.

No Node.js installation, build tools, or package manager is required.

## 🎮 How to Use

1. Open Beat Blocks in your browser.
2. Select a musical genre from the preset buttons.
3. Click individual blocks in the 16-step grid to activate or deactivate sounds.
4. Press Play to start the sequencer.
5. Adjust BPM, master volume, and swing.
6. Select an active block to open the block editor.
7. Customize its volume, pitch, waveform, and sustain.
8. Mute individual tracks or adjust their volume.
9. Set the export duration and select MP3 or WAV.
10. Click Export to generate and download your beat.

## 📁 Project Structure

```text
beat-blocks/
│
├── index.html
└── README.md
```

The application is currently implemented as a single HTML file containing the interface, styling, JavaScript logic, instrument synthesis, sequencer, visualizer, and export functionality.

## 📱 Responsive Design

Beat Blocks includes a responsive layout designed for different screen sizes.

- Two-column desktop interface.
- Single-column layout on smaller screens.
- Horizontally scrollable sequencer grid.
- Light and dark appearance support.
- Touch-friendly interactive controls.

## 🔊 Audio Architecture

The application uses browser-native audio synthesis instead of relying on pre-recorded instrument samples.

The sound generation system combines:

- Oscillators for tonal sound generation.
- BufferSource nodes for noise generation.
- BiquadFilter nodes for frequency shaping.
- GainNode for volume and amplitude envelopes.
- AnalyserNode for real-time waveform visualization.
- OfflineAudioContext for rendering audio before export.

This approach allows instruments to be generated and customized dynamically.

## 🔮 Future Improvements

Potential development opportunities:

- Save and load custom beat patterns.
- Export and import project files.
- MIDI export support.
- Additional instrument libraries.
- Multi-pattern song arrangement.
- More advanced effects such as reverb, delay, and distortion.
- Per-track equalizer and effects.
- Audio sample import functionality.
- Enhanced mobile touch controls.

## 📄 License

This project is available for personal learning and experimentation. Add an explicit open-source license if you intend to permit reuse, modification, or redistribution.

---

**Create beats. Experiment with sounds. Build your rhythm.**

Made with ❤️ using JavaScript and the Web Audio API.
