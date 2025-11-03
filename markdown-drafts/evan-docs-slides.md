## Writing Documentation

Evan Williams

29 October 2025

---
<!-- .element: data-auto-animate="true" -->

## Overview 

--
<!-- .element: data-auto-animate="true" -->

## Overview 

- Why?
- Who is it for? <!-- .element: class="fragment" -->
- Types <!-- .element: class="fragment" -->
- Planning <!-- .element: class="fragment" -->
- Writing <!-- .element: class="fragment" -->
- Material for MkDocs <!-- .element: class="fragment" -->
- LLMs <!-- .element: class="fragment" -->

---
<!-- .element: data-auto-animate="true" -->

## Why? 

--
<!-- .element: data-auto-animate="true" -->

## Why? 

We make awesome tools!

Single source of truth <!-- .element: class="fragment" -->

Discoverability <!-- .element: class="fragment"  -->

Note: 
We make awesome tools! Documentation helps everyone use them to the fullest, even future you.

Documentation acts as a single, canonical source of truth.

Related: documentation liberates knowledge from Slack jail. We shouldn't need to search through various channel histories to read about that one specific feature.

---

<!-- .element: data-auto-animate="true" -->

## Who is it for?

--

<!-- .element: data-auto-animate="true" -->

## Who is it for?

Different types of users have different needs

User personas <!-- .element: class="fragment" -->


Note:
- Different types of users will have different needs, and may require more work to understand

- It might help to create user personas based on what you know about your users

This presentation is mostly focusing on documenting our internal libraries. It might not be necessary to make user personas for all of our internal docs, but knowing about them can still help guide your writing 


--

<!-- .element: data-auto-animate="true" -->

## Who is it for?

User personas

<div class="r-stack">

|      Lydia    |              | 
|----------|--------------|
| Developer skill | Advanced |
| Languages | Python, TypeScript |
| Dev Environment | MacOS, Linux |
| Role | Tech Lead |
<!-- .element: class="fragment fade-out" style="color: white "-->



|     Jack     |              | 
|----------|--------------|
| Developer skill | Beginning, intermediate |
| Languages | Python |
| Dev Environment | MacOS, Linux |
| Role | Junior developer |
<!-- .element: class="fragment" style="color: white "-->

</div>

Note:
- A user persona is a semi-fictional character created to represent your ideal reader or readers
- To build a user persona, compile a list of the essential characteristics you’ve learned about your users through your research and discussions with users.


--

<!-- .element: data-auto-animate="true" -->

## Who is it for?

Different types of users have different needs

User personas

Goals and user stories <!-- .element: class="fragment" -->

Note:

--

<!-- .element: data-auto-animate="true" -->

## Who is it for?

Goals and user stories

Write down goals <!-- .element: class="fragment" -->

As a [type of user], I want [activity] so that I can [goal]. <!-- .element: class="fragment" -->

<div class="r-stack fragment">

Lydia: As a tech lead, I want to spin up a new dashboard quickly so that I can show a prototype to a high-value customer. <!-- .element: class="fragment fade-out" -->

Jack: As a junior developer, I want to customize visualizations so that I can implement our newly-created UX style guide. <!-- .element: class="fragment" -->

</div>

Note:
- Goals are the things your users want to do with your software. Goals will focus your efforts on documenting the most relevant information.
- Write the goals down so you can see how well the documentation addresses these goals later.

- User stories typically follow this format.

- Different users may have different goals, even if their roles are similar. Here's an example for Lydia...

- and one for Jack

--

<!-- .element: data-auto-animate="true" -->

## Who is it for?

Different types of users have different needs

User personas

Goals and user stories

Friction log <!-- .element: class="fragment" -->

Note:

--

<!-- .element: data-auto-animate="true" -->

## Who is it for?

Friction log

Try your software as a user would <!-- .element: class="fragment" -->

Log each step sequentially <!-- .element: class="fragment" -->

Expected behavior <-> actual behavior <!-- .element: class="fragment" -->

Note:

- A friction log is a journal in which you 
- try your software as a user would and record your experiences. 

