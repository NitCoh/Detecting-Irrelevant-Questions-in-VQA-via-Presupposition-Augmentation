# Detecting-Irrelevant-Questions-in-VQA-via-Presupposition-Augmentation
My Master's Thesis (BGU CS NLP Group)

In this work, we study the relevance of a question in the context of an image.
The setting is given an image, and a question in natural language,
we want to assess whether the question is relevant to the image. 
For example, given an image that shows a dog running on a beach, a question
asking about the location of a washing machine in the kitchen should be
flagged as irrelevant. We define relevance from a presupposition perspec-tive
and apply relevance theory to model the task of Visual Question Answering (VQA) in conversational settings.

Our key contributions are:
1. We provide a manual analysis of the challenging aspects of differ-
ent questions in GQA and categorize the types into eight different
classes of difficulty.
2. We developed a novel distance metric to compare presupposition to
the given context via Scene Graphs relying on the notion of accom-
modation process from Relevance Theory.
3. We provide a new data set of irrelevant questions that contain 100k
generated questions of different types.
4. We train an irrelevant question detector and demonstrate its perfor-
mance on the GQA Testdev split. We identify that about 2% of the
questions in this standard data set are actually irrelevant.


## Code
The code is available at the Irrelevant_Question_Generation_Pipeline notebook, originally created in Google Colab.
Few notes:
1. The code is anonymized in terms of paths to files, so you need to fill out the necessary paths.
2. All external files needed to run the notebook uploaded to this repo.
3. External files who arent avilable in this repo, could be found in Visual Genome or GQA websites.

## Generated Data

### Pre-defined Templates
https://drive.google.com/drive/folders/1KStBus0EPDvuSqrlPU2Wd4Y2AGwJTlds?usp=share_link

### GQA Questions
https://drive.google.com/drive/folders/1MsBo41_sKn7MMddk7P0ewiwe5fp-4Quy?usp=share_link

P.S we didn't run the pipeline for whole elements (scene graphs and gqa questions), thus
the data is partial and more can be generated.

## Accommodation-Based Pre-trained Metric
Final model (weights), metrics and evaluation can be found here:
https://drive.google.com/drive/folders/1-OmSfeKVWZ1r4lAd4EpggFMAFbh64jo9?usp=share_link
