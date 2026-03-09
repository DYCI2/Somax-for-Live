# Somax for Live

As part of the [REACH project](https://reach.ircam.fr/) in the Music Representations Team at IRCAM, **Somax for Live** brings the real-time interactive capabilities of [Somax 2](https://github.com/DYCI2/Somax2) directly into Ableton Live. 

Implemented as a collection of Max for Live devices, Somax for Live allows users to interactively co-create with the system within Live’s native environment. It combines the temporal and stylistic modeling of the core Somax engine with the flexibility of Live’s clips, automations, and control interfaces. This tight coupling between musical intelligence and production tools encourages a fluid dialogue between human and machine musicianship, enabling adaptive accompaniment, generative composition, and exploratory performance practices within an accessible and modular setup.

Developed by Manuel Poletti in collaboration with Marco Fiorini, this new integration bridges advanced symbolic AI improvisation with a widely used digital audio workstation, opening new creative workflows for composers, performers, and producers.

## Requirements

* **Ableton Live:** Live 11 or 12 (Suite, or Standard with the Max for Live add-on)
* **Max:** Max 8.6 or later (Ensure Live is configured to use your bundled/system Max application)
* **OS:** macOS 10.13 or later *(Note: The included Python server is compiled for macOS)*

## Installation

Because Somax for Live relies on a custom background Python server, it uses a specific folder structure rather than a standard Ableton Live Pack installation.

1. Go to [Releases](https://github.com/DYCI2/Somax-for-Live/releases) and download the latest version.
2. Unzip the downloaded folder and place it in your Ableton **User Library**. 
   * The standard path on macOS is `~/Music/Ableton/User Library/`. 
   * *(Optional: To keep things organized, you can create a folder named `IRCAM` inside your User Library and place the Somax for Live folder inside it).*

> ⚠️ **Important:** Do not separate the server files. Ensure that the Max for Live Server device (`Somax Server.amxd`) and the server application (`somax_server.app`) remain together in the `Presets/Audio Effects/Max Audio Effect/Imported` folder. The device dynamically searches for the server right next to it.

**Note on macOS Security & First Launch:** * The first time you launch Somax for Live, macOS may present security dialogues asking you to give permission to the external server or specific Max externals. Accept each of these to proceed.

* Because of these system permissions and background initializations, **the very first launch might take up to a few minutes**. This delay only happens the first time.
* Once the server is loaded, the Somax Server application icon in your macOS Dock will start bouncing. It may continue bouncing for a few minutes even after the application has successfully started and connected—**this is completely normal and not an error**.

## Getting Started

1. Open Ableton Live.
2. Open the provided **`Somax For Live.als`** session included in the folder.
3. Follow the self-documented steps directly within the Live session. The session is designed to guide you step-by-step through connecting the server, loading corpora, and interacting with the generative agents.
   * **Video Walkthrough:** For a comprehensive visual guide to the interface and musical workflow, please watch our [Somax for Live Getting Started Video on YouTube](INSERT_YOUTUBE_LINK_HERE).

## Documentation and Resources

Because Somax for Live shares the exact same cognitive and generative engine as the Somax2 Max/MSP application and library, the core concepts remain identical.

* **Video Tutorial:** Watch our [Somax for Live Getting Started Video on YouTube](INSERT_YOUTUBE_LINK_HERE) for deep dives into specific features and workflows.
* **Core Somax 2 Engine:** For deep dives into the underlying architecture, visit the main [Somax 2 GitHub Repository](https://github.com/DYCI2/Somax2).
* **Videos, Demos, and Publications:** Can be found on the [Somax2 project page](http://repmus.ircam.fr/somax2).
* **Corpora:** Due to space limitations, only a few small audio corpora are included. Check the [Somax2 Project page](http://repmus.ircam.fr/somax2) for more corpora.

## Credits

Somax2 (c) Ircam 2012-2026

Somax2 is a totally renewed version of the Somax reactive co-improvisation paradigm born in the Music Representations Team at Ircam - STMS. It is part of the research projects ANR MERCI (Mixed Musical Reality with Creative Instruments) and [ERC REACH](https://reach.ircam.fr/) (Raising Co-creativity in Cyber-Human Musicianship) directed by Gérard Assayag.

* **Somax for Live Porting:** Manuel Poletti in collaboration with Marco Fiorini
* **Somax 2 Development & Documentation:** Joakim Borg and Marco Fiorini
* **Somax Creation:** Gérard Assayag and Laurent Bonnasse-Gahot
* **Pre-version 2 & Adaptations:** Axel Chemla Romeu Santos
* **Early Prototype:** Olivier Delerue

Thanks to Georges Bloch and Mikhaïl Malt for their continuous expertise.
Thanks to Bernard Borron, Bernard Magnien, Carine Bonnefoy, Joëlle Léandre, Fabrizio Cassol, Marco Fiorini, and Anaïs del Sordo for their musical material used in the distribution corpus.

## Contacting the Team

See the [Project Page](http://repmus.ircam.fr/somax2).