- To record your experience, log each step sequentially,
- noting the behavior you expect and the actual behavior of your software. The bigger the gap between expectation and reality, the bigger the opportunity to improve your docs or software.

--

<!-- .element: data-auto-animate="true" -->

## Who is it for?

Friction log

Goal: start using Corg.ly API <!-- .element: class="fragment" data-fragment-index="0" -->

Task: sign up for a paid Corg.ly account <!-- .element: class="fragment" data-fragment-index="0" -->

Note:

Here's an example friction log from Docs for Developers about getting started using an API from the fictional company Corg.ly, which translates dog barks to human language.

The goal is to start using the API. The first thing to do is sign up for a paid account.

--

<!-- .element: data-auto-animate="true" -->

## Who is it for?

Friction log

- Opened Corg.ly website. <!-- .element: class="fragment" data-fragment-index="1" -->
- Navigated to web form for sign-up. Had to scroll to the bottom of the page. Difficult to find. Maybe add to top of page? <!-- .element: class="fragment" data-fragment-index="1" -->
- Completed form. Put in credit card information. <!-- .element: class="fragment" data-fragment-index="1" -->
- Clicked submit button. Did not receive confirmation it had been submitted. No error generated. <!-- .element: class="fragment" data-fragment-index="1" -->

... <!-- .element: class="fragment" data-fragment-index="1" -->

Note:

Each step is writted down, including feedback if necessary.


--

<!-- .element: data-auto-animate="true" -->

## Validate user understanding

--

<!-- .element: data-auto-animate="true" -->

## Validate user understanding

Analyze support tickets <!-- .element: class="fragment" -->

Slack messages/video chats <!-- .element: class="fragment" -->

Dogfooding <!-- .element: class="fragment" -->

Note:
Support tickets/bug reports are a goldmine for things to fix in software and documentation. This is more relevant for external users.

Questions raised in Slack messages and video chats indicate that documentation doesn't sufficiently cover the topics asked about. Consider answering those questions in the documentation.

Dogfooding: using your own products or services within an organization to test and experience them before wider release. Anything that you, as library authors and maintainers, find confusing will probably confuse others. When you come across something confusing, try to fix it!

---

<!-- .element: data-auto-animate="true" -->

## Types 

--

<!-- .element: data-auto-animate="true" -->

## Types

READMEs

Getting Started <!-- .element: class="fragment" -->

Conceptual <!-- .element: class="fragment" -->

Procedural <!-- .element: class="fragment" -->

Reference <!-- .element: class="fragment" -->

Note:

There are five types of documentation, though two of them have subtypes that I'll discuss.

---

<!-- .element: data-auto-animate="true" -->

## READMEs

--

<!-- .element: data-auto-animate="true" -->

## READMEs

Summarizes a collection of code

Helps users understand why your code exists <!-- .element: class="fragment" -->

What problems does it solve? <!-- .element: class="fragment" -->

Why does it matter? <!-- .element: class="fragment" -->


---

<!-- .element: data-auto-animate="true" -->

## Getting Started

--

<!-- .element: data-auto-animate="true" -->

## Getting Started

Build trust with users

Guide users through first-time user experience <!-- .element: class="fragment" -->

Translate the user's interest into using the library <!-- .element: class="fragment" -->


Note:
Getting started documentation:

is an opportunity to build trust with users that the documentation will be helpful

guides users through first impressions and first-time user experience

should translate the user's interest into actually developing with the library

--

<!-- .element: data-auto-animate="true" -->

## Getting Started

Sections:

- What the library is and core features <!-- .element: class="fragment" -->
- What problem it solves <!-- .element: class="fragment" -->
- Where to go for help <!-- .element: class="fragment" -->
- How to install <!-- .element: class="fragment" -->
- Minimal usage example <!-- .element: class="fragment" -->
- Links to other sections <!-- .element: class="fragment" -->

Note:
Possible sections include


--

<!-- .element: data-background-iframe="https://ai.pydantic.dev" data-background-interactive -->

<!-- .element: data-auto-animate="true" -->

Note:

This is a getting started page from PydanticAI. It has all the essential parts of getting started documentation

---

<!-- .element: data-auto-animate="true" -->

## Conceptual

--

