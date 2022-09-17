# himham-jak.github.io

This website mainly hosts the <a href="https://himham-jak.github.io/gamefile_reader.html">Jak and Daxter Audio Editor</a>.

The editor currently supports the following actions: 

|               | Opening       | Playing       | Exporting    | Injecting      | Saving       |
| ------------- | ------------- |  ------------- | ------------- | ------------- | ------------- |
| Jak 1 VAGWAD  |           ✔️  |           ❌  |           ❌  |           ✔️  |           ✔️  |
| Jak 2 VAGWAD  |           ❌  |           ❌  |           ❌  |           ❌  |           ❌  |
| Jak 1 SBK     |           ✔️  |           ❌  |           ❌  |           ❌  |           ❌  |
| Jak 2 SBK     |           ✔️  |           ✔️  |           ✔️  |           ❌  |           ❌  |
| Jak 1 MUS     |           ✔️  |           ✔️  |           ✔️  |           ❌  |           ✔️  |
| Jak 2 MUS     |           ✔️  |           ✔️  |           ✔️  |           ❌  |           ✔️  |

## Tips:

All playback for input and output should have the following settings:
- *.wav format
- Monophonic (for now, Jak II may be different)
- Sample rate of 48khz

To inject VAGWAD, you'll need to convert a wav with the above settings into the adpcm headerless audio format. This can be accomplished by using 
the <a href="https://github.com/himham-jak/adpcm/">converter</a> from the PS2SDK. FFMPEG does not currrently support the correct codec for this.
