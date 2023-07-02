# Introduction  Hello, everybody. Welcome back to the Stack Overflow podcast, a place to talk all
things software and technology. I am Ben Popper, director of content here at Stack Overflow. Join as
I often am by my colleague and collaborator, the editor of our blog, The Illustrious Newsletter
Manager, the experienced technical writer, Ryan Donovan. Oh, thank you. Thank you. Glad to be here.
# AI and ML in Writing and Testing Code  So Ryan, a couple of topics that have come up recently on
the pod and are buzzing around in the discourse for, I think, software developers in general is AI
and ML, the degree to which it can help with writing code or testing code. We recently had the folks
on from Codeium to chat about this. And our guest today has some ideas in similar veins, probably as
his own approach. And I'm excited to hear about it. So from your perspective, Ryan, it's like
writing testing is something no developer really wants to do. And saying I got to this level of test
coverage just so I could pass means you write bad test coverage. And so maybe this is one of those
areas where it's like automation will not eliminate jobs. It'll just make everybody's lives better.
I don't know. What do you think? Yeah, I mean, I remember the days when there was a lot of manual
testing and we had a whole team of QA folks going through the program and clicking buttons. So I
think the less on-tech you can have between the developer and the actual testing, better. It's
repeatable, reliable. All right.  # Introduction of Sayed Hamid  So without further ado, we'd like
to welcome Sayed Hamid, who is the founder and CEO at SOFIE, onto the program. Thank you for having
me, Ben and Ryan. Nice meeting you. Nice to meet you too. So Sayed, for folks who don't know, tell
us a little bit about your background. I know you spent two decades at Microsoft and we're an
engineering manager there. They are maybe the top dog. Again, history has a way of repeating and
rhyming and going in circles when it comes to AI and their partnership with OpenAI and all the
things that they're pushing out at a tremendous pace. Talk to us a little bit about your time there,
what you learned, what it was like working there, and maybe reflect a little on how they ended up in
the pole position. Yeah. So I actually started right out of college at Microsoft back in '97 and
started as a software test engineer and grew through the ranks and part of the eight-member
leadership team that was responsible for all the developer and tester activities within the company
and worked on pretty much six, seven different divisions from back in the day, the MSN, the
narrowband and the very broadband, and the latest as on compilers and languages for Dynamics product
line. And I saw this problem firsthand, how difficult it was to just test and release and do that
every day on a day-on-day basis. And it was frustrating. And I see that as opportunity that, hey,
it's a much bigger problem than just Microsoft alone. It's industry problem. And then finally, I
kind of decided to jump the ship and I started surfing.  # Automating Testing and Scriptless Testing
So tell us a little bit about-- started at the beginning talking about the automating testing. I
know people write, "Scripps, you want to do scriptless testing. How does that work?" So before I go
into that one, I think it's important to kind of look at day in a life of a QA, or how people have
to go and test it. So testing comes a little bit later. But if you look at just the flow, like right
from the CI/CD integration, setting up environment, using different frameworks like APMs, LENIUM,
and different tools, and then creating the automation. And the fourth element is actually executing
at a scale. So all those four components actually creates a lot of friction. So how I see the
problem is not just kind of-- I have a scriptless automation to create automation, but actually
transform the user experience. In this case, the QA right from setting up the environment, running
it at a scale, and doing it today. What people do is, as you know, they write a bunch of scripts
with CI/CD integration. They write a bunch of scripts to set up environment, setting up devices or
environment, and then kind of using the right code to do that. And I think that's where we actually
come into the picture, that we have taken a little bit different approach in the sense that it's
taking a progression of the software testing. And if you also look at kind of the progression, you
have the manual testing, you had the automated testing, and then you have now the no-code testing.
So how we see the future is more of an intelligent testing. And what does an intelligent testing
mean in this case? It's that software's ability to identify itself how to test. We have reached a
point where we think that with the technology, we are able to kind of create tests or to generate
the test and be able to execute it. So that's the kind of at the 10,000-foot level our approaches.
# Self-Healing Code and AI in Software Development  It's really interesting. I had mentioned before
the show that Ryan and I are working on a piece. It's something along the lines of self-healing code
is the future of software development. And so the idea is that there have been things you might add
to a CI/CD pipeline or a GitHub action. Like you said, that you might write some scripts that were
useful for this. But with the entrance now of really powerful AI that is really good at reading and
understanding code, creating its own, and look at maybe a specific code base and understand the
dependencies, the packages, the style, even of the code, it seems like what you're suggesting and
what we've been having really interesting conversations with people about is that as you're writing
the code, or maybe after you've written it while it's still and not in prod, you're able to run
things that say, this is a good test. This looks like an area that needs to be shaped up. Basically,
adding pull requests that you can then look at that would help you automate some of what you were
saying is quite burdensome, that overhead you described of several, several steps before you can
even get to the tester, right? It actually goes even further than that. We obviously have a product
that we announced a month back. I can now actually look at your functional spec or a story in your
Confluence page. And I can actually generate the test cases route out of that. And map it to what I
have tested before. It's amazing what we can accomplish today. Obviously, it's not going to fully
replace people, but it's just as you mentioned, right? It's going to augment. So imagine the world
that as soon as I'm a product manager or a program manager, and if I write my story and system is
smart enough because I have already tested your product or your software, I can actually bring those
things together. And actually, we have been able to demonstrate that and it's been resonating quite
well. And it's like, you know, with that capability, because one of the key capabilities that OpenAI
brings is that I can take any software because at the end of the day, it's a test diagram, right?
Take that one, create your own model, and start mapping it to not only the source code that you
mentioned, hey, for a given product change, tell me what's impacted, but also identify a new feature
and create the test that I can auto create, or we call it the test case generation, and be able to
execute that seamlessly. - Right, well, if you're not saying generative, you have to add generative
so that your company will be highly valued. - That's a good one. We were in this space before this
generative world becomes so common that it is now.  # Challenges in AI-Driven Testing  It's
interesting, writing the test case off of the functional specs. Obviously, somebody can write janky
code to do the thing, and it doesn't do the thing. So if you're just looking at the code, you're
like, well, that did the thing badly like it was supposed to, like the code says it does. Do you
think there will come a time where people are just writing functional specs and the AI does the
rest? - I think we are going that path, but it's still far from it. And what are the challenges with
it? So there are three types of challenges. One you already highlighted that, hey, if somebody
writes a bad code, you can't figure it out. Obviously, it's the same thing is that the functional
spec also has the same problem, right? If somebody writes a bad one, then you're gonna have a bad
outcome, right? But is that one of the things that we see in the, especially in the legacy or older
product where people are going through the digital transformation, a lot of things is not
documented, right? So you get partial information and you may cause more damage than the solution.
And the third problem that we see in this is a lot of dependency on, especially in line-up business
application, there's a lot of dependency on different type of test data that determines how things
move. But regardless, I think we are going in that path. And I do believe that in next couple of
years, there will be a lot more advancement that we can actually think now because right now people
are building all the things on top of OpenAI.  # Non-Deterministic Testing and Mock Data  Yeah,
there was the demo. They haven't released the multimodal model yet, right? But I draw the sketch of
my website on the napkin. I take a picture and it spits out the HTML. So that's like a very toy
example, but like you said, somebody who's way more advanced, who's writing a story or a functional
sort of outline might be able to get something that's a bit more tangible. - Yeah, and I think the
biggest challenge that we'll have, and we are already seeing that, is that how do you get to the
baseline? What I mean by baseline is, suppose you're testing a mobile application, right? So you
have to know the full story, right? All the artifacts of the product, menus, items, transactions and
all those things, right? I think once you get to that baseline or build your model, multimodal, then
actually you can start mapping it to more and more other aspects of it that can help us generate the
test cases and be able to execute that. By the way, related to that is, today we can take any
contextual text, just simply saying, hey, log in using Office 365, do this, and you can actually
convert that into an Appian code out of the box through OpenAI. So there's already a building blocks
of it. So generating a test case is there. The ability to generate code is there, right? So it's the
ability to kind of stitch this together into a seamless experience that will cross-form the QX
period. - Yeah, I had an experience myself being a pretty unskilled coder, trying to do these
things. And exactly like you said, it was the area of stitching together, the front end code with
the backend database with the area I was running the Node.js application. And in my mind, what I
started to realize was the cloud providers that bring all this together. So that as you're talking
to the service, you're saying, like you said, I need a login page here, I need a little bit of OAuth
here, I need a database of this size, I need it to be able to scale, depending on the amount of
demand. And this is how I'd like to go about my front end design. And if those things are natively
integrated, it's clear to the AI how to connect those pieces, it becomes incredibly powerful, 'cause
that's where a lot of the friction is right now. - Exactly, and that's exactly what our approach has
been, right? And to run your question earlier, how does I see kind of the Scripless transforming is
actually that's the next generation of it, right? That Scripless is very focused on creating tests,
it's not about generating, executing, and bringing and reporting everything together. And another
thing that we have seen, which is very powerful, is that ability to understand your quality report
and what do I mean by that? So today, if you're again, as an example, if you're having a mobile
application, you have to have a visual quality separate, you have to have performance data separate,
you have to have a testing metrics separate, right? So now with OpenAI, you can actually just ask
question, hey, I'm releasing an application in this particular country, what do I need to go do it?
Hey, what is step is taking the longest performance and what are the preceding steps? So actually
you can start analyzing these results in a very unique way that gets consumable by anyone in the
team instead of writing custom reports.  # Handling Non-Deterministic Tests and Mock Data  Yeah, we
did a couple of pieces on testing on the blog a while back, talking about how the best tests are
deterministic, right? They have a functional core on a scriptless level. How do you handle those
things that aren't deterministic? Say data from a database or the time or things that will vary
every time? - Yeah, that's one of the things there. We see kind of two types of example in a non-
deterministic test. One is that especially if you have a dynamic content, that you have a dynamic
content, and two, you have a hybrid app or dynamic apps that doesn't give you all the controls and
all those things, right? So one of the things that we have done, companies and different companies
have created is the different modules, right? So now you can actually analyze the image, like for
example, the one-time password configuration, right? So you can actually now what you can do is that
you can do a three-prong approach, meaning you can actually analyze the image and understand what
are the constructs of it, and then you can actually apply certain data sites that are preconfigured.
You can actually generate that on the fly. And the third is actually bring those kind of together in
a non-deterministic way. So I totally agree, it's a challenge. The more and more apps become
dynamic, the more challenging it becomes. But there are a few techniques that people have been using
it to address that.  # Use of Mock Data  Yeah. Do you recommend or do you use mock data or fake data
at all? - As we don't. We actually have our own, actually, patent on it. So we have seen, if you
use, especially in the testing, depending on what testing you are doing, it's if you're doing a unit
testing, the mock should be reasonable. But since we address more of a QA persona, right? We believe
that for those when the mock is actually, can give you a lot of, yeah, things looks good and they
are actually not. So we have actually have kind of not followed the mock.  # Focus on Mobile Testing
I noticed that it seems you focused on mobile. When I go to your website, that seems to be what
you're calling out the most and a lot of big name clients there, sort of talking about the apps that
you've helped them. Is there a reason that you're particularly focused on the mobile space? And I
guess maybe talk to us a little bit after that about like, what is your tech stack? You mentioned
you got started a few years before kind of the recent revolution, but it sounds like you also have
learned how to tap into open AI and things like that as of late. So why mobile and what's the tech
stack behind all this? - Yeah. So what we were seeing is that when we started the company, we had to
focus on certain things, right? We realized that the mobile was a bigger problem. Every company,
especially B2C and others, have to have a mobile presence. And the last reports that I had seen is
that that was growing much faster. So people spend more and more time on mobile, both in the mobile
browser as well as mobile apps. So we support both mobile browser, mobile apps. But also we noticed
is that one of the pain point that people had on the mobile is that in order to test the mobile, you
have to call certain API steps that as Ryan mentioned, retrieve data and perform actions. So we
actually do mobile browser, mobile apps and APIs as part of one suite. And we felt that that's kind
of growing fast and was a more pain point that we wanted to address. So that was an intent for
addressing that.  # Tech Stack  Yeah, I guess, you know, now I'd love to know a little bit about
your tech stack. Like what did you side work with and how has that evolved over the few years you've
been in business, especially as, you know, kind of a seismic change has occurred with the latest
wave of generative AI stuff. - Yeah, so we have kind of a three core components of the product. One
is obviously the presentation layer, then we have all backend and then we have our own machine
learning models, right? So these are kind of the three product category. In the backend pieces, we
actually run Azure. And the reason we use Azure is basically, you know, because we needed the
redundancy across multiple environment. And also we work with enterprise. So, you know, the
compliance and SSO makes it much easier and simpler. And we were also part of the Microsoft startup
ecosystem as well. So we use kind of Azure as our backend, our front end is kind of Node.js and, you
know, the mean stack Angular and other pieces that we use. And then for machine learning, we have
actually our own models that we have created. We have our own models that actually, we use actually
in the machine learning, we use it's like around seven, eight different algorithms from OCR
recognition to building our own models and prediction on what elements are there. So we had a kind
of a combination of the things. And the one thing that we do is also that you can access any device
and write in iOS under 10 seconds from anywhere in the world, with as if you're using it physically.
So that actually requires a lot of optimization. So we have like a whole network infrastructure
layer that actually drives that efficiency.  # Learnings from Microsoft  I joined Microsoft right
out of college, right? So I think I should write a book on failure. Literally, and because a couple
of things that are the foundational thing that I learned, number one is that realization that what
as founder don't know, don't know. So that itself is a very simple word, but it is very significant.
As an example, I'm the lone founder. So when I started it, I had no idea about sales and marketing,
right? Knowing that what you don't know, it's very important so that you surrounded with the people
who can compliment the skills. And you can, as one person or an unfounded, you can't bring
everything to the table, right? And unfortunately, early days of Microsoft, you kind of egoistic to
a certain extent, and that needs to be done. So that's one kind of foundational principle, right?
Two, is that as I spend more time at Microsoft, my understanding of the ecosystem was through
Microsoft Lens, right? And industries far bigger than this Microsoft, right? So that was one big
learning, exactly. It literally took me a year to really kind of figure out, you know, hey, where it
is. And if you know, in 2015, '16, '17 time frame, Microsoft wasn't in the mobile space as well. So
I was doing something that was completely different, right? So like industry problems was a really
bigger learning that I had. And the third one is really it's all about people, right? And that's one
thing that I was really, I looked at Microsoft, that Microsoft was very focused on people
development and others, that you are as successful as your team, right? Micro or macro markets
things aside, but it is a strength of your people that makes or breaks the company. So I think that
are the three, the principle that I now try to go use at managing several hundred people at
Microsoft, and now going back, growing the team from one end to end, and really rolling up the
sleeves and doing it. So it's a different mindset to say the least.  ## Original Transcript  [MUSIC
PLAYING]  Hello, everybody.  Welcome back to the Stack Overflow podcast, a place  to talk all things
software and technology.  I am Ben Popper, director of content here at Stack Overflow.  Join as I
often am by my colleague and collaborator,  the editor of our blog, The Illustrious Newsletter
Manager,  the experienced technical writer, Ryan Donovan.  Oh, thank you.  Thank you.  Glad to be
here.  So Ryan, a couple of topics that have come up recently  on the pod and are buzzing around in
the discourse  for, I think, software developers in general is AI and ML,  the degree to which it
can help with writing code or testing  code.  We recently had the folks on from Codeium to chat
about this.  And our guest today has some ideas in similar veins,  probably as his own approach.
And I'm excited to hear about it.  So from your perspective, Ryan, it's like writing testing  is
something no developer really wants to do.  And saying I got to this level of test coverage just  so
I could pass means you write bad test coverage.  And so maybe this is one of those areas  where it's
like automation will not eliminate jobs.  It'll just make everybody's lives better.  I don't know.
What do you think?  Yeah, I mean, I remember the days  when there was a lot of manual testing  and
we had a whole team of QA folks going through the program  and clicking buttons.  So I think the
less on-tech you can have between the developer  and the actual testing, better.  It's repeatable,
reliable.  All right.  So without further ado, we'd like to welcome Sayed Hamid, who  is the founder
and CEO at SOFIE, onto the program.  Thank you for having me, Ben and Ryan.  Nice meeting you.  Nice
to meet you too.  So Sayed, for folks who don't know,  tell us a little bit about your background.
I know you spent two decades at Microsoft  and we're an engineering manager there.  They are maybe
the top dog.  Again, history has a way of repeating and rhyming  and going in circles when it comes
to AI  and their partnership with OpenAI and all the things  that they're pushing out at a
tremendous pace.  Talk to us a little bit about your time there, what you learned,  what it was like
working there, and maybe reflect a little  on how they ended up in the pole position.  Yeah.  So I
actually started right out of college at Microsoft back  in '97 and started as a software test
engineer  and grew through the ranks and part of the eight-member leadership  team that was
responsible for all the developer and tester  activities within the company and worked on pretty
much six,  seven different divisions from back in the day, the MSN,  the narrowband and the very
broadband,  and the latest as on compilers and languages  for Dynamics product line.  And I saw this
problem firsthand,  how difficult it was to just test and release and do that  every day on a day-
on-day basis.  And it was frustrating.  And I see that as opportunity that, hey,  it's a much bigger
problem than just Microsoft alone.  It's industry problem.  And then finally, I kind of decided to
jump the ship  and I started surfing.  So tell us a little bit about--  started at the beginning
talking about the automating testing.  I know people write, "Scripps, you  want to do scriptless
testing.  How does that work?"  So before I go into that one, I think  it's important to kind of
look at day in a life of a QA,  or how people have to go and test it.  So testing comes a little bit
later.  But if you look at just the flow,  like right from the CI/CD integration,  setting up
environment, using different frameworks  like APMs, LENIUM, and different tools,  and then creating
the automation.  And the fourth element is actually  executing at a scale.  So all those four
components actually  creates a lot of friction.  So how I see the problem is not just kind of--  I
have a scriptless automation to create automation,  but actually transform the user experience.  In
this case, the QA right from setting up the environment,  running it at a scale, and doing it today.
What people do is, as you know, they  write a bunch of scripts with CI/CD integration.  They write a
bunch of scripts to set up  environment, setting up devices or environment,  and then kind of using
the right code to do that.  And I think that's where we actually come into the picture,  that we
have taken a little bit different approach in the sense  that it's taking a progression of the
software testing.  And if you also look at kind of the progression,  you have the manual testing,
you had the automated testing,  and then you have now the no-code testing.  So how we see the future
is more of an intelligent testing.  And what does an intelligent testing mean in this case?  It's
that software's ability to identify itself how to test.  We have reached a point where we think that
with the technology,  we are able to kind of create tests or to generate the test  and be able to
execute it.  So that's the kind of at the 10,000-foot level  our approaches.  It's really
interesting.  I had mentioned before the show that Ryan and I  are working on a piece.  It's
something along the lines of self-healing code  is the future of software development.  And so the
idea is that there have been things you might add  to a CI/CD pipeline or a GitHub action.  Like you
said, that you might write some scripts that  were useful for this.  But with the entrance now of
really powerful AI  that is really good at reading and understanding code,  creating its own, and
look at maybe a specific code base  and understand the dependencies, the packages, the style,  even
of the code, it seems like what you're suggesting  and what we've been having really interesting
conversations  with people about is that as you're writing the code,  or maybe after you've written
it while it's still and not  in prod, you're able to run things that say,  this is a good test.
This looks like an area that needs to be shaped up.  Basically, adding pull requests that you can
then look at  that would help you automate some of what you were saying  is quite burdensome, that
overhead  you described of several, several steps  before you can even get to the tester, right?  It
actually goes even further than that.  We obviously have a product that we announced a month back.
I can now actually look at your functional spec or a story  in your Confluence page.  And I can
actually generate the test cases route out of that.  And map it to what I have tested before.  It's
amazing what we can accomplish today.  Obviously, it's not going to fully replace people,  but it's
just as you mentioned, right?  It's going to augment.  So imagine the world that as soon as I'm a
product manager  or a program manager, and if I write my story  and system is smart enough because I
have already  tested your product or your software,  I can actually bring those things together.
And actually, we have been able to demonstrate that  and it's been resonating quite well.  And it's
like, you know, with that capability,  because one of the key capabilities that OpenAI brings  is
that I can take any software because at the end of the day,  it's a test diagram, right?  Take that
one, create your own model,  and start mapping it to not only the source code  that you mentioned,
hey, for a given product change,  tell me what's impacted, but also identify a new feature  and
create the test that I can auto create,  or we call it the test case generation,  and be able to
execute that seamlessly.  - Right, well, if you're not saying generative,  you have to add
generative so that your company  will be highly valued.  - That's a good one.  We were in this space
before this generative world  becomes so common that it is now.  - It's interesting, writing the
test case  off of the functional specs.  Obviously, somebody can write janky code to do the thing,
and it doesn't do the thing.  So if you're just looking at the code,  you're like, well, that did
the thing badly  like it was supposed to, like the code says it does.  Do you think there will come
a time  where people are just writing functional specs  and the AI does the rest?  - I think we are
going that path,  but it's still far from it.  And what are the challenges with it?  So there are
three types of challenges.  One you already highlighted that, hey,  if somebody writes a bad code,
you can't figure it out.  Obviously, it's the same thing is that  the functional spec also has the
same problem, right?  If somebody writes a bad one,  then you're gonna have a bad outcome, right?
But is that one of the things that we see in the,  especially in the legacy or older product  where
people are going through the digital transformation,  a lot of things is not documented, right?  So
you get partial information  and you may cause more damage than the solution.  And the third problem
that we see in this  is a lot of dependency on,  especially in line-up business application,
there's a lot of dependency on different type of test data  that determines how things move.  But
regardless, I think we are going in that path.  And I do believe that in next couple of years,
there will be a lot more advancement  that we can actually think now  because right now people are
building  all the things on top of OpenAI.  - Yeah, there was the demo.  They haven't released the
multimodal model yet, right?  But I draw the sketch of my website on the napkin.  I take a picture
and it spits out the HTML.  So that's like a very toy example,  but like you said, somebody who's
way more advanced,  who's writing a story or a functional sort of outline  might be able to get
something  that's a bit more tangible.  - Yeah, and I think the biggest challenge that we'll have,
and we are already seeing that,  is that how do you get to the baseline?  What I mean by baseline
is,  suppose you're testing a mobile application, right?  So you have to know the full story, right?
All the artifacts of the product, menus, items,  transactions and all those things, right?  I think
once you get to that baseline  or build your model, multimodal,  then actually you can start mapping
it  to more and more other aspects of it  that can help us generate the test cases  and be able to
execute that.  By the way, related to that is,  today we can take any contextual text,  just simply
saying, hey,  log in using Office 365, do this,  and you can actually convert that  into an Appian
code out of the box through OpenAI.  So there's already a building blocks of it.  So generating a
test case is there.  The ability to generate code is there, right?  So it's the ability to kind of
stitch this together  into a seamless experience  that will cross-form the QX period.  - Yeah, I had
an experience myself  being a pretty unskilled coder,  trying to do these things.  And exactly like
you said,  it was the area of stitching together,  the front end code with the backend database
with the area I was running the Node.js application.  And in my mind, what I started to realize was
the cloud providers that bring all this together.  So that as you're talking to the service,  you're
saying, like you said, I need a login page here,  I need a little bit of OAuth here,  I need a
database of this size,  I need it to be able to scale,  depending on the amount of demand.  And this
is how I'd like to go about my front end design.  And if those things are natively integrated,  it's
clear to the AI how to connect those pieces,  it becomes incredibly powerful,  'cause that's where a
lot of the friction is right now.  - Exactly, and that's exactly what our approach has been,  right?
And to run your question earlier,  how does I see kind of the Scripless transforming  is actually
that's the next generation of it, right?  That Scripless is very focused on creating tests,  it's
not about generating, executing,  and bringing and reporting everything together.  And another thing
that we have seen,  which is very powerful,  is that ability to understand your quality report  and
what do I mean by that?  So today, if you're again, as an example,  if you're having a mobile
application,  you have to have a visual quality separate,  you have to have performance data
separate,  you have to have a testing metrics separate, right?  So now with OpenAI, you can actually
just ask question,  hey, I'm releasing an application  in this particular country, what do I need to
go do it?  Hey, what is step is taking the longest performance  and what are the preceding steps?
So actually you can start analyzing these results  in a very unique way that gets consumable  by
anyone in the team instead of writing custom reports.  - Yeah, we did a couple of pieces on testing
on the blog a while back,  talking about how the best tests are deterministic, right?  They have a
functional core on a scriptless level.  How do you handle those things that aren't deterministic?
Say data from a database or the time  or things that will vary every time?  - Yeah, that's one of
the things there.  We see kind of two types of example  in a non-deterministic test.  One is that
especially if you have a dynamic content,  that you have a dynamic content,  and two, you have a
hybrid app or dynamic apps  that doesn't give you all the controls  and all those things, right?  So
one of the things that we have done,  companies and different companies have created  is the
different modules, right?  So now you can actually analyze the image,  like for example, the one-
time password configuration, right?  So you can actually now what you can do  is that you can do a
three-prong approach,  meaning you can actually analyze the image  and understand what are the
constructs of it,  and then you can actually apply certain data sites  that are preconfigured.  You
can actually generate that on the fly.  And the third is actually bring those kind of together  in a
non-deterministic way.  So I totally agree, it's a challenge.  The more and more apps become
dynamic,  the more challenging it becomes.  But there are a few techniques  that people have been
using it to address that.  - Yeah.  Do you recommend or do you use mock data or fake data at all?  -
As we don't.  We actually have our own, actually, patent on it.  So we have seen, if you use,
especially in the testing,  depending on what testing you are doing,  it's if you're doing a unit
testing,  the mock should be reasonable.  But since we address more of a QA persona, right?  We
believe that for those when the mock is actually,  can give you a lot of, yeah, things looks good
and they are actually not.  So we have actually have kind of not followed the mock.  - I noticed
that it seems you focused on mobile.  When I go to your website,  that seems to be what you're
calling out the most  and a lot of big name clients there,  sort of talking about the apps that
you've helped them.  Is there a reason that you're particularly focused  on the mobile space?  And I
guess maybe talk to us a little bit after that  about like, what is your tech stack?  You mentioned
you got started a few years before  kind of the recent revolution,  but it sounds like you also have
learned how to tap into  open AI and things like that as of late.  So why mobile and what's the tech
stack behind all this?  - Yeah.  So what we were seeing is that when we started the company,  we had
to focus on certain things, right?  We realized that the mobile was a bigger problem.  Every
company, especially B2C and others,  have to have a mobile presence.  And the last reports that I
had seen is that  that was growing much faster.  So people spend more and more time on mobile,  both
in the mobile browser as well as mobile apps.  So we support both mobile browser, mobile apps.  But
also we noticed is that one of the pain point  that people had on the mobile is that  in order to
test the mobile,  you have to call certain API steps  that as Ryan mentioned, retrieve data and
perform actions.  So we actually do mobile browser, mobile apps  and APIs as part of one suite.  And
we felt that that's kind of growing fast  and was a more pain point that we wanted to address.  So
that was an intent for addressing that.  - Yeah, I guess, you know,  now I'd love to know a little
bit about your tech stack.  Like what did you side work with  and how has that evolved over the few
years  you've been in business, especially as, you know,  kind of a seismic change has occurred
with the latest wave of generative AI stuff.  - Yeah, so we have kind of a three core components  of
the product.  One is obviously the presentation layer,  then we have all backend  and then we have
our own machine learning models, right?  So these are kind of the three product category.  In the
backend pieces, we actually run Azure.  And the reason we use Azure is basically, you know,  because
we needed the redundancy across multiple environment.  And also we work with enterprise.  So, you
know, the compliance and SSO makes it much easier  and simpler.  And we were also part of the
Microsoft startup ecosystem  as well.  So we use kind of Azure as our backend,  our front end is
kind of Node.js and, you know,  the mean stack Angular and other pieces that we use.  And then for
machine learning,  we have actually our own models that we have created.  We have our own models
that actually,  we use actually in the machine learning,  we use it's like around seven, eight
different algorithms  from OCR recognition to building our own models  and prediction on what
elements are there.  So we had a kind of a combination of the things.  And the one thing that we do
is also that you can access  any device and write in iOS under 10 seconds  from anywhere in the
world,  with as if you're using it physically.  So that actually requires a lot of optimization.  So
we have like a whole network infrastructure layer  that actually drives that efficiency.  - Yeah, I
remember a friend of mine  was running his own mobile game company  and he would go to conferences
just to pick up test devices.  - Yep.  Yeah.  So as you will allow testing sort of  actually or
virtually on devices.  - Actually, we have actual real devices  that's in our data center in
Seattle.  And one of the things that we do very uniquely,  and that's what we were talking about,
how we can read our model is actually  when you go to any device and start playing  with the
application under the hood, we are training it.  So where you're clicking on it, what you're doing
it.  So that's all feeds into our machine learning system  and said, okay, where the users are doing
it.  And that's how we are able to kind of do it  with high accuracy and run the generate the test
case  and be able to run that faster.  - Interesting.  So you mentioned that you had worked at
Microsoft  and that this startup kind of came  through the Microsoft ecosystem.  Tell us a little
bit of, yeah,  I guess were there things you learned there,  principles for the way you organize
teams  or think about software engineering  or something that came out of maybe  having a sort of
pseudo partnership with them  is going through their accelerator  that have played a big role in
what Sophie is.  - I joined Microsoft right out of college, right?  So I think I should write a book
on failure.  Literally, and because a couple of things  that are the foundational thing that I
learned,  number one is that realization  that what as founder don't know, don't know.  So that
itself is a very simple word,  but it is very significant.  As an example, I'm the lone founder.  So
when I started it, I had no idea about sales  and marketing, right?  Knowing that what you don't
know,  it's very important so that you surrounded  with the people who can compliment the skills.
And you can, as one person or an unfounded,  you can't bring everything to the table, right?  And
unfortunately, early days of Microsoft,  you kind of egoistic to a certain extent,  and that needs
to be done.  So that's one kind of foundational principle, right?  Two, is that as I spend more time
at Microsoft,  my understanding of the ecosystem  was through Microsoft Lens, right?  And industries
far bigger than this Microsoft, right?  So that was one big learning, exactly.  It literally took me
a year to really kind of figure out,  you know, hey, where it is.  And if you know, in 2015, '16,
'17 time frame,  Microsoft wasn't in the mobile space as well.  So I was doing something that was
completely different, right?  So like industry problems was a really bigger learning  that I had.
And the third one is really it's all about people, right?  And that's one thing that I was really,
I looked at Microsoft,  that Microsoft was very focused on people development  and others, that you
are as successful as your team, right?  Micro or macro markets things aside,  but it is a strength
of your people  that makes or breaks the company.  So I think that are the three,  the principle
that I now try to go use  at managing several hundred people at Microsoft,  and now going back,
growing the team from one end to end,  and really rolling up the sleeves and doing it.  So it's a
different mindset to say the least.  - Cool.  (upbeat music)  - All right, everybody, it is that
time of the show.  Let's shout out a Stack Overflow user  who came on to the site,  shared a little
bit of knowledge  and helped to rescue a question  from the Dust bit of history.  A lifeboat badge
awarded to Todd Jacobs  for coming to rescue a question  and providing a great answer.  How to check
whether a string is an integer in Ruby.  Todd has got you covered and helped over 17,000 people.  So
we appreciate it, Todd.  I am Ben Popper.  I am the director of content here at Stack Overflow.
Find me on Twitter @benpopper.  Email us with questions or suggestions,  podcasts at Stack Overflow.
And if you like the show,  leave us a rating and a review.  Really helps.  - I'm Ryan Donovan.  I
edit the blog here at Stack Overflow.  You can find the blog at stackoverflow.blog.  And if you
wanna reach out to me,  you can find me on Twitter @Rthor Donovan.  - I'm Sayid Hamid, founder and
CEO of Sophie.ai,  no code automation platform for mobile apps.  Try us out at Sophie.ai  and let
your mobile app tested by AI.  - Very cool.  All right, everybody.  Thanks for listening and we will
talk to you soon.  (upbeat music)  (upbeat music)  (upbeat music)  (upbeat music)  (upbeat music)
(upbeat music)  (upbeat music)