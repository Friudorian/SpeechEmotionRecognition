# Speech Emotion Recognition

# English Abstract

The project had the purpose of searching for which audio features were most representative for an emotional interpretation. For this reason, a database widely used in literature was chosen: the Berlin Database for Emotional speech, containing sentences pronounced by actors and categorized in 7 emotions: joy, anger, disgust, fear, neutral, boredom, sadness. From these sentences, various features have been extracted, including MFCC, pitch, root-mean-square energy and these features have been evaluated using different classifiers, with the additional purpose of comparing performance with literature. In particular, were used: K-NN, KNN after PCA and SVM (linear and RBF kernels) which obtained interesting performances (measured by cross-validation) (72.3% accuracy of K-NN after PCA, 83, 5% SVM accuracy with linear kernel). In conclusion, a Perceptron Multi-Layer neural network was developed, which achieved a performance of 89.3% accuracy.

The project documentation is written in Italian.

# Abstract
Il progetto si presuppone lo scopo di ricercare quali feature audio siano piu rappresentative per un’interpretazione affettiva. Per questo e stato scelto un database molto usato in letteratura: il Berlin Database for Emotional speech, contenente frasi pronunciate da attori e
categorizzate in 7 emozioni: gioia, rabbia, disgusto, paura, neutro, noia, tristezza. Da tali frasi sono state estratte varie feature, tra cui MFCC, pitch, root-mean-square energy e queste feature sono state valutate mediante diversi classificatori, con l’ulteriore scopo di paragonare le performance con la letteratura. In particolare sono stati usati K-NN, KNN dopo PCA e SVM con (kernel lineare e rbf) i quali hanno ottenuto performance (misurate mediante cross-validaton) interessanti (72,3% di accuracy di K-NN dopo PCA, 83,5% di accuracy di SVM con kernel lineare). In conclusione e stata sviluppata una rete neurale Multi-Layer Perceptron che ha raggiunto la performance di 89,3% accuracy.

# Piccolissima guida alla repository

Progetto dei corsi di Interazione Naturale e Modelli di Computazione Affettiva A.A. 2017/18

La relazione è contenuta in SpeechEmotionRecognition.pdf.

Il sistema è composto da 3 notebook jupyter:
1) Estrazione Delle Feature.ipynb: In tale notebook si scorre l’intero dataset per estrarre le feature da ogni file.
2) Baseline: In tale notebook.ipynb si eseguono K-NN, KNN dopo PCA, SVM lineare e rbf sul dataset composto dalle feature estratte da ogni file.
3) Neural Network.ipynb: In tale notebook viene eseguita la rete neurale MLP sul dataset composto dalle feature estratte da ogni file.

Il migliore risultato ottenuto dalla rete è salvato nell'opportuno file Neural Network.html.

I file .p rappresentano i due dataset con migliori performance: Tutte_Features.p è composto da tutte le features estratte globalmente,
ed ha avuto le migliori performance nei baseline. NDA_NOPAD_MFCC&PitchOnly.p è composto da MFCC a 50 coefficienti e Pitch, globali,
ed ha ottenuto le migliori performance della rete neurale.
