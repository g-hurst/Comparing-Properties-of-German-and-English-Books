## 1 Overview
This project was completed as a use case for the [LexicalRichness](https://github.com/LSYS/LexicalRichness) tool. This project takes seven books listed below in `figure 1` and compares some lexicographical properties between the English and German versions of the text. 

| Book Title                        | Author                 | 
| :---                              |    :----:              | 
| A Christmas Carol                 | Charles Dickens        | 
| Alices Adventures in Wonderland   | Lewis Carroll          | 
| Macbeth                           | Shakespeare            |
| Romeo and Juliet                  | Shakespeare            |
| Oliver Twist                      | Charles Dickens        |
| Peter Pan                         | James Barrie           |
| Treasure Island                   | Robert Louis Stevenson |
<p align=center>
    <em> Figure 1: Books Used In Study </em>
</p>

## 2 Study

This exploration was done to calculate and compare some of the lexicographical properties of text once it has been translated from English to German. Seven unique books were analyzed. <b>The results of this exploration describe the few books that were analyzed, but since the sample size is so small, this can NOT be used to generalize translation of any book from English to German.</b> All of the plots and caluclations made can be found in the notebook `richness study.ipynb` [here](https://github.com/g-hurst/Comparing-Properties-of-German-and-English-Books/blob/main/richness%20study.ipynb). 

### 2.1 Measurement of Words and Terms

The first property of the books explored was the length of the text. This was quantified by getting the total number of words in each book. In addition to this, the number of unique terms in each book was also calculated. The number of words in each book was plotted in Figure 2.1, and the number of terms in each book was plotted in Figure 2.2. In addition to this, the number of words vs number of unique terms for each book was plotted in Figure 2.3. <br>

Looking at Figure 2.1 and 2.2, it can be seen that the English version of the books have more words on average, but the German translations have more unique terms. Figure 2.3 shows that the number of unique terms tends to increase with the word count in each book, and the number of unique terms in the German translations increases more rapidly than their English originals. 

<p align=center>
    <img alt="words" src="https://github.com/g-hurst/Comparing-Properties-of-German-and-English-Books/blob/main/figures/words.png">
    <br>
    <em>Figure 2.1: Bar chart of words in each book</em>
</p>

<p align=center>
    <img alt="terms" src="https://github.com/g-hurst/Comparing-Properties-of-German-and-English-Books/blob/main/figures/terms.png">
    <br>
    <em>Figure 2.2: Bar chart of terms in each book</em>
</p>

<p align=center>
    <img alt="terms" src="https://github.com/g-hurst/Comparing-Properties-of-German-and-English-Books/blob/main/figures/words%20vs%20terms%20scatter.png">
    <br>
    <em>Figure 2.3: Scatter plot of the words vs terms in each book</em>
</p>

### 2.2 Measurement of Maas's Lexical Diversity and Moving Average 

The chosen lexicographical characteristics to analyze were Maas???s measurement of lexical diversity and the average sliding type-token ratio. Maas???s measurement of lexical diversity is a metric calculated with the number of words and terms found within the text and was chosen to represent the readability of the entire text as a whole. The sliding type-token ratio was selected to represent the average readability of any portion of the text. More about the definition of these measurements can be found on the [LexicalRichness github page](https://github.com/LSYS/LexicalRichness). <br>

Figure 2.4 shows Maas???s diversity of each notebook, and it can be observed that the English books have a higher diversity on average. The percent difference between the English and German books was a 15.96% decrease from English to German. The bar chart in Figure 2.5 shows the sliding token-type average of each book and follows the opposite trend seen in Figure 2.4. The percent difference between English and German books was a 7.43% increase from English to German. 

<p align=center>
    <img alt="maas diversity" src="https://github.com/g-hurst/Comparing-Properties-of-German-and-English-Books/blob/main/figures/maas%20diversity.png">
    <br>
    <em>Figure 2.4: Bar chart of Maas's lexical diversity in each book</em>
</p>

<p align=center>
    <img alt="moving avg" src="https://github.com/g-hurst/Comparing-Properties-of-German-and-English-Books/blob/main/figures/moving%20avg.png">
    <br>
    <em>Figure 2.5: Bar chart of sliding ttr average in each book</em>
</p>

## 3 Discussion
<b> Note: Since the sample size for this project was so small, these conclusions are likely unique to this set of books and may not be able to generalize all English to German translation. </b> <br>

One unique aspect found in this study was how while English books had higher overall word counts, the German translation had an higher unique terms. This could indicate that the English to German translation is not always one to one. Maybe a single sentence in English can be translated in multiple sentences in German, and the best translation in German is picked based on the context. With a bit of knowledge about the German language, compound words may also factor into this odd relationship. <br>

The difference in words and terms holds true when the sliding average was taken for each book. Thus, if the reader were to pick one of these translated books, it would be more likely that they would open up to a more lexically diverse section of text. The total diversity of the entire text (measured by Maas???s metric) was higher in every English text. Since teh Maas diversity is inversly related to the lexical richness, the same concludsion can be drawn for the entire text. 
