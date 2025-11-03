---
title: EEG Decoding During Inner Speech Using a Brain-Machine Interface
---

# EEG Decoding During Inner Speech Using a Brain-Machine Interface
> Quick demo showcasing how our model decodes inner (imagined) speech from EEG signals and synthesises audible speech in offline.
- This version was precisely timed segment.

---

## Protocol Video
<iframe width="720" height="405" src="https://www.youtube.com/embed/Hh71r9p2UAg"
        title="Protocol video" frameborder="0" allowfullscreen></iframe>

---
## 1. Audio Samples (Short Phrases)

> - Original (recorded speech)
> - EEG-Imagined (offline reconstruction directly from EEG-derived neural features)
> - Streaming (real-time simulation with 400 ms window)
> - TTS (LLM-based text correction and speaker-adapted TTS)

| No. | Phrase | Original&nbsp;Audio | EEG-Imagined&nbsp;Audio | Streaming&nbsp;Audio | TTS&nbsp;Audio | 
|:--:|----------------------|--------------------|-----------------------|-----------------------|-----------------------|
| 1 | **go** | <audio controls src="audio/ver3/sub003/target/0.wav"/> | <audio controls src="audio/ver3/sub003/pred/generator/0.wav"/> | <audio controls src="audio/ver3/sub003/pred/streaming/0.wav"/> | <audio controls src="audio/ver3/sub003/pred/tts/0.wav"/> | 
| 2 | **home** | <audio controls src="audio/ver3/sub003/target/1.wav"/> | <audio controls src="audio/ver3/sub003/pred/generator/1.wav"/> | <audio controls src="audio/ver3/sub003/pred/streaming/1.wav"/> | <audio controls src="audio/ver3/sub003/pred/tts/1.wav"/> | 
| 3 | **time** | <audio controls src="audio/ver3/sub003/target/2.wav"/> | <audio controls src="audio/ver3/sub003/pred/generator/2.wav"/> | <audio controls src="audio/ver3/sub003/pred/streaming/2.wav"/> | <audio controls src="audio/ver3/sub003/pred/tts/2.wav"/> | 
| 4 | **today** | <audio controls src="audio/ver3/sub003/target/3.wav"/> | <audio controls src="audio/ver3/sub003/pred/generator/3.wav"/> | <audio controls src="audio/ver3/sub003/pred/streaming/3.wav"/> | <audio controls src="audio/ver3/sub003/pred/tts/3.wav"/> | 
| 5 | **wait** | <audio controls src="audio/ver3/sub003/target/4.wav"/> | <audio controls src="audio/ver3/sub003/pred/generator/4.wav"/> | <audio controls src="audio/ver3/sub003/pred/streaming/4.wav"/> | <audio controls src="audio/ver3/sub003/pred/tts/4.wav"/> | 
| 6 | **go to school** | <audio controls src="audio/ver3/sub003/target/5.wav"/> | <audio controls src="audio/ver3/sub003/pred/generator/5.wav"/> | <audio controls src="audio/ver3/sub003/pred/streaming/5.wav"/> | <audio controls src="audio/ver3/sub003/pred/tts/5.wav"/> | 
| 7 | **i am home** | <audio controls src="audio/ver3/sub003/target/6.wav"/> | <audio controls src="audio/ver3/sub003/pred/generator/6.wav"/> | <audio controls src="audio/ver3/sub003/pred/streaming/6.wav"/> | <audio controls src="audio/ver3/sub003/pred/tts/6.wav"/> | 
| 8 | **today is sunday** | <audio controls src="audio/ver3/sub003/target/7.wav"/> | <audio controls src="audio/ver3/sub003/pred/generator/7.wav"/> | <audio controls src="audio/ver3/sub003/pred/streaming/7.wav"/> | <audio controls src="audio/ver3/sub003/pred/tts/7.wav"/> | 
| 9 | **wait a second** | <audio controls src="audio/ver3/sub003/target/8.wav"/> | <audio controls src="audio/ver3/sub003/pred/generator/8.wav"/> | <audio controls src="audio/ver3/sub003/pred/streaming/8.wav"/> | <audio controls src="audio/ver3/sub003/pred/tts/8.wav"/> | 
| 10 | **what time is it** | <audio controls src="audio/ver3/sub003/target/9.wav"/> | <audio controls src="audio/ver3/sub003/pred/generator/9.wav"/> | <audio controls src="audio/ver3/sub003/pred/streaming/9.wav"/> | <audio controls src="audio/ver3/sub003/pred/tts/9.wav"/> | 


## 2. Audio Samples (Full Sentences)

