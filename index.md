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

> ※ This section presents the results of **400 ms window realtime streaming simulation** decoding.

| No. | Phrase               | Original&nbsp;Audio | EEG-Imagined&nbsp;Audio |
|:--:|----------------------|--------------------|-----------------------|
| 1 | **go**                | <audio controls src="audio/01/tar_go.wav"/> | <audio controls src="audio/01/pred_go.wav"/> |
| 2 | **go to school**      | <audio controls src="audio/01/tar_gotoschool.wav"/> | <audio controls src="audio/01/pred_gotoschool.wav"/> |
| 3 | **home**              | <audio controls src="audio/01/tar_home.wav"/> | <audio controls src="audio/01/pred_home.wav"/> |
| 4 | **I am home**         | <audio controls src="audio/01/tar_iamhome.wav"/> | <audio controls src="audio/01/pred_iamhome.wav"/> |
| 5 | **time**              | <audio controls src="audio/01/tar_time.wav"/> | <audio controls src="audio/01/pred_time.wav"/> |
| 6 | **what time is it**   | <audio controls src="audio/01/tar_whattimeisit.wav"/> | <audio controls src="audio/01/pred_whattimeisit.wav"/> |
| 7 | **today**             | <audio controls src="audio/01/tar_today.wav"/> | <audio controls src="audio/01/pred_today.wav"/> |
| 8 | **today is sunday**   | <audio controls src="audio/01/tar_todayissunday.wav"/> | <audio controls src="audio/01/pred_todayissunday.wav"/> |
| 9 | **wait**              | <audio controls src="audio/01/tar_wait.wav"/> | <audio controls src="audio/01/pred_wait.wav"/> |
|10 | **wait a second**     | <audio controls src="audio/01/tar_waitaseconds.wav"/> | <audio controls src="audio/01/pred_waitaseconds.wav"/> |


## 2. Audio Samples (Full Sentences)

> ※ This section presents the results after applying **LLM-based text correction** and **speaker-adapted TTS correction**.

| No. | Phrase | Original&nbsp;Audio | EEG-Imagined&nbsp;Audio |
|:--:|----------------------|--------------------|-----------------------|
| 1 | **I am a student at this school** | <audio controls src="audio/02/tar_iamastudentatthisschool.wav"/> | <audio controls src="audio/02/pred_iamastudentatthisschool.wav"/> | 
| 2 | **I lost my notebook yesterday** | <audio controls src="audio/02/tar_ilostmynotebookyesterday.wav"/> | <audio controls src="audio/02/pred_ilostmynotebookyesterday.wav"/> | 
| 3 | **please close the window before you go** | <audio controls src="audio/02/tar_pleaseclosethewindowbeforeyougo.wav"/> | <audio controls src="audio/02/pred_pleaseclosethewindowbeforeyougo.wav"/> | 
| 4 | **the library was very quiet** | <audio controls src="audio/02/tar_thelibrarywasveryquiet.wav"/> | <audio controls src="audio/02/pred_thelibrarywasveryquiet.wav"/> | 
| 5 | **we played baseball at the park** | <audio controls src="audio/02/tar_weplayedbaseballatthepark.wav"/> | <audio controls src="audio/02/pred_weplayedbaseballatthepark.wav"/> | 
| 6 | **he gave me information about the rule** | <audio controls src="audio/02/tar_hegavemeinformationabouttherule.wav"/> | <audio controls src="audio/02/pred_hegavemeinformationabouttherule.wav"/> | 
| 7 | **I saved document on the desktop** | <audio controls src="audio/02/tar_isaveddocumentonthedesktop.wav"/> | <audio controls src="audio/02/pred_isaveddocumentonthedesktop.wav"/> | 
| 8 | **I used a dictionary to find the word** | <audio controls src="audio/02/tar_iusedadictionarytofindtheword.wav"/> | <audio controls src="audio/02/pred_iusedadictionarytofindtheword.wav"/> | 
| 9 | **she waited for me near the airport** | <audio controls src="audio/02/tar_shewaitedformeneartheairport.wav"/> | <audio controls src="audio/02/pred_shewaitedformenear theairport.wav"/> |
|10 | **the classroom was empty when i arrived** | <audio controls src="audio/02/tar_theclassroomwasemptywheniarrived.wav"/> | <audio controls src="audio/02/pred_theclassroomwasemptywheniarrived.wav"/> |


## 3. Audio Samples (Short Phrases)

> ※ This section presents **offline EEG-decoded audio reconstructed directly** from neural features.

