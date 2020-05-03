**Prologue**

Who doesn't love to hear that a book you've read is being adapted to the big screen? To judge the casting decisions? The sweet anticipation that accompanies more and more details being leaked by advertisements and star appearances on late-night comedy shows? Being able to interrupt the friend you dragged to the theater with delicious trivia, or by disparaging a deviation from the original plot? For me, it's like an elaborate Christmas present. Something I always wanted, and get to open piece by piece, from a giver who clearly has some kind of multiple-personality disorder. But that person isn't there. I don't have to pretend to like it. I could easily generate a list of complaints, sans guilt. This also makes liking an adaptation feel that much more magnanimous: I, from afar, grant this film my approval. Even though I thoroughly enjoyed the book, maybe even reread the series. And even though I thought Emma Watson was totally wrong for that role, I can admit - to the void - that she ended up being a great ambassador for the franchise, and maybe one or two of the plot deviations weren't all that bad after all. You're welcome, world. Onto Celeste Ng's or Dennis Lehane's latest.

**Database of Books-to-Movies**

This is a database of books that were adapted to film. I built it using APIs from [goodreads](https://www.goodreads.com/api), [omdb](http://www.omdbapi.com/), and [Wikipedia](https://www.mediawiki.org/wiki/API:Main_page). My purpose and hope is that by running some rudimentary anayltics, I'll be able to uncover some commonalities in what makes a good film adaptation, and a poor one.

**PyLadies-DC tutorial**

PyLadies is a kickass organization. I recently took on the role of event organizer for my local, Washington DC based chapter. The jupyter notebook here is for a data mining tutorial that I led 21Apr2020. I'm leaving it up for PyLadies and anyone else to use as a guide for exploring this database. It's nothing fancy.

**Issues**

Please please please let me know if the data is off. I had to do lots of clever things to join all these datasets together in a time-efficient manner. And you know what they say: mo' issues, mo' quality.

**Known Issues**
- Each book resolves to one film. I don't intend to add this complexity any time soon.
- I only used books written in English. I am open to expanding this to foreign-language books that were adapted to english films currently, and foreign language films eventually. (I'm learning to crawl, here)
- The most popular book was chosen. In some cases, this is not the original book. It could be fan fiction. I do hope to get feedback to change this.
- Only movies with an exact name match were chosen (subtitles, or anything following a colon was discarded from the search/original/target title). Books like "Clueless" will not match to Emma by Jane Austen, for example. Also, books like The Lost World by Arthur Conan Doyle will resolve to the second film in the Jurassic Park series, unless manually changed. I do want to correct all of these improper resolutions: please submit an issue if you see this.
- Books that weren't matched to films via automation were dropped. If you notice a book-movie pair that should be included, please submit an issue.

**Future Work**

- Add series-adaptations. This would add a level of complexity to the analysis, but as streaming becomes more popular, more books are being adapted to series formats. Ex: HBO's Game of Thrones, Hulu's Handmaid's Tale, and Netflix's Orange is the New Black.
- Add graphic novels; a larger category than I originally thought. Ex: V for Vendetta, 300, Sin City, Blue is the Warmest Color, and oh yeah, every superhero movie ever. This category is tricky however. The more prolific series, like Batman, don't map cleanly or 1:1 to films. It is also my opinion that these films tends to be highly divergent from their sources (just my opinion!) Regardless, will be interesting to explore and contrast.