<!-- .element: data-auto-animate="true" -->

## Conceptual

Help users understand the library's concepts and ideas

Describe how it works <!-- .element: class="fragment" -->

Avoid implementation details <!-- .element: class="fragment" -->

Keep pages concise <!-- .element: class="fragment" -->

Limit the number of concepts explained in a single page <!-- .element: class="fragment" -->

--

<!-- .element: data-auto-animate="true" -->

## Conceptual

Sections:

- Brief intro paragraph <!-- .element: class="fragment" -->
- Technical overview <!-- .element: class="fragment" -->
- Subconcepts in their own sections <!-- .element: class="fragment" -->
- Additional resources <!-- .element: class="fragment" -->

Note:

Possible sections include:

- brief intro paragraph: a few sentences (or less) introducing the concept
- technical overview of how it works
- subconcepts in their own sections
- additional resources: tutorials, how-tos, example implementations

TODO: include a page from TanStack Query after this

--

<!-- .element: data-background-iframe="https://tanstack.com/query/latest/docs/framework/react/guides/queries" data-background-interactive -->

<!-- .element: data-auto-animate="true" -->

Note:

The TanStack libraries also have excellent documentation. Here's an example concept page from TanStack Query that introduces a concept, gives a technical overview of how it works, includes subconcepts in their own sections, and has a link for further reading. It's no longer than it needs to be to explain the concept.

---

<!-- .element: data-auto-animate="true" -->

## Procedural

--

<!-- .element: data-auto-animate="true" -->

## Procedural

Tutorial

How-To <!-- .element: class="fragment" -->

--

<!-- .element: data-auto-animate="true" -->

## Procedural

Specific goal, structured steps

One step = one user action <!-- .element: class="fragment" -->

Stand on its own <!-- .element: class="fragment" -->

Limit the number of steps <!-- .element: class="fragment" -->

Avoid long explanations <!-- .element: class="fragment" -->

Note:

- shows readers how to accomplish a specific goal by following a set of structured steps
- a single step should describe a single action a user takes
- make the guide stand on its own as much as possible
- keep the number of steps limited to what's absolutely necessary
    - longer procedures can overwhelm users, and have a higher maintenance burden
- avoid long explanations and lots of prose
- "A good practice is to write procedures that allow a user to see two or more steps on a standard monitor screen. If you find your procedure contains many explanations, consider separating that information out into a conceptual guide. Note that this doesn’t apply to code examples."

--

<!-- .element: data-auto-animate="true" -->

## Tutorial

--

<!-- .element: data-auto-animate="true" -->

## Tutorial

Teach users how to achieve a specific goal

Focus on learning concepts <!-- .element: class="fragment" -->

Help users set up an environment <!-- .element: class="fragment" -->

Test data <!-- .element: class="fragment" -->

10 steps or fewer <!-- .element: class="fragment" -->

Note:

- Good tutorials provide users with an environment they can use for learning
- and may even offer test data or tools to use.

- If your tutorial includes more than ten steps, you’re trying to solve for a use case that’s too complex, or you’re combining too many actions in one document.

--

<!-- .element: data-auto-animate="true" -->

## How-to

--

<!-- .element: data-auto-animate="true" -->

## How-to

Show how to solve business problems

More applied than tutorials <!-- .element: class="fragment" -->

Implement real code <!-- .element: class="fragment" -->

Simplicity and clarity <!-- .element: class="fragment" -->

Reinforce the problem the guide solves <!-- .element: class="fragment" -->

Single page <!-- .element: class="fragment" -->

Note:

-  How-to guides are the core type of procedural content. A how-to guide shows how users can solve actual business problems by performing specific steps with your software.

- A single document that helps them build a solution to their problem. Include prerequisites at the start of your guides.

- While tutorials focus on learning, a how-to guide is based on action with users implementing real code.

- Keep words simple, make actions clear, and continuously reinforce the problem the guide solves. This document should provide a guided experience with helpful guardrails to keep users on track

--

<!-- .element: data-auto-animate="true" -->

## How-to

Sections:

