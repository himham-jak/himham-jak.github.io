# himham-jak.github.io

This website mainly hosts the <a href="https://himham-jak.github.io/gamefile_reader.html">Jak and Daxter Audio Editor</a>.

The editor currently supports the following actions: 

|               | Opening       | Playing       | Exporting    | Injecting      | Saving       |
| ------------- | ------------- |  ------------- | ------------- | ------------- | ------------- |
| Jak 1 VAGWAD  |           ✔️  |           ✔️  |           ✔️  |           ✔️  |           ✔️  |
| Jak II VAGWAD  |           ❌  |           ❌  |           ❌  |           ❌  |           ❌  |
| Jak 3 VAGWAD  |           ❌  |           ❌  |           ❌  |           ❌  |           ❌  |
| Jak 1 SBK     |           ✔️  |           ❌  |           ❌  |           ❌  |           ❌  |
| Jak II SBK     |           ✔️  |           ✔️  |           ✔️  |           ❌  |           ❌  |
| Jak 3 SBK     |           ❌  |           ❌  |           ❌  |           ❌  |           ❌  |
| Jak 1 MUS     |           ✔️  |           ✔️  |           ✔️  |           ❌  |           ✔️  |
| Jak II MUS     |           ✔️  |           ✔️  |           ✔️  |           ❌  |           ✔️  |
| Jak X Anything |           ❌  |           ❌  |           ❌  |           ❌  |           ❌  |

## Tips:

All playback for input and output should have the following settings:
- *.wav format
- Monophonic (for now, Jak II may be different)
- Sample rate of 48khz

To inject VAGWAD, you'll need to convert a wav with the above settings into the adpcm headerless audio format. This can be accomplished by using 
the <a href="https://github.com/himham-jak/adpcm/">converter</a> from the PS2SDK. FFMPEG does not currently support the correct codec for this.

## Known Issues:
- Jak 1 SBK is not read perfectly. There should be only 2 types of grains, but there are 3. Also some sounds read as 80hr long.
- Jak 1 VAGWAD doesn't have a working stop button.
- Jak 1 COMMON.MUS fails to open.
- Jak 1 VAGWAD can only inject sounds smaller than the sound they're replacing.
