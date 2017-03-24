# In the Beginning was BBS

One of the earliest methods of communication on the internet was through message boards, or bulletin board systems. Using this software users could:

1. Type messages on their own computer.
2. Upload their messages to a server for others to read.
3. Download messages that others had written, from the server.

We will try and replicate these three features in our first app. Before doing so it is important to remember that we have to break big, complex problems into a series of smaller, more managable challenges. 

As an homage to these early boards we will call our first app, Thunka-boards:

![Thunka-boards](img/Thunka-boards.png)

## 1. Display Text in a Label

To get started with we'll take some text from a textbox and display it in a label.

### Design

The design for this app is really simple. You just need three components; a label, a textbox and a button. Simply drag-and-drop the components from the palette on the left onto Screen1 in the middle.

![Drag and Drop](img/get_and_set.gif)

It **is** possible to rename your components, and for larger apps I would strongly recommend that you do so, but for now we will have three components on Screen1 with their default names. 

![Get and Set Design](img/comp_get_and_set.png)

And you app will, initially, look like this:

![Design Basic](img/design_gas_basic.png)

Try experimenting with the properties to make it look a bit more user friendly:
![Better Design](img/design_gas.png)


<button>Open This Design in Thunkable</button>
<button>Download the .aia Template</button>

### Blocks

![Get and Set Blocks](img/get_and_set_blocks1.gif)

The code for this app is also reasonably straightforward. **When** the button is clicked we **get** the text from TextBox1 and **set** it as the text in Label1

<!-- ![Get and Set Blocks](img/blocks_get_and_set.png) -->

Once we've got this very basic app working it's time to add in some more code to make it work even better.

![Get and Set, better!](img/get_and_set_blocks2.gif)

When using Thunkable, you will see many blocks with a blue gear icon on them. This is known as a **mutator** because it allows you to mutate - or alter - the shape of a block. In our bulletin board we want to append new messages on to the end of old messages, in other words the new messages should be added onto the end of the existing messages. In order to display new messages on a new line we use the *\n* escape character, which behaves as if you pressed the <kbd>Return</kbd> key on your keyboard.

![mutators](img/mutator.gif)

Finally, we can improve the overall user experience (UX) of this app by clearing out TextBox1 after we have got the text from it. This is achieved by setting the text property to be an empty piece of text, also known as an empty **string**.

![First Improvment](img/blocks_gas_better.png)

The blue question marks that you see on the blocks here are called **comments**. These are notes that the programmer writes to explain what a certain block, or group of blocks, should do. Try right-clicking on a block now and adding in some comments of your own.

### What's Happening?

When anything happens on your phone, from pressing a button up to recieving a phone call, your phone handles this as an event. Something has happened and you phone has to deal with it. In our app we take text from one component and display it in another, but in future apps the idea of event handlers is going to be very important. 

![Key Idea: Events](img/key_event.png)

In our app, any time that the button is pressed the **When Button1.Click** event happens. The code inside the event then happens in order, starting at the top and working its way downwards. 
First the label is changed to show the new message. The dark green set block is known as a **setter** because it allows us to write, or set, new data in place of old. In our app we are replacing the old text in Label1 with new text which we get from TextBox1. The light green *TextBox1.Text* and *Label1.text* blocks are known as **getters** because the allow us to read - or get - data from a component.

## 2. Upload the Text

At the moment all our messages are stored (temporarily!) on our phone only. This is fine for a note taking app, but it's not much use for communication. Let's add some more components to our app to communicate with the cloud. 

### Design

This is the first time we've seen a non-visible componet. This simply means that the component does not appear on screen, but we can program it in just the same way that we would program any other component.

![TinyWebDB](img/comp_thunkaboards.png)

If you're using a component for the first time it is usually a good idea to consult the documentation (docs) to learn more about how it works. For instance, you can find all the documentation for the storage components - including the TinyWebDB - [here](http://thunkable.com/reference/components/storage_components.html)

### Blocks

TinyWebDB will work fine right out of the box, but be aware that you will need to set up your own cloud service if plan on having lots of users. You can read more about this in the [Thunkable Documentation](http://thunkable.com/explore/custom-tinywebdb-service.html)

### What's Happening?

![Store Value](img/store_value.gif)
![When Value Stored](img/when_value_stored.gif)
![When Got Value](img/when_got_value.gif)
![Screen Init](img/when_screen_initialize.gif)
![Button Clicked](img/btn_get_value.gif)


## Progression


Now that you have the ability to capture text input and you're familiar with the TinyWebDB, why not try and make a note taking app? Apps like [Evernote](https://play.google.com/store/apps/details?id=com.evernote) are hugely popular and they allow user to save notes both on their phones and in the cloud.

## Recap

In this chapter we've learned about:

Variables - data which can change
Getters - for getting, or reading, a value from a variable
Setters - for setting, or writing, a value to a variable.
Mutator - for changing the shape of a block
Comments - leaving notes for other humans
Strings - pieces of text

## Up Next

Everything here looks great - the only drawback is that our user has to constantly refresh the app to check for new messages. This is ok for infrequent communication like a forum, but in the next app we'll take a look at moving from this pull based system to a push based one to enable real-time chat.