- Intro paragraph <!-- .element: class="fragment" -->
- Prerequisites <!-- .element: class="fragment" -->
- Steps to accomplish the goal <!-- .element: class="fragment" -->
- Next steps/additional resources <!-- .element: class="fragment" -->

Note:

Possible sections include:

- Intro paragraph: frame the problem to be solved
- Prerequisites, linking to other relevant pages if necessary
- Steps to accomplish the goal. Links here might distract users. They may think, If they're linking to a concept, it’s probably important, which could quickly leave them with an overwhelming number of open tabs.
- additional resources: next steps, related concepts. Links go here, instead of in the middle of the guide

---

<!-- .element: data-auto-animate="true" -->

## Reference

--

<!-- .element: data-auto-animate="true" -->

## Reference

API Reference

Glossary <!-- .element: class="fragment" -->

Troubleshooting <!-- .element: class="fragment" -->

Changelog <!-- .element: class="fragment" -->

Code samples <!-- .element: class="fragment" -->

Note:

There are five types

--

<!-- .element: data-auto-animate="true" -->

## Reference

Crucial for developers <!-- .element: class="fragment" -->

Cause and effect / effect and cause <!-- .element: class="fragment" -->

Note:

General notes for reference docs:

- Developers lean heavily on reference documentation while building

- Reference documentation is all about cause and effect: which actions produce which results

- Troubleshooting documentations inverts this: it's about undesired effects and their causes

--

<!-- .element: data-auto-animate="true" -->

## API Reference

--

<!-- .element: data-auto-animate="true" -->

## API Reference

Trusted reference

Autogenerated <!-- .element: class="fragment" -->

Based in the source code <!-- .element: class="fragment" -->

Note:

- API documentation is a trusted reference for your users to start building

- The best way to provide a comprehensive reference of your API is to annotate your code with descriptive comments and autogenerate a reference from the source

- Developers are accustomed to an API reference existing separately from the product and the rest of the documentation. While conceptual and procedural documentation offers more context, an API reference is rooted in the source code

--

<!-- .element: data-background-iframe="https://docs.pydantic.dev/latest/api/base_model/" data-background-interactive -->

<!-- .element: data-auto-animate="true" -->

Note:

Pydantic has excellent documentation. This page is the API documentation for the BaseModel class. Attributes and properties are listed, as are methods and their parameters, return types, and errors raised.

--

<!-- .element: data-auto-animate="true" -->

## Glossary

--

<!-- .element: data-auto-animate="true" -->

## Glossary

Collection of terms and definitions

Note:

Collection of terms and definitions specific to your library, field, or industry. Probably not very relevant for interal documentation

--

<!-- .element: data-auto-animate="true" -->

## Troubleshooting

--

<!-- .element: data-auto-animate="true" -->

## Troubleshooting

Workarounds for known problems

Known limitations/edge cases <!-- .element: class="fragment" -->

Focus on the solution <!-- .element: class="fragment" -->

Note:

- Troubleshooting docs list workaround for known problems. A documented workaround shows users a solution that may not be intuitive, but still gets the job done despite known limitations.

- Known limitations typically include edge cases—actions that you may not have expected or recommended users to attempt. Be clear with your users about which edge cases are unsupported.

- Avoid too much explanation on why the problem happens, focus on the solution instead

--

<!-- .element: data-auto-animate="true" -->

## Troubleshooting

Description of the problem <!-- .element: class="fragment" -->

Steps to fix it <!-- .element: class="fragment" -->

Note:
Be sure to include a description of the problem, and the steps required for the solution


--

<!-- .element: data-auto-animate="true" -->

## Changelog

--

<!-- .element: data-auto-animate="true" -->

## Changelog

Historical record of the project

Chronological <!-- .element: class="fragment" -->

Autogenerated from commit messages <!-- .element: class="fragment" -->


Note:

- provides a historical record of the library's development

- typically in reverse chronological order

- changelogs are best autogenerated from commit messages, with a tool like Commitizen
    - cz can also handle incrementing version numbers
    - encourages writing meaningful commit messages

--

<!-- .element: data-auto-animate="true" -->

## Changelog

Typical sections: <!-- .element: class="fragment" -->

