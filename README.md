#speech-recognition

var speech = new Speech.SpeechToText(
'token': token;
);

speech.listen({
    onStart: function() {
        console.log('starting');
    },
    onResult: function(e) {
        console.log(e.text);
    },
    onError: function(e) {
        console.log('error', e);
    },
    onEnd: function(e) {
        console.log('end', e);
    }
});
```

## Install
Add this package to your project using the below command

```shell
npm install https://github.com/abhishekkshinde/stt.git 
```