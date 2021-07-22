# Graduation-Project

Project Name:<h3>Medical Prescription Handling Using AI Techniques</h3>

Description: Handwritten Text Recognition system that Help pharmacists and normal people to read a doctor’s handwritten prescription.

Based On:

1.[Medicine Box: Doctor’s Prescription Recognition Using Deep Machine Learning](https://www.sciencepubco.com/index.php/ijet/article/view/18785)

2.[Doctor’s Cursive Handwriting Recognition System Using Deep Learning](https://ieeexplore.ieee.org/document/9073521)

Main Idea:
- Help pharmacists and normal people to read a doctor’s handwritten prescription using “CRNN” Computer Vision system. 
- Using the recognized text and search for the most similar Drug names using an existing API for Drugs.
- Save all prescriptions and medical information in a digital format to avoid losing or using any papers.

Used Technologies: 
- TensorFlow: Model Architecture from [SimpleHTR](https://github.com/githubharald/SimpleHTR). 
- Flask: Creating an API to receive image from mobile app and return recognized text and a list of most similar Drug names.  
- Google Colab: For training the model and as a development server during the test.
- MySQL: Creating a Database to store all users information.      

Explanation:

Train a Convolutional-Recurrent Neural Network "CRNN" model using [Handwritten English Words from IAM dataset](https://fki.tic.heia-fr.ch/databases/iam-handwriting-database),
using saved model to predict new handwritten words (drug names).

Since the training was operating using Normal English words, so it was predicted that there would be some error ratio in the recognized Drug names to reduce error 
we used the recognized text from the model and search for the most similar Drug names using an existing API for Drugs [getSpellingSuggestions](https://rxnav.nlm.nih.gov/api-RxNorm.getSpellingSuggestions.html).



