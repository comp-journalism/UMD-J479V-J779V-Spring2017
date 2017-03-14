# News Bots for Addressing "Fake News"

# Deadline Timeline 
Note: Deadlines are at 10am on the day listed

* Monday, 3/13/17 Project out
* Monday, 4/3/17 Project Proposal DUE (email to nad@umd.edu)
* Monday, 4/24/17 Project Progress Report Presentation DUE (in class presentation)
* Monday, 5/8/17 Final Project Presentation DUE (in class presentation)
* Thursday, 5/11/17 Final Project Report DUE (email to nad@umd.edu)

# Project Description
Your final project will involve designing and developing a News Bot for Twitter that is oriented towards addressing the "fake news" phenomenon in some way. The goal is for you to think through what journalistic aims a news bot could accomplish on Twitter in the "fake news" domain and connect that with what is feasible for you to implement in Python to create a real functioning bot. 

**Project Team**  
You have been assigned a team to work with on the final project. You'll notice that people have different backgrounds on your team. Please contact your team mates ASAP to set up a time to meet and get started on the project. Here are the [teams](https://github.com/comp-journalism/UMD-J479V-J779V-Spring2017/wiki/Final-Project-Teams). If you need contact information for your partner let the professor know (or check any of the emails sent to the whole class). 

**Getting Started**  
For some inspiration you might start by [reading about the development](https://source.opennews.org/en-US/learning/automating-transparency/) of the [@CongressEdits](https://twitter.com/congressedits) bot. You should also review the [News Bots paper](http://www.nickdiakopoulos.com/wp-content/uploads/2011/07/newsbots_final.pdf) by Lokot & Diakopoulos for design ideas. And you can peruse a [news bots list](https://twitter.com/ndiakopoulos/lists/news-bots) to give you a sense of what's been done before. There are a lot of news bots out there and the expectation for this project is that you will exercise your creativity and come up with a new idea that hasn't been done before. Your bot should have some form of editorial intent, it should be a *news* bot! And it should somehow address the "fake news" phenomena, understood broadly. To learn more about the topical area you can start with Claire Wardle's [Fake News. It's Complicated](https://medium.com/1st-draft/fake-news-its-complicated-d0f773766c79#.jdiiucqn6). For other ideas, you might review Eli Pariser's [Design Solutions for Fake News](https://docs.google.com/document/d/1OPghC4ra6QLhaHhW8QvPJRMKGEXT7KaZtG_7s5-UQrw/edit#heading=h.l4uvrs8m75xh)

Initially you could brainstorm some options for bots by considering dimensions of inputs, outputs, algorithms, and intents. Think about what inputs the bot might have (where would you get that data?), what the outputs would be, whether it will be an interactive bot (will it respond to others?), and overall what it should *do* and why. 

Here's an overview of the design space, though you should feel free to step outside this framework to accommodate new ideas you may have:

<img src="https://github.com/comp-journalism/UMD-J479V-J779V-Spring2016/blob/master/Asgn3/newsbot-design.png" width = "600">

Your bot must have some form of data component to it, such as by incorporating open civic, government, or other (social media? news?) data. You can also use any available APIs that provide data, or help you transform data on-the-fly (e.g. by analyzing it, or understanding text such as [Amazon Lex](http://docs.aws.amazon.com/lex/latest/dg/what-is.html)). Finding interesting data and APIs can be very time consuming and you should be sure you understand any limitations of data you've found. You may need to do some exploration and preliminary analysis to even understand what the possibilities and limitations of the data set are and how your treatment of the data could be interesting journalistically. Of course you should be sure that your data is clean enough to be feeding the bot (e.g. if the data you find isn't clean you may need to spend time wrangling it, in which case you might want to [read up](https://infoactive.co/data-design/ch07.html) [more](https://infoactive.co/data-design/ch08.html) on data wrangling). 

Your bot should also have some variability and some form of a "persona" designed into it (e.g. thoughtful handle / name, image, bio, etc). You should consider similar aspects to the first assignment in terms of automated writing and take into account how you can embed more engaging writing into how the bot presents itself. 


**Implementation**  
As you consider what bot you want to create, you should think about the feasibility of the implementation, including:
- Will your bot hit any rate limits: https://dev.twitter.com/rest/public/rate-limiting
- Will your bot run afoul of the Twitter automation guidelines: https://support.twitter.com/articles/76915 (e.g. please make sure you are not spamming other users on Twitter!)
- Will your bot run in a reasonable amount of time
- Will your bot have access to the inputs/data that it needs as it runs

You will implement your bot using a python library called Tweepy. I have created a [tutorial on the library](https://github.com/comp-journalism/UMD-J479V-J779V-Spring2017/blob/master/tutorials/Tweepy-tutorial.ipynb) so that you can familiarize yourself with (some of) the capabilities of the library such as tweeting, searching, or looking at trends. You should also review that tutorial linked there for details on how to create a twitter account, app, and get the necessary keys and tokens to be able to make your bot programmatically tweet. Also, don't be afraid to look at the [Tweepy Documentation](http://tweepy.readthedocs.io/en/v3.5.0/). 

Then, to get started with the implementation download the [skeleton Jupyter Notebook ](https://github.com/comp-journalism/UMD-J479V-J779V-Spring2017/blob/master/Homework/bot-skeleton.ipynb) which includes functions that will greatly simplify your development. You can flesh out the editorial logic of your bot by filling in code in the sections marked as "TODO" in that skeleton notebook. 


**Transparency**  
As part of the final report explained below you should describe what information you can make transparent about how your bot functions. The goal of journalistic transparency is to develop trust with the public by providing information that allows them to assess the validity and reliability of the journalism. 

For an articulation of dimensions you can consider making transparent about your bot please use these articles as guides:
- [Algorithmic Transparency in the News Media](http://www.nickdiakopoulos.com/wp-content/uploads/2016/07/Algorithmic-Transparency-in-the-News-Media-Final.pdf). 
- [Towards Editorial Transparency in Computational Journalism](http://www.nickdiakopoulos.com/wp-content/uploads/2011/07/Towards-Editorial-Transparency-in-Computational-Journalism-Final.pdf)

**Project Proposal**  
Your project proposal will succinctly describe (~500 words) the bot you intend to create. You should have already spent time collecting some data and doing some preliminary exploratory analysis. In the proposal write-up include information about the data you have acquired, what the data describes, where you got it, how you processed or cleaned it, and any limitations you have identified. You should also present your conceptual idea for what the bot will do, and rationalize why doing that thing is interesting from a news and/or journalism perspective with respect to "fake news". What is the intent of the bot? Also look ahead and describe any challenges you foresee in how you will implement your ideas. 

You should email a PDF to nad@umd.edu with a file name of "Final_Project_Proposal_<project_title>.pdf" by the deadline listed above. Be sure to include your team number and names of team members on the PDF. 

**Project Progress Report Presentation**  
In order to help assess the strengths and weaknesses of your project you will have ~20 minutes (15 minutes of presentation and 5 minutes for questions and feedback) to present your project to the class on the date listed above. This presentation will give you a chance to both receive feedback from other class members as well as to offer your own critiques of their work. You should show evidence of substantial progress on implementing your bot and you can use this time to demo what you have, explain the intent of the project, the design process you've used, and what data resources you're using. Make sure to describe and motivate your project for the class, and describe what you have left to work on, as well as if there is anything you need help with.

**Final Project Presentation**  
Final project presentations of 20 minutes (again 15 minutes for presentation and 5 minutes for feedback) will be made in class on the date listed above. This should be the buffed up and polished version of the progress report presentation you gave previously. Make sure to motivate the project, explain the data and APIs you used, how you conceptualized and implemented the bot, and what the news or journalism rationale for the bot is. This will be an open “public” session with invited guests from the college. For all intents and purposes your project should be done by now. 

**Project Report**  
Your project report is due via email to nad@umd.edu as a PDF with file name “Final_Project_\<project_title\>.pdf” by the date listed above. Also include a .zip file of your project's code so that it can be loaded and viewed. In addition to the information that you presented in your final project proposal and final project presentation, please also describe and reflect on your project, in particularly any additional tools you used to implement the project. Why did you decide to design the bot the way you did? What was hard or easy about the project? What would you do differently next time? Importantly, be sure to describe in some detail the work that each team member did and how it was broken out.  

**EXTRA CREDIT**
For upto 2 points of extra credit, put your project on Github with adequate documentation so that others can reuse the bot. Include the link to the public Github repository in your project report. 
