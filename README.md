# Twitter-country-geolocation
Dataset with country and coordinates of a collection of twitter users

This dataset is the original one used to infer Twitter users home country given the collection of nouns (proper and generic) from users past tweets (https://www.sciencedirect.com/science/article/pii/S0167923619300442).

The data, collected in the period between January/February 2018, are related to a sample of 3,289 twitter account. The information regarding the ground truth country are based on a duble check system that matched the metadata information (the address provided by the user in his/her Twitter account) and the analysis of location indicative words (LIW) given the historical tweets for each account.

From the original tweets we extracted only the nouns and thus the dataset reported includes the following information:

1. List of nouns for each user,
2. the address provided by the user in his/her Twitter account (metadata information),
3. latidute and longitude of the address,
4. ground truth country.


The dataset does not provide users account names for privacy reasons.

The dataset is stored as python list with .pickle extension. To load it:

import pickle 
pickle_in = open("country_geolocation.pickle","rb")
country_location = pickle.load(pickle_in)

If you use this dataset, please cite:
@article{zola2019twitter,
  title={Twitter user geolocation using web country noun searches},
  author={Zola, Paola and Cortez, Paulo and Carpita, Maurizio},
  journal={Decision Support Systems},
  year={2019},
  publisher={Elsevier}
}

Thank you!


