# conllu-perceptron-tagger

A (very) simple perceptron tagger for CoNLL-U files, intended for use as a teaching
aid.

This is wholely based on the following code:

* https://explosion.ai/blog/part-of-speech-pos-tagger-in-python
* https://github.com/sloria/textblob-aptagger

I've basically taken the code and wrapped it for parsing CoNLL-U format files. 

### My additions to the tagger

I tryed to add some rules to the tagger and improve it's result for French language.
With start setting it gaves a result like this on the test data:

![Image of first try](https://raw.githubusercontent.com/kssamoylenko/conllu-perceptron-tagger/master/try1_estimation.png)

Then, with adding some rools it gets better like this:

![One rule added](https://raw.githubusercontent.com/kssamoylenko/conllu-perceptron-tagger/master/try2_estimation.png)
![Some more rules added](https://raw.githubusercontent.com/kssamoylenko/conllu-perceptron-tagger/master/try5_estimation.png)

The last one seemed like not bad. But when I tried the updated tagger on the test data, it turned into this:
![Final results](https://raw.githubusercontent.com/kssamoylenko/conllu-perceptron-tagger/master/final.png)

Not as great as I hoped, but anyway, it's better then it was at the beginnig, even just a little bit :)
