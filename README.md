# DeepChemStable
DeepChemStable: chemical stability prediction using attention-based graph convolution network

## Environment
Python 3.6.3 </br>
Tensorflow 1.1.0 </br>
RDkit 2018.03.4 </br>
autograd 1.2 </br>
numpy 1.14.2 </br>
pandas 0.23.4 </br>

## Model
The trained model weights are stored in `fingerprint_variables.bin`, `prediction_variables.bin`. </br>
Use the `predict.py` to predict. </br>
The predictions are saved in the file `results.csv`. </br>

## Usage
`>python predict.py *yourfilepath* *amount*` </br>
Examples: `>python predict.py test.csv 5` </br>

Data file format: </br>
&nbsp;&nbsp;&nbsp;&nbsp;Datafile should be CSV file; </br>
&nbsp;&nbsp;&nbsp;&nbsp;The header must be "substance_id, smiles, label"; </br>
&nbsp;&nbsp;&nbsp;&nbsp;In "label" column, use "1" for unstable, "0" for stable. </br>