- Bug fixes <!-- .element: class="fragment" -->
- New features <!-- .element: class="fragment" -->
- Breaking changes <!-- .element: class="fragment" -->

Note:

--

<!-- .element: data-auto-animate="true" -->

## Code samples

--

<!-- .element: data-auto-animate="true" -->

## Code samples

Two basic kinds:

- Executable <!-- .element: class="fragment" -->
- Explanatory <!-- .element: class="fragment" -->


Note:
- Executable: code that can run after being copied and pasted
- Explanatory: not runnable, usually an output readers can learn from or compare against

--

<!-- .element: data-auto-animate="true" -->

## Code samples

Principles:

- Explained <!-- .element: class="fragment" -->
- Concise <!-- .element: class="fragment" -->
- Clear <!-- .element: class="fragment" -->

Executable code must also be: <!-- .element: class="fragment" -->

- Usable <!-- .element: class="fragment" -->
- Trustworthy <!-- .element: class="fragment" -->

Note:
- Explained: It’s displayed alongside a written description, whether in the main body of text or in code comments to provide context and explanation where needed.

- Concise: It provides the exact amount of information needed by the reader.

- Clear: It follows conventions a reader would expect of the language the sample is written in.

- Additionally, executable code must be

- Usable (and extensible): It’s clear how the reader uses the sample and where they need to input their own data.

- Trustworthy: It’s pastable, works, and only does what a reader expects.

--

<!-- .element: data-background-iframe="https://docs.pydantic.dev/latest/examples/files/#json-data" data-background-interactive -->

<!-- .element: data-auto-animate="true" -->

Note:

Going back to Pydantic docs, this example page has both explanatory and executable code. Both code samples follow the principles we just discussed

---
<!-- .element: data-auto-animate="true" -->

## Planning

--
<!-- .element: data-auto-animate="true" -->

## Planning

Content outline

- Title <!-- .element: class="fragment" -->
- Content type <!-- .element: class="fragment" -->
- Brief description <!-- .element: class="fragment" -->

Note:

Create a high-level outline of what types of content to include

--

<!-- .element: data-auto-animate="true" -->

## Library documentation

Note:

What should our internal library documentation contain?

--

<!-- .element: data-auto-animate="true" -->

## Library documentation

Getting started

Concepts <!-- .element: class="fragment" -->

Reference <!-- .element: class="fragment" -->

Examples/Tutorials <!-- .element: class="fragment" -->

Note:



--

<!-- .element: data-background-iframe="https://tanstack.com/query/latest/docs/framework/react/overview" data-background-interactive -->

<!-- .element: data-auto-animate="true" -->

Note:

Here's one more look at the docs for TanStack Query. These sections are clearly broken out: getting started, concepts, reference, examples.

---

<!-- .element: data-auto-animate="true" -->

## Writing

--

<!-- .element: data-auto-animate="true" -->

## Writing

Define the title/goal

Create an outline <!-- .element: class="fragment" -->

Consider flow of information <!-- .element: class="fragment" -->

Note:


--

<!-- .element: data-auto-animate="true" -->

## Writing

Consider flow of information

- Meet users needs <!-- .element: class="fragment" -->
- Complete and fully explained <!-- .element: class="fragment" -->
- Makes sense consecutively <!-- .element: class="fragment" -->
- Ask for feedback <!-- .element: class="fragment" -->


Note:

- does the order of information meet your users needs?
- are there any steps you're skipping or that aren't fully explained?
- do they make sense in consecutive order?
- ask for feedback from colleagues (who are also your users!)

--

<!-- .element: data-auto-animate="true" -->

## Writing

Define the title/goal

Create an outline

Consider flow of information

Write a draft <!-- .element: class="fragment" -->

Note:

--

<!-- .element: data-auto-animate="true" -->

## Writing

Write a draft

- Headers <!-- .element: class="fragment" -->
- Paragraphs <!-- .element: class="fragment" -->
- Procedures <!-- .element: class="fragment" -->
- Lists <!-- .element: class="fragment" -->
- Callouts <!-- .element: class="fragment" -->


Note:

Expand on the outline. First add headers, then flesh out the sections with

- paragraphs
- procedures
- lists
- callouts

