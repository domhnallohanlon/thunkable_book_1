# In the Beginning was BBS

One of the earliest method of communication on the internet was through message boards, or bulletin board systems. Using this software users could:

1. Type messages on their own computer.
2. Upload their messages to a server for others to read.
3. Download messages that other had written, from the server.

We will try and replicate these three features in our first app. Before doing so it is important to remember that we have to break big, complex problems into a series of smaller, more managable challenges. 

As an homage to these early boards we will create our own app, Thunka-boards:

![Thunka-boards](img/Thunka-boards.png)

## 1. Display Text in a Label

To get started with we'll take some text from a textbox and display it in a label.

### Design

The design for this app is really simple. You just need three components; a label, a textbox and a button.

![Get and Set Design](img/comp_get_and_set.png)

<button>Open This Design in Thunkable</button>
<button>Download the .aia Template</button>

### Blocks

The code for this app is also reasonably straightforward. When the button is clicked we **get** the text from TextBox1 and **set** it as the text in Label1

![Get and Set Blocks](img/blocks_get_and_set.png)

### What's Happening?

When anything happens on your phone, from pressing a button up to recieving a phone call, your phone handles this as an event. Something has happened and you phone has to deal with it. In our app we take text from one component and display it in another, but in future apps the idea of event handlers is going to be very important. 

![Key Idea: Events](img/key_event.png)

## 2. Upload the Text

At the moment all our messages are stored (temporarily!) on our phone only. This is fine for a note taking app, but it's not much use for communication. Let's add some more components to our app to communicate with the cloud. 

### Design

This is the first time we've seen a non-visible componet. This simply means that the component does not appear on screen, but we can program it in just the same way that we would program any other component.

### Blocks

TinyWebDB will work fine right out of the box, but be aware that you will need to set up your own cloud service if plan on having lots of users. 

### What's Happening?



## Progression

You can improve the user experience (UX) of this app by clearing out TextBox1 after we have got the text from it. 

## Recap

In this chapter we've learned about:

Variables - data which can change
Getters - for getting, or reading, a value from a variable
Setters - for setting, or writing, a value to a variable.



