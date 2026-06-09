<p align="center"><img width="157" height="65" alt="myk7bannersmall" src="https://github.com/user-attachments/assets/bdcebd18-44f5-4593-b591-79e30c1bd023" /></p>

**_<p align="center">Vintage Cassette Tape Audio Effects.</p>_**

---

![Version](https://img.shields.io/badge/Version-1.0.0-brightgreen?style=flat-square)
![macOS Support](https://img.shields.io/badge/macOS-Sonoma%20%7C%20Sequoia%20%7C%20Tahoe-000000?style=flat-square&logo=apple&logoColor=white)
![Architecture](https://img.shields.io/badge/Architecture-Intel%20%7C%20Arm64%20%7C%20U2B-black?labelColor=606060&style=flat-square&logo=apple&logoColor=white)
![Format](https://img.shields.io/badge/Format-Standalone%20%7C%20AU%20%7C%20VST3-00CED1?style=flat-square)
![DAW](https://img.shields.io/badge/DAW-Ableton%20Live%2012%2B-000000?style=flat-square&logo=abletonlive&logoColor=white)

---

<p align="center"><img width="695" height="639" alt="myk7preview" src="https://github.com/user-attachments/assets/6acaf768-4964-4d72-b530-694dca1cd375" /></p>

---

## 𝐅𝐞𝐚𝐭𝐮𝐫𝐞𝐬

- **Authentic Tape Simulation**: Add realistic tape instability with Wow and Flutter controls.
- **Analog Saturation**: Dial in warm, asymmetrical saturation to recreate the harmonic richness of magnetic tape.
- **Tape Failure**: Simulate random tape dropouts, degradation and age with the Failure parameter.
- **13 Curated Presets**: Instantly recall classic tape machine characteristics (from pristine studio decks to broken portastudios).
- **Live Output Recording**: Capture your recordings.
- **Interactive Drawing Spectrogram**: Visualize your audio in real-time.
- **Standalone Desktop Application**: Low-latency processing on macOS, no internet required, no browser required.

---

## 𝐒𝐲𝐬𝐭𝐞𝐦 𝐑𝐞𝐪𝐮𝐢𝐫𝐞𝐦𝐞𝐧𝐭𝐬

- **macOS**: 14.0 (Sonoma), 15.0 (Sequoia) or 16.0 (Tahoe).
- **Architecture**: Intel (x64), Apple Silicon (Arm64) or Universal (U2B)
- **DAW (Plugin mode)**: Ableton Live 12 or 11, Logic Pro, Reason with the [BlackHole](https://github.com/ExistentialAudio/BlackHole) virtual audio driver for DAW routing in Standalone mode.
> Audio Unit (AU) & VST3 plugins formats are currently under development.

---

## 𝐈𝐧𝐬𝐭𝐚𝐥𝐥𝐚𝐭𝐢𝐨𝐧

### 𝐒𝐭𝐚𝐧𝐝𝐚𝐥𝐨𝐧𝐞
1. Download the latest [`My K7`](https://github.com/KouseiMusic/My-K7/releases/tag/My-K7-1.0.0).
2. Extract & Drag `My K7` to your `Applications` folder.
3. Open `My K7`.
4. Click on `Load`.

### 𝐀𝐮𝐝𝐢𝐨 𝐔𝐧𝐢𝐭 (𝐀𝐔) 
> 𝐔𝐧𝐝𝐞𝐫 𝐃𝐞𝐯𝐞𝐥𝐨𝐩𝐦𝐞𝐧𝐭

### 𝐕𝐒𝐓𝟑 
> 𝐔𝐧𝐝𝐞𝐫 𝐃𝐞𝐯𝐞𝐥𝐨𝐩𝐦𝐞𝐧𝐭

---

## 𝐂𝐨𝐧𝐭𝐫𝐨𝐥𝐬

- **Real-time Audio Processing:** Load any audio sample and apply vintage cassette tape effects on the fly.
- **Tape Mechanisms:** Replicate motor inconsistencies and mechanical wear.
- **Magnetic Degradation:** Shape the tonal balance and introduce analog distortion.

### 𝐓𝐚𝐩𝐞 𝐂𝐡𝐚𝐫𝐚𝐜𝐭𝐞𝐫𝐢𝐬𝐭𝐢𝐜𝐬

| Control | Description | Range |
| :--- | :--- | :--- |
| **Wow** | Introduces a slow, randomized pitch fluctuation simulating tape motor speed variations. | 0 to 100 |
| **Flutter** | Adds faster, higher-frequency pitch modulation simulating capstan and pinch roller imperfections. | 0 to 100 |
| **Saturate** | Pushes the signal into soft-clipping distortion, mimicking hot recording levels on magnetic tape. | 0 to 100 |
| **Failure** | Introduces random volume dropouts, high-frequency loss and noise bursts typical of damaged or aged tape. | 0 to 100 |

### 𝐆𝐥𝐨𝐛𝐚𝐥 𝐂𝐨𝐧𝐭𝐫𝐨𝐥𝐬

| Control | Description |
| :--- | :--- |
| **Load** | Opens a file dialog to select and load a new audio file (standard audio formats supported). |
| **Presets** | Dropdown menu featuring 13 distinct tape model configurations. |
| **Volume** | Master output volume control dial. |
| **Record** | Start and stop live recording of the master output. |
| **Play** | Starts playback of the loaded sample. |
| **Pause** | Pauses playback at the current position. |
| **Stop** | Stops playback and returns the playhead to the beginning. |
| **Theme Switcher** | A hidden toggle at the top right to switch between Kawaii and Doodle visual identities. |

---

## 𝐂𝐫𝐞𝐝𝐢𝐭𝐬

This software is developped in collaboration with [My Melody](https://github.com/My-Melodies).

---

## 𝐃𝐀𝐖 𝐔𝐬𝐚𝐠𝐞

**Standalone + BlackHole**: Install the [`BlackHole`](https://github.com/ExistentialAudio/BlackHole) virtual audio driver, set `My K7` output to `BlackHole` in macOS `Audio MIDI Setup`, and route `BlackHole` as an input track in your DAW. This allows you to record the output in real time or resample it.

**Audio Unit (AU) & VST3**: Plugins formats are under development. When available they will support full parameter automation and direct DAW audio routing without BlackHole.

---

_This software is free. Don't forget to give it a ⭐ on Github if you liked the project._

---

<p align="center"><code>𝒦𝑜𝓊𝓈𝑒𝒾</code></p>
<p align="center"><code>2026</code></p>