Don't try to make the first draft perfect. Just start writing! It's easier to edit imperfect writing than it is to look at a blank document and create something perfect the first time

--

<!-- .element: data-auto-animate="true" -->

## Writing

Define the title/goal

Create an outline

Consider flow of information

Write a draft

Edit <!-- .element: class="fragment" -->

Note:


--

<!-- .element: data-auto-animate="true" -->

## Writing

Edit

Don't fix everything at once <!-- .element: class="fragment" -->

Multiple passes, one aspect at a time: <!-- .element: class="fragment" -->

- Technical accuracy <!-- .element: class="fragment" -->
- Completeness <!-- .element: class="fragment" -->
- Structure <!-- .element: class="fragment" -->
- Clarity and brevity <!-- .element: class="fragment" -->

Peer review <!-- .element: class="fragment" -->

Note:

- Don't try to fix everything in one go. 

- Edit for one specific aspect in a single pass:
    - technical accuracy
    - completeness
    - structure
    - clarity and brevity

- Ask for peer review

--

<!-- .element: data-auto-animate="true" -->

## Writing

Advice <!-- .element: class="fragment" -->

Most important info first <!-- .element: class="fragment" -->

No large blocks of text, long documents <!-- .element: class="fragment" -->

Write for skimming: <!-- .element: class="fragment" -->

- Readers come to your documentation looking for information <!-- .element: class="fragment" -->
- Readers read very little of what you write <!-- .element: class="fragment" -->

Note:

- State the most important information first
- Break up large blocks of text
- Break up long documents
- Write for skimming
    - There are two fundamental, paradoxical truths about readers of technical documentation:
        - Readers come to your documentation looking for information.
        - Readers read very little of what you write.

---

<!-- .element: data-auto-animate="true" -->

## Material for MkDocs

--

<!-- .element: data-auto-animate="true" -->

## Material for MkDocs

Lots of projects use it

Markdown: easy to write and maintain <!-- .element: class="fragment" -->

Fast and modern <!-- .element: class="fragment" -->

Great functionality <!-- .element: class="fragment" -->

Note:

- LOTS of projects use it. Many users are already familiar with the interface and features
    - PyPI
    - Pydantic
    - Astral (uv, ruff)
    - FastAPI/Typer/SQLModel
    - Polars
    - LlamaIndex
    - Trivy
- Docs are written in markdown, which is easy to write and maintain
    - The barrier to entry is substantially lower than ReST
    - if we make it easier to write/modify documentation, it's more likely that we will do it
- resulting websites are fast and look modern
- A lot of functionality is baked in, especially if you include plugins
    - snippets from working tests/examples
    - good search
    - language-specific code formatting/highlighting
    - annotations for those code examples
    - admonitions
    - automatically generate API Reference pages from docstrings
    - versioning
    - dark mode

---

<!-- .element: data-auto-animate="true" -->

## LLMs for docs

Note:

LLMs can be quite useful for getting started with writing documentation. Like Daniel mentioned in his talk on how he uses AI, LLMs are great at getting something on the page so you're not staring at a blank screen.

--

<!-- .element: data-auto-animate="true" -->

## LLMs for docs

Create outlines

Create example data <!-- .element: class="fragment" -->

Write minimal examples <!-- .element: class="fragment" -->

Large-scale feedback <!-- .element: class="fragment" -->

Targeted edits <!-- .element: class="fragment" -->

Note:

LLMs can include your entire repo in context and create outlines. It works better if you keep the scope small, like: "write an outline for getting started documentation. include a brief description of the project and installation instructions"

Create realistic example data for procedural documents

Write fully-functioning minimal examples. You'll want to run them to make sure they actually work

Large-scale feedback: check for missing concepts, does the flow work, does the organization make sense, etc

Targeted edits: is this sentence confusing, make this paragraph more concise, etc

---

## Sources

Bhatti, J., Corleissen, Z. S., Lambourne, J., Nunez, D., & Waterhouse, H. (2021). *Docs for Developers: An Engineer’s Field Guide to Technical Writing.* Apress. https://doi.org/10.1007/978-1-4842-7217-6

---

## Questions?