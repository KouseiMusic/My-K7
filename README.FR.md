<p align="center"><img width="157" height="65" alt="myk7bannersmall" src="https://github.com/user-attachments/assets/bdcebd18-44f5-4593-b591-79e30c1bd023" /></p>

**_<p align="center">Effets Audio Cassette Vintage.</p>_**

---

![Version](https://img.shields.io/badge/Version-1.1.0-brightgreen?style=flat-square)
![macOS Support](https://img.shields.io/badge/macOS-Sonoma%20%7C%20Sequoia%20%7C%20Tahoe-000000?style=flat-square&logo=apple&logoColor=white)
![Architecture](https://img.shields.io/badge/Architecture-Universal-black?labelColor=606060&style=flat-square&logo=apple&logoColor=white)
![Format](https://img.shields.io/badge/Format-Standalone%20%7C%20AU%20%7C%20VST3-00CED1?style=flat-square)
![DAW](https://img.shields.io/badge/DAW-Ableton%20Live%2012%2B-000000?style=flat-square&logo=abletonlive&logoColor=white)

---

<p align="center"><img width="711" height="652" alt="myk7preview" src="https://github.com/user-attachments/assets/05ef1d24-9456-4dd2-9259-da1362efefa2" /></p>

---

## 𝐅𝐨𝐧𝐜𝐭𝐢𝐨𝐧𝐧𝐚𝐥𝐢𝐭é𝐬

- **Authentique Simulation**: Ajoutez une instabilité de bande réaliste avec Wow et Flutter.
- **Saturation Analogique**: Ajustez une saturation asymétrique et chaleureuse pour recréer la richesse harmonique de la bande magnétique.
- **Tape Failure**: Simulez les pertes de signal aléatoires, la dégradation et l'usure avec Failure.
- **16 Presets**: Rappelez instantanément les caractéristiques de machines à bande classiques (des platines de studio haut de gamme aux portastudios cassés).
- **Enregistrement** : Capturez vos enregistrements directement.
- **Spectrogramme interactif**: Visualisez votre audio en temps réel.
- **Application Standalone**: Traitement à faible latence sur macOS, sans besoin d'internet ni de navigateur.

---

## 𝐂𝐨𝐧𝐟𝐢𝐠𝐮𝐫𝐚𝐭𝐢𝐨𝐧 𝐑𝐞𝐪𝐮𝐢𝐬𝐞

- **macOS**: 14.0 (Sonoma), 15.0 (Sequoia) ou 16.0 (Tahoe).
- **Architecture**: Intel (x64), Apple Silicon (Arm64) ou Universal (U2B).
- **DAW (mode Plugin)**: Ableton Live 12 ou 11, Logic Pro, Reason avec le pilote
audio virtuel [`BlackHole`](https://github.com/ExistentialAudio/BlackHole) pour le routage DAW en mode Standalone.

> Les formats plugins Audio Unit (AU) & VST3 sont actuellement en cours de
développement.

---

## 𝐈𝐧𝐬𝐭𝐚𝐥𝐥𝐚𝐭𝐢𝐨𝐧

### 𝐒𝐭𝐚𝐧𝐝𝐚𝐥𝐨𝐧𝐞

1.  Téléchargez la dernière version de [`My K7`](https://github.com/KouseiMusic/My-K7/releases/download/My_K7_1.1.0/My.K7.app.macOS.Universal.zip).
2.  Dézippez et glissez `My K7` vers votre dossier `Applications`.
3.  Ouvrez `My K7`.
4.  Cliquez sur `Load`.

### 𝐀𝐮𝐝𝐢𝐨 𝐔𝐧𝐢𝐭 (𝐀𝐔)

> 𝐄𝐧 𝐜𝐨𝐮𝐫𝐬 𝐝𝐞 𝐝é𝐯𝐞𝐥𝐨𝐩𝐩𝐞𝐦𝐞𝐧𝐭

### 𝐕𝐒𝐓𝟑

> 𝐄𝐧 𝐜𝐨𝐮𝐫𝐬 𝐝𝐞 𝐝é𝐯𝐞𝐥𝐨𝐩𝐩𝐞𝐦𝐞𝐧𝐭

---

## 𝐂𝐨𝐧𝐭𝐫ô𝐥𝐞𝐬

- **Traitement audio en temps réel**: Chargez n'importe quel échantillon audio et appliquez des effets de cassette vintage à la volée.
- **Mécanismes de bande**: Répliquez les incohérences du moteur et l'usure mécanique.
- **Dégradation magnétique**: Façonnez l'équilibre tonal et introduisez une distorsion analogique.

### 𝐂𝐚𝐫𝐚𝐜𝐭é𝐫𝐢𝐬𝐭𝐢𝐪𝐮𝐞𝐬 𝐝𝐞 𝐥𝐚 𝐛𝐚𝐧𝐝𝐞

| Contrôle     | Description                                                                                                          | Plage   |
| :----------- | :------------------------------------------------------------------------------------------------------------------- | :------ |
| **Wow**      | Introduit une fluctuation de fréquence lente et aléatoire simulant les variations de vitesse du moteur.                | 0 à 100 |
| **Flutter**  | Ajoute une modulation de fréquence plus rapide simulant les imperfections du cabestan et du galet presseur.          | 0 à 100 |
| **Saturate** | Pousse le signal dans une distorsion soft-clipping, imitant les niveaux d'enregistrement élevés.                     | 0 à 100 |
| **Failure**  | Introduit des baisses de volume aléatoires, des pertes de hautes fréquences et des bruits typiques d'une bande usée. | 0 à 100 |

### 𝐂𝐨𝐧𝐭𝐫ô𝐥𝐞𝐬 𝐆𝐥𝐨𝐛𝐚𝐮𝐱

| Contrôle           | Description                                                                                          |
| :----------------- | :--------------------------------------------------------------------------------------------------- |
| **Load**           | Ouvre une fenêtre pour sélectionner et charger un nouveau fichier audio.                             |
| **Presets**        | Menu déroulant proposant 13 configurations distinctes de modèles de bande.                           |
| **Volume**         | Molette de contrôle du volume de sortie général.                                                     |
| **Record**         | Démarre et arrête l'enregistrement en direct de la sortie Master.                                    |
| **Play**           | Lance la lecture de l'échantillon chargé.                                                            |
| **Pause**          | Interrompt la lecture à la position actuelle.                                                        |
| **Stop**           | Arrête la lecture et replace la tête de lecture au début.                                            |
| **Theme Switcher** | Un interrupteur caché en haut à droite pour basculer entre les identités visuelles Kawaii et Doodle. |

--- 

## 𝐂𝐫é𝐝𝐢𝐭𝐬

Ce logiciel est développé en collaboration avec [My Melody](https://github.com/My-Melodies).

---

## 𝐔𝐭𝐢𝐥𝐢𝐬𝐚𝐭𝐢𝐨𝐧 𝐞𝐧 𝐃𝐀W

Standalone + BlackHole : Installez le pilote audio virtuel [`BlackHole`](https://github.com/ExistentialAudio/BlackHole), réglez la
sortie de `My K7` sur `BlackHole` dans la `Configuration audio et MIDI` de macOS et
configurez `BlackHole` comme entrée de piste dans votre DAW. Cela vous permet
d'enregistrer la sortie en temps réel ou de la ré-échantillonner.

Audio Unit (AU) & VST3 : Les formats plugins sont en développement. Lorsqu'ils
seront disponibles, ils supporteront l'automatisation complète des paramètres et
le routage audio direct sans BlackHole.

---

## 𝐂𝐡𝐚î𝐧𝐞 𝐝𝐞 𝐒𝐢𝐠𝐧𝐚𝐥

```

┌─────────────────────────────────────────────────────────────────────┐
│                        MY K7 — SIGNAL PATH                          │
└─────────────────────────────────────────────────────────────────────┘

    [Audio]
       │
       ├──────────────────────────────────────────┐
       │  (wet path)                              │  (dry bypass)
       ▼                                          │
  ┌─────────┐   ┌─────────┐   ┌─────────┐         │
  │   HPF   │──▶│   LPF   │──▶│  Peaking│         │
  │(lo cut) │   │(hi cut) │   │   EQ    │         │
  └─────────┘   └─────────┘   └─────────┘         │
       │    ▲   Preset model fingerprint          │
       │    └─── (HPF / LPF / PEQ per preset)     │
       ▼                                          │
  ┌──────────┐   ┌────────────┐                   │
  │Waveshaper│──▶│ Bitcrusher │                   │
  │(Saturate)│   │ (Worklet)  │                   │
  └──────────┘   └────────────┘                   │
       │          4× oversample                   │
       ▼                                          │
  ┌──────────────────────────────┐                │
  │         Delay Line           │◀──┐            │
  │   ┌──────────┐ ┌──────────┐  │   │            │
  │   │  Wow LFO │ │Flutter   │  │   │            │
  │   │  (0.5Hz) │ │LFO(15Hz) │  │   │            │
  │   └────┬─────┘ └────┬─────┘  │   │            │
  │        └────────────┘        │   │            │
  │         delayTime mod        │   │            │
  └──────────────────────────────┘   │            │
       │                             │            │
       ▼                             │            │
  ┌──────────┐  ┌──────────┐         │            │
  │ Flutter  │  │  Noise   │         │            │
  │  Amp Mod │  │ (hiss +  │         │            │
  │  (×gain) │  │  pops)   │         │            │
  └────┬─────┘  └────┬─────┘         │            │
       └─────────────┘               │            │
               │                     │            │
               ▼                     │            │
         ┌──────────┐                │            │
         │ Failure  │                │            │
         │  Gain    │── (dropout     │            │
         │          │    events) ────┘            │
         └──────────┘                             │
               │                                  │
               ▼                                  │
         ┌──────────┐                             │
         │ Wet Vol  │◀── Volume × satAttenuation  │
         └──────────┘                             │
               │                                  │
               ▼                                  │
         ┌──────────┐   ┌──────────┐              │
         │  Master  │◀──│ Dry Gain │◀─────────────┘
         │   Gain   │   │ (bypass) │
         └──────────┘   └──────────┘
               │
               ▼
         ┌──────────┐
         │ Limiter  │  threshold: −1 dBFS
         │(20:1 BR) │  attack: 1 ms
         └──────────┘  release: 100 ms
               │
               ▼
         ┌──────────┐   ┌────────────┐
         │  Output  │──▶│  Analyser  │──▶ [Spectrogramme]
         │   Gain   │   │  (FFT)     │
         └──────────┘   └────────────┘
               │
               ▼
        ┌────────────────────┐   
        │ Audio Output / DAW │   
        └────────────────────┘  
``` 

---

Ce logiciel est gratuit. N'oubliez pas de lui donner une ⭐ sur Github si vous
avez aimé le projet.

---

<p align="center"><code>𝒦𝑜𝓊𝓈𝑒𝒾</code></p>
<p align="center"><code>2026</code></p>
