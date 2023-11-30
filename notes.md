<b>: The Bring Attention To element
The <b> HTML element is used to draw the reader's attention to the element's contents, which are not otherwise granted special importance. This was formerly known as the Boldface element, and most browsers still draw the text in boldface. However, you should not use <b> for styling text or granting importance. If you wish to create boldface text, you should use the CSS font-weight property. If you wish to indicate an element is of special importance, you should use the <strong> element.

Usage notes
Use the <b> for cases like keywords in a summary, product names in a review, or other spans of text whose typical presentation would be boldfaced (but not including any special importance).
Do not confuse the <b> element with the <strong>, <em>, or <mark> elements. The <strong> element represents text of certain importance, <em> puts some emphasis on the text and the <mark> element represents text of certain relevance. The <b> element doesn't convey such special semantic information; use it only when no others fit.
Similarly, do not mark titles and headings using the <b> element. For this purpose, use the h1 to h6 tags. Further, stylesheets can change the default style of these elements, with the result that they are not necessarily displayed in bold.
It is a good practice to use the class attribute on the <b> element in order to convey additional semantic information as needed (for example <b class="lead"> for the first sentence in a paragraph). This makes it easier to manage multiple use cases of <b> if your stylistic needs change, without the need to change all of its uses in the HTML.
Historically, the <b> element was meant to make text boldface. Styling information has been deprecated since HTML4, so the meaning of the <b> element has been changed.
If there is no semantic purpose to using the <b> element, you should use the CSS font-weight property with the value "bold" instead in order to make text bold.

<em>: The Emphasis element
The <em> HTML element marks text that has stress emphasis. The <em> element can be nested, with each level of nesting indicating a greater degree of emphasis.

Usage notes
The <em> element is for words that have a stressed emphasis compared to surrounding text, which is often limited to a word or words of a sentence and affects the meaning of the sentence itself.

Typically this element is displayed in italic type. However, it should not be used to apply italic styling; use the CSS font-style property for that purpose. Use the <cite> element to mark the title of a work (book, play, song, etc.). Use the <i> element to mark text that is in an alternate tone or mood, which covers many common situations for italics such as scientific names or words in other languages. Use the <strong> element to mark text that has greater importance than surrounding text.

<i> vs. <em>
Some developers may be confused by how multiple elements seemingly produce similar visual results. <em> and <i> are a common example, since they both italicize text. What's the difference? Which should you use?

By default, the visual result is the same. However, the semantic meaning is different. The <em> element represents stress emphasis of its contents, while the <i> element represents text that is set off from the normal prose, such as a foreign word, fictional character thoughts, or when the text refers to the definition of a word instead of representing its semantic meaning. (The title of a work, such as the name of a book or movie, should use <cite>.)

This means the right one to use depends on the situation. Neither is for purely decorative purposes, that's what CSS styling is for.

An example for <em> could be: "Just do it already!", or: "We had to do something about it". A person or software reading the text would pronounce the words in italics with an emphasis, using verbal stress.

An example for <i> could be: "The Queen Mary sailed last night". Here, there is no added emphasis or importance on the word "Queen Mary". It is merely indicated that the object in question is not a queen named Mary, but a ship named Queen Mary. Another example for <i> could be: "The word the is an article".

<i>: The Idiomatic Text element
The <i> HTML element represents a range of text that is set off from the normal text for some reason, such as idiomatic text, technical terms, taxonomical designations, among others. Historically, these have been presented using italicized type, which is the original source of the <i> naming of this element.

Try it

Attributes
This element only includes the global attributes.

Usage notes
Use the <i> element for text that is set off from the normal prose for readability reasons. This would be a range of text with different semantic meaning than the surrounding text. Among the use cases for the <i> element are spans of text representing a different quality or mode of text, such as:
Alternative voice or mood
Taxonomic designations (such as the genus and species "Homo sapiens")
Idiomatic terms from another language (such as "et cetera"); these should include the lang attribute to identify the language
Technical terms
Transliterations
Thoughts (such as "She wondered, What is this writer talking about, anyway?")
Ship or vessel names in Western writing systems (such as "They searched the docks for the Empress of the Galaxy, the ship to which they were assigned.")
In earlier versions of the HTML specification, the <i> element was merely a presentational element used to display text in italics, much like the <b> element was used to display text in bold letters. This is no longer true, as these tags now define semantics rather than typographic appearance. A browser will typically still display the contents of the <i> element in italic type, but is, by definition, no longer required to do so. To display text in italic type, authors should use the CSS font-style property.



<strong>: The Strong Importance element
The <strong> HTML element indicates that its contents have strong importance, seriousness, or urgency. Browsers typically render the contents in bold type.

Try it

Attributes
This element only includes the global attributes.

Usage notes
The <strong> element is for content that is of "strong importance," including things of great seriousness or urgency (such as warnings). This could be a sentence that is of great importance to the whole page, or you could merely try to point out that some words are of greater importance compared to nearby content.

Typically this element is rendered by default using a bold font weight. However, it should not be used to apply bold styling; use the CSS font-weight property for that purpose. Use the <b> element to draw attention to certain text without indicating a higher level of importance. Use the <em> element to mark text that has stress emphasis.

Another accepted use for <strong> is to denote the labels of paragraphs which represent notes or warnings within the text of a page.

<b> vs. <strong>
It is often confusing to new developers why there are so many ways to express the same thing on a rendered website. <b> and <strong> are perhaps one of the most common sources of confusion, causing developers to ask "Should I use <b> or <strong>? Don't they both do the same thing?"

Not exactly. The <strong> element is for content that is of greater importance, while the <b> element is used to draw attention to text without indicating that it's more important.

It may help to realize that both are valid and semantic elements in HTML and that it's a coincidence that they both have the same default styling (boldface) in most browsers (although some older browsers actually underline <strong>). Each element is meant to be used in certain types of scenarios, and if you want to bold text for decoration, you should instead actually use the CSS font-weight property.

The intended meaning or purpose of the enclosed text should be what determines which element you use. Communicating meaning is what semantics are all about.

<em> vs. <strong>
Adding to the confusion is the fact that while HTML 4 defined <strong> as indicating a stronger emphasis, HTML 5 defines <strong> as representing "strong importance for its contents." This is an important distinction to make.

While <em> is used to change the meaning of a sentence as spoken emphasis does ("I love carrots" vs. "I love carrots"), <strong> is used to give portions of a sentence added importance (e.g., "Warning! This is very dangerous.") Both <strong> and <em> can be nested to increase the relative degree of importance or stress emphasis, respectively.