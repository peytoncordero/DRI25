title: 'Text Analysis Workshop'
description: 'Digital technologies have made vast amounts of text available to researchers, and this same technological moment has provided us with the capacity to analyze that text faster than humanly possible. The first step in that analysis is to transform texts designed for human consumption into a form a computer can analyze. Using Python and the Natural Language ToolKit (commonly called NLTK), this workshop introduces strategies to turn qualitative texts into quantitative objects. Through that process, we will present a variety of strategies for simple analysis of text-based data.'
cover_image: '/images/workshops/img7.jpg'
programming_language: "jupyter"

learning objectives:
<<<<<<< HEAD
	- Expand data manipulation possibilities beyond quantitative data
	- Compare digital humanities and social science approaches to textual analysis.
	- Shed light on the system of relations behind the generation of data and packages.
	- Experiment and play with data, this time with canonical or well-established corpora
- Understand the conceptualization and operationalization steps of analysis.
	- Use and examine NLTK, an opportunity to look under the hood of Python package
	- Prepare texts for computational analysis, using stemmers and lemmatizers, and stop words removal
	- Learn and practice for loops, list comprehension

estimated time:
	- 2 hours

dependencies:
	workshop prerequisites:
    	python:
        	description: (required) This workshop relies heavily on concepts from previous Python workshops, and having a basic understanding of how to use the commands discussed in this workshop serves as a foundation for conducting text analysis.
        	required: true
    	command-line:
        	description: (recommended) This workshop makes some reference to concepts from the Command Line workshop, and having basic knowledge about how to use the command line will be central for anyone who wants to learn about text analysis with Python and NLTK.
        	recommended: true
	installations:
    	pythonguide:
        	description: (Required) You can use any installation of Python (but make sure it is of version 3). For our purposes, Anaconda will provide everything necessary for all the workshops that are part of the DHRI curriculum.
        	required: true
    	nltk:
        	description: (required) You will need to install the NLTK package into your Python packages for the purposes of this workshop. This guide will help you along the way.
        	required: true
	insights:
    	jupyter-notebooks:

=======
    - How to prepare texts for computational analysis, including strategies for transforming texts into numbers
    - How to use NLTK methods such as `concordance` and `similar`
    - How to clean and standardize your data, including powerful tools such as stemmers and lemmatizers
    - Compare frequency distribution of words in a text to quantify the narrative arc
    - Understand stop words and how to remove them when needed.
    - Utilize Part-of-Speech tagging to gather insights about a text
    - Transform any document that you have (or have access to) in a .txt format into a text that can be analyzed computationally
    - How to tokenize your data and put it in a format compatible with Natural Language Toolkit.

estimated time:
    - 10 hours

dependencies:
    workshop prerequisites:
        python:
            description: (required) This workshop relies heavily on concepts from the Python workshop, and having a basic understanding of how to use the commands discussed in the workshop will be central for anyone who wants to learn about text analysis with Python and NLTK.
            required: true
        command-line:
            description: (recommended) This workshop makes some reference to concepts from the Command Line workshop, and having basic knowledge about how to use the command line will be central for anyone who wants to learn about text analysis with Python and NLTK.
            recommended: true
    installations:
        pythonguide: 
            description: (Required) You can use any installation of Python (but make sure it is of version 3). For our purposes, Anaconda will provide everything necessary for all the workshops that are part of the DHRI curriculum.
            required: true
        nltk:
            description: (required) You will need to install the NLTK package into your Python packages for the purposes of this workshop. This guide will help you along the way.
            required: true
    insights:
        jupyter-notebooks:
            description: (recommended) This workshop uses Jupyter Notebooks to process the Python commands in a clear and visual way. Anyone who wants to follow along in the workshop on text analysis with Python and NLTK should read this very short introduction to how to use Notebooks.
>>>>>>> parent of 20a275f (learning objectives)

readings:
	- "[A Beginner’s Tutorial to Jupyter Notebooks](https://towardsdatascience.com/a-beginners-tutorial-to-jupyter-notebooks-1b2f8705888a)"
	- "[What is text analysis](https://www.scribbr.com/methodology/textual-analysis/)"

projects:
	- "[Short list of academic Text & Data mining projects](https://libguides.bc.edu/textdatamining/projects)"
	- "[Building a Simple Chatbot from Scratch in Python](https://github.com/parulnith/Building-a-Simple-Chatbot-in-Python-using-NLTK)"
	- "[Classifying personality type by social media posts](https://github.com/TGDivy/MBTI-Personality-Classifier)"

ethical considerations:
	- In working with massive amounts of text, it is natural to lose the original context. We must be aware of that and be careful when analyzing it.
	- It is important to constantly question our assumptions and the indexes we are using. Numbers and graphs do not tell the story, our analysis does. We must be careful not to draw hasty and simplistic conclusions for things that are complex. Just because we found out that author A uses more unique words than author B, does it mean that A is a better writer than B?

resources:
	- "[Jupyter Notebook shortcuts, tips and tricks](http://maxmelnick.com/2016/04/19/python-beginner-tips-and-tricks.html)"
---

# Text as Data

<<<<<<< HEAD
When we think of "data," we often think of numbers, things that can be summarized, statisticized, and graphed. Rarely when I ask people "what is data?" do they respond "_Moby Dick_." And yet, more and more, text is data. Whether it is _Moby Dick_, or every romance novel written since 1750, or today's newspaper or twitter feed, we are able to transform written (and spoken) language into data that can be quantified and visualized.

[needs a rewrite]
=======
When we think of "data," we often think of numbers, things that can be summarized, statisticized, and graphed. Rarely when I ask people "what is data?" do they respond "_Moby Dick_." And yet, more and more, text is data. Whether it is _Moby Dick_, or every romance novel written since 1750, or today's newspaper or twitter feed, we are able to transform written (and spoken) language into data that can be quantified and visualized. That has been done for a while, but now we can do it in a much larger scale, in a much faster way.
>>>>>>> parent of 20a275f (learning objectives)

Approaching this similar to how one learns quantitative analysis…we start the basics like mean median mode. 
What are basic ways to think about text as data?
How do we get data ready to be analyzed?
What can we learn from the data? 
The data we use 
## Corpora

> Definition of a corpus: “any collection of more than one text”

In your own research, as we’ve learned in the data literacy portion, the relationship between finding data and research question is iterative. 

In this workshop, we will hold the big theoretical questions and use a commonly used, publicly available set of texts for our corpus - NLTK

But you can think about a corpus as *any* collection of texts that are somehow related to each other. 

* 
* 
* 

There are infinitely many corpora, and, sometimes, you will want to make your own—that is, one that best fits your research question.

The route you take from here will depend on your research question. 

What’s an example of textual corpora in your field of research?

SOME MORE SCAFFOLDING?
## Note on Ethics
How is textual corpus generated? 

