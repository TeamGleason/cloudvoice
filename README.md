# cloudvoice
CloudVoice is a Text To Speech (TTS) provider for Microsoft Windows that implements the SAPI-5 speech interface and forwards TTS commands to cloud providers

To implement a SAPI 5 TTS engine, see [this sample from the Windows SDK](https://github.com/pauldotknopf/WindowsSDK7-Samples/blob/3f2438b15c59fdc104c13e2cf6cf46c1b16cf281/winui/speech/engines/samplettsengine/samplettsengine/ttsengobj.cpp#L373).

The idea is to:

 * Bridge SAPI-5 into cloud TTS engine(s)
 * Fall back to a local SAPI provider if there is an error calling the cloud TTS engine
