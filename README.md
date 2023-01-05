# Identifying-between-two-modes-of-Z-boson-decay-
Using TensorFlow to create a model with an accuracy of 90% that can distinguish between two modes of Z boson decay.  For my work, I will consider two events here (Zee & Zmumu) as follows:
1) Zee is an event in which a Z boson turns into an electron and a positron.
2) Zmumu is an event in which a Z boson turns into a muon and an anti-muon.

I use two datasets, which are available on the CERN Open Data portal, Zee.csv and Zmumu.csv, each of which contains 10000 records. Datasets derived from the Run2011A. These data were selected from the primary datasets in order to obtain candidate Z boson events. 

I use TensorFlow to create a model that can distinguish between two events (Zee & Zmumu). To do this, every record in Zee.csv is labeled with 0 and every record in Zmumu.csv is labeled with 1.

In the end, I found that validation loss is decreasing before the 600th epoch, so the model is underfitting. However, after the 600th epoch, Validation loss is increasing, indicating an overfitted model. At the 600th epoch, when the model is either perfectly fitted or in a local minimum, the neural network model achieved an accuracy of 90%.