* 
* 
* 


## A Note About Languages

Languages are inherently social, fraught with the power dynamics inherent in any social phenomenon. Many existing tools for textual analysis, including the NLTK package in this workshop, do support many other languages, due to amazing contributions from the Python Text Analysis community. The support, however, varies according to the desired task. Not all functions and tools will be available for all the supported languages. The good news is that the available tools keep growing in quantity and quality.

What’s languages are most frequently used for web content as of January 2023, by share of websites?


https://www.statista.com/statistics/262946/most-common-languages-on-the-internet/


**Additional resources for non-English textual analysis**

This is beyond the scope of this workshop but here are some starting off points to 

## Package

Some terminology as we bring in our packages:
There are packages, which are just collection of modules and these modules are just files that contains a set of functions.  

We are specifying which module we want to bring in from what package
There are also some built in functions or actions that can be taken upon a text.

What is this percentage sign? Magic function! With this backend, the output of plotting commands is displayed in Jupyter notebook, directly below the code cell that produced it. The resulting plots will then also be stored in the notebook document, not separate popup window.


## Evaluation

Which of the following could be considered a corpus?

<Quiz>
- My 2 year-old nephew’s random iPad mashings
- Your grocery list for this past week
- All of our grocery lists from this past week
- Your grocery lists from 2013-2023
- Random sample of tweets with #blessed
</Quiz>

## Keywords

Do you remember the glossary terms from this section?

- [NLTK](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/nltk.md)
- Package

# Using the NLTK Corpus

In the following sections, we are going to learn how to work with the NLTK Corpus and go through a series of methods that come built-in to NLTK that allow us to turn our words into numbers and visualizations.

## So What Corpus are We Using?
Loading our copus we’re using into our JupyterLite notebook

Start with a new JupyterLite file

**Review Jupyterlite commands**
 * Two modes – Edit Mode (to edit code, press Enter on any cell) and Command Mode (to run the code, press Escape on any cell)
 * When in Command Mode
 	* Add new cells with “A”; delete cells with “B”

All three of these commands can be written in the same cell and run all at once (<kbd>shift</kbd> + <kbd>enter</kbd>) or in different cells.

If you don't see an error when you run the notebook—that is, if there is no output—you can move on to the next step. It is not rare in programming that when you do things right, the result will be nothing happening. This is what we like to call a _silent success_.

**Libraries** are sets of instructions that Python can use to perform specialized functions. The Natural Language ToolKit (`nltk`) is one such library. As the name suggests, its focus is on language processing.


```
import nltk
import pyodide_http
pyodide_http.patch_all()
```

We will also need the `matplotlib` library later on, so import it now:


```
from wordcloud import WordCloud
import matplotlib.pyplot as plt
%matplotlib inline
```

`matplotlib` is a library for making graphs. In the middle of this tutorial, we are going to make a dispersion plot of words in our texts.

Finally, because of a quirk of Jupyter notebooks, we need to specify that `matplotlib` should display its graphs in the notebook (as opposed to in a separate window), so we type this command (this is technically a Jupyter command, not Python):


```

nltk.download('all-corpora')
```

OR 

```
nltk.download('genesis')
nltk.download('gutenberg')
nltk.download('inaugural')
nltk.download('nps_chat')
nltk.download('treebank')
nltk.download('webtext')
nltk.download('wordnet')
```

Next, we need to load all of the NLTK corpora into our program. 

