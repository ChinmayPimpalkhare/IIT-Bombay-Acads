This assignment was done by members of the group Audio_Linguists, the members being
1. Vikhyat Agrawal     (200260058) 
2. Saksham Katiyar     (20D100022) 
3. Chinmay Pimpalkhare (200100115) 
4. Ankur Verma         (20D070014) 

Some comments about Q2B
We have submitted the file for Q2A which was run for 30 epochs and the required test WER obtained. For Q2B, we did not train the Q2A 
model again for 30 epochs as we concluded that pretraining was not happening during the inheritance phase due to a change in the 
architecture. The file for Q2B hence contains the fully trained (30 epoch) PowerConv model. 

Details about the model implemented in Q4
1. We experimented by adding multiple PowerConv layers. Further, to preserve the stability of gradient propagation, we decided to 
add residual connections. We added additional fully connected layers to increase the model depth and complexity. As a result, the 
model took longer time to learn the parameters.
 
*****IMP*****
With the model improvement in Q4, we have been able to achieve a 1 point reduction in the test WER and CER on the
Q2B test dataset. 
We have used the same notebook from Q2B as a template on which we have built upon. We were not able to figure out how to
read the transcriptions without adhering to the data structure created by the hparams file. We also looked up the transcribe_file
function provided by Speechbrain but it was not available in the BaseASR template. Hence, we have not been able to generate 
transcriptions on the blindtest dataset and load the csv to Kaggle.

We request you to kindly go through the model improvements done by us and award us partial 
marks on the basis of the work done by us. 

References
1. https://github.com/vadimkantorov/ctc/tree/master (for the implementation of the code for CTC) 
2. https://github.com/speechbrain/speechbrain/tree/develop/recipes/LibriSpeech/ASR 