> - Original (recorded speech)
> - TTS (LLM-based text correction and speaker-adapted TTS)

| No. | Phrase | Original&nbsp;Audio(sub6) | TTS&nbsp;Audio | Original&nbsp;Audio(sub12) | TTS&nbsp;Audio | 
|:--:|----------------------|--------------------|-----------------------|-----------------------|-----------------------|
| 1 | **airport** | <audio controls src="audio/ver4/sub006/target/10.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/10.wav"/> |  <audio controls src="audio/ver4/sub012/target/10.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/10.wav"/> | 
| 2 | **baseball** | <audio controls src="audio/ver4/sub006/target/11.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/11.wav"/> |  <audio controls src="audio/ver4/sub012/target/11.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/11.wav"/> | 
| 3 | **classroom** | <audio controls src="audio/ver4/sub006/target/12.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/12.wav"/> |  <audio controls src="audio/ver4/sub012/target/12.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/12.wav"/> | 
| 4 | **dictionary** | <audio controls src="audio/ver4/sub006/target/13.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/13.wav"/> |  <audio controls src="audio/ver4/sub012/target/13.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/13.wav"/> | 
| 5 | **document** | <audio controls src="audio/ver4/sub006/target/14.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/14.wav"/> |  <audio controls src="audio/ver4/sub012/target/14.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/14.wav"/> | 
| 6 | **information** | <audio controls src="audio/ver4/sub006/target/15.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/15.wav"/> |  <audio controls src="audio/ver4/sub012/target/15.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/15.wav"/> | 
| 7 | **library** | <audio controls src="audio/ver4/sub006/target/16.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/16.wav"/> |  <audio controls src="audio/ver4/sub012/target/16.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/16.wav"/> | 
| 8 | **notebook** | <audio controls src="audio/ver4/sub006/target/17.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/17.wav"/> |  <audio controls src="audio/ver4/sub012/target/17.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/17.wav"/> | 
| 9 | **student** | <audio controls src="audio/ver4/sub006/target/18.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/18.wav"/> |  <audio controls src="audio/ver4/sub012/target/18.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/18.wav"/> | 
| 10 | **window** | <audio controls src="audio/ver4/sub006/target/19.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/19.wav"/> |  <audio controls src="audio/ver4/sub012/target/19.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/19.wav"/> | 
| 11 | **she waited for me near the airport** | <audio controls src="audio/ver4/sub006/target/20.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/20.wav"/> |  <audio controls src="audio/ver4/sub012/target/20.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/20.wav"/> | 
| 12 | **we played baseball at the park** | <audio controls src="audio/ver4/sub006/target/21.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/21.wav"/> |  <audio controls src="audio/ver4/sub012/target/21.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/21.wav"/> | 
| 13 | **the classroom was empty when i arrived** | <audio controls src="audio/ver4/sub006/target/22.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/22.wav"/> |  <audio controls src="audio/ver4/sub012/target/22.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/22.wav"/> | 
| 14 | **i used a dictionary to find the word** | <audio controls src="audio/ver4/sub006/target/23.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/23.wav"/> |  <audio controls src="audio/ver4/sub012/target/23.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/23.wav"/> | 
| 15 | **i saved document on the desktop** | <audio controls src="audio/ver4/sub006/target/24.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/24.wav"/> |  <audio controls src="audio/ver4/sub012/target/24.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/24.wav"/> | 
| 16 | **he gave me information about the rule** | <audio controls src="audio/ver4/sub006/target/25.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/25.wav"/> |  <audio controls src="audio/ver4/sub012/target/25.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/25.wav"/> | 
| 17 | **the library was very quiet** | <audio controls src="audio/ver4/sub006/target/26.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/26.wav"/> |  <audio controls src="audio/ver4/sub012/target/26.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/26.wav"/> | 
| 18 | **i lost my notebook yesterday** | <audio controls src="audio/ver4/sub006/target/27.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/27.wav"/> |  <audio controls src="audio/ver4/sub012/target/27.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/27.wav"/> | 
| 19 | **i am a student at this school** | <audio controls src="audio/ver4/sub006/target/28.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/28.wav"/> |  <audio controls src="audio/ver4/sub012/target/28.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/28.wav"/> | 
| 20 | **please close the window before you go** | <audio controls src="audio/ver4/sub006/target/29.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/29.wav"/> |  <audio controls src="audio/ver4/sub012/target/29.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/29.wav"/> | 



---

## Paper & Code
> ※ It's not finished yet.
- **Paper PDF**: [link](#)
- **GitHub Repository**: [link](#)
---

_© 2025 BrainXAI Lab – Pukyong National University_
