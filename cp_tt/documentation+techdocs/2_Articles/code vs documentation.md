
Apply all of our pragmatic principles to documentation as well as to code.
- PRAGMATIC PROGRAMMER IS GOOD FOR THIS AS WELL??

Times you need to present the same documentation in different formats: a printed document, Web pages, online help, or perhaps a slide show. The typical solution relies heavily on cut-and-paste, creating a number of new independent documents from the original. This is a bad idea: a document's presentation should be independent of its content. If you are using a markup system, you have the flexibility to implement as many different output formats as you need. You can choose to have <H1>Chapter Title</H1> generate a new chapter in the report version of the document and title a new slide in the slide show. Technologies such as XSL and CSS can be used to generate multiple output formats from this one markup.

As long as your original markup is rich enough to express all the concepts you need (including hyperlinks), translation to any other publishable form can be both easy and automatic. You can produce online help, published manuals, product highlights for the Web site, and even a tip-a-day calendar, all from the same source-which of course is under source control and is built along with the nightly build.
