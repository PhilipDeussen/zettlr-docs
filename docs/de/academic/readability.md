# Lesbarkeit

Gutes Schreiben umfasst viele Aspekte. Neben prägnantem Inhalt brauchen deine Texte auch eine abwechslungsreiche Mischung aus kurzen und langen Sätzen. Darüberhinaus solltest du von zu vielen komplexen und komplizierten Wörtern absehen. Ebenso ist es sinnvoll die Absätze kurz zu halten, den Aktiv zu verwenden und die Absätze dementsprechend zu strukturieren.

Seit der Entwicklung von Text hat die menschliche Kreativität viele Tipps zum Schreiben zu Tage gefördert. Während Zettlr dir die perfekte Umgebung zum Schreiben bietet und somit die großartige _Leserlichtkeit_ deines Textes sicherstellt, so musst du dich auch um die Lesbarkeit kümmern. Glücklicherweise hat Zettlr seit der Version `1.4` das richtige Werkzeug für dich: Den **Lesbarkeitsmodus**.

> Bitte bedenke, dass die Punktzahl der Lesbarkeit nur eine von mehreren Maßnahmen ist, um zu bestimmen, wie einfach dein Text zu lesen ist. Diese solltest du nicht allzu ernst nehmen. Falls also der Lesbarkeits-Algorithmus einen Satz mit tiefem Rot markieren sollte heißt das nicht zwangsläufig, dass du den umschreiben solltest. Stattdessen schaue lieber auf den Kontext des Satzes, um die Qualität des Satzes festzustellen, denn dieser wird vom Algorithmus nicht beachtet. **Unsere Empfehlung ist, dass du deinen Text zuerst ohne den Modus schreibst und diesen nur dann für einige Passagen aktiviest, bei denen du das Gefühl hast, dass diese schwierig zu verstehen sein könnten.**

## Was der Lesbarkeitsmodus macht

In der kürzesten Definition ist der Lesbarkeitsmodus ein Syntax-Highlighting-Modus für CodeMirror, der dir eine einfache Punktzahl für jeden deiner Sätze berechnet, um dir einen ersten Eindruck der Lesbarkeit zu geben. Jeder deiner Sätze wird dabei in einer Farbe von grün bis rot markiert, wobei grün hier für eine gute Verständlichkeit des Satzes steht und rot für eine schlechte.

Der Modus kann vier verschiedene Algorithmen verwenden: Die [Dale-Chall-Formel](https://en.wikipedia.org/wiki/Dale%E2%80%93Chall_readability_formula), den [Gunning-Fog Index](https://en.wikipedia.org/wiki/Gunning_fog_index), den [Coleman-Liau-Index](https://en.wikipedia.org/wiki/Coleman%E2%80%93Liau_index), und den [Automated Readability Index](http://www.readabilityformulas.com/automated-readability-index.php). Diese unterscheiden sich in der Annahme, was schwer zu verstehen ist und in der Härte der Bewertung der Sätze. Nicht jeder dieser Indizes ist eine gute Wahl für jede Art von Text. Du solltest genau überlegen, welchen Algorithmus du wählst.

### Die Dale-Chall-Formel

Die Dale-Chall-Formel wurde von Edgar Dale und Jeanne Chall während der frühen Tag der Bildungsforschung erstellt. Diese zielt darauf ab, ein Maßstab für die die Lesbarkeit von Texten für Schulkinder zu sein. Dazu wird eine Liste bestehend aus 3.000 Wörtern benutzt, die für amerikanische Viertklässler leicht zu verstehen sind. Basierend darauf wird eine Punktzahl berechnet, die ungefähr zwischen 0 und 10 liegt und ungefähr die Jahren an Bildung wiederspiegelt, um den Text zu verstehen. Hat eine Satz also eine 10, so brauchst du eine Universitätsabschluss. Ein Wert von 0 würde bedeutet, dass dieser Satz auch von Anfängern verstanden werden könnte.

**Du solltest den Dale-Chall Index verwenden, wenn** du Texte für ein breites Publikum schreibst, da dir der Algorithmus anrechnet, wenn du kurze und prägnante Sätze benutz ohne dich dazu zu drängen Sätze besonders kurz zu machen.

### Der Gunning-Fog Index

Gunning-Fog wurde in der Anfangszeit von Boulevardzeitungen und einfacher Lesbarkeit entwickelt. Im Jahr 1952 suchte Robert Gunning nach einer Möglichkeit, die Bücher und Zeitungen, die er publizierte messbar zu machen. Der Gunning-Fox Index gibt deshalb einen Wert an, der ungefähr mit der Anzahl an Jahren der Schulausbildung korreliert, um den Text zu verstehen. 


Gunning-Fog has been created in the early days of tabloid and easy reading. In 1952, Robert Gunning was searching for a way to make the books and newspapers he was publishing measurable. The Gunning-Fog index therefore returns a score that correlates approximately with the years of formal education needed for a reader to understand a text. Still, being a businessman and therefore interested in a high dispersion of his publications, Gunning's algorithm tends to give high scores even to relatively easy to understand texts. If you cycle through the different algorithms, you will note that Gunning-Fog tends to paint everything ~~black~~ red.

**You should use the Gunning-Fog index, if** you want to write short advertisement texts (e.g. for websites) that cannot count on a basic intrinsic motivation to read.

### Coleman/Liau-index

With the plunge of computer prices, computer-aided statistics became a popular option to process huge amounts of data and spit out a meaningful measurable. The Coleman/Liau-index is from this era and is an algorithm that does not rely on syllable counts or lists with "difficult words". Therefore, the Coleman/Liau-index is extremely accurate in its implementation in Zettlr. As do the others, it gives a score that approximates the years of formal education needed to comprehend a sentence. Additionally, Coleman/Liau gives reasonable results and does not push you to writing short sentences necessarily.

**You should use the Coleman/Liau-index, if** you need an accurate measurement of the readability of any text. It does not go well with one-word-sentences, but will give understandable scores even to harder to understand texts.

### Automated Readability Index (ARI)

The Automated Readability Index follows en suite the Coleman/Liau, as it is a newer formula to calculate readability scores based on simple statistical analysis. It is the most "forgiving" of the algorithms and produces results that do not prompt you to re-write half of your text because of a red highlighting colour.

**You should use the Automated Readability Index, if** you are writing more demanding texts such as academic papers, as it will give lower scores even for some difficult sentences.

### A Note on "Difficult Words"

In its own implementation, Zettlr does not ship with a list of easy to comprehend words that the Dale-Chall requires. Instead, it uses a different approach. The list of easy to understand words differs from time to time and, obviously, from language to language. Therefore, Zettlr takes into account another measurable to determine words deemed difficult: Language variance.

Difficult words for Zettlr are defined as being longer than two times the standard deviation of the average word length. As Coleman and Liau have put it in their 1975 paper _A Computer Readability Formula Designed for Machine Scoring_, the length of words is a much better indicator for the difficulty of words than the number of syllables. Therefore, the algorithm can score sentences in any western script language, not only English. You can look up the algorithm explanation [on our readability feature page](https://zettlr.com/readability).

Additionally, Zettlr makes one more change to the algorithms: While all four algorithms were devised to be applied to full texts, the readability mode will take each sentence, one at a time, and therefore leave out their context. In general this approximates the difficulty of the sentence, but obviously may mark some sentences as green that are difficult to understand in their given context, while it will mark some sentences red that still fit into the given context.
