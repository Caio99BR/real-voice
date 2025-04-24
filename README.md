# real-voice
Scripts for working with real voice recordings in Synthesizer V Studio Pro

## What is this for?
Typically, "tuning" a voice in a vocal synthesizer means drawing a pitch curve over MIDI notes. The timing of the notes is rarely altered.

I wanted to take a different approach — extracting the pitch curve from a real singer and adjusting the timing to match it. By "timing," I mean the lengths of phonemes and pauses.
This method also tends to sound more natural — after all, it’s partially based on a real human performance. I call this approach "Voice Copy." It’s not entirely accurate; only certain prosodic features are copied.

The scripts in this repository are designed to make that process easier.

## Installation
To use these scripts, you must have Dreamtonics' [Synthesizer V Studio Pro](https://dreamtonics.com/en/synthesizerv/), which supports scripting.
Everything has been tested on Windows, but it should work on any platform where Studio Pro is supported.

1. Download this [ZIP archive](https://github.com/Caio99BR/real-voice/archive/refs/heads/main.zip)
2. Unzip it
3. Move the entire `real-voice-main` folder to the SynthV scripts folder, typically located at:
   `C:\Users\<your_username>\Documents\Dreamtonics\Synthesizer V Studio\scripts\`
4. You can also access this folder from SynthV’s main menu: **Scripts → Open Scripts Folder**, then rename `real-voice-main` to anything you like, e.g., `realVoice`

After restarting SynthV Studio (or rescanning scripts), you should see these scripts in the Scripts menu:

- `RV Filter Pitch` *(obsolete – use Praat's Convert / Smooth function instead)*
- `RV Load Envelope` *(obsolete – create separate notes for consonants instead)*
- `RV Load Pitch` *(updated v3)*
- `RV Notes from TextGrid` *(updated v3, exclamation mark functionality removed)*
- `RV Notes to TextGrid` *(v1)*
- `RV Quantize Pitch` *(v2)*
- `RV Randomize Onsets` *(v1)*
- `RV Split Note` *(updated v3)*

**Tip:** Set up keyboard shortcuts for frequently used scripts:
For example, `Alt+X` for **RV Load Pitch** and `Alt+C` for **RV Split Note**.

## Required Software
You’ll also need [Praat](https://www.fon.hum.uva.nl/praat/), a phonetic analysis tool, installed and runnable.
It’s available for multiple platforms.

## Demo Videos
For instructions on how to use these scripts, check out my demonstration videos on YouTube:
[▶ Playlist](https://youtube.com/playlist?list=PLHA_yIumhQPDJ3PULhXeE-gypioT-eear)

## Known Issues
Files with non-English characters in their paths (e.g., Chinese, Korean, Japanese) may not load correctly.
