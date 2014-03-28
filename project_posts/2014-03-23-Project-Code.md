The past several days we have played with different technologies and ways of doing speech recognition. These include 
* Google speech recognition API https://www.google.com/intl/en/chrome/demos/speech.html
* Nuance speech recognition http://dragonmobile.nuancemobiledeveloper.com/public/index.php?task=home
* Java Speech API - JSAPI1.0 implementation
The team also hacked a working prototype of speech recognition subsystem in Java Speech API.

## Example Code - 1 
NOTE: Sample Java snippet for speech recognition.
```
    RuleGrammar grammar = recognizer.loadJSGF(fileReader);
    grammar.setEnabled(true);
    // Add the listener to get results
    recognizer.addResultListener(new SpeechToTextConverter());
    // Commit the grammar
    recognizer.commitChanges();
    recognizer.waitEngineState(Recognizer.LISTENING);
    // Request focus and start listening
    recognizer.requestFocus();
    recognizer.resume();
    recognizer.waitEngineState(Recognizer.FOCUS_ON);
    recognizer.forceFinalize(true);
    recognizer.waitEngineState(Recognizer.DEALLOCATED);

```

## Example Code - 2 (Luke Kuza et. al.)
NOTE: Uses Google Speech API 
```
 public GoogleResponse getRecognizedDataForWave(File waveFile, int maxResults) throws IOException{
        FlacEncoder flacEncoder = new FlacEncoder();
        File flacFile = new File(waveFile + ".flac");
        flacEncoder.convertWaveToFlac(waveFile, flacFile);
        String response = rawRequest(flacFile, maxResults, 8000);//Transcodes to 8000 automatically
        //Delete converted FLAC data
        flacFile.delete();
        GoogleResponse googleResponse = new GoogleResponse();
        parseResponse(response, googleResponse);
        return googleResponse;
    }

```