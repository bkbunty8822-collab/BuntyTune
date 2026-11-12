# BuntyTune v0.5 – by Bunty – auto-key pitch correction + vocal enhance, all in one VST3

Params
- Scale: "Auto (detect)" = plugin finds the song's key itself (needs ~1-2 sec of singing), or pick Key + Chromatic/Major/Minor/Minor Pentatonic manually.
- Key: used only when Scale is not Auto. If you KNOW the song's key, set it manually - most accurate.
- Retune Speed (ms): 1-10 = robotic effect, 10-30 = hidden correction, 50-200 = very natural.
- Natural (Vibrato Keep): 0 = pitch fully flat on the note, 1 = keeps all vibrato/expression. 0.3-0.6 is a good start.
- Mix: dry/wet.

Build: push this folder to a GitHub repo -> Actions tab -> "Build BuntyTune VST3" -> download artifact.
Copy BuntyTune.vst3 to C:\Program Files\Common Files\VST3\ and rescan plugins in your DAW.

## Vocal Enhance chain (after pitch correction)
Low Cut (80Hz) -> Compressor (Threshold/Ratio/Attack/Release/Makeup) -> Presence @3.5k -> Air @10k -> Output Gain
Good starting point for Hindi/news voiceover: Low Cut 80, Threshold -18, Ratio 3, Attack 8, Release 120, Makeup 3, Presence +2, Air +2.
For singing: Ratio 2-3, Threshold -20, Retune Speed 15-30, Natural 0.4.

## Interface
Custom dark/gold BuntyTune UI (820x470): PITCH, COMPRESSOR, ENHANCE panels. Fully original design.

## Raag scales (for Bhojpuri / Indian music)
Scale list also has Bhairavi, Kafi, Khamaj, Bhairav. Pick Key = the Sa (tonic) of your song. For gamak/meend heavy vocals: Retune Speed 40-120ms, Natural 0.7-1.0.
