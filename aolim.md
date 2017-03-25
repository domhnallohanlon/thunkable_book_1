# AOL Instant Messenger

AOL launched their instant messenger in 1997 and it changed messenging for an entire generation. It dominated the IM market in North American, with millions choosing AIM over  alternatives such as ICQ or MSM. If you're too young to remember these pieces of software then do a quick search or check them out on YouTube.

The second app we're going to buid will be **T**hunkable **I**nstant **M**essenger, or TIM for short.

![TIM Logo](img/tim.png)

## How it works

The user interface is simple, and deliberately so. In essence all we need is a label, a button and a textbox. To get up and running quickly we'll use [firebase](https://firebase.google.com/) to handle incoming and outgoing messages. You don't need a firebase account to get the demo working, but if you plan on publishing your app to the Play Store then you should really [sign up](https://console.firebase.google.com/) for your own account.

## What You'll Be Building
A peer-to-peer chat app that highlights who is speaking with colourful usernames and which updates in real time.

## Design

This minimal design is very similar to Thunkaboards, but we take greater care with the positioning of the components. In the `Layout` drawer of the designer we can find horizontal and vertical arrangements which give us great control over component positioning. We have a label, with width and height set to fill parent, and scrollable is selected. In order to change the colour of the text in the label, make sure that the HTML Format property is also selected. 

![components](img/tim_components.png)

## Blocks

The blocks are a little more complex than the previous app as we need a bit more background knowledge to understand everything. We'll learn a little bit about how computers display colours and how to represent data using  HTML. In order to get everything working we need to break all of these requirements into a set of smaller, simpler sub-tasks to do. The whole point of this app is to transmit messages instantly, so we'll start there.

1. Send data with Firebase
2. Use procedures
3. HTML
4. Colours

### 1. Real-Time Chat with Firebase

![starting off](img/firebase_initialize.png)
![real time](img/firebase_data_changed.png)

### 2. Using Procedures


### 3. HTML

HTML is the language of the internet. The  language consists of tags that give meaning to the information inside them.

![html intro](img/html_intro.png)

### 4. Colours

## Chat Bot

## Recap

In this chapter we've learned about:

