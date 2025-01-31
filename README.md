*Virtual Jarvis - AI Voice Assistant*

Introduction:
Virtual Jarvis is a Python-based voice assistant that responds to voice commands and executes various tasks such as opening websites, playing YouTube videos, and searching the web. It uses speech recognition, text-to-speech conversion, and web automation to provide a hands-free experience.

Features
1. Voice Recognition: Listens and processes voice commands using Google's Speech Recognition API.
2. Text-to-Speech (TTS): Converts text responses into speech using the pyttsx3 library.
3. Web Automation:
     -Opens Google, YouTube, Facebook, and LinkedIn.
     -Searches the web using pywhatkit.
     -Plays YouTube videos by voice command.
4. Continuous Listening Mode: Keeps listening for the wake word "Jarvis" to activate.
5. Exit Command: Say "stop" to exit the program.

Requirements:
-Ensure you have the following Python libraries installed:
  pip install speechrecognition pyttsx3 pywhatkit pyaudio
-If pyaudio fails to install, try:
  pip install pipwin
  pipwin install pyaudio

How It Works:
1. Initialize the Engine: pyttsx3 initializes text-to-speech conversion.
2. Wake Word Activation: The assistant waits for the keyword "Jarvis".
3. Command Recognition: After activation, it listens for a command and executes an appropriate function.

Response Execution:
- If the command contains "open google", it opens Google.
- If the command contains "play", it plays a YouTube video.
- If the command contains "search", it searches the web.
- If the command is "stop", the assistant stops running.

Usage:
1. Run the script: python jarvis.py
2. Speak "Jarvis" to activate, then issue commands such as:
3. "Open Google"
4. "Play [song name]"
5. "Search Python programming"
6. "Stop" (to exit)

Error Handling:
1. Timeout: If no speech is detected within 2 seconds, it times out.
2. Unrecognized Speech: If the assistant cannot understand the input, it will prompt you to try again.
3. Internet Connection Issues: If the API request fails, an error message is displayed.
