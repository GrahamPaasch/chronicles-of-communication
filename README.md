# Chronicles of Communication

A curated digital archive and immersive VR experience that chronicles the evolution of communication methods from pre-internet eras to the modern age.

## Table of Contents

* [Introduction](#introduction)
* [Timeline of Communication Advancements](#timeline-of-communication-advancements)
* [Immersive VR Experiences](#immersive-vr-experiences)
* [Immersive VR Museum Exhibits](#immersive-vr-museum-exhibits)
* [Project Structure](#project-structure)
* [Installation](#installation)
* [Usage](#usage)
* [Contributing](#contributing)
* [License](#license)

## Introduction

This project documents key milestones in human communication and provides immersive VR simulations of each stage. Users will experience how message delivery, reception and social coordination evolved from ancient methods to digital networks.

## Timeline of Communication Advancements

* **Prehistoric – Ancient (pre-1200 BCE):** Horns, flags and mounted messengers.
* **1200 BCE:** Carrier pigeons used for long-distance messages.
* **1792:** Semaphore telegraph towers implement visual code across regions.
* **1837:** Electric telegraph patented by Cooke and Wheatstone.
* **1876:** Telephone invented by Alexander Graham Bell.
* **1886:** First Yellow Pages directory published in Louisville, KY.
* **1906:** First radio broadcast by Reginald Fessenden.
* **1920s:** Expansion of shortwave radio networks.
* **1965:** Electronic mail systems emerge on mainframes.
* **1978:** Ward Christensen launches the first BBS.
* **1983:** ARPANET adopts TCP/IP, forming the early Internet.
* **1990:** World Wide Web created by Tim Berners-Lee.
* **1990s:** Online forums and IRC enable real‑time group chat.
* **2000s:** Social media platforms transform online interaction.
* **2010s–Present:** VR/AR platforms facilitate immersive communication.

## Immersive VR Experiences

Each timeline entry includes a VR module simulating the communication context:

* **Ancient Scenario:** Wear headset; mounted courier follows horn signals.
* **Semaphore Tower:** Operate visual arms to encode and decode messages.
* **Telegraph Operator:** Tap Morse code and observe transmission delays.
* **Switchboard Room:** Route telephone calls via manual switchboards.
* **Yellow Pages Booth:** Search physical directory and place a call.
* **Radio Studio:** Broadcast audio segments to virtual shortwave listeners.
* **BBS Session:** Dial in, navigate menus and post messages in real time.
* **Web Browser:** Explore early web pages and hyperlink structures.
* **VR Social Hub:** Join avatars in a shared virtual environment.

## Immersive VR Museum Exhibits

Our vision is to build AI-generated, cost-effective VR experiences using digitized artifacts from existing collections. Sources such as [Telecom History](https://telecomhistory.org/exhibitsmain.html) and the [Connections Museum](https://en.wikipedia.org/wiki/Connections_Museum) ensure historical accuracy.

### Featured Exhibits

* **1923 Panel Switch** – early automatic switching hardware.
* **1942 No. 1 Crossbar** – reliable crossbar technology.
* **Vintage switchboards** – manual patch-cord systems.

### Asset Pipeline

1. 3D scanning of artifacts.
2. Retopology with LOD models.
3. Spatial audio capture.

### Visitor Experience Flow

1. Enter a period office.
2. Travel through a wire-tunnel.
3. Operate an interactive switchboard.
4. Remove the headset for an AR reveal.

### Pricing Model

At $10k per exhibit with ten released each year, recurring revenue could reach roughly $100k annually.
## Project Structure

```
chronicles-of-communication/
├── README.md
├── timeline/
│   └── data.json
├── vr-modules/
│   ├── ancient/
│   ├── telegraph/
│   └── web/
├── assets/
│   ├── audio/
│   └── models/
└── docs/
    └── design-specs.md
```

## Installation

1. Clone repository.
2. Install dependencies:

   ```bash
   npm install
   ```
3. Build VR modules:

   ```bash
   npm run build
   ```

## Usage

1. Launch local server:

   ```bash
   npm start
   ```
2. Open VR environment in compatible headset.
3. Select timeline stage from menu.

## Contributing

1. Create branch for feature or fix.
2. Submit pull request with description of changes.
3. Adhere to code style and include tests for new modules.

## License

MIT License. See [LICENSE](LICENSE).
