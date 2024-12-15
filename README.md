# Audio Anonymization Pipeline  

## Overview  
With the growing adoption of voice assistants like Moshi, ChatGPT, and Gemini 2.0, audio data has become a significant source of personal information. However, audio recordings often contain sensitive details such as names, addresses, and phone numbers, raising concerns about privacy and regulatory compliance.  

Audio anonymization has become an essential technique to protect individual privacy and comply with regulations like GDPR and HIPAA. This repository focuses on implementing a pipeline to anonymize audio by removing Personally Identifiable Information (PII) words.  

### What is Audio Anonymization?  
Audio anonymization can be categorized into two main approaches:  
1. **Anonymizing the speaker's identity**: This involves signal processing and voice morphing techniques to alter the speaker's voice.  
2. **Removing PII words**: This approach detects and removes sensitive information, such as names and locations, from audio recordings.  

In this repository, we focus on the second approach, providing a comprehensive end-to-end solution for identifying and anonymizing PII words in audio data.  

---

## Audio Anonymization Pipeline  
The pipeline consists of three main steps:  

1. **Audio Transcription**:  
   Convert audio recordings into text using a Speech-to-Text model. This implementation uses the OpenAI Whisper model for accurate transcription.  

2. **PII Detection**:  
   Detect PII words in the transcribed text using Named Entity Recognition (NER) techniques. This step identifies entities like names, addresses, and other sensitive details.  

3. **Audio Replacement**:  
   Replace the time ranges corresponding to detected PII words in the audio with a beep sound. Alternatively, you can replace the PII with a fake name, silence, or completely remove that portion of the audio.  

---

## Features  
- Accurate transcription using state-of-the-art Speech-to-Text models.  
- Robust PII detection using advanced NER techniques.  
- Flexible anonymization options: beep sound, fake names, silence, or removal.  

---

## Applications
- Ensuring privacy in customer support calls.
- Compliance with privacy regulations (GDPR, HIPAA, etc.).
- Safeguarding sensitive information in audio datasets for research or public use.

For the complete guide please visit the following article: https://medium.com/@manou.mohammedi/audio-anonymization-techniques-and-tools-for-privacy-protection-8cde87e1b90f
