Features and Updates
------------------------------------
Many thanks to George Berry, Ewan Klein, Pierpaolo Pantone for key contributions to make VADER better.  The new updates includes capabilities regarding:

#. Refactoring for Python 3 compatibility, improved modularity, and incorporation into `[NLTK] <http://www.nltk.org/_modules/nltk/sentiment/vader.html>`_ ...many thanks to Ewan & Pierpaolo.
#. Restructuring for much improved speed/performance, reducing the time complexity from something like O(N^4) to O(N)...many thanks to George.
#. Simplified pip install and better support for vaderSentiment module and component import. (Dependency on vader_lexicon.txt file now uses automated file location discovery so you don't need to manually designate its location in the code, or copy the file into your executing code's directory.)
#. More complete demo in the ``__main__`` for ``vaderSentiment.py``. The demo has:

	* examples of typical use cases for sentiment analysis, including proper handling of sentences with:

		- typical negations (e.g., "*not* good")
		- use of contractions as negations (e.g., "*wasn't* very good")
		- conventional use of **punctuation** to signal increased sentiment intensity (e.g., "Good!!!")
		- conventional use of **word-shape** to signal emphasis (e.g., using ALL CAPS for words/phrases)
		- using **degree modifiers** to alter sentiment intensity (e.g., intensity *boosters* such as "very" and intensity *dampeners* such as "kind of")
		- understanding many **sentiment-laden slang** words (e.g., 'sux')
		- understanding many sentiment-laden **slang words as modifiers** such as 'uber' or 'friggin' or 'kinda'
		- understanding many sentiment-laden **emoticons** such as :) and :D
		- understanding sentiment-laden **initialisms and acronyms** (for example: 'lol')

	* more examples of **tricky sentences** that confuse other sentiment analysis tools
	* example for how VADER can work in conjunction with NLTK to do **sentiment analysis on longer texts**...i.e., decomposing paragraphs, articles/reports/publications, or novels into sentence-level analyses
	* examples of a concept for assessing the sentiment of images, video, or other tagged **multimedia content**
	* if you have access to the Internet, the demo has an example of how VADER can work with analyzing sentiment of **texts in other languages** (non-English text sentences).