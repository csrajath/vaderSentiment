====================================
About the Scoring
====================================

* The ``compound`` score is computed by summing the valence scores of each word in the lexicon, adjusted according to the rules, and then normalized to be between -1 (most extreme negative) and +1 (most extreme positive). This is the most useful metric if you want a single unidimensional measure of sentiment for a given sentence. Calling it a 'normalized, weighted composite score' is accurate. 
 
  It is also useful for researchers who would like to set standardized thresholds for classifying sentences as either positive, neutral, or negative.  
  Typical threshold values (used in the literature cited on this page) are:

 #. **positive sentiment**: ``compound`` score >=  0.5
 #. **neutral  sentiment**: (``compound`` score > -0.5) and (``compound`` score < 0.5)
 #. **negative sentiment**: ``compound`` score <= -0.5

* The ``pos``, ``neu``, and ``neg`` scores are ratios for proportions of text that fall in each category (so these should all add up to be 1... or close to it with float operation).  These are the most useful metrics if you want multidimensional measures of sentiment for a given sentence.