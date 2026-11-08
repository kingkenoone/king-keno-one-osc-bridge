# King Keno One OSC Bridge

Connect OSC devices and applications to MIDI workflows in your DAW. King Keno One OSC Bridge is a Windows VST3 instrument with configurable OSC addresses, network endpoints and MIDI mappings.

## Download

[Download the Windows x64 VST3 package](https://github.com/kingkenoone/king-keno-one-osc-bridge/raw/refs/heads/main/downloads/KingKenoOne-OSC-Bridge-0.2.1-Windows-x64-Plugin-Only.zip)

The ZIP contains the plug-in and an English setup guide. Close your DAW, extract the ZIP, copy the entire VST3 bundle into a VST3 folder, and restart or rescan your DAW.

## What it does

- Receives OSC messages over IPv4 and UDP and turns them into MIDI CC or short note triggers.
- Sends matching incoming MIDI CC and note values back as OSC messages.
- Supports configurable addresses, ports, MIDI channels and mappings.
- Saves settings with the DAW project.

Incoming messages trigger a mapping when they contain no argument or a positive integer or float. A zero argument is ignored. Note triggers last 100 ms.

## DAW setup

Load the bridge as a VST3 instrument. To receive its MIDI output in another instrument, select the bridge output as the MIDI input of a second instrument track and enable monitoring. In Studio One, check the receiving track's input selector separately from its instrument output. MIDI routing has been confirmed in Studio One.

MIDI-based DAW transport control requires host-specific routing and has not been confirmed for every host. REAPER's native OSC transport support is a separate feature.

## Companion app

King Keno One Easy OSC for Android can act as an OSC controller. The app is currently in testing. The bridge works with other OSC-capable devices and software that use its supported message formats.

## Requirements and licensing

- Windows x64 and a VST3-compatible host.
- An OSC sender or receiver using IPv4 and UDP.
- Built with JUCE 8.0.8.

