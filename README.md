# Silly Beaver V0.4

The V0.3 microphone diagnostic left its getUserMedia audio stream running.
V0.4 automatically releases the microphone before starting browser SpeechRecognition.

## Test sequence
1. Tap Test microphone.
2. Speak for 4 seconds.
3. Wait for: "Microphone works and has been released."
4. Tap Test transcription.
5. Speak a full sentence immediately.

If microphone works but transcription still ends without a transcript, the likely issue is the browser/Android SpeechRecognition service rather than the physical microphone.
