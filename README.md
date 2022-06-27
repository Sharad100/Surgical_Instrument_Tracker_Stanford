# Surgical_Instrument_Tracker

This repo contains a training and testing algorithm for a ConvLSTM Surgical Tool Tracker. The model architecture (R+CL+C) can be found in this https://arxiv.org/pdf/1812.01366.pdf paper which includes a weakly supervised convolutional LSTM approach for tool tracking in laparoscopic videos. The model trains on the cholec80 dataset which contains 80 videos of cholecystectomy surgeries. The dataset also contains text files with frame-wise tool binary presence labels. 

I started with the evaluation script in this github link: https://github.com/CAMMA-public/ConvLSTM-Surgical-Tool-Tracker. I augmented it to train with a gradiant descent optimizer and an unweighted cross entropy as the loss function.

I trained this ConvLSTM model using a google colab Pro account but to maintain continuity across training videos, I had to checkpoint and restore model weights. Code for that is not included here
