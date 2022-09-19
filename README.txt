This project exemplifies how to train a custom-named entity model from Magic the Gathering (MTG) data using spacy and python.
This NER model is capable of recognizing game-specific entities such as Tap/Create (game actions) or Battlefield/Graveyard (field zones) in a card's text.

The project contains the following files:

1) DataCleansed.csv: contains MTG atomic card data with which the model is created (this file was created in a previous project - check the MTG_ML_Project repository).
2) ner_model.ipynb: Jupyter notebook with all the coding and explanations about the model's creation.
3) mtg_NER_training_data.spacy: DocBin object with all the training examples (this file is created inside file 2).
4) MTG_NER folder: custom NER model made with MTG data (this folder is created from the terminal, using data from file 3).
5) CombinedModel folder: custom model which consists of the en_core_web_sm model (which comes with the spacy library), but with the default ner component replaced with our MTG_NER model
(this folder is created inside file 2).
6) base_config.cfg: base configuration file - this is an incomplete file with only custom options (created in https://spacy.io/usage/training#quickstart).
7) config.cfg: complete configuration file created with base_config.cfg + filled in default values (this file is created from the terminal, using file 6).

 
