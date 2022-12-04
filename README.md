# STAT 133 - Concepts in Computing with Data

- __Description__: This is an introductory-to-intermediate level course on computational data analysis with an emphasis on four major cornerstones:

    + :1234: common data formats, and principles of data manipulation (e.g. wrangling, reshaping, tidying)
    + :bar_chart: principles of data visualization and their role in data analysis projects
    + :wrench: computational tools to carry out the data analysis cycle, organize your workflow, and create reports (via dynamic documents and web-apps)
    + :computer: basic principles for writing code, and programming concepts (with emphasis on data analysis)

- __Note__: Because Stat 133 is one of the core courses for Statistics majors, the underlying goal is to provide foundations for "computing with data" so that stat majors, as well as other data-dependent majors (e.g. Data Science, Applied Math, CogSci, Economics, etc), have the basic computational skills for subsequent upper division courses (e.g. Stat 150, 151A, 152, 153, 154, 155, 157, 158, 159).

- __Instructor__: Gaston Sanchez

- __Lecture__: 3 days p/week; 1-hour each day

- __Lab__: weekly 2-hour computer lab sessions

- __Assignments__: biweekly HW assignments

- __Exams__: usually one midterm exam, and final test

- __Texts and Notes__:
    + [Breaking the Ice with R](https://www.gastonsanchez.com/R-ice-breaker)
    + [Tidy Hurricanes](https://www.gastonsanchez.com/R-tidy-hurricanes)
    + [R Coding Basics](https://www.gastonsanchez.com/R-coding-basics)
    + [Rolling Dice](https://www.gastonsanchez.com/R-rolling-dice)
    + [Strings](https://www.gastonsanchez.com/R-strings)
    + [Web Technologies in R](https://www.gastonsanchez.com/R-web-technologies)
    + Prof. Sanchez's slides

- __Prerequisites__: This course does not have any prerequisites, although it would be nice if you have taken introductory courses in statistics and programming.


-----


## 1. Introduction, and The Big Picture (part I)

:card_index: __ABOUT__:

We begin with the usual review of the course policies, logistics, overall expectations, topics in a nutshell, etc.

At the conceptual level I describe the main stages of the data analysis cycle. Likewise, I introduce a framework for looking at the notion of "Data" from 3 interconnected perspectives. 

At the computational level you'll get started with R and RStudio.

<br>

:book: __READING__: 

- Slides
- [Breaking the Ice with R](https://www.gastonsanchez.com/R-ice-breaker)

<br>

:pencil2: __TOPICS__:

+ __Introduction__
    - The Data Analysis Cycle (DAC)
    - First contact with R and RStudio


-----


## 2. The Big Picture (part II)

:card_index: __ABOUT__:

We keep discussing some of the Big Picture elements around the notion of Data. The goal is to describe how data can actually be seen from a triangular perspective involving:

- how can we store and format data
- how do we tend to think about data (in a more abstract, conceptual, mathy way)
- how do programs/languages handle data

We continue the discussion about the Big Picture elements. At the lowest logistical level, Data Analysis Projects (DAPs) are essentially made of files and directories. At the practical level, DAPs should (ideally) start with a Research Question. Also, we describe how data can actually be seen from a triangular perspective (i.e. my "3 Views of Data").

Additionally, you'll get introduced to Markdown and its use in dynamic computational documents (e.g. `Rmd` and `qmd` files).


<br>

:book: __READING__: 

- Slides on Big Picture elements

<br>

:pencil2: __TOPICS__:

+ __Data Perspectives__
    - Data from the statistician/data-scientist point of view
    - Data from the digital storage perspective
    - Data from the programming languages perspective


-----


## 3. Tabular Data (part I)

:card_index: __ABOUT__:

One of the main parts of the course involves working data structured in tabular format (i.e. tables), which is the most ubiquitous format in which data is stored, handled, and manipulated. 

While it is true that raw data may not necessarily be organized in a table, sooner or later, you'll be dealing with data in tabular format in most Data Analysis Projects.

Because datasets in tabular format are so omnipresent, we need to talk about how tables are typically stored, learn good principles of data organization, and the so-called notion of "tidy data".


<br>

:book: __READING__: 

- [Tidy Hurricanes](https://www.gastonsanchez.com/R-tidy-hurricanes)

<br>

:pencil2: __TOPICS__:

+ __Data Tables__
    - Manipulation of data-tables using a modern and syntactic approach following the data plying framework provided by the package `"dplyr"` (which is part of `"tidyverse"`).
    - Introduction to the `"ggplot2"` system for making graphics based on data tables (based on Lee Wilkinson's _Grammar of Graphics_).


-----


## 4. Tabular Data (part II), and Datavis (part I)

:card_index: __ABOUT__:

In this week, we go over some important considerations for when data is stored in a spreadsheet. Likewise, we review the role that a Data Dictionary (aka data codebook, metadata) plays in any data analysis project.

In addition, we begin our second major topic of this course: __Data Visualization__. Paraphrasing the old saying "a graphic is worth a thousand numbers". No other means of data representation allows us to understand data better than visual displays. But in order to make good graphics we need to learn the fundamental concepts for data visualization (e.g. Datavis intro, the visual system, visual perception).

<br>

:book: __READING__: 

- [Tidy Hurricanes](https://www.gastonsanchez.com/R-tidy-hurricanes)
- Slides on data visualization

<br>

:pencil2: __TOPICS__:

+ __Data Tables__
    - Considerations when importing (and exporting) tables in R
    - More dplyr functions and the so-called pipes (e.g. with the piper `%>%` operator).


-----


## 5. Data Visualization (part II), and Unix commands (I)

:card_index: __ABOUT__:

In this module we describe the human Visual System. Datavis guru William Cleveland puts it this way:

> "While graphics technology is moving along at a rapid pace, the human visual system has remained the same."

If you want to learn what makes a graphic good, and how to make good graphics, you need to learn about our visual system (formed by our eyes + our brain) and its interaction with light.

At the computational level, we provide an introduction to common basic Unix commands. As we know, Data Analysis Projects (DAPs) are essentially made of files and directories, therefore we need to review some fundamental concepts such as the file-system, the command line interface, and some basic shell commands.

<br>

:book: __READING__: 

- Slides about Data Visualization
- Slides about the Command Line Interface

<br>

:pencil2: __TOPICS__:

+ __Visualization__
    - Visual System
    - Visual Perception


-----


## 6. Data Visualization (part III), and Unix commands (II)

:card_index: __ABOUT__:

As datavis expert Donna Wong acknowledges:

> "With computer technology, anyone can create graphics, but few of us know how to do it well."

With so many chart options, and various software tools, how can you determine what type of graph should you use? To answer this question, we continue reviewing more topics on data visualization, this week focusing on more practical aspects and guidelines for creating effective graphics. Likewise, we keep discussing the use of color, we introduce the famous "data-ink ratio" principle, and we provide a quick review of good and bad published charts.

At the computational level, having covered the basics of command line in the preceding module, you will also learn how to perform basic manipulation of data-table files with some unix filters and pipes.

<br>

:book: __READING__: 

- Slides about Data Visualization
- Slides on Unix filters that get along with files containing data tables

<br>

:pencil2: __TOPICS__:

+ __Visualization__
    - Colors, their RGB model, and their hexadecimal notation
    - HSV and HSL models and their cylindrical spaces
    - Color schemes and color palettes
    - Chart tasting


-----


## 7. R Programming Concepts: Data Types and Objects

:card_index: __ABOUT__:

One of the "3 Data Perspectives" has to do with the way programming languages and computing environments handle data. We describe data types and their implementation in R objects like vectors and arrays. We'll focus on concepts like atomicity, coercion, vectorization, recycling, and subsetting. Likewise, we describe more generic data objects such as lists.

<br>

:book: __READING__: 

- [R Coding Basics](https://www.gastonsanchez.com/R-coding-basics)

<br>

:pencil2: __TOPICS__:

+ __Data objects__
    - Vectors and data types in R
    - Manipulation of basic data objects in R, using bracket notation (e.g. `vec[...]`), 
    - Further review of atomic and non-atomic objects.


-----


## 8. R Programming Concepts: Functions and Conditions

:card_index: __ABOUT__:

You don't need to be an expert programmer to be a data scientist, but learning more about programming allows you to automate common tasks, and solve new problems with greater ease. We'll discuss how to write basic functions, the notion of R expressions, and an introduction to conditionals.

<br>

:book: __READING__: 

- [R Coding Basics](https://www.gastonsanchez.com/R-coding-basics)

<br>

:pencil2: __TOPICS__:

+ __Programming constructs__
    - Writing simple functions in R
    - R compound expressions and the use of curly braces `{...}` 
    - Conditions: `if-else` statments


-----


## 9. R Programming Concepts: Iterations and Loops

:card_index: __ABOUT__:

In addition to writing functions to reduce duplication in your code, you also need to learn about iteration, which helps you when you need to do the same operation several times. Namely, we review control flow structures such as for loops, while loops, repeat loops, and the apply family functions.

<br>

:book: __READING__: 

- [R Coding Basics](https://www.gastonsanchez.com/R-coding-basics)

<br>

:pencil2: __TOPICS__:

+ __Programming constructs__
    - Iterative constructs: `for` loop, `while` loop, `repeat` loop
    - `apply()` family functions
    - More details about functions in R


-----


## 10. R Programming Concepts: Simulations and Shiny Apps

:card_index: __ABOUT__:

We look at some basic problems involving working with random numbers which have many applications in science and computer programming, especially when there are significant uncertainties in a phenomenon of interest. 

Jointly, we discuss _Shiny apps_ which provide a nice "sandbox" to put everything that we've seen so far together (working with data tables, data visualization, R programming concepts, etc) in order to produce a basic web-app for a data-based product. To be more precise, we'll use shiny apps to better visualize the results of some simulations, making it quick and simple to deliver interactive analysis and graphics on any web browser.


<br>

:book: __READING__: 

- [Rolling Dice](https://www.gastonsanchez.com/R-rolling-dice)

<br>

:pencil2: __TOPICS__:

+ __Simulations and Shiny Apps__
    - Simulations with games of chance
    - First contact to shiny apps


-----


## 11. Text Data: Regex (p)art I)

:card_index: __ABOUT__:

Why should you learn about character string manipulation and working with text data? Well, because a considerable amount of information and data is precisely in the form of text. And sooner or later (I would say sooner than later) you will have to deal with some kind of string manipulation for your data analysis. So it’s better to be prepared for such tasks and know how to perform them inside the R environment.

To unleash the power of string manipulation, we need to take things to the next level and learn about 
__Regular Expressions__ (or regex). Namely, regex allows us to describe a certain amount of text called "patterns". We'll describe the basic concepts of regex and the common operations to match text patterns.


<br>

:book: __READING__: 

- Slides

<br>

:pencil2: __TOPICS__:

+ __Intro to Regex__
    - What are regular expressions
    - Literal characters
    - Basic metacharacters: wildcard, escape, and sets


-----


## 12. Text Data: Regex (part II)

:card_index: __ABOUT__:

Computing with Data involves not just computing with numbers but also with text. The fundamental idea is to think of character strings and text as data that can be analyzed. In order do this, we continue discussing some of the basic principles behind regular expressions.


<br>

:book: __READING__: 

- Slides

<br>

:pencil2: __TOPICS__:

+ __More Regex__
    - Character ranges
    - Posix classes
    - Anchors
    - Quantifiers, and intervals
    - Look arounds


-----


## 13. Text Mining

:card_index: __ABOUT__:

Computing with Data involves not just computing with numbers but also with text. The fundamental idea is to think of character strings and text as data that can be analyzed. In order do this, we need to cover some of the basic principles behind Text Mining. Simply put, text mining is the process of distilling actionable insights from text.


<br>

:book: __READING__: 

- [Text Mining with R](https://www.tidytextmining.com/) (by Julia Silge & David Robinson)

<br>

:pencil2: __TOPICS__:

+ __Text Mining Basics__
    - Bag of words, tokens, and corpus
    - Tokenization
    - Word frequency analysis
    - N-grams
    - Sentiment Analysis


-----


## 14. Web Technologies

:card_index: __ABOUT__:

In this module we look at so-called web technologies for computing with data. Time permitting, we'll review HTTP which is the protocol used by computers to communicate and exchange information online. This understanding will allow us to discuss APIs (application Programming Interfaces) which are a common standard to get access to information and data provided by websites (without the need to do web scraping).


<br>

:book: __READING__: 

- [Web Technologies in R](https://www.gastonsanchez.com/R-web-technologies)

<br>

:pencil2: __TOPICS__:

+ __Web Technologies__
    - XML dialects
    - Xpath expressions
    - Webscraping
    - JSON data
    - APIs


