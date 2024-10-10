# seq2seq4gec-en
- Code for the module paper for Grammatical Error Correction course at the University of Potsdam, summer semester'24.
- Author mail: polina.danilovskaia@uni-potsdam.de

## What is the project about?
- Grammatical Error Correction (GEC) is a task concerned with automatically correcting ungrammatical texts.
- For example, with a GEC tool, a sentence _Two butterflies is flying_ should be rewritten as _Two butterflies are flying_.
- In this repository you can find the implementation of a GEC model based on seq2seq approach.
- The GEC models were trained on an English essay dataset using [SentencePiece](https://github.com/google/sentencepiece) tokenizer. All models were evaluated with GLEU.
- The project was primarily done for learning purposes during the course at University of Potsdam.

## Repo Description
In the repository you can find Jupyter notebooks with code used for:
- preprocessing and tokenizing the WI&LOCNESS dataset
- models training
- GLEU evaluation
  
A link to download trained models is also provided. 

Only the preprocessed WI&LOCNESS dataset is included in the repo, if you want to have a look at the original dataset, please download it from [here](https://www.cl.cam.ac.uk/research/nl/bea2019st/#:~:text=W%26I%2BLOCNESS%20v2.1%3A%20DOWNLOAD%0ADescribed%20at%20the%20start%20of%20this%20section%20(Bryant%20et%20al.%2C%202019%3B%20Granger%2C%201998)).

## Examples
Even for the best of the models, there is still room for improvement in the accuracy of grammatical error correction: 

- **Original:** _It has been suggested that the Single Union could be based on a basic federal structure_
- **Correction by model 2:** _It has been suggested that the Soutpres will be been a a of of in the , , as the , , ,_

- **Original:** _It has also been alleged that the jackpots are too high ._
- **Correction by model 3:** _It has been suggested that the fairies are the the_ 

## Requirements
The code was run and tested in Google Colab, which provides an environment with all necessary libraries pre-installed.

## Acknowledgements
I thank Meng Li for teaching an introductory
seminar on Grammatical Error Correction at the
University of Potsdam in summer semester 2024
and providing the model architecture the implementation was
builded upon.
