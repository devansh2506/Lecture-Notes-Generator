# Lecture Notes Generator
Lecture Notes Generator is a Colab-based project that automates the process of converting educational video lectures into clean, structured, and study-ready notes. It extracts audio from a video, transcribes the speech using OpenAI's Whisper model, and then generates high-quality, formatted notes using Google's Gemini API.

## Architecture

Audio Extraction: The system takes a lecture video as input and extracts its audio using the moviepy library.

Speech Transcription:The extracted audio is transcribed into text using OpenAI’s Whisper model (base version), which converts spoken content into written form.

Text Cleaning and Note Generation:

The raw transcription is sent to Google's Gemini API along with a prompt that instructs the model to:

1)Remove introductions, conclusions, and irrelevant commentary.

2)Retain only lecture-relevant content.

3)Format the notes clearly using numbered points.

4)Write any mathematical content in proper symbolic form.

## Lecture Source

Video Title: Regularization Part 1: Ridge (L2) Regression

YouTube Search Link:

https://www.youtube.com/results?search_query=Regularization+Part+1_+Ridge+(L2)+Regression.mp4

Sample Download:
You can download the video used in this model as a sample file: Sample Video.mp4.zip

## Output

The final output is a clean, structured list of study notes formatted using numbered points. Mathematical formulas are preserved in symbolic form, making it easy for students to revise complex topics.

## Acknowledgements

OpenAI Whisper: For accurate audio transcription.

Google Gemini API: For generating structured and intelligent notes from raw transcripts.

MoviePy: For video/audio processing.

Colab: For providing a simple and free cloud environment for development.
