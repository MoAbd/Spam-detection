# Spam-detection
Implementation of  ANN for email spam-detection using TensorFlow  
The idea is simple - given an email you’ve never seen before, determine whether or not that email is Spam or not.

It is simple ,but very efficient as I reached 99.6% accuracy .

*The code is tested on python 2.7.11 and should work on python 2.x*

-------------------------------------------------------------------------------------------------------------------------
## Files description:

The data provided is from a kaggle [competition](https://inclass.kaggle.com/c/adcg-ss14-challenge-02-spam-mails-detection) 

- `TR.tar.gz` FILES contains 2500 mails both in Ham(1721) labelled as 1 and Spam(779) labelled as 0
- `spam-mail.tr.label` is the associated training labels.
- `ExtractContent.py`  extract the subject and body of the email.

> In a python compatible environment, 

> 1, invoke the script by command 

> ./ExtractContent.py

>  2, input source directory -- where you store the source files

>  For exmaple
   C:\EMAILPro\CSDMC2010_SPAM\TEST

> 3, input destination directory -- where you want the extracted body to be

> For example
  C:\EMAILPro\CSDMC2010_SPAM\TEST_NEW
    
> 4, we are done.

- `email_input.py`  vectorize the emails text,and outputs  trainX.csv, trainY.csv, testX.csv, and testY.csv 
- `data.tar.gz` contains trainX.csv, trainY.csv, testX.csv, and testY.csv
- `BagOfWords.p` contains all unique words from the data to use it later 
- `Spam detection.ipynb` Ipython notebook that train the model and call emails from ur Gmails to classify

#### The email format description:
 
*The format of the .eml file is definde in RFC822, and information on recent 
standard of email, i.e., MIME (Multipurpose Internet Mail Extensions) can be
find in RFC2045-2049.*

#### NOTE:
*In the notebook U will find how the model works , and how to authenticate ur Gmail*


