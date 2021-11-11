# NLP-Python-Beginners
NLP-Natural Language Processing in Python for Beginners ISBN 9781803249193

## Notes 

### Chapter 1
Nothing of real value, it was an introduction to the instructors
Summary of what NLP and uses


### Chapter 2
Intro into Regular Expressions

### Chapter 3
going over the special characters of regular expressions [$&+,:;=?@#|'<>.-^*()%!]
A lot of regex stuff 

if you are comfortable with regexs and can use google so far nothing special

[0-9] all characters in the set
[^0123] all characters exept for these
[0123^] 0,1,2,3,^ = > ^ hat character only works when in the begin

Basically learn how to use regex, 

### Chapter 4
more regex -> compile regex for string replacement and searching
finditer example

### Chapter 5
more regex -> logical OR symbol '|'

### Chapter 6
string modification
split() -> splits string into list
sub() -> replace the match in the string
subn() -> replace the match and returns new string

### Chapter 7
Text Processing
Corpus -> large body of text
Vocabulary -> unique words in the Corpus
Tokens -> List of words in a document
spaCy Library


### Chapter 8

[Training Data](https://www.kaggle.com/nicapotato/womens-ecommerce-clothing-reviews)


Data Cleaning and preparation for classification,
negative/positive review classification,
One Hot Encoding,
have to review this one again i would say,
i think i missed something.

Not sure how it goes from words to matrix to training??????????
-----------------
So we are getting the words from all the review text
Spliting in to train and test list
populating the vocabulary from the train set
build a matrix from the training list

OMG its taking so long !!!!!!

i done something wrong the x and y labels are the ratings between 1-5 and not the positive and negative

change the numbers to text still only getting positive values on the predicted label axis, the other 2 labels are been populated with zero

|  | Negative | Neutral | Positive |
| ----------- | ----------- | ----------- |
| Negative | 0 | 0 | 0 |
| Neutral | 0 | 0 | 0 |
| Positive | 598 | 756| 4545 |

### Chapter 9
Goes over the problem of Tokenization

->Build the Vocabulary
->word encoding
->train classifier

Byte Pair Encoding 
getting the vocabulary into the lowest subwords used for tokenization


### Chapter 10

Text Pre-Processing
same words represented in different ways can have a impact on your outcome

USA -> U.S.A.
fed -> Fed

case folding issue: US -> us they are not equal

Lemmatization
----------
am, are, is -> be
car, cars, car's, cars' -> car

Stemming
----------
root extract from the word
getting the small meaningfull unit that make up words

Stems: the core meaning
Affixes: parts that adhere to stems

Ational -> ate relational -> relate
ing -> null -> motoring -> motor
sses -> ss grasses -> grass

Sentence Segmantation
----------
knowing when to split a string into sentences
the period is used in abbreviations so can cause problems

### Chapter 11
Spelling correction application

Edit Distance -> counting the min a mount of editing to make word match

pip install editdistance


### Chapter 12