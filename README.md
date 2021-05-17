# BCI-Audiovisual-Speech
A collection of anonymised data and relevant code used for the implementation of Bayesian Casual Inference in my dissertation project.

In the project we implemented Bayesian Causal Inference to model multisensory integration with temporally asynchronous audiovisual speech.

The code is an adaptation of the model from Magnotti, Ma & Beauchamp (2013), and two of the computational strategies (model selection & probability matching) outlined in Wozny et al., (2010).


![SIM_DATA_PLOT](https://user-images.githubusercontent.com/74515191/118531394-b5727f80-b73d-11eb-9fca-e2a1b933f678.png)

Pictured above are the results of the data simulation across 15,000 trials. As you can see the probability matching strategy predicts substantially more 'lapses' in relatively straightforward stimulus conditions (i.e 0 or +400 async). You should be able to replicate this simulation using the CIMS-SIM.ipynb code & the SIM_DATA.xlsx file.

After the model was fit (using the CIMS-FIT.ipynb file) we plotted the observed data, CIMS-MS and CIMS-PM model predictions vs the original Magnotti et al. (2013) dataset.!

[GROUP_PLOT_NF](https://user-images.githubusercontent.com/74515191/118531687-04201980-b73e-11eb-91d0-d8f1ad185000.png)

Unfortunately it appears that our dataset wasn't simulated to be similiar to human performance. This largely limited the models ability to fit any of the data, as it is based on the assumption that human performance in simultaneity judgement tasks follows a gaussian -- see Vroomen & Keetels (2010) _Attention, Perception & Psychophysics_.

To look a little closer at this we plotted all of the subjects performance and model predictions at an individual level.

![PARTICIPANT LEVEL PREDS](https://user-images.githubusercontent.com/74515191/118532038-6da02800-b73e-11eb-82d5-60e2206c7ba4.png)

As you can see, the model nearly always predicts an upwards peak in the middle of the stimulus conditions - and this accounts for our low average explained variance of each model CIMS-MS -- (R2 = 0.27), CIMS-PM -- (R2 = 0.31).


