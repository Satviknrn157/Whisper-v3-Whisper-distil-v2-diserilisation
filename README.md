## Whisper-V3 VS whisper-distil-v2

### Objective:
   To evaluate the performance of OpenAI's Whisper models for speaker diarization across audio files of varying lengths and to determine the feasibility of the task.

### Observation :
● The evaluation involved transcription tests on audio files categorized by duration: short (4 minutes), medium (7 minutes), and large (17 minutes).   
● The distil-whisper model consistently outperformed the whisper-v3 model in terms of speed, with greater efficiency observed as the audio file size increased.    
Specifically, the distil-whisper model was approximately 30%, 45%, and 55% faster than the whisper-v3 model for short, medium, and large files, respectively.   
● Both models demonstrated the capability to accurately identify and count the number of speakers present in the audio files.   
● Timestamp accuracy was consistent between the two models, with both providing reliable timestamps that corresponded well with one another.    
● The models were competent in aggregating and concatenating transcriptions coherently until a new speaker was detected.   
● output illustrated that both models produced few word errors, indicating high transcription accuracy.   
● Distil-whisper exhibited more grammatical errors compared to whisper-v3, suggesting that the latter offers superior linguistic precision.   
● In terms of resource utilization, distil-whisper was noted to be lighter and faster, while maintaining a high degree of accuracy.   
Incorporating Flash-Attention 2 yielded a speed boost in model performance, enhancing the efficiency of the transcription process.    
● The use of generate_kwargs={"language": "english"}   
● generate_kwargs={"language": "english"}        
○ proved beneficial for the whisper-v3 model in focusing on English language transcriptions. This feature was not applicable to the distil-whisper model        
Code block for whisper-distil and whisper-v3 is attached in the files    