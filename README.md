# UN-Speech-Classification

The data used for this notebook can be found on https://unstats.un.org/unsd/methodology/m49/overview/ for decoding the ISO-3 Country Code
And https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/0TJX8Y for the speeches
There is also https://worldhappiness.report/ed/2021/ the happiness report which is not extensively used for our models, yet could provide some good info

The GDC Data has been tokenized and has had stopwords removed

There are 4 classification methods used inside:\
  1)A Multinomial Naive Bayes approach to classify a region of the world based on the words used on their speech\
  2)A Multinomial Naive Bayes approach to classify country of the world based on the words being used\
  3)A Complement Naive Bayes approach to classify a country of the world based on the words being used\
  4)A Complement Naive Bayes approach to classify a region of the world based on the words being used\
  

The models displayed 94%,96% 94%, 96% accuracy when compared to our test set using the k-fold validation method through Grid Search algorithm.
