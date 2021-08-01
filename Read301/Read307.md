# Perfect Team

the researchers found that there were five key characteristics of enhanced teams:

* Psychological safety: Everyone feels safe in taking risks around their team members, and that they won’t be embarrassed or punished for doing so.

* Dependability: Everyone completes quality work on time.

* Structure and clarity: Everyone knows what their specific expectations are. These expectations must be challenging yet attainable.

* Meaning: Everyone has a sense of purpose in their work (i.e., financial security, supporting family, helping the team succeed, etc.).

* Impact: Everyone sees that the result of their work actually contributes to the organization’s overall goals.

imagine you have been invited to join one of two groups.

Team A is composed of people who are all exceptionally smart and successful. When you watch a video of this group working, you see professionals who wait until a topic arises in which they are expert, and then they speak at length, explaining what the group ought to do. When someone makes a side comment, the speaker stops, reminds everyone of the agenda and pushes the meeting back on track. This team is efficient. There is no idle chitchat or long debates. The meeting ends as scheduled and disbands so everyone can get back to their desks.

Team B is different. It’s evenly divided between successful executives and middle managers with few professional accomplishments. Teammates jump in and out of discussions. People interject and complete one another’s thoughts. When a team member abruptly changes the topic, the rest of the group follows him off the agenda. At the end of the meeting, the meeting doesn’t actually end: Everyone sits around to gossip and talk about their lives.

if you are given a choice between the serious-minded Team A or the free-flowing Team B, you should probably opt for Team B. Team A may be filled with smart people, all optimized for peak individual efficiency. But the group’s norms discourage equal speaking; there are few exchanges of the kind of personal information that lets teammates pick up on what people are feeling or leaving unsaid. There’s a good chance the members of Team A will continue to act like individuals once they come together, and there’s little to suggest that, as a group, they will become more collectively intelligent.

# REST

## 1.Who is Roy Fielding?

He helped write the first web servers, that sent documents across the internet… and then he did a ton of research explaining why the web works the way it does. His name is on the specification for the protocol that is used to get pages from servers to your browser.

## 1.Why don’t the techniques that we use today work well when we need to be able to talk to all of the machines in the world?

Because they weren't designed to be used like that. When Fielding and his colleagues started building the web, being able to talk to any machine anywhere in the world was a primary concern. But most of the techniques developers later used to get computers to talk to each other didn't have those requirements. You just needed to talk to a small group of machines.



## 1.What is the HTTP protocol that Fielding and his friends created?

is all about applying verbs to nouns. For instance, when you go to a web page, the browser does an HTTP GET on the URL you typed in and back comes a web page.

Web pages usually have images, right? Those are separate resources. The web page just specifies the URLs to the images and the browser goes and does more GETs using the HTTP protocol on them until all the resources are obtained and the web page is displayed. But the important thing here is that very different kinds of nouns can be treated the same. Whether the noun is an image, text, video, an mp3, a slideshow, whatever. I can GET all of those things the same way given a URL.

## 1.What does a GET do?

It gets you resources over the web.

## 1.What does a POST do?

If one system wants to add something to another system.

## 1.What does PUT do?

If a system wants to replace something in another system.


## 1.What does PATCH do?

to do a partial update, it'll hopefully use PATCH.

