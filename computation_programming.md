---
title: Computational thinking in programming
teaching: 30
exercises: 10
---

::::::::::::::::::::::::::::::::::::::: objectives

- Understand the importance of decomposition in programming
- Learn how to break down a problem into discrete parts for programming
- Recognize the difference between linear and branching code
- Apply pattern recognition to adapt existing code for new problems

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- Why is decomposition crucial in programming?
- How can we break down a problem like counting words in a text?
- What is the difference between linear and branching code?
- How can pattern recognition help in programming?

::::::::::::::::::::::::::::::::::::::::::::::::::

*Decomposition* is crucial in any kind of problem breakdown, but especially so in programming. The computer must be told **precisely** what to do, and in what order, so problems must be broken down into discrete parts and each section coded appropriately.

#### Defining Inputs and Outputs

Before we can tell the computer *what* to do (the algorithm), we must clarify *what data* we are working with. Every computational problem involves a transformation:

1.  **Input:** What is the starting state? What data do we have? What format is it in?
2.  **Output:** What is the desired goal? What should the result look like?

If we don't define these clearly, we cannot design effective steps to bridge the gap.

Suppose we want to find the ten words most commonly used in a text.

**Input:** A digital text file (e.g., a book chapter).
**Output:** A list of the top 10 most frequent words.

The *process* (or algorithm) is the series of steps that turns that specific Input into that specific Output.

How might we go about that?

#### Linear code

While there are many different ways to do this task, this is one way, where all the commands are run in a linear sequence, e.g.,

![Counting words in a text](fig/count-words.png){alt="counting words in a text" width="60%"}

First we save the file in `.txt` format to eliminate all the "smart" formatting created by programs like Word (as they would otherwise introduce a messy bunch of extraneous characters). Then we progressively eliminate everything from the text that is not a word, i.e. punctuation. 

Converting all the words to lower case means we end up with a single version of each word - not two. This is important because, to a computer, `Word` (starting with an upper case letter) does not equal `word` (starting with a lower case letter) - it treats them as two separate entities. 

By replacing spaces with `new line` characters, each word will end up on its own line, which makes them easy to sort alphabetically and then count.

Each part of the sequence would need to be individually programmed. Fortunately, programmers can adapt code that others have already used to do similar tasks, such as code to identify letter, number or word frequency. Once you are coding, this is where the computational thinking skill of *pattern recognition* comes in - identifying similar code that can be used for or adapted to the specific problem you want to solve. 

--------

#### Branching code

Programming rarely works in such a linear fashion. Code generally includes branching so that different pathways can be taken, depending on whether or not certain conditions are met, e.g., different responses to a `Yes/No` or `True/False` decision, as in the example here.

![Branching code](fig/workflow.png){alt="Branching code" width="90%"}

----------------

:::challenge
## Hiking Preparation Strategy

Our friends have finally made it out of the forest and back to civilisation. Their experience, while unpleasant, has not put them off hiking. Draw a structure diagram of the planning they need to do for next time to avert another disaster.
:::

:::::::::::::::::::::::::::::::::::::::: keypoints

- Decomposition is essential for breaking down problems into discrete parts in programming.
- Computers require precise instructions, and problems must be broken down accordingly.
- Linear code runs commands in a sequence, while branching code allows for different pathways based on conditions.
- Pattern recognition helps programmers adapt existing code for new problems.

::::::::::::::::::::::::::::::::::::::::::::::::::
