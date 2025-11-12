<style>
table {
  table-layout: fixed;
  width: 100%;
}
th, td {
  word-wrap: break-word;
  white-space: normal;
}
audio {
  width: 160px;
  max-width: 100%;
}
table th:first-child,
table td:first-child {
  width: 48px;
  max-width: 60px;
  white-space: nowrap;
  text-align: center;
}
.video-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 24px;
  width: 100%;
  margin-top: 16px;
}
.video-card {
  display: flex;
  flex-direction: column;
  gap: 12px;
}
.video-card p {
  margin: 0;
  font-weight: 600;
}
.video-wrapper {
  position: relative;
  width: 100%;
  padding-top: 56.25%;
  border-radius: 12px;
  overflow: hidden;
  background: #000;
}
.video-wrapper iframe {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  border: 0;
}
@media (max-width: 900px) {
  audio { width: 120px; }
  .video-grid {
    gap: 16px;
    grid-template-columns: 1fr;
  }
}
</style>

# EEG Decoding During Inner Speech Using a Brain-Machine Interface
> Quick demo showcasing how our model decodes inner (imagined) speech from EEG signals and synthesises audible speech in offline.
- This version was precisely timed segment.

---

## Protocol Video

<div class="video-grid">
  <div class="video-card">
    <p>Demo</p>
    <div class="video-wrapper">
      <iframe src="https://youtu.be/oYGz_XE0T4c"
              title="Protocol video" allowfullscreen></iframe>
    </div>
  </div>
  <div class="video-card">
    <p>Protocol</p>
    <div class="video-wrapper">
      <iframe src="https://youtu.be/XE1uSoxDvAQ"
              title="Protocol video" allowfullscreen /></iframe>
    </div>
  </div>
</div>

---
## 1. Audio Samples (Short Phrases)

> - Original (recorded speech)
> - EEG-Imagined (offline reconstruction directly from EEG-derived neural features)
> - Streaming (real-time simulation with 400 ms window)
> - TTS (LLM-based text correction and speaker-adapted TTS)

| No. | Phrase | Original(sub3) | EEG-Imagined | Streaming | TTS | 
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

| No. | Phrase | Original(sub6) | TTS | Original(sub12) | TTS | 
|:--:|----------------------|--------------------|-----------------------|-----------------------|-----------------------|
| 1 | **she waited for me near the airport** | <audio controls src="audio/ver4/sub006/target/20.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/20.wav"/> |  <audio controls src="audio/ver4/sub012/target/20.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/20.wav"/> | 
| 2 | **we played baseball at the park** | <audio controls src="audio/ver4/sub006/target/21.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/21.wav"/> |  <audio controls src="audio/ver4/sub012/target/21.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/21.wav"/> | 
| 3 | **the classroom was empty when i arrived** | <audio controls src="audio/ver4/sub006/target/22.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/22.wav"/> |  <audio controls src="audio/ver4/sub012/target/22.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/22.wav"/> | 
| 4 | **i used a dictionary to find the word** | <audio controls src="audio/ver4/sub006/target/23.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/23.wav"/> |  <audio controls src="audio/ver4/sub012/target/23.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/23.wav"/> | 
| 5 | **i saved document on the desktop** | <audio controls src="audio/ver4/sub006/target/24.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/24.wav"/> |  <audio controls src="audio/ver4/sub012/target/24.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/24.wav"/> | 
| 6 | **he gave me information about the rule** | <audio controls src="audio/ver4/sub006/target/25.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/25.wav"/> |  <audio controls src="audio/ver4/sub012/target/25.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/25.wav"/> | 
| 7 | **the library was very quiet** | <audio controls src="audio/ver4/sub006/target/26.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/26.wav"/> |  <audio controls src="audio/ver4/sub012/target/26.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/26.wav"/> | 
| 8 | **i lost my notebook yesterday** | <audio controls src="audio/ver4/sub006/target/27.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/27.wav"/> |  <audio controls src="audio/ver4/sub012/target/27.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/27.wav"/> | 
| 9 | **i am a student at this school** | <audio controls src="audio/ver4/sub006/target/28.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/28.wav"/> |  <audio controls src="audio/ver4/sub012/target/28.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/28.wav"/> | 
| 10 | **please close the window before you go** | <audio controls src="audio/ver4/sub006/target/29.wav"/> | <audio controls src="audio/ver4/sub006/pred/tts/29.wav"/> |  <audio controls src="audio/ver4/sub012/target/29.wav"/> | <audio controls src="audio/ver4/sub012/pred/tts/29.wav"/> | 



---

## Paper & Code
> ※ It's not finished yet.
- **Paper PDF**: [link](#)
- **GitHub Repository**: [link](#)
---

_© 2025 BrainXAI Lab – Pukyong National University_
