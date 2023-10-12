# Fear of Large Codes

**Hero Image:**

 - <img src='../../images/Blog_2310_BigCode.png' />

#### Contributed by [Francesco Rizzi](https://github.com/fnrizzi)

#### Publication date: October 26, 2023

<!-- Possible deck sentence, if needed
The solution to "the fear of large codes" might start from considering software development as first-class part of research. Or maybe will come from AI?
-->

Recently, while scrolling the notifications on LinkedIn, I came across a [news article](https://oden.utexas.edu/news-and-events/news/Shane-McQuarrie-wins-BGCE-Prize/) from UT Austin.
The article announced an award received by one graduate student in their
prestigious CSEM (Computational Science, Engineering, and Mathematics) program.
While reading the article, the following two statements from his advisor caught my attention:
"...he is not afraid to get his hands dirty with large-scale codes and data sets, ..." and
"...recognizes that software is a part of his research product...".
To a general reader, these words might not sound anything special. To me, however, they highlight
two critical aspects shared by a lot of graduate students, resonating with something I [talked about at SC22](https://github.com/fnrizzi/sc22_bof_slides).
And, more broadly, I would argue they still affect the community involved in scientific research as a whole.
Why? Let me elaborate on them.

### Fear of large codes

In general, a graduate research program is aimed at exploring a very specific scientific problem or question.
What distinguishes it from a lower-level degree is the level of detail expected when exploring this topic -- a Ph.D. program is intended to produce "experts".
In the STEM area, one frequently used approach to attack research problems is through a "proof-of-concept" (POC): this involves a simplified problem that has the advantage of being tractable, while still maintaining "features" of the full problem.
Note that this is not always possible, as simplifications are not always warranted, and some problems must be addressed head-on.
In the field of computational science, a POC is typically
a small, self-contained code written from scratch, usually using a language known to the student, often a "productivity-oriented" language such as Python or Matlab.
With this approach, the student has full control of the code, can work autonomously, and retains ample freedom to change the implementation as needed.
The feeling of being in this kind of situation is one to remember: you feel in control, knowing all the details, the various shortcuts taken in this short program, and any modification is relatively inexpensive to do since the code is small enough that writing and rewriting it is a feasible effort.
As one of my colleagues used to say: "I love when I can prototype ideas and explore them with a Python script of a couple hundred lines!".

However, such a "sandbox reality" has a limited lifetime.
At some point, the POC will no longer be sufficient to make the "deep" progress expected, and problems of greater complexity need to be studied.
This is typically the turning point when larger-scale software comes into the picture, and it also marks the time when many graduate students face the "fear of large codes".
A large code is diametrically opposed to the POC experience: a student now has only partial control; has to work in a team comprising multiple people; has to systematically deal with version control, where even small changes require more work; other developers might change the code "under your feet" requiring the student to constantly update; developers who wrote parts of the code have left and nobody remaining knows the inner workings of some functions; and, finally, the student has to dig deep into the code to understand it because of the lack of documentation.
With all these factors and unknowns playing a role, the fear of facing such a seemingly hard task grows, and with it, the pressure to deliver.

It is natural to ask at this point: why is this fear of large codes so common?
After all, not all students are like the one mentioned at the beginning of this article, praised for his "lack of fear" of getting his hands dirty with large codes.
What if there was a way for *most* students to work on large codes without necessarily needing years of development experience and, most importantly, without being afraid of them?
You may think this a utopian view, but I would argue that such a reality *could* exist.
Imagine a code (started as a small project, but on its way to becoming a large one) developed from the beginning with *accessibility* and *sustainability* in mind: the design is modular and flexible (e.g., the open-closed principle is meticulously met), documentation is complete, and the test suite is well-developed.
If this were the case, I believe that any person with even a minimum set of skills should be able to contribute -- such a code need not be feared, but rather appreciated and liked by users who are comfortable using it in their learning and research.
However, there is a caveat, in that more often than not, the time scale of developing a "pristine" code conflicts with funding and research timelines... which brings me to the following point.

### Software development should be more valued when doing research

Despite software's fundamental role in computational science, some research efforts are still carried out treating software just as a means to an end. 
This is particularly common in projects driven by graduate students.
For example, it is common to see codes developed only for a paper, and then the codes are forgotten, or research proposals written without explicitly mentioning software development as a critical deliverable.
I would argue that this approach must change for software to be sustainable, accessible, and maintainable.
Software development should be a first-class entity in a research effort focusing on computational sciences.
Obviously, reconciling this with the actual research questions to address and balancing it all out, budget-wise, is hard.
But, for the sake of the argument, what could happen if this were the case?
In other words, what could happen if a non-trivial part of a research budget was explicitly dedicated to the software development required?
For graduate students, this would have a key benefit: it would allow students to learn many skills along the way, e.g. team development, testing, and software quality, that would later prove critical for the job market.
After all, many graduate students and junior researchers are the computational scientists of the future.
More broadly, for a research idea or a proposal, I see two critical benefits: (a) solid, robust software would decrease the chances of doing something incorrectly and, therefore, increase the trustworthiness of the results and benefit scientific reproducibility; (b) any research code developed from the ground up with good practices would less likely be forgotten and more likely to become the starting point for a production code.


### What if AI models take over?

Some people believe the rise of AI and large language models (LLMs) will change the way we write and understand software.
In fact, some experts in the field of programming believe that humans writing software, the corresponding documentation, and the whole idea of software maintainability will eventually become obsolete. 
Why? 
Because, assuming a powerful enough AI/LLM system were available, this AI system will write the software, and then its documentation in a matter of minutes.
Furthermore, there will not be any need to maintain this software since the cost of constantly re-writing it from scratch and replacing it will be small -- negligible compared to the cost of humans developing software.
At this point, you might wonder: if all of this is coming in the (near) future, does it mean everything said above fails to hold? 
Will the fear of large codes disappear since AI systems can help us understand code, no matter how complex it is, and contribute to it without the need to have deep software skills?
Will it still be necessary to form good software engineers and pick up these skills early on?

### Author bio

Francesco Rizzi is CTO and principal scientist at NexGen Analytics. Broadly speaking, he works in the field of scientific computing---which he is really passionate about.
He is currently engaged in multiple projects, from performance portability and linear algebra to generic programming, model reduction of large-scale applications, and uncertainty quantification.
Prior to NexGen, he was senior technical staff in the Scalable Modeling & Analysis Systems at Sandia National Labs.
He holds an M.Sc. in Computational Physics from the University of Udine (Italy), and an M.Sc./Ph.D. in Mechanical Engineering from The Johns Hopkins University.

<!---
Publish: yes
Topics: "software engineering"
--->
