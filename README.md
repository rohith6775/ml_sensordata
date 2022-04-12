# ml_sensordata


data_link= https://archive.ics.uci.edu/ml/machine-learning-databases/00196/


data description : 

 datasets used from UCI MACHINE LEARNING Repository 
 
People used for recording of the data were wearing four tags (ankle left, ankle right, belt and chest). 
   Each instance is a localization data for one of the tags. The tag can be identified by one of the attributes.
   
    Number of Instances: 164860  Number of Attributes: 8 
  1) Sequence Name {A01,A02,A03,A04,A05,B01,B02,B03,B04,B05,C01,C02,C03,C04,C05,D01,D02,D03,D04,D05,E01,E02,E03,E04,E05} 
      - A, B, C, D, E  = 5 people
   2) Tag identificator {010-000-024-033,020-000-033-111,020-000-032-221,010-000-030-096}	
	  - ANKLE_LEFT = 010-000-024-033
	  - ANKLE_RIGHT = 010-000-030-096
	  - CHEST = 020-000-033-111
      - BELT = 020-000-032-221
   3) timestamp (Numeric) all unique
   4) date FORMAT = dd.MM.yyyy HH:mm:ss:SSS (Date) 
   5) x coordinate of the tag (Numeric)
   6) y coordinate of the tag (Numeric)
   7) z coordinate of the tag (Numeric)
   8) activity  {walking,falling,'lying down',lying,'sitting down',sitting,'standing up from lying','on all fours','sitting on the ground','standing up from sitting','standing up from sitting on the ground'}


ML ALOG USED:
            Random Forest Classifier
            AdaBoost Classifier
            GBC
  AS multi-classification  and nominal target so I moved with Classifier
  
  Why I choosed Random Forest Classifier(RFC)?
   The chosen data has large instances where RFC can  maintain the accuracy of a large proportion of data and high accuracy.
