Tweet-Sentiments
================

Takes in a tweet file and returns a new file with the zipcodes and sentiment values.

make_tweets reads a file of tweets line by line and
calls the make_tweet function to create a dictionary
out of each tweet.
make_tweet takes in a line of a tweet and creates a
dictionary with the keys text, time, lat, lon.
tweet_text takes in a line of a tweet and returns the
text of the tweet.
tweet_words takes in a line of a tweet and strips away
all of the punctuation. it returns a list of the words
in the tweet.
tweet_time takes in a line of a tweet and returns the
time.
tweet_location takes in a line of a tweet and returns
a tuple with the lat and lon.
make_zip_list takes in a csv file of zipcodes and calls
the make_zip function on each line of the file to return
a list of dictionaries
make_zip takes in a single line of a csv file represented
as a list and makes a dictionary with the keys zip, state,
lat, lon, and city
find_zip calls the geo_distance function to calculate the
distances between a given tweet location and all the
zipcodes in the csv file. it returns the closest zipcode.
find_state does the same thing as find_zip but returns
the state of the location.
geo_distance returns the distance between two locations
add_geo adds the keps zip and state to each dictionary in
the list of dictionaries.
write_tweets writes all of the dictionaries returned from
add_geo to a new file.

