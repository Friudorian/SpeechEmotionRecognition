# INMCA_Faleri
La relazione è contenuta in SpeechEmotionRecognition.pdf.

Il sistema è composto da 3 notebook jupyter:
1) Estrazione Delle Feature.ipynb: In tale notebook si scorre l’intero dataset per estrarre le feature da ogni file.
2) Baseline: In tale notebook.ipynb si eseguono K-NN, KNN dopo PCA, SVM lineare e rbf sul dataset composto dalle feature estratte da ogni file.
3) Neural Network.ipynb: In tale notebook viene eseguita la rete neurale MLP sul dataset composto dalle feature estratte da ogni file.

Il migliore risultato ottenuto dalla rete è salvato nell'opportuno file Neural Network.html.

I file .p rappresentano i due dataset con migliori performance: Tutte_Features.p è composto da tutte le features estratte globalmente,
ed ha avuto le migliori performance nei baseline. NDA_NOPAD_MFCC&PitchOnly.p è composto da MFCC a 50 coefficienti e Pitch, globali,
ed ha ottenuto le migliori performance della rete neurale.