| No. | Phrase               | Original&nbsp;Audio | EEG-Imagined&nbsp;Audio |
|:--:|----------------------|--------------------|-----------------------|
| 1 | **go**                | <audio controls src="audio/03/tar_go.wav"></audio> | <audio controls src="audio/03/pred_go.wav"></audio> |
| 2 | **go to school**      | <audio controls src="audio/03/tar_gotoschool.wav"></audio> | <audio controls src="audio/03/pred_gotoschool.wav"></audio> |
| 3 | **home**              | <audio controls src="audio/03/tar_home.wav"></audio> | <audio controls src="audio/03/pred_home.wav"></audio> |
| 4 | **I am home**         | <audio controls src="audio/03/tar_iamhome.wav"></audio> | <audio controls src="audio/03/pred_iamhome.wav"></audio> |
| 5 | **time**              | <audio controls src="audio/03/tar_time.wav"></audio> | <audio controls src="audio/03/pred_time.wav"></audio> |
| 6 | **what time is it**   | <audio controls src="audio/03/tar_whattimeisit.wav"></audio> | <audio controls src="audio/03/pred_whattimeisit.wav"></audio> |
| 7 | **today**             | <audio controls src="audio/03/tar_today.wav"></audio> | <audio controls src="audio/03/pred_today.wav"></audio> |
| 8 | **today is sunday**   | <audio controls src="audio/03/tar_todayissunday.wav"></audio> | <audio controls src="audio/03/pred_todayissunday.wav"></audio> |
| 9 | **wait**              | <audio controls src="audio/03/tar_wait.wav"></audio> | <audio controls src="audio/03/pred_wait.wav"></audio> |
|10 | **wait a second**     | <audio controls src="audio/03/tar_waitasecond.wav"></audio> | <audio controls src="audio/03/pred_waitasecond.wav"></audio> |


## 4. Audio Samples (Short Prases & Full Sentences)

> ※ This section presents the results after **speaker-adapted TTS correction**.

| No. | Phrase | Original&nbsp;Audio | EEG-Imagined&nbsp;Audio |
|:--:|----------------------|--------------------|-----------------------|
| 1 | **student** | <audio controls src="audio/04/tar_student.wav"></audio> | <audio controls src="audio/04/pred_student.wav"></audio> |
| 2 | **I am a student at this school** | <audio controls src="audio/04/tar_i_am_a_student_at_this_school.wav"></audio> | <audio controls src="audio/04/pred_i_am_a_student_at_this_school.wav"></audio> |
| 3 | **notebook** | <audio controls src="audio/04/tar_notebook.wav"></audio> | <audio controls src="audio/04/pred_notebook.wav"></audio> |
| 4 | **I lost my notebook yesterday** | <audio controls src="audio/04/tar_i_lost_my_notebook_yesterday.wav"></audio> | <audio controls src="audio/04/pred_i_lost_my_notebook_yesterday.wav"></audio> |
| 5 | **window** | <audio controls src="audio/04/tar_window.wav"></audio> | <audio controls src="audio/04/pred_window.wav"></audio> |
| 6 | **please close the window before you go** | <audio controls src="audio/04/tar_please_close_the_window_before_you_go.wav"></audio> | <audio controls src="audio/04/pred_please_close_the_window_before_you_go.wav"></audio> |
| 7 | **library** | <audio controls src="audio/04/tar_library.wav"></audio> | <audio controls src="audio/04/pred_library.wav"></audio> |
| 8 | **the library was very quiet** | <audio controls src="audio/04/tar_the_library_was_very_quiet.wav"></audio> | <audio controls src="audio/04/pred_the_library_was_very_quiet.wav"></audio> |
| 9 | **baseball** | <audio controls src="audio/04/tar_baseball.wav"></audio> | <audio controls src="audio/04/pred_baseball.wav"></audio> |
|10 | **we played baseball at the park** | <audio controls src="audio/04/tar_we_played_baseball_at_the_park.wav"></audio> | <audio controls src="audio/04/pred_we_played_baseball_at_the_park.wav"></audio> |
|11 | **information** | <audio controls src="audio/04/tar_information.wav"></audio> | <audio controls src="audio/04/pred_information.wav"></audio> |
|12 | **he gave me information about the rule** | <audio controls src="audio/04/tar_he_gave_me_information_about_the_rule.wav"></audio> | <audio controls src="audio/04/pred_he_gave_me_information_about_the_rule.wav"></audio> |
|13 | **document** | <audio controls src="audio/04/tar_document.wav"></audio> | <audio controls src="audio/04/pred_document.wav"></audio> |
|14 | **I saved document on the desktop** | <audio controls src="audio/04/tar_i_saved_document_on_the_desktop.wav"></audio> | <audio controls src="audio/04/pred_i_saved_document_on_the_desktop.wav"></audio> |
|15 | **dictionary** | <audio controls src="audio/04/tar_dictionary.wav"></audio> | <audio controls src="audio/04/pred_dictionary.wav"></audio> |
|16 | **I used a dictionary to find the word** | <audio controls src="audio/04/tar_i_used_a_dictionary_to_find_the_word.wav"></audio> | <audio controls src="audio/04/pred_i_used_a_dictionary_to_find_the_word.wav"></audio> |
|17 | **airport** | <audio controls src="audio/04/tar_airport.wav"></audio> | <audio controls src="audio/04/pred_airport.wav"></audio> |
|18 | **she waited for me near the airport** | <audio controls src="audio/04/tar_she_waited_for_me_near_the_airport.wav"></audio> | <audio controls src="audio/04/pred_she_waited_for_me_near_the_airport.wav"></audio> |
|19 | **classroom** | <audio controls src="audio/04/tar_classroom.wav"></audio> | <audio controls src="audio/04/pred_classroom.wav"></audio> |
|20 | **the classroom was empty when i arrived** | <audio controls src="audio/04/tar_the_classroom_was_empty_when_i_arrived.wav"></audio> | <audio controls src="audio/04/pred_the_classroom_was_empty_when_i_arrived.wav"></audio> |




---

## Paper & Code
> ※ It's not finished yet.
- **Paper PDF**: [link](#)
- **GitHub Repository**: [link](#)
---

_© 2025 BrainXAI Lab – Pukyong National University_
