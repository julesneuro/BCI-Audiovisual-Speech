# BCI-Audiovisual-Speech
A collection of anonymised data and relevant code used for the implementation of Bayesian Casual Inference in my dissertation project.

In the project we implemented Bayesian Causal Inference to model multisensory integration with temporally asynchronous audiovisual speech.

The code is an adaptation of the model from Magnotti, Ma & Beauchamp (2013), and two of the computational strategies (model selection & probability matching) outlined in Wozny et al., (2010).


![SIM_DATA_PLOT](https://user-images.githubusercontent.com/74515191/118531394-b5727f80-b73d-11eb-9fca-e2a1b933f678.png)

Pictured above are the results of the data simulation across 15,000 trials. As you can see the probability matching strategy predicts substantially more 'lapses' in relatively straightforward stimulus conditions (i.e 0 or +400 async). You should be able to replicate this simulation using the CIMS-SIM.ipynb code & the SIM_DATA.xlsx file.

