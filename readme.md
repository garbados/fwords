# Function Words

Compilation of function words in different languages, with some access methods in JavaScript / CoffeeScript. As of this writing, only English function words are listed.

While the lists aspire to be exhaustive, language is far too squishy for that. As such, contributions are welcome, encouraged, and occasionally begged for.

## Install

npm install fwords

## Usage

`fwords` is just an object with keys for each supported language (as a two-character code like "en" for English), and therein, keys for each functional category. Specifically:

* `aux`: auxiliary verbs
* `conj`: conjunctions
* `det`: determiners
* `prep`: prepositions
* `pron`: pronouns
* `quant`: quantifiers

In CoffeeScript:

	require('../index') (fwords) -> 
		console.log fwords.en.aux
	> ['be able to', 'can', 'could', 'dare', 'had better', 'have to', 'may', 'might', 'must', 'need to', 'ought', 'ought to', 'shall', 'should', 'used to', 'will', 'would']

## Acknowledgments

Thanks to the efforts of Leah Gilner and Franc Morales at [Sequence Publishing](http://www.sequencepublishing.com) for listing English function words! N.B. I did some minor editing to help machines parse the lists more easily, ex: "1, 2, 3, 4, etc." -> "\d+"