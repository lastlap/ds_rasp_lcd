# ds_rasp_lcd
Text to Speech, Speech to Text and Integrated System for Raspberry pi

DeepSpeech scorer and tflite files can be taken from their official repo.
ed 
DeepSpeech is used to convert speech to text and display on connected lcd.

Pico2wave is used to convert text to speech and display on connected lcd.

System packages:
```
python==3.8
python3-pyaudio
libatlas-base
python3-smbus
pico2wave
```

Python Packages:
```
scipy
numpy
deepspeech==0.9.3
webrtcvad
halo
PyAudio
```

File Structure:

I2C_LCD_driver.py - Contains functions for connected LCD to run

rasp_lcd.py - Speech to Text Engine(S2T) using Deepspeech. Result is displayed on LCD.

tts.py - Text to Speech Engine(TTS) using pico2wave. Result displayed on LCD.

rasp_int.py - Integrated System of both TTS and S2T.
