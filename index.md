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
## Audio Samples (Short Phrases)

> ※ This section presents the results of **400 ms window realtime streaming simulation** decoding.

| No. | Phrase               | Original&nbsp;Audio | EEG-Imagined&nbsp;Audio |
|:--:|----------------------|--------------------|-----------------------|
| 1 | **go**                | <audio controls src="audio/tar_go.wav"></audio> | <audio controls src="audio/pred_go.wav"></audio> |
| 2 | **go to school**      | <audio controls src="audio/tar_gotoschool.wav"></audio> | <audio controls src="audio/pred_gotoschool.wav"></audio> |
| 3 | **home**              | <audio controls src="audio/tar_home.wav"></audio> | <audio controls src="audio/pred_home.wav"></audio> |
| 4 | **I am home**         | <audio controls src="audio/tar_iamhome.wav"></audio> | <audio controls src="audio/pred_iamhome.wav"></audio> |
| 5 | **time**              | <audio controls src="audio/tar_time.wav"></audio> | <audio controls src="audio/pred_time.wav"></audio> |
| 6 | **today**             | <audio controls src="audio/tar_today.wav"></audio> | <audio controls src="audio/pred_today.wav"></audio> |
| 7 | **today is sunday**   | <audio controls src="audio/tar_todayissunday.wav"></audio> | <audio controls src="audio/pred_todayissunday.wav"></audio> |
| 8 | **wait**              | <audio controls src="audio/tar_wait.wav"></audio> | <audio controls src="audio/pred_wait.wav"></audio> |
| 9 | **wait a second**     | <audio controls src="audio/tar_waitaseconds.wav"></audio> | <audio controls src="audio/pred_waitaseconds.wav"></audio> |
|10 | **what time is it**   | <audio controls src="audio/tar_whattimeisit.wav"></audio> | <audio controls src="audio/pred_whattimeisit.wav"></audio> |


## Audio Samples (Full Sentences)

> ※ This section presents the results after applying **LLM-based text correction** and **speaker-adapted TTS correction**.

| No. | Phrase | Original&nbsp;Audio | EEG-Imagined&nbsp;Audio |
|:--:|----------------------|--------------------|-----------------------|
| 1 | **I am a student at this school** | <audio controls src="audio/tar_iamastudentatthisschool.wav"></audio> | <audio controls src="audio/pred_iamastudentatthisschool.wav"></audio> | 
| 2 | **I lost my notebook yesterday** | <audio controls src="audio/tar_ilostmynotebookyesterday.wav"></audio> | <audio controls src="audio/pred_ilostmynotebookyesterday.wav"></audio> | 
| 3 | **please close the window before you go** | <audio controls src="audio/tar_pleaseclosethewindowbeforeyougo.wav"></audio> | <audio controls src="audio/pred_pleaseclosethewindowbeforeyougo.wav"></audio> | 
| 4 | **the library was very quiet** | <audio controls src="audio/tar_thelibrarywasveryquiet.wav"></audio> | <audio controls src="audio/pred_thelibrarywasveryquiet.wav"></audio> | 
| 5 | **we played baseball at the park** | <audio controls src="audio/tar_weplayedbaseballatthepark.wav"></audio> | <audio controls src="audio/pred_weplayedbaseballatthepark.wav"></audio> | 
| 6 | **he gave me information about the rule** | <audio controls src="audio/tar_hegavemeinformationabouttherule.wav"></audio> | <audio controls src="audio/pred_hegavemeinformationabouttherule.wav"></audio> | 
| 7 | **I saved document on the desktop** | <audio controls src="audio/tar_isaveddocumentonthedesktop.wav"></audio> | <audio controls src="audio/pred_isaveddocumentonthedesktop.wav"></audio> | 
| 8 | **I used a dictionary to find the word** | <audio controls src="audio/tar_iusedadictionarytofindtheword.wav"></audio> | <audio controls src="audio/pred_iusedadictionarytofindtheword.wav"></audio> | 
| 9 | **she waited for me near the airport** | <audio controls src="audio/tar_shewaitedformeneartheairport.wav"></audio> | <audio controls src="audio/pred_shewaitedformenear theairport.wav"></audio> |
|10 | **the classroom was empty when i arrived** | <audio controls src="audio/tar_theclassroomwasemptywheniarrived.wav"></audio> | <audio controls src="audio/pred_theclassroomwasemptywheniarrived.wav"></audio> |

---

## Paper & Code
> ※ It's not finished yet.
- **Paper PDF**: [link](#)
- **GitHub Repository**: [link](#)
---

_© 2025 BrainXAI Lab – Pukyong National University_
