# Music Instrument Classification
In this project we use CNN based models to classify instruments using the Freesound audio data set. Our proposed architecture computes the Mel-spectrogram from the input audio
data and feeds it to a CNN based model. To add robustness to the model, we use a novel data augmentation technique based on the CutMix Algorithm. We optimise the architecture using Hyperparameter Tuning and Pruning, and analyse the model by generating the Class Activation Maps and by conducting an Ablation Study. For detailed information regarding this work, please read our detailed [report](https://github.com/siddharth16112004/Music_Instrument_Classification/blob/main/Music%20Instrument_Classification.pdf). 

We have taken an open source dataset called ‘Free Sound Audio tagging data’ for classification of musical instruments. The unfiltered version of the dataset had 9400 unique
audio samples stored in .wav format and there were 41 unique classes of instruments



<p>
<img src="images/MFCC.jpg" style="float: left; width: 40%; margin-right: 1%; margin-bottom: 0.5em;">
<img src="images/Pruning.png" style="float: left; width: 35%; margin-right: 1%; margin-bottom: 0.5em;">
<img src="images/cam1.png" style="float: left; width: 22%; margin-right: 1%; margin-bottom: 0.5em;">
(a) Schematic Representation of Preprocessing steps in computing the MFCC coefficients (b) Representation of Pruning (c) A sub matrix of the attention map across the DCT coefficients  
<p style="clear: both;">


This Music instrument classification models can be used in building Content Based Recommender Systems, in Genre Identification tasks and can be extended to provide solutions for
similar problems in other domains, for example in anomaly detection for mechanical systems.

## Key Contributions

1. We make use of CutMix Algorithm on the Mel Spectrograms to augment input data and add robustness to the model.
2. Hyper Parameter Tuning using keras tuner with Random search algorithm.
3. Model Pruning to obtain a lighter model with similar performance metrics as the original model(without pruning).
4. Class Activation Maps to identify neurons that play a significant role in identifying a class.
5. Ablation study to understand the importance of individual layer from the proposed model architecture. 
6. We have also done a thorough comparative analysis of our model with traditionally used instrument classification models.
