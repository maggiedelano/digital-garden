---
title: "Syntopical Reading in Roam"
toc: true
---

# Overview
In the sixth iteration of Roam Book Club (RBC), I led a group of Roam Book Club members through a syntopical reading of [So Good They Can't Ignore You](https://www.calnewport.com/books/so-good/) by Cal Newport and [Range](https://davidepstein.com/the-range/) by David Epstein. Over the course of seven weeks, we inspected each book, came up with questions, terms, and propositions related to each book, and shared findings with each other during live breakout sessions and in a shared Roam Graph and group zettelkasten called the "Hivemind." In this post I'll introduce syntopical reading, discuss how syntopical reading can be implemented in a tool agnostic way, and then discuss how I set up the implementation of syntopical reading in [[Roam Research]]. I'll also cover how my implementation of syntopical reading can be used to create a group zettelkasten we in RBC are calling the Hivemind. If you'd like to follow along in your own graph, I've [uploaded](https://www.maggiedelano.com/RBC6_shareout.zip) a .zip file with exported pages from the original RBC6 graph.

# Introduction to Syntoptical Reading
There are a lot of reasons why people read books and join book clubs, including for entertainment, to learn something, and to answer your own questions (i.e. research of some kind). Each reason calls for a different approach to reading and writing about the book. Where most book clubs focus on reading for fun or to learn something from the author, this book club focused on a technique called syntopical reading to help us use our two books to answer our own questions. The two books (*So Good They Can't Ignore You* and *Range*) were chosen after I listened to a [podcast](https://www.buzzsprout.com/1121972/6035176) by the two authors where they talk about how many people think their ideas about having a successful career are contradictory, but that they themselves see synergies. It seemed like a great way to try our hand at evaluating each book and using each book to answer our own questions.

The workflow for syntopical reading is described in Chapter 20 of [How To Read A Book](https://en.wikipedia.org/wiki/How_to_Read_a_Book) by Mortimer J. Adler and Charles Van Doren. I adapted this workflow for use in RBC. The steps of syntopical reading included:

- selecting a bibliography (in this case, our two books)
- reading all the texts inspectionally (systematic skimming)
- selecting passages related to topic of interest
- coming to terms with the author
- getting the questions clear
- defining the issues between the passages/authors
- analyzing the resulting discussion 
- generating your own ideas based on what you've learned
- producing output based on your ideas

I recommend reading *How To Read A Book* itself if you want to learn more about each of these steps, as this post is long enough only focusing on implementation. If you are not able to read the book or prefer a quick overview, the Farnam Street Blog also has a pretty good [summary](https://fs.blog/how-to-read-a-book/) of the book.

# Implementing Syntopical Reading (Tool Agnostic)

Syntopical reading can be readily implemented in any personal knowledge management system. This section walks through an overview of how each of the steps were conducted, and in the next one I'll show some specifics of the implementation of syntopical reading in Roam Research.

## Inspectional Reading
When I first heard about inspectional reading I assumed it was just a fancy word for skimming, but it's actually an incredibly powerful tool when used in a systematic way. It can be used to get a quick sense of a text and whether it might be relevant to your research topic. I designed daily writing prompts that guided RBC members through the inspectional reading phase, where members completed the following tasks for each book:
- Looking at the title page, and, if the book has one, at its preface
- Studying the table of contents
- Checking the index 
- Reading the publisher's blurb
- Looking at the chapters that seem to be pivotal to its argument
- Turning the pages, dipping in here and there, reading a paragraph or two, sometimes several pages in sequence, never more than that
- Summarizing each chapter and the book as a whole from this short reading
- Answering what the overall structure of the book is, who the book is for, what the main ideas are, and what might have resonated that might be of future interest

We began with inspecting each book before each person knew exactly what they might be interested in exploring further, which is a little different than how one might implement this for research purposes. We also limited our reading to two books due to time constraints for the book club. However, even when working on one's own there will always be some tension between understanding what one wants to research and needing to read to refine the topic. This is a paradox that the authors of *How To Read A Book* say we will just have to accept and iterate on as we inspect further sources.

## Choosing a Top Level Question
After the inspectional reading was completed, RBC members were encouraged to brainstorm a "top level question" that they were interested in exploring for the rest of the book club. Though the authors of *How To Read A Book* focus on a "topic" for syntopical reading, I thought it made more sense to have a question to focus on as it forces you to refine your thinking a bit.[^3] Top level questions were things that could feasibly be answered (at least in part) by both books. My question, for example, was: "How can I help my students lead successful careers that leverage their general engineering degree and liberal arts education?" This brainstorming doesn't require any particular tool to conduct; you can free-write, list ideas with bullet points, use a mind mapping tool, go for a walk and record your ideas, etc.

[^3]: I think a focus on topic makes sense when you are totally new to an area you are researching, where you might not know enough to even formulate good questions, but the sooner you get to questions the better.

## Selecting Passages, Coming to Terms, Getting the Questions Clear
Once a top level question has been identified, it's time to prepare to read sections of the books in more detail. RBC members used their summarizations from the inspectional reading part, and additional skimming, to try to narrow down a few different passages to do a deeper reading of. They also identified and defined terms from the text or that they already knew that might be relevant. Examples included things like career capital, deliberate practice, and analogical thinking. Finally, each member identified supporting sub-questions, the answers to which would help support their "top-level" question. For example, for the question "How can I help my students lead successful careers that leverage their general engineering degree and liberal arts education?", sub-questions would include things like "What should someone just starting out in their career focus on?" or "What are some advantages of a liberal arts education?" Passages, terms, and questions can all be recorded and organized in any note taking system, but it helps if there's clear ways to follow links between ideas.

## Defining the Issues, Analyzing the Discussion, and Generating Our Own Ideas
After the passages, terms, and questions have been selected, it's time to do a deeper reading of each passage. The first step here is to take notes on the key arguments of each of the chapters, expressed as propositions (i.e. declarative statements or claims). For example, a proposition from Chapter 2 of *Range* might be "Anyone who wants a knowledge-career they love should get broad training." 

Next, after you have a set of propositions, you want to answer your sub-questions using the propositions you've generated from each author. Compare how each author would answer the given sub-question, and then evaluate whether what the different authors are saying is (in)compatible with one another or not. If they disagree, where do they disagree? Using this information, you can generate your own ideas and conclusions, choosing to agree with one or more of the authors or even constructing a synthesis or totally new idea based on what you've read. 

As you answer each sub-question, you will learn more about your topic of interest, and can refine your passages, terms, and questions accordingly as you move toward answering your top-level question.

## Producing Output
At this stage, you will have a set of questions with answers. Depending on what you want to do with the answer to your top-level question, you could stop here. But writing down your ideas and communicating them with someone else is not only an excellent way to challenge your own thinking, it allows you to use what you've learned in a meaningful way. For example, both [myself](https://www.maggiedelano.com/garden/unsolicited-career-advice) and RBC organizer [Kate Foy](https://katefoy.com/keep-your-hook-baited/) decided to write blog posts about our findings.

Going from an outline in Roam/your note taking app to writing in prose also forces you to come up with supporting evidence, examples, and transitions between your ideas. I've found that the process of going from outliner to prose and back to outline can be very helpful in producing this sort of output.[^2]

[^2]: If you are interested in this workflow you can check out a [Loom video](https://www.loom.com/share/bd635c2a394a409a9148812b642beed8) I recorded during the book club that discusses how I go back and forth between an outline in Roam to prose in [Obsidian](https://obsidian.md/) as I write.

# Implementing Syntopical Reading (Roam Workflow)

RBC members implemented the syntopical reading workflow over the course of several weeks using both daily writing prompts and weekly reading/writing assignments. In this section, I'll provide templates you can use in Roam that are lightly adapted from the book club and designed to be used at your own pace in your own graph.

## Inspectional Reading Template

- To conduct an inspectional reading, take the following steps, and answer the questions in the next block:
	- {{[[TODO]]}} Look at the title page, and, if the book has one, at its preface
	- {{[[TODO]]}} Study the table of contents
	- {{[[TODO]]}} Check the index
	- {{[[TODO]]}} Read the epigraph
	- {{[[TODO]]}} Read the publisher's blurb
	- {{[[TODO]]}} Look at the chapters that seem to be pivotal to its argument
	- {{[[TODO]]}} Skim the book from front to back, dipping in here and there, reading a paragraph or two, sometimes several pages in sequence, never more than that
- As you complete the above steps, answer the following questions:
	- {{[[TODO]]}} What is the structure of the book?
	- {{[[TODO]]}} Who do you think the book was written for?
	- {{[[TODO]]}} What are the main ideas covered in the book?
	- {{[[TODO]]}} What resonated with you as you skimmed the book?
	- {{[[TODO]]}} What questions did the book bring up for you?
	- {{[[TODO]]}} What words came up that might be terms?
	- {{[[TODO]]}} (Optional) write a short summary (1-2 sentences) of each chapter of the book

## Organizing Questions, Passages, Terms, and Propositions
After inspectional reading, a top level question is chosen, then passages, terms and sub-questions are selected. Finally, propositions are written up for each reading and then used to answer the sub-questions. Roam can be structured to keep track of all of this like the examples below (the first one is a general skeleton, and the second is one partially populated from my actual notes):  

### Example Template
Templates in Roam are focused around indentation under the main Questions page reference as the parent, followed by top level questions, and then sub-questions, terms, and passages. Sub-questions, terms, and passages all have relevant information nested under them as well. The passages section is used to take notes on the reading, including a Personal respond to reading (like fleeting notes from [How To Take Smart Notes](https://takesmartnotes.com/)), Summary (like literature notes), and Propositions (claims or permanent notes).

- [[Questions]]
	- [insert top level question 1 here]
		- sub-questions
			- [insert subquestions here]
		- [[Terms]]
			- [insert terms and definitions here]
		- [[Passages]]
			- [text]
				- [chapter]
					- [[Personal response to reading]]
						- ...
					- [[Summary]]
						- [[Terms]]
							- ...
					- [[Propositions]]
						- ...
	- (optional, add additional top level questions)
	
### Example Template, Partially Filled In
Here is an example of what a template might look like filled in, with some content omitted due to the levels of indentation and for brevity. You can also see what this looks like in Roam in [this Loom video](https://www.loom.com/share/bd635c2a394a409a9148812b642beed8).

- [[Q/How can I help my students lead successful careers that leverage their general engineering degree and liberal arts education?]]
	- sub-questions:
		- Early careers
			- [[Q/What should someone just starting out in their career focus on?]]
				- [[So Good They Can't Ignore You]]:
					- [[P/Anyone early in their career who wants a successful career should focus on building rare and valuable skills]]
						- how?
							- [[P/anyone who wants a knowledge-career they love should first learn how to find the deep structure of a domain]]
							- [[P/anyone who will have to find the deep structure underlying one domain and apply it to a novel domain should get broad training]]
				- [[Range]]:
					- [[P/Anyone early in their career who wants a successful career should sample widely]]
					- [[P/Anyone early in their career what wants a successful career should focus on skills that can be applied across domains]]
				- Synthesis
					- [[P/Liberal arts students who want a knowledge-career they love should use their four years to sample different domains and build rare and valuable skills across disciplines]]
						- Why should they do that?
							- [[P/anyone who wants a knowledge-career they love will have to function well in a wicked world]]
								- why?
							- [[P/anyone who will have to function well in a wicked world will have to solve novel problems]]
							- [[P/anyone who will have to solve novel problems will have to find the deep structure underlying one domain and apply it to a novel domain]]
								- how to find the deep structure underlying one domain?
									- [[P/Anyone who wants to find the deep structure underlying one domain should learn a field well enough to get to the adjacent possible]]
										- how?
											- [[P/Anyone early in their career who wants a successful career should focus on building rare and valuable skills]]
											- [[P/anyone who should get valuable skills should engage in deliberate practice]]
								- how to apply that training to a novel domain?
									- [[P/anyone who will have to find the deep structure underlying one domain and apply it to a novel domain should get broad training]]
	- [[Terms]]
		- [[T/successful career]]: a career you love
		- [[T/Ikigai]]: "a reason for being" combining what you are good at, what you love, what you can be paid for, and what the world needs
		- [[T/career capital]]: skills that you have that are rare and valuable
		- [[T/wicked environments]]: environments where the "rules of the game" are unclear and incomplete
		- [[T/lateral thinking]]: using existing information in new contexts
		- general engineering degree: a degree that does not involve taking more than 2-4 elective, upper level undergraduate courses in a given sub-discipline of engineering (e.g. mechanical, computer, electrical, chemical)
		- [[T/liberal arts education]]: a degree from a four year institution where the students are required to take almost half of their courses outside their major
	- [[Passages]]
		- [[Range]]
			- [[Chapter 2: How the Wicked World Was Made]]
				- [[Personal response to reading]]
				- [[Summary]]
					- [[Terms]]
						- [[T/the Flynn effect]]
						- [[T/abstraction]]
						- ...
				- [[Propositions]]
					- ...
		- [[So Good They Can't Ignore You]]
			- [[Chapter Five: The Power of Career Capital]]
				- [[Personal response to reading]]
				- [[Summary]]
				- [[Propositions]]
					- ...

### Question Template
Each question page with the `Q/` namespace had an optional template that could be applied that looks like this:
- Tags:: #Questions
	- First added by:: [insert your name here]
	- First added on:: [insert link to today's daily notes page here]
	- Passages::
		- [name 1]
			- [name 1's passages related to this question]
	- Source:: [insert where the question came from (a book, yourself, etc.)]
	- Related:: [insert related terms, questions, or propositions under here]
- Discussion:: (tag w/ date please!)
	- 

### Term Template
Each term page with the `T/` namespace had an optional template that could be applied that looks like this:

- Tags:: #Terms
	- First added by:: [insert your name here]
	- First added on:: [insert link to today's daily notes page here]
	- Definition::
		- [name 1]
			- [name 1's definition]
	- Source:: [insert where the term came from (a book, yourself, etc.)]
	- Related:: [insert related terms, questions, or propositions under here]
- Discussion:: (tag w/ date please!)
	- 

### Proposition Template
Each proposition page with the `P/` namespace had an optional template that could be applied that looks like this:

- Tags:: #Propositions
	- First added by:: [insert your name here]
	- First added on:: [insert link to today's daily notes page here]
	- Source:: [insert where the proposition came from (a book, yourself, etc.)]
	- Related:: [insert related terms, questions, or propositions under here]
- Discussion:: (tag w/ date please!)
	- 

## The Hivemind: Creating A Group Zettelkasten
Part of the beauty of using questions, terms, and propositions with fixed templates is that now a group zettelkasten can be created for everyone in the book club to benefit from the notes of others. RBC members who were interested in participating used the namespaces `T/`, `Q/` or `P/` before pages with terms, questions, or propositions, respectively to indicate the contents (e.g. `[[T/fermi thinking]]`) and that they were willing to share their work with the broader group. Then, I wrote [custom code](https://github.com/maggiedelano/roambookclub/blob/main/getMissingNotes.js) to query for all pages within the appropriate name space and manually populated index pages that organized all the terms, questions, and propositions for easy browsing.[^1]

[^1]: Advanced roam users may be wondering why I used namespaces and custom code for the Hivemind instead of using compound page titles like [[[[QUE]] - What does it mean to live a meaningful life?]]. I did it for several reasons. On the Roam end, namespaces can be removed from the interface for easier reading and are less ugly than compound pages, and they are easier to type. Namespaces are also compatible with export to other tools like [Obsidian](https://obsidian.md/) because all the files in a namespace are exported to a single folder, and Obsidian cannot handle compound page titles. I nest metadata under tags in the template to ensure that said data can be queried if desired.

Each of the pages had a discussion section that members could use to communicate with each other. It was very cool to get to see what everyone's questions were, and how many different terms wound up meaning close to the same thing. The Hivemind is definitely something RBC wants to explore in the future.  

Here's what part of the Question Index page looked like:

![|300](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FRBC-Public-Website%2F7v-mFuFr3c.png?alt=media&token=c4995ec7-f835-4745-b176-70d4ec2ae91d)
# Lessons Learned and Looking Forward
I learned a ton running this book club, including deepening my understanding of *How To Read A Book*, improving my syntopical reading workflow (which has been very helpful in my work and other research endeavors), and learning how to bring people together and how much value there is in learning in community with others. The process of inspectional reading feels like a super power once you start learning to implement it, especially in the context of research projects where the syntopical reading workflow helps you articulate specific questions you have. You can use inspectional reading to quickly hone in on those works and passages that are most relevant to your question, and it helps you from reading endlessly without considering the relevance to your research goals. The Hivemind allows each individual person to focus on questions that interest them, fleshing out terms and propositions as they answer them. Individuals can also easily contribute to the knowledge of others by suggesting passages, terms, or propositions for others' questions. Populating index pages helps identify common themes and connections, and allows for easy "entry points" into the Hivemind. We are continuing to refine the Hivemind in future iterations of RBC, and I'll be excited to see where we run with it.


# Acknowledgements
Thank you to everyone who helped organize and participated in this RBC, including Matt McKinlay, Mike Kramer, Kate Foy, Vincent Tam, Matt Brockwell, Chinarut Ruangchotvit, Naomi Peck, Brian Arrigo, Grigori Milov, Lindsey Johnston, Andy Henson, Beverly Hall, Jason Kleinberg, and many more.

# Footnotes

