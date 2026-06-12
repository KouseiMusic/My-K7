# 𝐌𝐲 𝐊𝟕 - 𝐂𝐡𝐚𝐧𝐠𝐞𝐥𝐨𝐠

## 𝟏.𝟏.𝟎 (𝟏𝟐-𝟎𝟔-𝟐𝟎𝟐𝟔)

### 𝐒𝐨𝐮𝐧𝐝 & 𝐏𝐞𝐫𝐟𝐨𝐫𝐦𝐚𝐧𝐜𝐞

- Fixed audio dropouts and stuttering during recording. The previous recording system ran on the same thread as the rest of the application, meaning brief spikes in CPU activity from moving knobs or opening menus could interrupt the audio stream. The recorder has been moved to a dedicated audio thread, isolating it from interface activity for glitch-free captures.

- Fixed a volume jump when starting a recording. The recorder was previously wired into the output path in a way that added a second copy of the signal to the speakers, causing a noticeable boost in level. The recorder now listens to the signal passively without contributing to the output, ensuring consistent monitoring levels.

- Fixed the Saturate knob producing harsh, digital-sounding distortion at moderate and high settings. The saturation circuit was operating without oversampling, introducing aliasing artefacts that gave the effect a brittle, unpleasant quality rather than the soft, rounded character of magnetic tape. It now processes at four times the normal rate before stepping back down, preserving warmth across the entire knob range.

- Fixed accumulated automation events causing the Failure effect and delay time to drift uncontrollably over long sessions. When Failure events fired in rapid succession, the underlying system would stack scheduling instructions rather than replacing them, eventually causing sustained mutes or a delay time that slowly wandered away from its intended position. Each new event now cleanly cancels any pending instructions before applying its own.

- Fixed a hard click or pitch glitch when stopping or reloading a sample. Calling stop on a source that had already finished naturally would throw an internal error, occasionally leaving the audio engine in an inconsistent state. This is now handled gracefully regardless of the source's current status.

- Fixed audio resources not being released when loading a new file or closing the application. Oscillators powering the Wow and Flutter effects, as well as the background noise source, were being left running silently in memory after a session ended. All internal audio components are now fully stopped and cleared before a new session begins or the window is closed.

- Added a transparent safety limiter at the final output stage. When combining heavy saturation with high Failure activity and Flutter amplitude modulation simultaneously, output levels could briefly exceed the safe ceiling of the audio system and cause audible distortion in the speakers or interface. The limiter reacts in 1 millisecond and is inaudible under normal conditions, only catching peaks that would otherwise clip.

- Fixed an issue where pressing Play after Pause would restart the sample from the beginning instead of resuming from the paused position. The transport now correctly picks up exactly where it left off.

- Fixed a race condition on startup where rapidly loading a file immediately after launch could result in the saturation and bitcrusher effects being bypassed for the duration of that session. The internal initialization sequence is now locked so that all processing components are guaranteed to be ready before any audio is routed through them.

### 𝐏𝐫𝐞𝐬𝐞𝐭𝐬

- Recalibrated all 13 presets to prevent clipping and ear fatigue. Several presets were reaching levels that were too dense for comfortable monitoring, or contained EQ curves that did not accurately reflect the character of the hardware they were modelling. Tonal balances, noise levels, and effect intensities have all been individually reviewed and adjusted to preserve each machine's personality while keeping the output safe and controllable at normal listening volumes.

- Added three new hardware presets, bringing the total to 16:

  - 𝐄𝐥𝐜𝐚𝐬𝐞𝐭 𝐄𝐋-𝟕: Sony's short-lived large-cassette format from 1976, engineered to rival open-reel quality. This preset captures its unusually extended low end, wide frequency response and near-silent transport, a sound that feels bigger than any cassette has a right to.

  - 𝐏𝐨𝐫𝐭𝐚𝐬𝐭𝐮𝐝𝐢𝐨 𝟐𝟒𝟒: The Tascam 4-track that defined bedroom recording in the 1980s. A narrow bandwidth, a honky presence in the upper mids, and an audible transport hiss that became the signature texture of lo-fi demos and home-recorded classics.

  - 𝐓𝐂-𝐊𝟓𝟓𝟓: Sony's flagship three-head cassette deck from 1981, one of the quietest and most accurate consumer tape machines ever made. This preset captures its whisper-quiet noise floor, extended high-frequency reproduction and the subtle warmth that only a precision transport can deliver.

### 𝐒𝐞𝐜𝐮𝐫𝐢𝐭𝐲

- Fixed a vulnerability that allowed unauthorized content to run within the application window. A strict policy now prevents any external scripts or injected content from interacting with the interface. The application also runs in a fully sandboxed environment, isolating it from the rest of the system.

- Removed an unnecessary third-party package (Express) that was included in the build by mistake. While unused by the application itself, its presence introduced known vulnerabilities. Its removal results in a cleaner, more secure installation.

- Fixed the application making unnecessary network requests on startup. The interface was attempting to load fonts from an external server, causing silent failures on offline systems. All fonts are now handled locally, requiring no internet access and improving privacy.

- Resolved 11 high-severity and 1 moderate-severity vulnerabilities in the build toolchain. The core runtime (Electron) and packaging tool (electron-builder) have been updated to their latest patched releases, clearing all known advisories including issues related to ASAR integrity, use-after-free callbacks, path traversal during extraction and service worker spoofing. None of these vulnerabilities were ever present in the installed application; they affected the build environment only. The audit report now returns zero issues.

---

## 𝟏.𝟎.𝟎 (𝟐𝟕-𝟎𝟓-𝟐𝟎𝟐𝟔)

- Vintage cassette tape simulation with authentic Wow, Flutter, Saturation and Failure controls.

- 13 curated presets modelling real hardware, from studio open-reel decks to worn portable machines.

- Preset EQ fingerprints per machine: high-pass and low-pass cutoffs, parametric mid coloration and individual noise floor levels tuned per deck.

- Live output recording to file with timestamped filename.

- Interactive waveform spectrogram with theme-aware rendering.

- Two visual themes: Kawaii and Doodle, switchable at any time without interrupting playback.

- Native support for macOS Sonoma, Sequoia and Tahoe (Intel x64, Apple Silicon arm64, Universal Binary).
