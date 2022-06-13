# Speech to Text, followed by translation


This simple project includes two components. First, **speech-to-text** using a pre-recorded wav file (other formats are compatible too) or with audio detected on microphone. Second components is **translation** of the microphone text to multiple user chosen languages.

## Speech-to-Text

For this part, I am using speech_recognition library. It supports multiple APIs including Google Cloud Speech API, Microsoft Bing Voice Recognition, IBM Speech to Text and a few more. For the purpose of this simple tool, we would be using Google Cloud Speech API.

We use Recognizer() class of this library to listen to audios (either recorded or via microphone), pass it Google API, and we have our audio converted to speech, which can now be printed.

## Translation

deep_translator library in python is free to use, supports multiple translators and includes multiple languages. We can check the languages supported by any translator using get_supported_languages() on its object. Some of the translators it integrates include Google (used here), Mymemory, DeepL, PONS, Yandex, etc.

It truly makes translating between languages very easy.

Herein, I am using a while loop, so that user can translate in multiple languages of his/her choice.

Please refer the code file for more details and actual outputs.
