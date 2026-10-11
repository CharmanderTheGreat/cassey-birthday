# The Ridleys - Birthday Tribute Web Application

A responsive, single-page interactive web application built as a personalized birthday gift and tribute. The project features an indie band visual theme inspired by The Ridleys, complete with encrypted content gating, an audio player, a dynamic photo gallery, and interactive celebratory elements.

---

## Features

### 1. Passkey Access Gate
- **Restricted Entry**: Content is locked behind a password verification system on page load.
- **Client-Side Cryptography**: Uses the native Web Crypto API (PBKDF2 key derivation paired with 256-bit AES-GCM encryption) to securely decrypt and dynamically inject site data into the DOM upon entering the correct passkey.
- **Interactive UI**: Includes input shake validation for incorrect attempts and an optional toggle to reveal or mask characters.

### 2. Turntable Audio Player
- **Indie-Folk Soundscape**: Houses a custom 5-track music interface styled after vinyl record decks.
- **Vinyl Animation**: Realistic spinning vinyl disc graphic that activates during playback and pauses smoothly when stopped.
- **Playback Controls**: Features Play/Pause, Next Track, Previous Track, track jump pills, dynamic time elapsed/duration counters, and a custom two-tone progress track slider.

### 3. Photo Gallery
- **Curated Snapshots**: A 4-column responsive gallery card system displaying snapshots with custom track labels and descriptions.
- **Responsive Layout**: Fluid CSS grid adapting from single-column mobile views to multi-column desktop displays.

### 4. Interactive Cake and Celebration
- **Illustrated Cake**: Custom SVG illustration with animated flame effects.
- **Candle Blowing Mechanic**: Allows the user to blow out the candle, which triggers an animated smoke visual and an on-screen confetti shower.
- **Replayability**: Includes a relight button enabling the user to repeat the candle-blowing experience.

### 5. Ambient Tap Effects
- **Touch and Click Feedback**: Generates dynamic drifting music and celebration symbols wherever the user taps or clicks across the viewport.

---

## File Structure

```text
├── index.html          # Main application containing structure, styling, and logic
├── images/             # Image directory
│   ├── 1.jpg           # Album cover track 01
│   ├── 2.jpg           # Album cover track 02
│   ├── 3.jpg           # Album cover track 03
│   ├── 4.jpg           # Album cover track 04
│   ├── 5.jpg           # Album cover track 05
│   ├── 6.jpg           # Gallery photo 01
│   ├── 7.jpg           # Gallery photo 02
│   ├── 8.jpg           # Gallery photo 03
│   └── 9.jpg           # Gallery photo 04
└── song/               # Audio directory
    ├── 1.mp3           # Audio track 01
    ├── 2.mp3           # Audio track 02
    ├── 3.mp3           # Audio track 03
    ├── 4.mp3           # Audio track 04
    └── 5.mp3           # Audio track 05
```

---

## Tech Stack

* **Markup**: HTML5
* **Styling**: Tailwind CSS (via CDN) and custom CSS3 animations
* **Typography**: Google Fonts (Cabinet Grotesk, Instrument Serif, Plus Jakarta Sans, Space Mono)
* **Icons**: FontAwesome 6
* **Confetti Engine**: Canvas Confetti
* **Cryptography**: Web Crypto API (PBKDF2, AES-GCM)