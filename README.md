# RC-Text-Extraction
Text detection using Vision API and Spacy NER for reading RCs

# Fields that the model can extract
- License plate number or Regn number
- VIN number or Chassis number (typically 17 digit long)
- Name
- Engine number
- Registration date
- Mfg. date

# Approach and Methodology
- Used Cloud Vision API to extract text from images
- Upload the images to DataTurks and annotated them manually
- Used the annotated data from DataTurks to train a Spacy model for Name Entity Recognition (NER)
- The model performed nicely even though it was trained on only 40 data points

# How to run the project
- Clone the repository
- Create a Service Account on GCP to use Cloud Vision API, dowload and store the secret key
- Open NB named `NER_testing.ipynb` to test the model.
