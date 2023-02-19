# Digital-archiving---OCR

Organization: EPISEN - Engineering school - Technologies for Health

Project realised by Yona Uzan - Clément Maureau

Digital archiving: Optical Character Recognition for the digital archiving of medical records

The project consists in training a dataset to predict a text with two models, LSTM (BI-LSTM) and transformers.
The transformer was trained on 14/25 epoch and obtained an accuracy of 65%. It is not provided with the hdf5 file because it exceeds 25 MB.  
Its goal is to eliminate some of the bureaucracy for patients, saving time for practitioners, doctors, nurses, etc.
But also to send more quickly to patients the documents that concern them, such as the report of an operation, for example.
Dataset used: IAM Handwriting Database
available here: [https://fki.tic.heia-fr.ch/databases/iam-handwriting-database](https://fki.tic.heia-fr.ch/databases/iam-handwriting-database)

## Descriptive analysis of the dataset
Images with a resolution of 300 dpi 
PNG format
256 gray levels 
115,320 words 
4 Folders: Words, Phrases, Shapes, Lines : 
Words, Phrases, Phrases, Indexed Lines 
With 4 .txt files : Words, Phrases, Shapes, Lines
## Description of the current deposit 
In this project, only the words classifier has been used. The principle remains the same for processing sentences: it suffices to change the delimiter to "|" when reading the words from the sentences.txt file. 
After this metadata, the names of the files with the corresponding metadata, which must be read with python so that each piece of information is taken into account. 
To use this pipeline, you need the following architecture: 
ascii/ascii/words.txt 
words/words/folders_names[ex:a01]\[ex:a01-000u]\filename[ex:a01-000u-00-00.png]. 

