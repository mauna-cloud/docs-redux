# Speech Services

## Convert voice input to text for backend processing

_Given_ I have a valid token for mauna services

_When_ I call the  tts.mauna.cloud with the token using the graphql query

_And_ Pass the audio in base64 string

_Then_ The STT service should return text corresponding to the audio.

## Convert Text output to speech audio

_Given_ I have a valid token for mauna services

_When_ I call the stt.mauna.cloud with the token using the graphql query

_And_ Pass the text using SSML tags for speech generation

_Then_ The TTS service should return the audio in base64 string which can be played using any audio player.