The pre-loaded NLTK texts should appear again. These are preformatted data sets. We will still have to do some minor processing, but having the data in this format saves us a few steps. At the end of this tutorial, we will make our own corpus. This is a special type of python object specific to NLTK (it isn't a string, list, or dictionary). Sometimes it will behave like a string, and sometimes like a list of words.


```
from nltk.book import *
```

Notice that each of the texts already have a variable name. _Moby Dick_ is `text1`, _Sense and Sensibility_ is `text2`, and so on. When we want to work with those books, we will call them by their variable name, as you'll see soon.


What does it look like we’re working with?


## Explore
Let's pick one of these books for exploration...
```
text2
```

What is this object? 
What can we do with it? 
What's a way that we can poke at this thing?
Other commands from previous workshops we can throw at this thing?

```
type(text4)

```
Huh that's interesting, what does that mean? Let's check out what is in the object. Let’s look at the first 10 elements in this object...



```
text3[0:10]
```
The most famous opening line…

Is this text structured.....? Recall date literacy

So what we'll be doing the rest of the workshop is to whittle down this text to a smaller list of words, a "more meaningful" list of words. 

How might this be different from other corpus that you work with?

If you got any error messages, check the code and make sure you typed everything correctly. Even spaces before words matter!


## Keywords

Do you remember the glossary terms from this section?

- [Corpus](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/corpus.md)
- [Jupyter Notebook](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/jupyter-notebook.md)
- [Library](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/library.md)
- [Matplotlib](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/matplotlib.md)

# Searching for the Words

Let’s start by analyzing any of the books, text1 through text10. 

Pick one and think about its topic. 

The first function we will look at is `concordance`. "Concordance" in this context means the characters on either side of the word. Our text is behaving like one giant string, so concordance will just count the number of characters on either side. By default, this is 25 characters on either side of our target word (including spaces), but [you can change that if you want](http://www.nltk.org/_modules/nltk/text.html#Text.concordance).

In the Jupyter Notebook, type:

```python
text1.concordance("whale")
```

The output shows us the 25 characters on either side of the word "whale" in _Moby Dick_. Let's try this with another word, "love." Just replace the word "whale" with "love," and we get the contexts in which Melville uses "love" in _Moby Dick_. `concordance` is used (behind the scenes) for several other functions, including `similar` and `common_contexts`.

Let's now see which words appear in similar contexts as the word "love." NLTK has a built-in function for this as well: `similar`.

```python
text1.similar("love")
```

Behind the scenes, Python found all the contexts where the word "love" appears. It also finds similar environments, and then what words were common among the similar contexts. This gives a sense of what other words appear in similar contexts. This is somewhat interesting in itself, but more interesting if we compare it to something else. Let's take a look at another text. What about _Sense and Sensibility_ (`text2`)? Let's see what words are similar to "love" in Jane Austen's writing. In the next cell, type:

```python
text2.similar("love")
```

We can compare the two and see immediately that Melville and Austen use the word "love" differently.

## Investigating "lol"

Let's expand from novels for a minute and take a look at the NLTK Chat Corpus. In chats, text messages, and other digital communication platforms, "lol" is exceedingly common. We know it doesn't simply mean "laughing out loud"—maybe the `similar` function can provide some insight into what it does mean.

```python
text5.similar("lol")
```

The resulting list is a lot of greetings, indicating that "lol" probably has more of a [phatic function](https://www.oxfordreference.com/view/10.1093/oi/authority.20110803100321840). Phatic language is language primarily for communicating social closeness. Phatic words stand in contrast to semantic words, which contribute meaning to the utterance.

If you are interested in this type of analysis, take a look at the `common_contexts` function in the [NLTK book](https://www.nltk.org/book/) or in the [NLTK docs](https://www.nltk.org/).

## Evaluation

Which one of the following sentences is correct?

<Quiz>
- The similar method brings a list of words that are similar in writing, but not necessarily in meaning, like "whale" and "while".
- Using the `concordance` method with a specific word, such as "whale", returns the words that surround "whale" in different sentences, helping us to get a glimpse of the contexts in which the word "whale" shows up.*
</Quiz>

## Keywords

Do you remember the glossary terms from this section?

- [Concordance](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/concordance.md)
- [Phatic Language](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/phatic-language.md)

# Positioning Words

In many ways, `concordance` and `similar` are heightened word searches that tell us something about what is happening near the target words. Another metric we can use is to visualize where the words appear in the text. In the case of _Moby Dick_, we want to compare where "whale" and "monster" appear throughout the text. In this case, the text is functioning as a list of words, and will make a mark where each word appears, offset from the first word. We will _pass_ this _function_ a _list_ of _strings_ to plot. In the next cell, type:

```python
text1.dispersion_plot(["whale", "monster"])
```

A graph should appear with a tick mark everywhere that "whale" appears and everywhere that "monster" appears. Knowing the story, we can interpret this graph and align it to what we know of how the narrative progresses, helping us develop a visual of the story — where the whale goes from being a whale to being a monster to being a whale again. If we did not know the story, this could give us hints of the narrative arc.

text2.dispersion_plot(["Brandon","Elinor","Lucy","Edward","Marianne"])

Looking at this plot, who is the main character?

Why might a tool like this be useful? A graph should appear with a tick mark everywhere each “character name” appears. Knowing the story, we can interpret this graph and align it to what we know of how the narrative progresses, helping us develop a visual of the story.

Now try with another book and another set of words: please report if you find a cool one!


## Challenge

Try this with `text2`, _Sense and Sensibility_, [as we saw here](#downloading-the-corpus). Some relevant words are "marriage," "love," "home," "mother," "husband," "sister," and "wife." Pick a few to compare. You can compare an unlimited number, but it's easier to read a few at a time. (Note that the comma in our writing here is _inside_ the quotation mark, because that is how proper English grammar works. However, in Python, you would have to put commas _outside_ of the quotation marks to create a _list_.)


## Solution

```python
text2.dispersion_plot(["love", "marriage"])
```

```python
text2.dispersion_plot(["husband", "wife"])
```

## Evaluation

Check all sentences below that are correct:

<Quiz>
- You can get a visual representation of occurrences of a word with the `dispersion_plot` method.*
- The `dispersion_plot` method allows you to input a list of strings, as long as you split them with commas.*
- Contrary to grammar rule, in a list of strings, the commas must come outside of the quotation marks.*
</Quiz>

# Types vs. Tokens

**Buffalo buffalo Buffalo buffalo buffalo buffalo Buffalo buffalo**

How many words are there on the screen?

A word "token" is a particular appearance of a given word in a text, these two appearances of “the”; a word "type" is the unique form of the word as a particular sequence of letters, which there are 2, at this stage of processing our text. This terminology is important to understand how we cutting down our list to be more meaningful.

Depends on whether you are asking whether words refers to tokens or types: token is an instance of a type, so let's try this again: how many types of words are on the screen? How many tokens?

How many words are in Moby Dick?
```
len(text1)
```

Let's find out how many times a given word appears in the corpus. In this case (and all cases going forward), our text will be treated as a list of words, using ‘count’ function. 



```
text1.count("whale")
```

We see that "whale" occurs 906 times.

How about “Whale”?

```python
text1.count("Whale")
```
How about “WHALE”?

```
text1.count("WHALE")
```

What is clear here is that the `count` method is case-sensitive.

Three types for the word whale:


| Type  | # of Tokens |
| ----- |:------:|
| whale | 906|
| Whale | 282|
| WHALE | 38 |


But what do we need to do to the corpus so that all of the types of “whale” get treated the same way? 

Why do we need each type to be treated the same way?

<Secret>

Make a list of all the words lowercase!

Bonus: That also means removing non-words (i.e. punctuation)

</Secret>

## Make a list of all the words lowercase!


Just like in cooking, let’s think about what we know and gather our ingredients to achieve our goal, “make a list of all the words lowercase”:

 * We want a new list of the same corpus (text1) - performing any operation on the original would be irreversible 
 * Python has a built-in function, ‘isalpha()’ that will allow us know (**True or False**) if a string object contains only alphabetic characters
 * Python has a built-in function, `lower()` that takes a character string and converts all the letters to lower case
 * Lastly, we have our original corpus object, text1

**Practice**

```
string = "ELI5"
print(string.isalpha())
print(string.lower())

```

Let’s think through what we can do with these four ingredients to make a list of all the words lowercase:


Logic of the code
<Secret>
Create new list.

In each element (in our case, it is each word) of the original corpus object, we ask, **True or False**,
 * If True, we want to convert it to lower case
 * If False, ignore it
Take this new lower case object and add it to our list

</Secret>

Code version

<Secret>

```
text1_tokens = []
for t in text1:
	if t.isalpha():
    	t = t.lower()
    	text1_tokens.append(t)
```
</Secret>


If everything went right, you should get no output. Remember the "silent success?"

## Make a list of all the words lowercase with ONE LINE OF CODE


Another way to perform the same action more tersely is to use what's called a [list comprehension](https://docs.python.org/3/tutorial/datastructures.html#list-comprehensions). A list comprehension is a shorter, faster way to write a for-loop. It is syntactically a little more difficult to read (for a human), but, in this case, it's much faster to process.

```
text1_tokens = [t.lower() for t in text1 if t.isalpha()]
```

## Take a Breath

Let's take a breath, because this was a difficulty spike. For loops are weird and not super intuitive. It usually takes some time for us to get used to them.

I suggest going back to the loop above, review it, try to understand why all indentations are where they are.

Feel like you understand it? Try deleting it and writing the loop yourself without looking at this guide.

Play around! What happens if we got rid of the if statement? What happens when you change the order of the commands? How about the indentation? Don't be afraid to break it.

If you feel like you are done playing with the loop, time to move to the next section to see the results.

## Evaluation

Check all sentences below that are correct:

<Quiz>
- "Whale", "WHALE", and "whale" are all different tokens of the same type.
- The `lower()` method returns the lowercase form of all of the alphabetical characters in a string.*
- The `isalpha()` method transforms integers in alphabetical strings.
- The `append()` method adds an item to the end of the list.*
</Quiz>


## Keywords

Do you remember the glossary terms from this section?


- [Token](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/token.md)
- [Tokenizing](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/tokenizing.md)
- [Type](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/type.md)

# Length and Unique Words

Great! Now `text1_tokens` is a list of all of the tokens in our corpus, with the punctuation removed, and all the words in lowercase. Let's check it:

```python
text1_tokens.count("whale")
```
And now we have 1226 tokens for "whale", which is the exact sum of the counts we did before. 

All the instances of "Whale", "whale", "WHALE" are now just "whale".
```python
text1_tokens.count("Whale")
```
```python
text1_tokens.count("WHALE")
```

Now we want to know how many words there are in our corpus—that is, how many tokens in total. 

Therefore, we can ask, "What is the length of that list of words?" Python has a built-in `len` function that allows you to find out the length of different types of objects. 

 * Pass it a list, and it will tell you how many items are in the list
 * Pass it a string, and it will tell you how many characters are in the string
 * Pass it a dictionary, and it will tell you how many items are in the dictionary. 

How does the length of text1_tokens compare to original text1 object?

```
len(text1)
len(text1_tokens)
```
From our list of tokens, how do we get a list of the types? AKA how do we want a list of unique words? 

Why would that be analytically important?

In order to get unique words, rather than just all words in general, we will make a **set** from the list. A `set` in Python works just like it would [in math](https://en.wikipedia.org/wiki/Set_(mathematics)), it's all the unique values, with any duplicate items removed.

```python
list_example = [2,3,4,12,3,12,3,1,32]
```

What should expect from set(list_example)?

<Secret>
32, 1, 2, 3, 4, 12
</Secret>

So let's find out the length of our set. just like in math, we can also nest our functions. So, rather than saying `x = set(text1_tokens)` and then finding the length of "x", we can do it all in one step.

How do we do that? 

<Secret>
len(set(text1_tokens))
</Secret>


# Lexical Density

Now we can calculate the **lexical density**, the number of unique words per total words. [Statistical studies](https://pdfs.semanticscholar.org/c2a8/56959d7f5880c98ccd4cfeb4b4f5b7133ec7.pdf) have shown that lexical density is a good metric to approximate lexical diversity—the range of vocabulary an author uses. This by no means suggests more or less sophistication.

Gertrude Stein's "A rose is a rose is a rose is a rose" would be rendered meaningless otherwise. Or the book Jack Nicholson was writing in the Shining? "All work and no play, makes Jack a dull boy," typed out into haunted eternity?

For our first pass at lexical density, we will simply divide the number of unique words by the total number of words:

```python
len(set(text1_tokens)) / len(text1_tokens)
```
## Challenge

Let's compare the lexical density of _Moby Dick_ with _Sense and Sensibility_. Make sure to:

1. Make all the words lowercase and remove punctuation.
2. Make a slice of the first 10,000 words.
3. Calculate lexical density by dividing the length of the set of the slice by the length of the slice.

Remember to be aware of the ethical implications for the conclusions that we might draw about our data. What assumptions might we be reifying about these writers?

## Solution

```python
text2_tokens = []
for t in text2:
	if t.isalpha():
    	t = t.lower()
    	text2_tokens.append(t)

text2_slice = text2_tokens[0:10000]

len(set(text2_slice)) / len(text2_slice)
```

## Evaluation

Check all sentences below that are correct:

<Quiz>
- The `len` method returns the length of the input, which can mean different things depending on its type. If it is a string, it will return the number of characters; if it is a list or dictionary, it will return the number of items.*
- The lexical density measures the number of unique words per total word, and it is an objective measure of writing quality.
- Comparing the lexical density between texts of different sizes can give a problematic result. A possible solution is to use list slice and compare parts of both texts of a similar size.*
</Quiz>

# Cleaning and Normalizing

Once we have a corpus—whether that is one text or millions—we usually want to clean and normalize it. There are three terms we are going to need:

- **Text normalization** is the process of taking a list of words and transforming it into a more uniform sequence. Usually, this involves removing punctuation, making the words all the same case, removing _stop words_, and either _stemming_ or _lemmatizing_ the words. It can also include expanding abbreviations or matching misspellings (but these are advanced practices that we will not cover).

You probably know what removing punctuation and capitalization refer to, but the other terms may be new:

- **Stop words** are words that appear frequently in a language, often adding grammatical structure, but little semantic content. There is no official list of stop words for any language, though there are some common, all-purpose lists built in to NLTK. However, different tasks require different lists. The purpose of removing stop words is to remove words that are so common that their meaning is diminished across a large number of texts.

- **Stemming and lemmatizing** both of these processes try to consolidate words like "laughs" and "laughing" to  "laugh" since they all mean essentially the same thing, they are just inflected differently. So again, in an attempt to reduce the number of words, and get a realistic understanding of the meaning of a text, these words are collapsed. Stemming does this by cutting off the end (very fast), lemmatizing does this by looking up the dictionary form (very slow).

Language is messy, and created for and by people, not computers. There is a lot of grammatical information in a sentence that a computer cannot use. For example, I could say to you:

> The house is burning.

and you would understand me. You would also understand if I say

> house burn.

The first has more information about tense, and which house in particular, but the sentiment is the same either way.

What's happening between "the house is burning" and "house burn"

We removed the stop words (_the_ and _is_), and removed punctuation and case, and simplified what was left (_burning_ becomes _burn_). 

This results in what is essentially a "bag of words," or a corpus of words without any structure. 

Because normalizing your text reduces the number of words (and therefore the number of dimensions in your data), and keeps only the words that contribute meaning to the document, this cleaning is usually desirable.

There is "clean" and "dirty" versions of text data. Sometimes our questions are about the clean data, but sometimes our questions are in the "dirt."

## A Note on Ethics

The act of cleaning/normalizing subscribes text to predetermined categories of meaning, forcing meaning into existing "boxes," so to speak. This doesn't mean that we should avoid cleaning or normalizing text, but that we should be aware of how some textual reductions have the potential to affect meaning. How does quantification reinforce differences or stratifications within our data? We have to be careful about the kinds of questions we are asking, and how we might be reproducing some of our assumptions in our inquiry.

To read more about ethics and text analysis, see Lauren Klein's "[Distant Reading After Moretti](https://arcade.stanford.edu/blogs/distant-reading-after-moretti)," where she questions, "Instead of first asking what can be modeled—what phenomena we can track at scale—we might instead ask: what might be hidden in this corpus?”

## Evaluation

Which one of the following sentences is correct:

<Quiz>
- Stop words are useless for text analysis, therefore the first step in any project is to remove them from the text.
- In any type of data analysis, we usually want to cleanse the data in order to prepare it for the analysis. In text analysis, this process is called "text normalization" and can involve tasks such as removing undesired words and punctuation.*
- Textual alterations can potentially change the original intended meaning. Therefore, we must always strive to work with the data exactly as it is in the source.
</Quiz>

## Keywords

Do you remember the glossary terms from this section?

- [Machine Learning](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/machine-learning.md)
- [Text Normalization](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/text-normalization.md)

# Word Cloud

Let's use another visual tool to see where we are in our data exploration process...a word cloud. It is a collection, or cluster, of words depicted in different sizes. The bigger and bolder the word appears, the more often it's mentioned within a text

We are all familiar and we can use our list of tokens. Why would our list of unique words not be appropriate for a word cloud?

text = text1_tokens
wordcloud = WordCloud().generate(text)
plt.imshow(wordcloud)

text = str(text1_tokens)
wordcloud = WordCloud().generate(text)
plt.imshow(wordcloud)

Is this useful? What are all these words? Does this tell me anything about Moby Dick? No, we need to clean this text!

# Data Cleaning: Removing Stop Words

We've completed one out of three steps of data cleaning.

1. Remove capitalization and punctuation
2. Remove stop words.
3. Lemmatize (or stem) our words, i.e. "jumping" and "jumps" become "jump."

This next section, we will be cleaning our corpus by removing the stop words. In seeing getting the most frequent words, a lot of them were extremeley common words, so we should get rid of them because they don't tell us anything meaningful about the text, very little semantic meaning and most often have grammatical functions. Usually, these are function words such as determiners, prepositions, auxiliaries, and others.

To use NLTK's stop words, we need to import the list of words from the corpus. 

```python
from nltk.corpus import stopwords
```

We need to specify the English list, and save it into its own variable that we can use in the next step:

```python
stops = stopwords.words('english')
```

Now let's take a look at those words:

```python
print(stops)
```

What's the logic we'll use to make a new list of the corpus without stop words?

<Secret>


we have a list of words from our corpus, we also have a list of words (stopword) we don't want in our new list, to check if every word is in this stopword list. 

If the word is not in that list, we will keep it...

Now we want to go through all of the words in our text, and if that word is in the stop words list, remove it from our list. Otherwise, we want it to skip it. (The code below is slow, so it may take some time to process).

</Secret>

**Code**

<Secret>


```python
text1_stops = []
for t in text1_tokens:
	if t not in stops:
    	text1_stops.append(t)
```

</Secret>


Now try it with the one-liner, AKA list comprehension

```python
text1_stops = [t for t in text1_tokens if t not in stops]
```

To check the result:

```python
print(text1_stops[:30])
```

## Verifying List Contents

Now that we removed our stop words, let's see how many words are left in our list:

```python
len(text1_stops)
```

## Revised Word Cloud


```python

text = str(text1_stops)
wordcloud = WordCloud().generate(text)
plt.imshow(wordcloud)

```

## How do we get rid of parantheses? 

Googling for the answers to your coding questions is an essential part of being a coder. let's try out how to google a problem and use the solution: how to get rid of are there apostrophes?

Word Cloud python library displays an apostrophe

https://stackoverflow.com/questions/59529467/word-cloud-python-library-displays-an-apostrophe-at-the-end-of-every-word

Direct Copy and Paste: 

```
string_text = ' '.join(tokenized_text)    
wordcloud = WordCloud(width=1600, height=800).generate(string_text)
```

How do we need to adapt it to our code with our variables?

```
string_text = ' '.join(text1_stops)    
wordcloud = WordCloud(width=1600, height=800).generate(string_text)
```

```
wordcloud = WordCloud().generate(string_text)
plt.imshow(wordcloud)
```


## Evaluation

Check all sentences below that are correct:

<Quiz>
- Stop words are words that usually don't contribute with much semantic content, like prepositions, determiners, etc.*
- To use stop words we need to import them from the nltk corpus, using the following code: `import stopwords from nltk.corpus`
- List comprehensions are faster ways of iterating and creating lists when compared with for loops.*
</Quiz>

## Keywords

Do you remember the glossary terms from this section?

- [Stop Words](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/stop-words.md)

# Data Cleaning: Lemmatizing Words

Now that we've removed the stop words from our corpus, the next step is to stem or lemmatize the remaining words. This means that we will strip off the grammatical structure from the words. For example, `cats ⭢ cat`, and `walked ⭢ walk`. This gets complicated, such as in the case of `men ⭢ man` and `sang ⭢ sing`. 

Lemmatization deals with this by looking up the word in a reference and finding the appropriate root. So I have to import this module.

NLTK comes with pre-built lemmatizers.

We will use the WordNet Lemmatizer from the NLTK Stem library, so let's import that now:

```python
from nltk.stem import WordNetLemmatizer
```

Because of the way that it is written "under the hood," an instance of the lemmatizer needs to be called. We know this from reading [the docs](https://www.nltk.org/).

```python
wordnet_lemmatizer = WordNetLemmatizer()
```

Let's quickly see what lemmatizing does.

```python
wordnet_lemmatizer.lemmatize("children")
```

Now try this one:

```python
wordnet_lemmatizer.lemmatize("better")
```

It didn't work, but...

```python
wordnet_lemmatizer.lemmatize("better", pos='a')
```

... sometimes we can get better results if we define a specific part of speech(pos). "a" is for "adjective", as we learned [here](http://www.nltk.org/_modules/nltk/corpus/reader/wordnet.html).

Now we will lemmatize the words in the list.

```python
text1_clean = []
for t in text1_stops:
	t_lem = wordnet_lemmatizer.lemmatize(t)
	text1_clean.append(t_lem)
```

And again, there is a faster version for you to use once you feel comfortable with list comprehensions:

```python
text1_clean = [wordnet_lemmatizer.lemmatize(t) for t in text1_stops]
```

## Verifying Clean List Contents

Let's check now to see the length of our final, cleaned version of the data, and then check the unique set of words. Notice how we will use the `print` function this time. 

JupyterLite does print commands without the `print` function, but it will only print one thing per cell (the last command), and we wanted to print two different things:

```python
print(len(text1_clean))
print(len(set(text1_clean)))
```

If everything went right, you should have the same length as before, but a smaller number of unique words. That makes sense since we did not remove any word, we only changed some of them.

Why don't you try that by yourself? Try to remember how to calculate lexical density without looking back first. It is ok if you have forgotten.

Now let's have a look at the words Melville uses in _Moby Dick_. We'd like to look at all of the _types_, but not necessarily all of the _tokens._ We will order this set so that it is in an order we can handle. In the next cell, type:

```python
sorted(set(text1_clean))[:30]
```

`sorted` combined with `set` should give us a list of all the unique words in _Moby Dick_ in alphabetical order, but we only want to see the first ones. Notice how there are some words we wouldn't have expected, such as 'abandon', 'abandoned', 'abandonedly', and 'abandonment'. This process is far from perfect, but it is useful. However, depending on your goal, a different process, like _stemming_ might be better.

## Evaluation

Check all sentences below that are correct:

<Quiz>
- Stemming and lemmatizing are different forms of reducing word variations to their roots.*
- `sorted(set(list_of_strings))` returns the unique items of `list_of_strings` in alphabetical order.*
</Quiz>

## Keywords

Do you remember the glossary terms from this section?

- [Lemmatization](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/lemmatization.md)
- [Lexical Density](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/lexical-density.md)

# Data Cleaning: Stemming Words

The code to implement this and view the output is below:

```python
from nltk.stem import PorterStemmer
porter_stemmer = PorterStemmer()
```

The Porter is the most common Stemmer. Let's see what stemming does to words and compare it with lemmatizers:

```python
print(porter_stemmer.stem('berry'))
print(porter_stemmer.stem('berries'))
print(wordnet_lemmatizer.lemmatize('berry'))
print(wordnet_lemmatizer.lemmatize('berries'))
```

Stemmer doesn't look so good, right? But how about checking how stemmer handles some of the words that our lemmatized "failed" us?

```python
print(porter_stemmer.stem('abandon'))
print(porter_stemmer.stem('abandoned'))
print(porter_stemmer.stem('abandonedly'))
print(porter_stemmer.stem('abandonment'))
```

Still not perfect, but a bit better. So the question is, how to choose between stemming and lemmatizing? As many things in text analysis, that depends. The best way to go is experimenting, seeing the results and choosing the one that better fits your goals.

As a general rule, stemming is faster while lemmatizing is more accurate (but not always, as we just saw). For academics, usually the choice goes for the latter.

Anyway, let's stem our text with the Porter Stemmer:

```python
t1_porter = []
for t in text1_clean:
	t_stemmed = porter_stemmer.stem(t)
	t1_porter.append(t_stemmed)
```

Or, if we want a faster way:

```python
t1_porter = [porter_stemmer.stem(t) for t in text1_clean]
```

And let's check the results:

```python
print(len(set(t1_porter)))
print(sorted(set(t1_porter))[:30])
```

A very different list of words is produced. This list is shorter than the list produced by the lemmatizer, but is also less accurate, and some of the words will completely change their meaning (like 'berry' becoming 'berri').

## Evaluation

Check all sentences below that are correct:

<Quiz>
- Both Stemming and Lemmatizing are far from perfect, so they must be used with caution.*
- There is no obvious best choice between Stemmers and Lemmatizers, so the best way to go is experimenting and seeing what results better fit your goals.*
</Quiz>

## Keywords

Do you remember the glossary terms from this section?

- [Stemming](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/stemming.md)

# Data Cleaning: Results

Now that we've seen some of the differences between both, we will proceed using our lemmatized corpus, which we saved as `text1_clean`:

```python
my_dist = FreqDist(text1_clean)
```

If nothing happened, that is normal. Check to make sure it is there by calling for the type of the "my_dist" object.

```python
type(my_dist)
```

The result should say it is a nltk probability distribution (`nltk.probability.FreqDist`). It doesn't matter too much right now what that is, only that it worked. We can now plot this with `matplotlib`'s function called `plot`. We want to plot the first 20 entries of the `my_dist` object.

```python
my_dist.plot(20)
```

![nltk plot distribution](/images/text-analysis/nltk_plot.png)

We've made a nice image here, but it might be easier to comprehend as a list. Because this is a special probability distribution object we can call the `most_common` on this, too. Let's find the twenty most common words:

```python
my_dist.most_common(20)
```

What about if we are interested in a list of specific words—perhaps to identify texts that have biblical references. Let's make a (short) list of words that might suggest a biblical reference and see if they appear in _Moby Dick_. Set this list equal to a variable:

```python
b_words = ['god', 'apostle', 'angel']
```

Then we will loop through the words in our cleaned corpus, and see if any of them are in our list of biblical words. We'll then save into another list just those words that appear in both.

```python
my_list = []
for word in b_words:
	if word in text1_clean:
    	my_list.append(word)
	else:
    	pass
```

And then we will print the results.

```python
print(my_list)
```

You can obviously do this with much larger lists and even compare entire novels if you wish, though it would take a while with this approach. You can use this to get similarity measures and answer related questions.

## Challenge

1. Try to get the same result of the loop above (the one with "my_list"), but this time with a list comprehension. Save this other list as "my_list2".

2. Compare both lists to see if they are identical.

## Solution

1. A solution using a list comprehension would look like this:

	```python
	my_list2 = [word for word in b_words if word in text1_clean]
	```

2. To compare the lists, you could run the following command:

	```python
	my_list == my_list2
	```

## Evaluation

Which one of the following sentences is correct:

- We can create a frequency distribution of a list of strings with `FreqDist` and plot it with the `plot` method.*
- `my_dist.most_common(50)` will check the first 50 words in the distribution and return you the most common one among them.

# Make Your Own Corpus

Now that we have seen and implemented a series of text analysis techniques, let's go to the Internet to find a new text. You could use something such as historic newspapers, or Supreme Court proceedings, or use any txt file on your computer. Here we will use [Project Gutenberg](http://www.gutenberg.org). Project Gutenberg is an archive of public domain written works, available in a wide variety of formats, including `.txt`. You can download these to your computer or access them via the url. We'll use the latter. We found _Don Quixote_ in the archive (see [here](http://www.gutenberg.org/files/996/996-0.txt)), and will work with that.

The Python package `urllib` comes installed with Python. Since we are only going to use the `urlopen` function, we will just import that one.

In the next cell, type:

```python
from urllib.request import urlopen
```

The `urlopen` function allows your program to interact with files on the internet by opening them. It does not read them, however—they are just available to be read in the next line. This is the default behavior any time a file is opened and read by Python. One reason is that you might want to read a file in different ways. For example, if you have a _really_ big file—think big data—you might want to read line-by-line rather than the whole thing at once.

Now let's specify which URL we are going to use. Though you might be able to find _Don Quixote_ in the Project Gutenberg files, please type this in so that we are all using the same format (there are multiple `.txt` files on the site, one with utf-8 encoding, another with ascii encoding). We want the utf-8 encoded one. The difference between these is beyond the scope of this tutorial, but you can check out this [introduction to character encoding](https://www.w3.org/International/questions/qa-what-is-encoding) from The World Wide Web Consortium (W3C) if you are interested.

Set the URL we want to a variable:

```python
my_url = "http://www.gutenberg.org/files/996/996-0.txt"
```

We still need to open the file and read the file. You will have to do this with files stored locally as well. (in which case, you would type the path to the file (i.e., `data/texts/mytext.txt`) in place of `my_url`)

```python
file = urlopen(my_url)

raw = file.read()
```

This file is in bytes, so we need to decode it into a string. In the next cell, type:

```python
don = raw.decode()
```

Now let's check on what kind of object we have in the "don" variable. Type:

```python
type(don)
```

This should be a string. Great! We have just read in our first file.

# Make Your Own Corpus (continued)

Now we are going to transform that string into a text that we can perform NLTK functions on. Since we already imported nltk at the beginning of our program, we don't need to import it again, we can just use its functions by specifying `nltk` before the function. The first step is to tokenize the words, transforming the giant string into a list of words. A simple way to do this would be to split on spaces, and that would probably be fine, but we are going to use the NLTK tokenizer to ensure that edge cases are captured (i.e., "don't" is made into 2 words: "do" and "n't"). In the next cell, type:

```python
don_tokens = nltk.word_tokenize(don)
```

You can check out the type of `don_tokens` using the `type()` function to make sure it worked—it should be a list. Let's see how many words there are in our novel:

```python
len(don_tokens)
```

Since this is a list, we can look at any slice of it that we want. Let's inspect the first ten words:

```python
don_tokens[:10]
```

That looks like metadata—not what we want to analyze. We will strip this off before proceeding. If you were doing this to many texts, you would want to use [Regular Expressions](https://regexone.com/). Regular Expressions are an extremely powerful way to match text in a document. However, we are just using this text, so we could either guess, or cut and paste the text into a text reader and identify the position of the first content (i.e., how many words in is the first word). That is the route we are going to take. We found that the content begins at word 320, so let's make a slice of the text from word position 320 to the end.

```python
dq_text = don_tokens[320:]
```

Now print the first 30 words to see if it worked:

```python
print(dq_text[:30]
```

Finally, if we want to use the NLTK specific functions:

- `concordance`
- `similar`
- `dispersion_plot`
- or others from the [NLTK book](https://www.nltk.org/book/)

we would have to make a specific NLTK `Text` object.

```python
dq_nltk_text = nltk.Text(dq_text)
```

And we could check that it worked by running:

```python
type(dq_nltk_text)
```

But if we only need to use the built-in Python functions, we can just stick with our list of words in `dq_text`.

## Challenge

Using the `dq_text` variable:

- Remove the stop words
- Remove punctuation
- Remove capitalization
- Lemmatize the words

If you want to spice your challenge up, do the first three operations _in a single if statement_. Google "python nested if statements" for examples.

## Solution

1. Lowercase, remove punctuation and stop words:

	```python
	dq_clean = []
	for word in dq_text:
    	if word.isalpha():
        	if word.lower() not in stops:
            	dq_clean.append(word.lower())
	print(dq_clean[:50])
	```

2. Lemmatize:

	```python
	from nltk.stem import WordNetLemmatizer
	wordnet_lemmatizer = WordNetLemmatizer()

	dq_lemmatized = []
	for t in dq_clean:
    	dq_lemmatized.append(wordnet_lemmatizer.lemmatize(t))
	```

## Evaluation

Check all sentences below that are correct:

<Quiz>
- `urlopen` can save the contents of a webpage into a variable.*
- To use NLTK functions on a string, we can transform it into a NLTK Text object.*
- NLTK let's you tokenize (split) a giant string into a list of substrings, considering punctuations and edge cases like `don't`.*
</Quiz>

## Keywords

Do you remember the glossary terms from this section?

- [Metadata](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/metadata.md)
- [Regular Expressions](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/regular-expressions.md)

# Part-of-Speech Tagging

_Note that we are going to use the pre-cleaned, `dq_text` object for this section._

POS (Part-of-Speech) tagging is going through a text and identifying which part of speech each word belongs to (i.e., Noun, Verb, or Adjective). Every word belongs to a part of speech, but some words can be confusing.

- Floyd is happy.
- Happy is a state of being.
- Happy has five letters.
- I'm going to Happy Cat tonight.

Therefore, part of speech is as much related to the word itself as its relationship to the words around it. A good part-of-speech tagger takes this into account, but there are some impossible cases as well:

- Wanda was entertaining last night.

Part of Speech tagging can be done very simply: with a very small _tag set_, or in a very complex way: with a much more elaborate tag set. We are going to implement a compromise, and use a neither small nor large tag set, the [Penn Tree Bank POS Tag Set](https://www.ling.upenn.edu/courses/Fall_2003/ling001/penn_treebank_pos.html).

This is the tag set that is pre-loaded into NLTK. When we call the tagger, we expect it to return an object with the word and the tag associated. Because POS tagging is dependent upon the stop words, we have to use a text that includes the stop words. Therefore, we will go back to using the `dq_text` object for this section. Let's try it out. Type:

```python
dq_tagged = nltk.pos_tag(dq_text)
```

Let's inspect what we have:

```python
print(dq_tagged[:10])
```

This is a list of ordered _tuples_. The Python native type _tuple_ is similar to a list, but can't be changed once it is created. They are also denoted with parentheses, rather than square brackets. Each element in the list is a tuple—or a pairing—consisting of `(word, POS-tag)`. This is great, but it is very detailed. I would like to know how many nouns, verbs, and adjectives I have.

First, I'll make an empty dictionary to hold my results. (If you don't know what a dictionary is and how they work, you can check a quick explanation [here](https://realpython.com/python-dicts/).) After that, I will go through this list of tuples and count the number of times each tag appears. Every time I encounter a new tag, I'll add it to a dictionary and then increment by one every time I encounter that tag again. Let's see what that looks like in code:

```python
tag_dict = {}

# For every word/tag pair in my list,
for (word, tag) in dq_tagged:
	if tag in tag_dict:
    	tag_dict[tag]+=1
	else:
    	tag_dict[tag] = 1
```

Now let's see what we got:

```python
tag_dict
```

This would be better with some order to it, but dictionaries are made to be unordered. When we google "sort dictionaries python" we find a solution in our great friend [_Stack Overflow_](https://stackoverflow.com/a/613218). Even though we cannot sort a dictionary, we can get a representation of a dictionary that is sorted.

Don't worry too much about understanding the following code, as it uses functions and methods we have not discussed, and are out of the scope of this course. It is useful to learn to reuse pieces of code even when we don't fully understand them.

Now let's do it and find out what the most common tag is.

```python
tag_dict_sorted = sorted(tag_dict.items(),
   		  reverse=True,
   		  key=lambda kv: kv[1])
```

Now let's check out what we have:

```python
print(tag_dict_sorted)
```

Your result should show that NN is the most common tag. We can look up what NN means in the [Penn Tree Bank](https://www.ling.upenn.edu/courses/Fall_2003/ling001/penn_treebank_pos.html). Looks like NN is a Noun, singular or mass. Great! This information will likely help us with genre classification, or identifying the author of a text, or a variety of other functions.

## Evaluation

Which of the following are correct?

<Quiz>
- POS tagging does not work well with stop words, therefore you should always clean your text from stop words before using it.
- Tuples are like lists, but you can't change their value once created.*
- `nltk.pos_tag` returns tuples of two values, the first being the word, and the second the tag.*
</Quiz>

## Keywords

Do you remember the glossary terms from this section?

- [part-of-speech (POS) tagging](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/part-of-speech.md)
- [Dictionaries](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/dictionaries.md)
- [Tuples](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/tuples.md)

# Theory to Practice

Congratulations! You are done with the Text Analysis workshop!  
 
As you may expect, this course was only the beginning of your journey. NLTK is a vast and ever expanding world. The possibilities are numerous, with exciting new things coming everyday.  
 
Our goal was to show some of those possibilities, and equip you with enough tools/knowledge/skills to be able to keep advancing. In this page we suggest you further readings and other tutorials for which we feel you might be ready. Don't be afraid to try! It is also useful to come back to this workshop with fresh eyes after a while. It will help you solidify some of the knowledge and make some things more clear.  
 
Have a happy journey!

## Review your knowledge: 10 questions from the lessons

__1. Check all sentences below that are correct: (Select all that apply)__

<Quiz>
- urlopen can save the contents of a webpage into a variable.*
- To use NLTK functions on a string, we can transform it into a NLTK Text object.*
- NLTK let’s you tokenize (split) a giant string into a list of substrings, considering punctuations and edge cases like don't.*
</Quiz>

Revisit lesson [Make Your Own Corpus (continued)](/workshops/text-analysis/?page=15) to learn more.

__2. Which of the following are correct? (Select all that apply)__

<Quiz>
- Tuples are like lists, but you can’t change their value once created.*
- nltk.pos_tag returns tuples of two values, the first being the word, and the second the tag.*
- POS tagging does not work well with stop words, therefore you should always clean your text from stop words before using it.
</Quiz>

Revisit lesson [Part-of-Speech Tagging](/workshops/text-analysis/?page=16) to learn more.

__3. Which of the following sentences is correct?__

<Quiz>
- A text is not data in itself, but can produce data if converted into numbers.
- Part-of-Speech (POS) tagging can help identifying verbs, adjectives and nouns in a text.*
- A corpus is any collection of texts, independently of being related to each other or not.
</Quiz>

Revisit lesson [Text as Data](/workshops/text-analysis/?page=2) to learn more.

__4. Which one of the following sentences is correct?__

<Quiz>
- Stop words are useless for text analysis, therefore the first step in any project is to remove them from the text.
- In any type of data analysis, we usually want to cleanse the data in order to prepare it for the analysis. In text analysis, this process is called "text normalization" and can involve tasks such as removing undesired words and punctuation.*
- Textual alterations can potentially change the original intended meaning. Therefore, we must always strive to work with the data exactly as it is in the source.
</Quiz>

Revisit lesson [Cleaning and Normalizing](/workshops/text-analysis/?page=3) to learn more.

__5. Which one of the following sentences is correct?__

<Quiz>
- The similar method brings a list of words that are similar in writing, but not necessarily in meaning, like "whale" and "while".
- Using the `concordance` method with a specific word, such as "whale", returns the words that surround "whale" in different sentences, helping us to get a glimpse of the contexts in which the word "whale" shows up.*
</Quiz>

Revisit lesson [Searching for Words](/workshops/text-analysis/?page=5) to learn more.

__6. Check all sentences below that are correct:__

<Quiz>
- You can get a visual representation of occurrences of a word with the `dispersion_plot` method.*
- The `dispersion_plot` method allows you to input a list of strings, as long as you split them with commas.*
- Contrary to grammar rule, in a list of strings, the commas must come outside of the quotation marks.*
</Quiz>

Revisit lesson [Positioning Words](/workshops/text-analysis/?page=6) to learn more.

__7. Check all sentences below that are correct:__

<Quiz>
- "Whale", "WHALE", and "whale" are all different tokens of the same type.
- The `lower()` method returns the lowercase form of all of the alphabetical characters in a string.*
- The `isalpha()` method transforms integers in alphabetical strings.
- The `append()` method adds an item to the end of the list.*
</Quiz>

Revisit lesson [Types vs Tokens](/workshops/text-analysis/?page=7) to learn more.

__8. Check all sentences below that are correct:__

<Quiz>
- The `len` method returns the length of the input, which can mean different things depending on its type. If it is a string, it will return the number of characters; if it is a list or dictionary, it will return the number of items.*
- The lexical density measures the number of unique words per total word, and it is an objective measure of writing quality.
- Comparing the lexical density between texts of different sizes can give a problematic result. A possible solution is to use list slice and compare parts of both texts of a similar size.*
</Quiz>

Revisit lesson [Lexical Density](/workshops/text-analysis/?page=9) to learn more.

__9. Check all sentences below that are correct:__

<Quiz>
- Stop words are words that usually don't contribute with much semantic content, like prepositions, determiners, etc.*
- To use stop words we need to import them from the nltk corpus, using the following code: `import stopwords from nltk.corpus`
- List comprehensions are faster ways of iterating and creating lists when compared with for loops.*
</Quiz>

Revisit lesson [Data Cleaning: Removing Stop Words](/workshops/text-analysis/?page=10) to learn more.

__10. Check all sentences below that are correct:__

<Quiz>
- Stemming and lemmatizing are different forms of reducing word variations to their roots.*
- `sorted(set(list_of_strings))` returns the unique items of `list_of_strings` in alphabetical order.*
</Quiz>

Revisit lesson [Data Cleaning: Lemmatizing Words](/workshops/text-analysis/?page=11) to learn more.

## Suggested Further Readings

- [A bit more advanced Jupyter Notebook tips and tricks](https://www.dataquest.io/blog/jupyter-notebook-tips-tricks-shortcuts/)
- [The NLTK documentation](https://www.nltk.org/)


## Other Tutorials

- [Sentiment Analysis for Exploratory Data Analysis](https://programminghistorian.org/en/lessons/sentiment-analysis)
- [A collection of Jupyter Notebooks on Mining the Social Web](https://github.com/mikhailklassen/Mining-the-Social-Web-3rd-Edition)
- [Introduction to Stylometry](https://programminghistorian.org/en/lessons/introduction-to-stylometry-with-python)

## Projects or Challenges to Try

- [*Our Machine Learning workshop?*](https://github.com/DHRI-Curriculum/machine-learning)
- [Exercises to practice working with strings](https://www.w3resource.com/python-exercises/string/)
- [Work on your Regular Expressions skills](https://regexone.com/)

## Discussion Questions

- How can your research benefit from text analysis?
- What are the limits of the kind of text analysis we just went throught? What is it good for? What is it not well suited to do?
- What are the potential pitfalls for using massive data?
- How can we use text analysis in teaching?


