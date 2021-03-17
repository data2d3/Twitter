# streaming tweets with tweepy

tweepy is a a well written and super easy to use to stream tweets. _computermacgyver's_ has written some excellent code to stream tweets. We will walk through his code in this video.  

# Code

The code for the tutorial can be found at [https://github.com/data2d3/Twitter/edit/main/tweepy_twitter-python-streamer](https://github.com/data2d3/Twitter/edit/main/tweepy_twitter-python-streamer)

I made a couple of small changes to _computermacgyver's_ excellent code [https://github.com/computermacgyver/twitter-python](https://github.com/computermacgyver/twitter-python) but the code is basically the same. The purpose is to create a video that walks through  _computermacgyver's_ excellent code.



# Steps

Install tweepy

```bash
$pip install tweepy
```

1. Update Auth.py with your credentials and have it in the same directory as streaming.py
  a.  Update the following lines with the information displayed in the web browser for your application: 

```python
    consumer_key="..." #Note this is now called API key	
    consumer_secret="..." #Note this is now called API secret
    access_token="..." 
    access_token_secret="...."
    #Replace the … with whatever values are shown in your web browser. Be sure to keep the quotation marks.
```

   b. Save the file as auth.py (not the same name as before)


2. Create a directory called Tweets
3. Within the Tweets directory, create a file called FILTER (all uppercase) with a list of keywords (as many as you want) one per line in the Tweets folder

  a.  note that you can use _touch_ on a Mac or linux to create a blank file called FILTER that you can edit in any text editor
```bash
$touch FILTER
```

5. Run the script python streaming.py

```bash
$ python streaming.py
```

or

```
$ python streaming.py >> logfile 2>> errorfile
```    

7. It will run indefinitely until you kill it or shut your computer down
8. The tweets will be saved as a .json file in the Tweets folder. We will discuss how to convert the data to .csv and explore it in other videos.



# Required Installs

You will need to install _tweepy_   

You can install python-twitter using::

    $ pip install tweepy 
    

# YouTube Tutorial

You can view the YouTube the walk through this code at 


##Reference
If you use this code in support of an academic publication, please cite:
   
    Hale, S. A. (2014) Global Connectivity and Multilinguals in the Twitter Network. 
    In Proceedings of the 2014 ACM Annual Conference on Human Factors in Computing Systems, 
    ACM (Montreal, Canada).

  
This code is released by _computermacgyver's_ under the [GPLv2 license](http://www.gnu.org/licenses/gpl-2.0.html). Please [computermacgyver](http://www.scotthale.net/blog/?page_id=9) if you wish to use the code in ways that the GPLv2 license does not permit.

More details, related code, and the original academic paper using this code is available at http://www.scotthale.net/pubs/?chi2014 .








