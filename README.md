# Spanish Kaldi Profile

A [Rhasspy](https://github.com/rhasspy/rhasspy) profile for Spanish (`es`).

Includes:

* A [Kaldi nnet3](https://kaldi-asr.org/doc/dnn3.html) speech to text model
    * See files in `acoustic_model/`
    * Recipe created with [ipa2kaldi](https://github.com/rhasspy/ipa2kaldi)
    * Word error rate: 2.03%
    * Trained on:
        * [Common Voice](https://commonvoice.mozilla.org) (295 hours)
        * [M-AILabs](https://www.caito.de/2019/01/the-m-ailabs-speech-dataset/) (108 hours)
        * [Carlos Fonseca](https://github.com/carlfm01/my-speech-datasets) (53 hours)
        * [Voxforge](http://voxforge.org/es) (52 hours)
* An [IPA](https://en.wikipedia.org/wiki/International_Phonetic_Alphabet) pronunciation lexicon based on [open-dict-data](https://github.com/open-dict-data/ipa-dict)
    * See `base_dictionary.txt.gz`
* A [phonetisaurus](https://github.com/AdolfVonKleist/Phonetisaurus) grapheme to phoneme model for predicting word pronunciations
    * See `g2p.fst.gz`
    * Trained on `base_dictionary.txt.gz`
* A tri-gram [ARPA language model](https://cmusphinx.github.io/wiki/arpaformat/)
    * See `base_language_model.txt.gz`
    * Text from audio transcriptions, [Common Voice](https://github.com/mozilla/common-voice/tree/master/server/data/es), and [Universal Dependencies](https://universaldependencies.org/)
