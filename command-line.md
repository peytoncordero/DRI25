---
title: 'Command Line Workshop'
cover title: 'Command Line'
description: 'The command line is a way to interact with our computer. It is an important skill for digital projects as it allows us to understand the architecture of computer systems. In this workshop, you will be able to learn basic commands while working on DHRIFT, which includes an emulated command line to practice through the workshop. This process will allow you to understand the logic of interacting with the computer and start feeling comfortable using the command line. At the end of the workshop, you will learn how to transfer these skills to your computer. After that, you will have working knowledge to continue learning according to the needs of your projects.'
cover_image: '/images/workshops/Cover_RT-11_help.jpg'

programming_language: 'computer'

learning objectives: 
    - description: 'At the end of this workshop, you will understand the command line in relation to the history of computers and the development of other ways for human-computer interaction. Additionally, you will be able to use the command line for
    - Navigating the file structure in a computer.
    - Creating new files and directories.
    - Moving content and files to new locations within the file structure. 
    - Searching within text files
    - Doing a basic exploration of a text dataset

estimated time: 
    description: 3 hours

prerequisites: 
    - None: 
        description: This workshop does not have any prerequisites. 
        required: true

instructors: 
    - 'Silvia Rivera Alfaro'

authors:
    - 'Silvia Rivera Alfaro'
    - 'Stefano Morello'
    - 'Kelsey Chatlosh'
    - 'Patrick Smyth'
    - 'Mary Catherine McKinniburgh' 
    - 'Jojo Karlin'
    - 'Kalle Westerling'

editors:
    - 'Di Yoong'
    - 'Lisa Rhody' 
    - 'Kalle Westerling'

readings:
    - Neal Stephenson's [In the Beginning... Was the Command Line](https://web.stanford.edu/class/cs81n/command.txt) is a useful piece to grasp the relationship between (and the affordances of) the command line and the GUI.
    - The paper [Accessibility of Command Line Interfaces](https://dl.acm.org/doi/fullHtml/10.1145/3411764.3445544) by Harini Sampath, Alice Merrick, Andrew Macvean, reflects on the challenges of interacting with the computer via command line for users with visual disabilities.
    - Douglas Rushkoff's [*Program or Be Programmed*](http://www.youtube.com/watch?v=BXjRaoTPlPE) based on his book with the same title.

ethical considerations:
    - "'The command line' is laden with masculine and military metaphors, which is reflective of the history of computing and programming. As Wendy Hui Kyong Chun discusses in On Software, or the Persistence of Visual Knowledge (2004), almost all computers (as in human computers) in the US during World War II were young women. Human computers received commands from analysts—predominantly men with the military—that they then had to interpret and act upon the machine. As Chun (p. 34) argued, 'computation depends on 'yes, sir' in response to short declarative sentences and imperatives that are in essence commands ... The command line is a mere operating system (OS) simulation.' If commands are how a user communicates with machines, the command line (of computers today) receives these commands as text that is typed in."

projects:
   - Feminist Linguistics Repository:
        description: Digital specialized repository of Indisciplinadxs, a community of Feminist Linguists from the Americas. The Command Line is used in the project for doing installations, configuring a home server, and collaborating remotely.   
        link: https://repositorio.linguisticafeminista.com/ 
   - Fair World 64: 
        description: A Text-Based Game of the 1964–1965 World's Fair. A recent digital capstone project by Christofer Gass runs a Python script on the command line.
        link: https://academicworks.cuny.edu/gc_etds/3786/
   
resources: 
    - Command Line Basics by The Odin Project:
        description: The Odin Project is an open learning resource. The Command Line Basics lessons include several projects for people interested in learning about the Command Line. 
        link: https://www.theodinproject.com/lessons/foundations-command-line-basics 
    - Awesome Bash:
        description: A curated list of useful Bash scripts and resources
        link: https://github.com/awesome-lists/awesome-bash 
---

# Introduction

Welcome to the Command Line Workshop! 

Here you will learn about communicating instructions to your computer. At the end of this workshop, you will be able to use the command line for

- Creating new files and directories 
- Navigating the file structure in a computer. 
- Moving content and files to new locations within the file structure. 
- Searching within text files. 
- Doing a basic exploration of a dataset. 

Understanding the logic of the command line and the architecture of the information on a computer are basic digital skills that will help you build up others. It will also help you advance more easily when you are learning programming languages. The basic knowledge you get from this workshop helps you to understand how you are interacting with your computer when programming and the kind of details that will make a difference in that process. 

The command line is a basic tool to create several projects. It allows you to

- Easily automate tasks such as creating, copying, and converting files.
- Set up your programming environment.
- Run programs you create.
- Access the (many) programs and utilities that do not have graphical equivalents.
- Access and control other computers remotely 
- Collaborate remotely in digital projects
- Install certain programs, including server-side software (or more advanced software-as-a-service software). 

Finally, there are other uses that you will find according to your interests and the places your future projects might take you. 

# What is the command line?

To get to this page of the workshop, you might have clicked on `next` or touched the bottom with your finger. In this way, you are interacting with your computer. The command line is another means of human-computer interaction. 

To be precise, the command line is a text-based interface that allows you to communicate with your computer. You input text commands and the interface interprets them into appropriate operating system functions. 

The command line interface (CLI) provides a faster and more efficient system interaction with our computers. This is why it is a basic skill to learn! 

In this image you can see how the Command Line Interface (CLI) looks on a Mac computer:

![It is a simple program with a plain background and letters. On the first line it says: Last Login: Wed Dec 27 16:34:06 on console. The second line says: base _silvira@Silvias-MBP ~ % immediately followed by the cursor showing it is where you write](/images/command-line/How-command-Line-looks-like.png "Terminal")

To refer to the CLI, people also use the terms bash, terminal, or shell. Although these terms imply different levels of abstraction in certain contexts, they are commonly used interchangeably in relation to the command line.

As we mentioned on the front page of this workshop, the command line is laden with masculine and military metaphors that come from the incarnated relationship of computer development and the technological arms race. To understand the relationship between computers and warfare, the essay [As We May Think](https://www.w3.org/History/1945/vbush/vbush-all.shtml), written in 1945, is a good source to reflect on the role of science in World War II. Another useful resource is [Hello, World - Command Line Heroes Season 2](https://www.redhat.com/en/command-line-heroes/season-2/hello-world), a podcast episode about Grace Hopper, who was a computer scientist, mathematician, and rear admiral. Hopper joined the US Navy Reserves during World War II and became a key pioneer in interacting with computers via  programming languages. 

## Command Line in History of Human-Computer Interaction

Technology changes over time and human-computer interactions go hand in hand with the developments in hardware. Thus to get to the command line, it is worth contextualizing it along with other ways of interacting with computers.

Let’s start by saying that the first “computers” were humans. It was an occupation: people were paid to develop mathematical operations before we had electronic computers. The majority were women, as they were contracted as cheaper labor, despite having the same abilities. We recommend [Human Computers at NASA](https://omeka.macalester.edu/humancomputerproject/), a digital archive on the hidden labor of African-American women at this institution starting in 1943. 

The first electronic programmable computer was ENIAC (Electrical Numerical Integrator and Calculator), a hardware of the size of a room (1,800 square feet) created in 1945 for warfare purposes. It was designed by two men and programmed by six women, whoever the references are usually to the hardware developers and not so much to the programmers. We recommend [The Forgotten Female Programmers Who Created Modern Tech](https://www.npr.org/sections/alltechconsidered/2014/10/06/345799830/the-forgotten-female-programmers-who-created-modern-tech), a 6-minute radio program that includes the voice of one of the ENIAC programmers and helps to understand the role of women in developing programming. 

As human-computer interaction depends on the available technology, ENIAC used punch cards. This is how a punched card looks: 

![Detail view of cards against dark grey background. for Pilot ACE computer built at the National Physical Laboratory c. 1950.](/images/command-line/Punch_cards.jpeg "Punch_cards_Pilot_ACE_c1950")

Punch cards have been around since 1725 to operate looms in textile manufacturing; in the 1800s they became key to the Industrial Revolution, as they were used to automate the operation of the loom. The proposal of [a mechanical computer device](https://en.wikipedia.org/wiki/Analytical_engine) using that technology dates from that time. Punch cards are made with a keypunch, a device for precisely punching holes. In its early times, it was manual and later on became electromechanical. This is a picture of a keypunch operator working for the US Census in 1950:

![An Afro-American woman working on an IBM keypunch.An Afro-American woman working on an IBM keypunch.](/images/command-line/Keypunch_operator.jpg "Keypunch_operator_1950_census_IBM_016")

## Sizing of the computers and human-computer interaction

Just think how sizing goes from computers of the size of a room to computers that can fit in our hands! For the computer using punch cards, people interacting with the machines required specialized knowledge, especially mathematics. Using those computers was an action that required physically traveling to a place and going into a specific room. 

Then computers started to size down. The interaction via command line dates from the mid-60s. The available hardware at that time was [computer terminals](https://en.wikipedia.org/wiki/Computer_terminal). The CLI emerged as a development for these machines, which included keyboards! The command line was much friendlier than the punch cards.

At that same time, another user-friendly-centered way of interacting with the computer started to emerge: the Graphic User Interface (GUI). While GUI can be navigated via a keyboard, an essential invention for the development of GUI was the mouse (1963) because it allows users to navigate the screen with the pointer and click on icons. At first, the interface was limited to specific programs but was later included in operating systems, such as macOS, Linux, and Windows, in the 1980s.

Currently, we have computers that can be transported in our hands, from smartphones to smartwatches. They are literally at our fingertips, as we interact with them via touchscreen. We can use them for as many tasks as we can imagine, from performing basic calculations to asking for directions on a map.

Despite all these developments, to this day, the Command Line Interface continues to be a faster and more efficient way to interact with our computers for people working with computers. In our case, this is especially important for some digital projects.  

# What is a text for the command line?

We mentioned that the command line is text-based. As humans, we are used to text with different fonts, sizes, bold and cursive letters, etc. These characteristics are for human interpretation of a text. 

"Text-based" in the context of computers is merely the strings of words. To give a general sense of "text" when it comes to computers, we need to contrast *text editors* and *word processors*.

## Word processors

Word processors are programs we use to write and edit a document, such as Microsoft Word or Google Docs. In them, we input text and the program allows us to make changes in the text appearance. We choose, for example, a new typografy and letter size and the program immediately displays the changes without showing us the code the computer is reading to render the formatting. 

![The image is a screenshot of Microsoft Word. We see what is written in the document. The title is “What do we mean by “text editor”?” The body of the text says: “While these words on this assumed “blank” document will hopefully print the way they look to you on your screen (with margins and fonts as you design them), this text is far from plain. In fact, Microsoft Word is a processor (emphasis on processor) with many hidden codes to help you with your desktop publishing. While these features enable many visual effects, the hidden codes become obstacles when you attempt to automate processing with the computer.](/images/command-line/worddoc.png "Word Doc")

To put it in another way, what looks like "just words!" for users is formatted text using codes that the computer executes. For example, the words of the Microsoft Word document reproduced above are comprised of an archive of extensible markup language (XML), instructions that only Microsoft Word can read. If we ask the command line to read that same Word .docx file, the result would be a mixture of symbols as we show below:

![This screenshot of the Command Line trying to read a .docx file shows a very long string of symbols, letters from different alphabets, and even characters that our fonts can not recognize (which show up as question marks). Here we reproduce only a very small part of the long result to give you a bit of the taste of the nonsense it is for humans: P K exclamation mark control character question mark l Z square bracket Content_Types square bracket .xml question mark question mark question mark question mark n question mark 0E](/images/command-line/CatWordDoc.png "Word Doc as visualized by Command Line")

The computer tried to read the hidden code, but only Microsoft Word could read those instructions. The styled text produced by word processors is known as *rich text*. 

Following [Unicode](https://www.unicode.org/versions/Unicode13.0.0/UnicodeStandard-13.0.pdf) (version 13.0), which is the international standard for displaying letters and symbols in a computer, “Rich text carries complex formatting information as well as text context [and its] representation may be implementation-specific or proprietary” (p.19). Surprising how much is going on behind the words shown on the screen in word processors! 

## Text editors

To interact with the computer, we need to use *plain text*, which is text without hidden formatting. It is produced in text editors following international standards. Thus, it has the advantages of being manipulable in different editors and readable within the command line. 

According to [Unicode](https://www.unicode.org/versions/Unicode13.0.0/UnicodeStandard-13.0.pdf) (version 13.0): “Plain text is a pure sequence of character codes” (p.18); it “is the underlying content stream to which formatting can be applied. [... It is] public, standardized, and universally readable” (p.19). We could say that plain text shows its cards—if it's marked up, the markup will be human-readable. 

Because we need plain text to interact with the computer, text editors are an important tool for programming and working in the command line. A text editor is a program that allows you to edit plain text files, such as .txt, .csv, or .md. 

Text editors are not used to edit rich text documents. Word processors should not be used to edit plain text files, because the formatting would prevent programs from running and configuration files from being read correctly.

While it doesn't matter which text editor you choose, you should try to become comfortable with at least one of them. In the end, choosing a text editor has as much to do with personality as it does with functionality!

## Evaluation

1. What is the command line? (Select one)

<Quiz>
- A program to edit plain text.
- A text-based interface to communicate with the computer.*
- A Graphical User Interface.
- A programming language.
</Quiz>

2. What is the difference between a plain text document and a rich text document?(Select all that apply)

<Quiz>
- Plain text contains no formatting, only line breaks and spacing.*
- Plain text cannot be marked up.
- Rich text is styled text, _i.e.,_ plain text completed by information such as font size, format, and colors.*
- One can't determine whether there is a difference between the two without looking at their content.
</Quiz>

**To think forward:**
- In what ways do you interact with computers in your everyday life? 
- What is the Command Line? How is it different from your text editor?

# Hands-on the command line!

Every command we learn in the next pages will require you to practice it. For this, we included an emulator of the command line on DHRIFT. 

To access the emulator, check the top-right side of the screen (or the top if you are using a small device). There is a rectangle with the text "Open Code Editor". When you click on it, the emulator will be displayed as part of the same windows where you are reading this text in your navigator. 

Once it is open, you can resize it by clicking on the left border of the rectangle and dragging it to the desired size. (Your mouse pointer should change into the resize icon, a horizontal two-sided arrow).

You can hide the emulator to continue reading through the workshop. For this, click on the “Close Code Editor” button, which will appear on the top. You can close it and reopen it everytime you need; the information you have entered will continue to be there!

We also want to share these tips to get ready:
 
**1. Go slow at first and check your spelling.** One of the biggest things you can do to make sure your code runs correctly and you can use the command line successfully is to make sure you check your spelling! Keep this in mind! If at first, something doesn't work, check your spelling! Unlike in human reading, where letters operate simultaneously as atomistic symbols and as complex contingencies, in coding, each character has a discrete function including (especially!) spaces. We invite you to read [From A to Screen](https://genius.com/Johanna-drucker-from-a-to-screen-annotated) by Johanna Drucker. 

**2. Pay attention to detail.** Keep in mind that the command line and file systems are usually pre-configured as cAsE-pReSeRvInG—so capitalizations also matter when typing commands and file and folder names.

**3. Don’t cheese the game.** While copying and pasting from this handy tutorial may be tempting to avoid spelling errors and other things, we encourage you not to! Typing out each command will help you remember them and how they work.

Now, you are ready to get started!

## Navigating the command line

**Command prompt $**

```console
$ 
```

We will refer to '$' as the 'command prompt.' It is the place where you type commands for the computer to execute. We will now learn some of the most common commands.

When you see the '$', you're in the right place. In the following lessons, we will refer to the command prompt using a '$'. 

However in different Operative Systems, the sign varies somewhat, and sometimes the sign is a '%' or a '#'. In all cases, we call it a command prompt. It lets us know the computer is ready to receive a command.

## Getting started: know thyself

You may also see your username to the left of the command prompt $. Let's try our first command. Type the following command and press enter on your keyboard:

```console
$ whoami
```

The `whoami` command should print out your username. On DHRIFT the response should be 

```console
user
```

On each computer, this would change according to the name username.

Congrats, you've executed your first command! This is a basic pattern of use in the command line: type a command, press enter on your keyboard, and receive output. 

Now that we know 'thyself', our next step should be to understand where we are. 

# The filesystem: information structure on the computer 

To work with the command line it is important to understand that, in computers, information is organized hierarchically. The method of organization and data structure is called the *filesystem*. 

We can think of a library as a metaphor for going inside a computer. Libraries have very systematic ways of organizing knowledge with a hierarchical system. When we approach a shelf, we can see that books are located by subject and that, even within a subject, there are subtopics, that can be categorized even further. The library contains many books and needs to be able to include new books over time. Additionally, libraries need to organize their books in a way that their many users can easily find the path in the building to access the shelf and retrieve any book they want from the collection. 

![Four videos together. One with a person taking a book from a bookshelf at a library. One video of boxes at an archive. A  person looking at the cards in the card catalog. A person opening a card catalog with their hand](/images/command-line/FileSystem.gif "Libraries and Archives")

The filesystem is named after a method to store paper documents. It is quite close to the idea of the library, where each book could be taken as a file. In fact, we could move from libraries to archives. Archives also organize knowledge, but they differ by keeping unpublished materials and gray literature. As many of those materials are files, they keep these files in folders. In this case, the organization should also enable us to easily find the path to the documents. 

The metaphor is not about the material means to keep the files, but about keeping a hierarchical global organization to contain information within a space. Computers are very alike libraries and archives in the amount of information they keep. The only difference is the materiality of the documents. 

## Issues of a metaphor

When the filesystem became a generalized name (around the 1960s), only a limited audience had access to computers. Those users, mostly researchers and specialists, might have a close relationship with the spaces we mentioned in the metaphor. Additionally, thinking of hardware, when computers were the size of a room, people shared a physical space to store information, just as the library of our metaphor. And a shared room requires as much organization as possible. 

As computers became smaller, anyone -with the purchasing power- could take home.  For many of these new users, the metaphor might have been more distant. However, files and folders were pretty common, and the users could relate to them. So, even if part of the information structure got fuzzy, the metaphor of the objects as a means to keep order was useful as one computer was shared per household or office. Later on, individuals started to have laptops as their personal digital space. And it is no secret that not everyone keeps their room tidy! 

Going back to the metaphor, now libraries store digital collections. We can visit them without the physical experience of the shelves and the information organized in the space. We also relate to new information structures in our everyday practices, as  the [Arium: Beyond the Desktop Metaphor](https://kilthub.cmu.edu/articles/thesis/Arium_Beyond_the_Desktop_Metaphor_A_new_way_of_navigating_searching_and_organizing_personal_digital_data/6723005) elaborates. 

The filesystem is not so much a metaphor we live by. This can challenge those teaching and learning about computers, as you can read in the article [File Not Found](https://www.theverge.com/22684730/students-file-folder-directory-structure-education-gen-z). However, as for the command line, understanding the hierarchical structure of the filesystem continues to be an essential task to be able to interact with the computer and give it commands!

## Orienting Yourself in the Command Line: Folders

We're going to try another command to understand. This time it will help us to understand where we are on the computer. Write the following command and press enter:
 
```console
$ pwd
```
You should get the output 

```console
/home/user on DHRIFT. 
```

The command pwd, which stands for "print working directory”, allows you to know the current working directory where you are located. "Print" as a word can be somewhat misleading. The command pwd won't print anything except on your screen. This command is easier to grasp when we interpret "print" as "display." Note that we are using the word "directory" interchangeably with "folder"—they both refer to the same thing.

Note that we are using the word "directory" interchangeably with "folder"—they both refer to the same thing, even though the folder is the container and the directory is how it relates to the hierarchy. As we mentioned, the information in the computer is organized hierarchically in the filesystem. You can draw these relationships in a tree. 

![Screen shot of the icons of folders organized as a tree of the filesystem in the MacOS GIU](/images/command-line/hierarchical-filesystem-example.png "An example of how a hierarchical filesystem looks")

That means there's a top-level or root folder on your system. That folder has other folders in it, and those folders have folders in them, and so on. The root or highest-level folder contains mostly files for the operating system, and we usually don’t have to go there. These folders are called just / on macOS and are called C: on Windows. 

On your computer, you should get something like  /Users/your-username, which means you're in the your-username directory in the Users folder inside the / or root directory. This directory is often called the "home" directory.

Now we know "where" we are. But what if we want to know what files and folders are contained in the same working directory where you are located right now? 

## What's in the folder?

To check what is contained in the folder, try entering:

```console
$ ls
```

In this command, “ls” stands for list. It is a request to list the contents of your current working directory. 

You should see a list of folders and files contained in the current working directory where you are located. Usually, it might include folders such as Documents, and Desktop, and you may also see some files. In the case of the DHRIFT emulator, you should see command-line-treasure-hunt and data. 

Wonder what's in the data folder? Let's try navigating to it with the following command:

```console
$ cd data
```
The cd command lets us "change directory." (Make sure the "d" in "data" is not capitalized.) If the command is successful, you won't see any output. This is normal—often, the command line will succeed silently. 

So how do we know it worked? Let's use our pwd command again! We should get:

```console
$ pwd
/home/user/data
```

Now try the command ls again, to see what's on the data folder! 

The commands pwd, ls, and cd are the three most commonly used in the terminal. Between them, you can orient yourself and move around.

One more command you might find useful right now is cd .. which will move you to one directory up in the filesystem. That's a cd with two periods after it:

```console
$ cd ..
```

Let's check it worked using our pwd again! 

```console
$ pwd
/home/user
```
## Evaluation

1. What command do you run if you are trying to identify where in the filesystem you are currently located/working?

<Quiz>
- $ `ls`
- $ `pwd`*
- $ `cd`
- $ `whoami`
</Quiz>

**Keywords**
- [Filesystem](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/filesystem.md)
- [GUI](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/gui.md)
- [Root](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/root.md)

# Creating files and folders 

So far, we've only performed commands that give us information. Let's use commands that create something new on the computer! 

![Animation of a collage that says hello world and has a vintage computer.](/images/command-line/HelloWorld.gif "Hello World")

## Creating files

We will start with a file.

First, make sure you're in your home directory:

```console
$ pwd
/home/user
```

Once you've made sure you're in there, let's try a new command:

```console
$ touch foo.txt
```

The touch command is used to create a file without any content. This command can be used when you don’t have any data yet to store in it. Touch creates a new file if it doesn’t exist, but when the file exists, it will only modify the time when it was last accessed. 

In this case we are creating a .txt which means it is a new plain text file, but it could have been a .csv file which could be a list or representing a spreadsheet in plain text.

If the command succeeds, you won't see any output. So, let’s make sure the file is now part of your folder by using the command ls

```console
$ ls
```

See any differences? If the command was successful and you were in the right place, you should see a file called foo.txt in the home folder. Pretty cool, right?

**Why the file is called foo.txt?**
As we mentioned in the ethical considerations of this workshop, the command line is laden with masculine and military metaphors. You could use any name, but foo is a common name in Computer Science which possibly comes from the unfortunate abbreviation for “fucked up beyond all repair” from the Second World War. 

## Handy Tip: Use the arrows on the keyboard! 

Let's say you liked that 'foo.txt' file so much you'd like another! In the command line emulator, press the <kbd>up arrow</kbd> on your keyboard. You'll notice this populates the line with the command that you just wrote: “touch foo.txt” 

If you keep pressing the up arrow you can see all the commands you wrote recently. You can navigate the comments with up and down arrows. 

As we start to write more complicated and longer commands in our terminal, the up arrow is a great shortcut so you don't have to spend lots of time typing. 

You can use your left/right arrows to move the insert cursor around on the screen so you can, for instance, change the file name to 'foot.txt' to create a different file.

## Creating folders 

OK, so we're going to create a projects folder!
First, let's check to make sure we're still in the Home folder with pwd:

```console
$ pwd
/home/user
```

Once you've double-checked you're there, we'll use the mkdir or "make directory" command to make a folder called projects:

```console
$ mkdir projects
```

Now run ls to see if a projects folder has appeared. Once you confirm that the projects folder was created successfully, cd into it.

```console
$ cd projects
```

And check that you are in the new folder

```console
$ pwd
/home/user/projects
```

OK, now you've got a projects folder! 

In this case ‘projects’ is the name of the folder, but it could be called any name we wanted. For example, if we use $ mkdir bananas, then the directory would be ‘bananas’

When you work on your computer and create folders, they should be visible on your graphical desktop too. 

## Moving a file to our new folder

Now that you have a folder for your projects, let’s move our first file to this folder. 

First, be sure you are located in the current location of the file, which is /home/user/projects. If you are not there, use the commands we have learned to make projects your working directory.You need to be in the folder where the file is located to execute the next command successfully. 

Once you are there, type the mv command followed by the name of the file you want to move and then the file path to your projects:

```console
$ mv foo.txt /home/user/projects
```

You can then navigate to that projects folder and use the ls command to check that the file is there. 

## Activities

**Challenge** 
- Check the directory you are in. 
- Create a subfolder 
- Now go to that folder and create a file on your own inside of it! 

Do you what to check the solution?

<Secret>
1. Type pwd to see where you are located. If you are not in the projects folder we just created, navigate to that folder using the commands cd and cd .., that we learned before
2. Type mkdir name-of-your-subfolder to create a subfolder.
3. Type cd name-of-your-folder to navigate to that folder.
4. Type name-of-your-file.txt to create a new text file.
5. Type ls to check whether you created the file correctly.
</Secret>

**Evaluation**

What does the <kbd>up arrow</kbd> do?

<Quiz>
- It quits the Terminal/GitBash.
- It undoes my last command.
- It inserts my last command.*
- It shows me what folder I am working in.
</Quiz>

**For further consideration**

- Think of your current form of organizing information on your computer or a specific cloud service where you storage information. Do you follow a specific system to organize it? Is it possible for you to draw a diagram of it? 

- Now, think of the how would be a good way to organize information when you create folders in that space - is it possible for you to draw a diagram?

- Finally, think of the different spaces where you store your information. Is it possible to draw a diagram of how you organize your information in general and how these spaces interact?

## Create your Command Line Cheat Sheet 

In this section, we’ll create a text file that we can use to keep all the commands we learn in this workshop. 

To know where we are creating this new file, first check where you are located:

```console
$ pwd
/home/user/projects
```

If you are in the projects folder, stay there. If you are not there, use

```console
$ cd ~
```

This last sign is called tilde. The command “cd ~” gets you to your user folder, home. 

Try the command pwd again, you should be in the home directory now /home/user/

Now that you are there, access projects

```console
$ cd projects
```

It might seem repetitive or basic to check our location once again, but when you are working in a bigger project, being able to document the location of files to be able to know the path to access them is a very important task. Think again of our metaphor of looking for a book in the library: to enter a big building full of books and being able to find the one you are looking for, you need to have a sense of the structure and now where the book is located. 

We are ready to create our first project: our very own cheat sheet! So let’s move forward with it. 

For this project, we will use “echo”. Echo is a command to print plain text. Write
 
```console
$ echo “Hello world from the command line”
```

The output will be a line of text on the command line:

```console
Hello world from the command line
```

This is the way in which the CLI prints the text. How can we ask the computer to print a text on a file instead of printing it on the command line? 

We use the redirect symbol (a greater-than symbol): 

```console
$ echo “This is my cheat sheet”  > cheat-sheet.txt
```

Now let’s check we created the file with the command 

```console
$ ls 
```

The output should include in the list a file called cheat-sheet.txt

But we also want to make sure that our phrase “This is my cheat sheet” is in the file! How can we do that? Write: 

```console
$ cat cheat-sheet.txt 
```

The command “cat” is used to request your computer to print the file. It stands for “concatenate,” because it links strings of characters or files together from end to end. 

The output should be the content of the file. In this case, the only content is 

```console
This is my cheat sheet.
```

## How can we add more content? 

Be aware. To write in the file we used redirect. Redirect takes the output that we would have on the CLI and overwrites it in the file. It means that if we use it again on the same file to add a different phrase it would erase what you wrote previously by overwriting it. In this case, we knew it was a new file so we were not worried about it! 

However, and with our pedagogical intention let’s overwrite the text by using the redirect symbol again. 

```console
$ echo “Ups! I am overwriting my cheat sheet!”  > cheat-sheet.txt 
```

Check the file: 

```console
$ cat cheat-sheet.txt 
```

The output is different now! 

How could we edit the text of our cheat sheet more practically? Try 

```console
$ nano cheat-sheet.txt 
```
Nano is a basic text editor. The output should look similar to this image: 

![The image shows how the nano editor, which is open with this command, looks](/images/command-line/nano.png "Nano")

 Once you are in the document, navigate the text with the keyboard arrows. Then change the information for:

```console
pwd     prints the working directory
ls      lists the content of a folder
cd      changes directory
cd ..   goes up one directory 
cd ~    goes to home directory 
touch   creates a new file
mv      move file
mkdir   creates a new folder 
echo    prints plain text 
>       is called tilde, prints into a specific file by overwriting it
```

When you finish, press <kbd> control + shift </kbd> to exit the text editor. Respond <kbd> control + Y </kbd> to save changes. 

Now we can check our file: 

```console
$ cat cheat-sheet.txt 
```

**Clarifying note:**  
There is also a way to add new text from the command line but without overwriting. It is using append “>>”. This symbol uses two greater-than symbols together, but for the computer field it is called “append”. 
If there is already text in the file, this is a quick option to add information. We are not trying it in the workshop as we wanted to be able to add longer text and multiple lines in a more efficient way. 

## Organizing your cheat sheet

Use pwd and cd to make sure you're in the folder with your cheat sheet. Then try:

```console
$ cat cheat-sheet.txt | sort
```

As output, you should see the contents of the cheat sheet file with each line rearranged in alphabetical order. Let’s say you want to save this output in a new file named MyCheatSheet.txt, you could use a > to print the output to a file, like this:

```console
$ cat cheat-sheet.txt | sort > MyCheatSheet.txt
```

To find that this new file was created use the command ls. You should see the file as part of your results.

**About these commands: the symbol |**

We used | as part of our last two commands. This symbol is called “pipe”. Pipes allow you to ask your computer to take the output of one command and use it as the input of the next one. This will allow us to combine multiple commands on a single line.

This diagram shows the process that pipes do:

![The image shows three commands connected with pipes and describes the flux in which the computer will complete one command, go to the next command, then go to the third command. Then, it has an arrow coming from the last part of the process indicading that only after completing all the commands we will have an output](/images/command-line/pipes.png "Pipes diagram")

To apply the diagram to our recent commands: 

To sort the document: 
- Command 1: $ cat cheat-sheet.txt
- Command 2: Sort

In this case we only want to see the final sorted result, so we want the computer to do both commands and show us only the final result. 

To create the new file with the sorted information: 
- Command 1: $ cat cheat-sheet.txt
- Command 2: sort > MyCheatSheet.txt

In this case want the sorted result to be saved in a new file, so we used the redirect symbol to create a new file as part of the second command.

## On naming files and folders

Just as organizing the information is important, the names of the files are important to facilitate our projects. So this is a note on digital best practices on naming files! 

Your cheat sheet is titled cheat-sheet.txt instead of cheat sheet.txt for a reason. Can you guess why? 

Let’s see if you guessed by making a test! 

Check you are in the folder named “projects”: 

```console
$ pwd
/home/user/projects
```

Create a new subfolder with in projects: 

```console
$ mkdir test
```
Go to that directory 

```console
$ cd test
```

Now try to make a file named cheat sheet.txt and after that try to print it on the command line 

```console
$ touch cheat sheet.txt
$ cat cheat sheet.txt
```

What was the output? To observe what happened when you created that file, ask the computer to list what is in the folder

```console
$ ls
```

Our graphical user interfaces (GUI) allow us to save files with spaces in the name, and we usually don’t think about the consequences of those naming practices. Now imagine you are attempting to open a very important file for your project with a name such as final data.txt using the CLI! 

Thus for digital best practices, we recommend making sure that file names contain no spaces. How? By using creative capitalization, dashes, or underscores instead. Keep in mind that the command line is case-preserving, which means that capitalization matters when you type commands. You might also avoid using periods in your file and folder names, as they sometimes can prompt you to confuse them with system files or file extensions (e.g., the full name of a PDF file is usually file.pdf). 

## FUN TIME: Treasure hunting! 

Use the commands we have learned so far to go on a treasure hunt in the DHRIFT emulator. 
1. Access the folder command-line-treasure-hunt
2. Once there, ask the computer to print the instructions on README.md

Right now you should be able to read those instructions! Pay attention to them and remember to pay attention to spelling and case sensitivity so that your commands work well! 

Good luck! 


![Image that looks like a vintage videogame and has a cat saying you can do it next to a treasure.](/images/command-line/TreasureHunting.gif "Treasure Hunting")

## Evaluation

What does effect does the following command produce? (select one)

```console
$ echo "Hello! My Name is Mark!" > introduction.txt
```

<Quiz>
- It adds the line "Hello! My Name is Mark!" to the existing content of the `introduction.txt` file.
- It checks whether the content of the `introduction.txt` file contains the line "Hello! My Name is Mark!"
- It replaces the content of the `introduction.txt` file with the line "Hello! My Name is Mark!"*
- None of the above.
</Quiz>

## Interlude: two command line secrets

1. **Clearing the terminal**

After running all the commands we have learned so far, the terminal might be quite full of text. For our next section, it might be nice to clear the terminal and have a fresh start. Use the command clear: 

```console
$ clear
```

The output should be the terminal clear! 

2. **Tab for completion** 

When you are navigating in the command line, typing folder and file names can seem to go against the promise of easier communication with your computer. Here comes tab completion, stage right!

When you need to type out a file or folder name—for example, the name of a file we created: cheat-sheet.txt —in the command line and want to move more quickly, you can just type out the beginning characters of that file name up until it's distinct in that folder and then click the tab key. And voilà! Clicking that tab key will complete the rest of that name for you, and it only works if that file or folder already exists within your working directory. 

In other words, anytime in the command line you can type as much of the file or folder name that is unique within that directory, and tab complete the rest! 

Only where you are located in the folder that contains the file the tab key will complete your writing. The same happens with almost all commands: they will only be executable if you are in the right location of the filesystem where the files are located. If not, the command will not be successful.

# Working with text data

The Command Line can be a very powerful tool to analyze text data, especially when we use it to analyze a large amount of text, one that would be too large to work with by hand. In this section, we will analyze. 

The data we will be using is already on the DHRIFT emulator. The path to find it is 

```console
/home/user/data 
```

Check where you are located using pwd. If you are not in that working directory, use the necessary commands to access that location.

Now that you are there, use ls to ask the list and find what our data set is. You should see a file named nypl_items.csv

Our data set is a list of public domain items from the New York Public Library. It's in .csv format, which is a plain text spreadsheet format. CSV stands for "comma-separated values," and each field in the spreadsheet is separated with a comma. It's all still plain text, though, so we can manipulate the data using the command line.

## Exploring the text file

We said this data is a large amount of text. Let’s make some simple tests to see the length. 

First, try using the cat command to look at the data. 

```console
$ cat nypl_items.csv 
```

What do you think in comparison to our earlier practice with the cat command? Now you might find the text being printed out goes by too fast to get any sense of it!  If the output is taking too long, you can click control + C [h]on your keyboard to cancel it.

**How long is that file anyway?** 

```console
$ cat nypl_items.csv | wc -w
```

With larger amounts the data it might take some seconds to run each command before printing the single output we are requesting. 

What is the output?

<Secret>
The total of words in the file should be 2,298,575.
</Secret>

**What is new in this command?**

We had two commands combined as one single line with a pipe. The first command is to display the text of nypl_items.csv. The second command is “wc -w”. It asks the computer to print the number of words. This is something we learned earlier. The hyphen is a new element for us. It marks that the immediate element that follows it is a flag. 

Flags indicate options that belog to specific commands. For example, in the command wc we have various options. We used “-w” to select the “number of words”, but it could also be “wc -l” to show the number of lines or “wc -m” to count the number of characters. You can try these other commands if you want to explore further. 

## Viewing Data in the command line

We saw that the cat command was not very useful for this large data set. Instead, let’s use another tool, the less command. It allows us to get data one page at a time.

```console
$ less nypl_items.csv
```
less gives you a paginated view of the data; it will show you the contents of a file or the output from a command or string of commands, page by page.
To view the file contents page by page, you may use the following keyboard shortcuts: 

-Press the <kbd>f</kbd> key to view forward one page
-Press the <kbd>b</kbd> key to view back one page.
-Press the key <kbd>q</kbd> to return to the command line.
Let’s try two more commands for viewing the contents of a file. The first one fo them is head:

```console
$ head nypl_items.csv
```

The output should be the very first section of the file, which is called head. The second command, by contrast, prints out the very last part of the file, which is called tail:

```console
$ tail nypl_items.csv
```
## Cleaning the data

We didn’t tell you this before, but there are duplicate lines in our data! Two, to be exact. Before removing them, let’s see how many entries are in our .csv file 

```console
$ cat nypl_items.csv | wc -l
100001
```

This tells us there are 100,001 lines in our file. 

To find and remove duplicate lines, we can use the uniq command combined via a pipe with other commands we used before. Let's try it out:

```console
$ cat nypl_items.csv | uniq | wc -l
99999
```

OK, the count went down by two because the uniq command removed the duplicate lines. But which lines were duplicated?

```console
$ cat nypl_items.csv | uniq -d
```

In this line we are combining two commands, the first one is to print out the data. The second one is the uniq command with the -d flag, which is the option to print out the lines that have duplicates.

## Activities

**Challenge**

Use the commands you’ve learned so far to create a new version of the nypl_items.csv file with the duplicated lines removed. Hint: we created a new version of our cheat sheet after sorting it alphabetically. 

<Secret>

```console
$ cat nypl_items.csv | uniq > clean_nypl_items.csv
```
This will allow you to create a new version of the nypl_items.csv file with the duplicated lines removed. You can decide any name you prefer for your file!

</Secret>

**Evaluation**

What do command linen flags allow you to do? (select one)

<Quiz>
Flags allow you to earmark the file you are working on.
Flags are useful to create a new version of the file you are working on while preserving the old version for future access.
Flags are a common way to specify options for the command line programs.* 
</Quiz>

## Search the data 

So we've cleaned our data set, but how do we find entries that use a particular term? Let's say I want to find all the entries in our data set that use the term "Paris."

Here we can use the grep command, which stands for "global regular expression print." The grep command processes text line by line and prints any lines that match a specified pattern. 

On the command line write

```console
$ cat nypl_items.csv | grep -i "paris"
```

This will print out all the lines that contain the word "Paris." The -i flag makes the command ignore capitalization. 

Now we can use our wc -l command to see how many lines that are:

```console
$ cat nypl_items.csv | grep -i "paris" | wc -l
191
```

In this last command, we have used the cat command to read nypl_items.csv, take the output, and pipe it into the grep -i command, which will ignore capitalization and find all instances of the word paris. We then take the output of that grep command and pipe it into the word count wc command with the -l lines option. The pipeline returns 191 letting us know that "Paris" (or "paris") occurs on 191 lines of our data set.

**Regular expressions**

In this command we used grep and said that it stands for regular expressions. Regular expressions are special strings representing a pattern to be matched in a search operation. grep gives us access to the power of regular expressions as we search for text.[k] Regular expressions (or regex) provide methods to search for text in more advanced ways, including specific wildcards, matching ranges of characters such as letters and numbers, and detecting features such as the beginning and end of lines. Regular expressions are commonly used in different programming languages.

## Activities

**Challenge**

Use the grep command to explore our .csv file a bit. What areas are best covered by the data set? 

If you want to get a little more milage out of the `grep` command, refer to [this tutorial on grep and regular expressions](https://www.digitalocean.com/community/tutorials/using-grep-regular-expressions-to-search-for-text-patterns-in-linux). If you want to experiment with regular expressions in an easy-to-use environment, numerous regex test interfaces are available from [a simple google search](https://www.google.com/search?w&q=regex+tester), such as [RegExr](https://regexr.com/), which includes a handy cheat sheet.

**Evaluation**

What do pipes allow you to do? (select all that apply)

<Quiz>
- Pipes let you take the output of one command and use it as the input for another.*
- Pipes allow you to combine multiple commands in a single line.*
- Pipes let you work on multiple files at the same time.
</Quiz>

Let's think about the grep command. Select all that pertain to the command.

<Quiz>
- It searches the given file for lines containing a match to the given strings or words.*
- It can be combined with other commands, so as to produce a search that matches their output.*
- It produces a new file with the lines containing the strings or words you are searching.
- It delete the strings or words you are searching from a file.
</Quiz>

## Review
Go to your projects folder and open your cheat-sheet.txt file using the nano command to add the new commands learned in the workshop: 

```console
wcword      count 
sort        to organize the content of the file in alphabetically by line
mv          to move files 
less        to ge a paginated view of the data. To navigate thes paginated view use: “f” for forward, b for back, q for quit - this is not “control + C” because ‘less’ waits for user input
head        to only see the first part of the file, e.g. head nypl_items.csv
tail        to only see the last part of the file, e.g. tail nypl_items.csv
uniq        (stands for unique) to print repeat lines only once
grep        stands for “global regular expression print’ 
wc -w       asks to print the number of words
sort -f     makes sort noncase sensitive
ls -l       shows the long list (the details of the content)
wc -l       shows the number of lines
wc -m       counts the number of characters 
head -n #   shows a specific number of lines of the head, e.g. head -n 1 nypl_items.csv 
tail-n #    shows a specific number of lines of the head, e.g. tail -n 3 nypl_items.csv
```
**Bonus:**
We included the flag -n in the commands for your cheat sheet. It works as an option for head and tail, to show only a specific number of lines. You can select the number of lines you want to see by replacing the number simbol for the specific number of lines you want. 

# Summary of the workshop

You've made it through your introduction to the command line! By now, you have experienced some of the power of communicating with your computer using text commands. Now is a good time to do a quick review! 

The command line interface is a way to interact with our computer and that it continues being more efficient and faster than other system interactions. 

We learned that, for CLI, we need plain text. To understand the reasons we explored the difference between word processors and text editors. And how those programs, create rich text and plain text respectively

Via DHRIFT’s command line emulator, we interact with the computer on bash (or Terminal). We practiced commands for

1) Navigating the file structure in a computer (pwd, ls, cd, cd .., cd~).
2) Creating new files and directories (ouch, echo, mkdir).
3) Moving content (with redirect > and pipes |) and files (with mv) to new locations within the file structure.
4) Searching within text files (cat, grep, less, head, tail, uniq)
5) Doing a basic exploration of a text dataset (nypl_items.csv)

And we documented those commands on a cheat sheet that can be used for reference!

The basic steps you learned today will help as you'll further your digital skills. For example, you might work with the command line interface to set up your version control with git or you'll have your text editor open while writing Python scripts or building basic websites with HTML and CSS. Having a grasp of command line basics will not only make you more familiar with how your computer and basic programming work, but it will also give you access to tools and communities that will expand your research.

In the next pages, we will explain how you can transfer this knowledge to your computer. We also share resources for independent learning. 

## Final Evaluation

Here are some questions from to review the lessons of the workshop:

_1. What does the <kbd>up</kbd> arrow command do? (Select one of the following)__

<Quiz>
- It inserts my last command.*
- It quits the Terminal/GitBash.
- It undoes my last command.
- It shows me what folder I am working in.
</Quiz>

__2. What do command line flags allow you to do? (Select one of the following)__

<Quiz>
- Flags are a common way to specify options for command line programs.*
- Flags allow you to earmark the file you are working on.
- Flags are useful to create a new version of the file you are working on, while preserving the old version for future access.
</Quiz>

__3. What effect does the following command produce?__

```console
$ echo "Hello! My Name is Mark!" > introduction.txt
```
(Select one of the following)

<Quiz>
- It replaces the content of the introduction.txt file with the line “Hello! My Name is Mark!”*
- It adds the line “Hello! My Name is Mark!” to the existing content of the introduction.txt file.
- It checks whether the content of the introduction.txt file contains the line “Hello! My Name is Mark!”
- None of the above.
</Quiz>

__4. What do pipes allow you to do? (Select all that apply)__

<Quiz>
- Pipes let you take the output of one command and use it as the input for another.*
- Pipes allow you to combine multiple commands in a single line.*
- Pipes let you work on multiple files at the same time.
</Quiz>

__5. What command do you run if you are trying to identify where in the filesystem you are currently located/working? (Select all that apply)__

<Quiz>
- `$ pwd`*
- `$ ls`
- `$ cd`
- `$ whoami`
</Quiz>

__6. Let's think about the `grep` command. Select all that pertain to the command.__

<Quiz>
- It searches the given file for lines containing a match to the given strings or words.*
- It can be combined with other commands, so as to produce a search that matches their output.*
- It produces a new file with the lines containing the strings or words you are searching.
- It delete the strings or words you are searching from a file.
</Quiz>

__7. What is the difference between a plain text document and a rich text document? (Select all that apply)__

<Quiz>
- Plain text contains no formatting, only line breaks and spacing.*
- Rich text is styled text, i.e., plain text completed by information such as font size, format, and colors.*
- Plain text cannot be marked up.
- One can’t determine whether there is a difference between the two without looking at their content.
</Quiz>

**For further consideration**

- What are some of the operations that the command line allowed you to do today that you could have not performed with the Graphical User Interface? 
- What new information have you learned about your relationship with your machine in this workshop?

# Transferring knowledge to your computer

Now that you understand the CLI, you can apply this knowledge in your computer. 

As we mentioned, technology changes according to the available hardware. However, computers also changed according to the proprietary programs promoted by different companies such as Mac and Windows. As we saw with word processors, proprietary software implies terminals for command lines that are not necessarily equal for everyone. 

Thus, in this section, we help you get to the Command Line depending on the Operating System you use. We will talk about MacOS, Windows, and finally Linux.

## MacOS Users

If you're using macOS:
1. Click the Spotlight Search button (the magnifying glass) in the top right of your desktop.
2. Type “terminal” into the bar that appears.
3. Select the first item that appears in the list.
4. When the Terminal pops up, you will likely see either a window with black text over white background or colored text over a black background.

IMAGE of Terminal in macOS 

Please note: You can change the color of your Terminal or BashShell background and text by selecting Shell from the top menu bar, and then selecting a theme from the menu under New Window.

Bonus points: if you want to get the groove of just typing instead of pointing and clicking, you can hold the command (⌘) key and press space to pull up Spotlight search, start typing Terminal, and then hit enter to open a terminal window. This will pull up a terminal window without touching your mousepad. For super bonus points, try to navigate like this for the next fifteen minutes, or even the rest of this session—it is tricky and sometimes a bit tiring when you start, but you can pick up speed when you practice!

## Windows Users

Windows's own non-UNIX version of the command line. To use it:

1. Open the start menu or press the Windows key at the same time that the letter R. 
2. Type “cmd” and you will run the command box. 
3. Press enter
 
Another option for Windows users, if they want to use a UNIX version, is Git Bash. If you haven't installed it yet, you can follow these instructions. A reason to use Git Bash as the command line on Windows is to run the same commands as you would on a computer running macOS or Linux. Git Bash includes core utilities available on Linux that are not available on Windows.

After the installation:
1. Look for Git Bash in your programs menu and open it.
2. If you can't find the git folder, just type git bash in the search box and select git bash when it appears.
3. Open the program.
4. When the terminal pops up, you will likely see either a window with black text over a white background or colored text over a black background. You know you're in the right place when you see the $.
Note that the sign for you being in the right place might also be a % or a # depending on your operating system.

IMAGE of Terminal on Windows 

Bonus points: if you really want to get the groove of just typing instead of pointing and clicking, you can press windows to open the Start menu, start typing git bash, and then hit enter to open a git bash window. This will pull up a command window without touching your mousepad.

## Linux Users

The first option is to go to the applications menu. There will be a terminal icon. Click to launch it. 

The second option is to use the Search button (the magnifying glass) a, write “terminal”, “command”, “prompt” or “shell”. Launch the terminal. 

PENDIENTE IMAGEN

# Resources to continue learning

- Are you wondering how (else) the command line can be deployed for your scholarship? [Dennis Tenen and Grant Wythoff's "Sustainable Authorship in Plain Text using Pandoc and Markdown"](https://programminghistorian.org/en/lessons/sustainable-authorship-in-plain-text-using-pandoc-and-markdown) have some answers for you.
- [Stephen Ramsay](https://www.unl.edu/english/stephen-ramsay) is a scholar that has thought at length about the way the command line is (or can be!) embedded in a researcher's praxis. If you're interested in reading his work, here are two of his finest essays: ["Life on the Command Line"](https://files.zotero.net/eyJleHBpcmVzIjoxNTkyNjY1MDk3LCJoYXNoIjoiODFkNDJmZmU1ZjU3YzRmMDE2YTQ1ZmQwY2YzOTUwYmIiLCJjb250ZW50VHlwZSI6InRleHRcL2h0bWwiLCJjaGFyc2V0IjoidXRmLTgiLCJ6aXAiOjF9/07826342b83ea870f846cfa48f1b0eb8d3d51b78ceb1b05b1e014467d7241904/life-on-the-command-line.html) and ["Programming with Humanists: Reflections on Raising an Army of Hacker-Scholars in the Digital Humanities"](https://www.openbookpublishers.com/htmlreader/DHP/chap09.html)

**Other Tutorials**
- [*Data Science at the Command Line*](https://www.datascienceatthecommandline.com/) is an open access e-book by Jeroen Janssens, a hands-on guide that can help you become a more efficient and productive data scientist through the use of the command line.
- [BashGuide](http://mywiki.wooledge.org/BashGuide) offers some good practice techniques for taking your BASH skills to a higher level by teaching you write some simple scripts.

**Projects or Challenges to Try**
- [More command line challenges](https://github.com/DHRI-Curriculum/command-line/blob/main/sections/15-challenges.md) devised by the GCDI team are available here.
- When working with digital tools, it's usually a good idea to familiarize with their documentation. Here's the [Bash Reference Manual](https://www.gnu.org/savannah-checkouts/gnu/bash/manual/bash.html), where you can find Bash features for beginners and advanced users.
- [Pandoc](https://programminghistorian.org/en/lessons/sustainable-authorship-in-plain-text-using-pandoc-and-markdown) is an online software that allows users to convert file types through the command-line (from markdown to PDF, for example).
- [youtube-dl](https://ytdl-org.github.io/youtube-dl/index.html) is a command-line exercise to download videos from YouTube.com. It requires the Python interpreter.
- Feeling super brave? You might want to give [MALLET (MAchine Learning for LanguagE Toolkit)](http://mallet.cs.umass.edu/) a shot! MALLET is a "a Java-based package for statistical natural language processing, document classification, clustering, topic modeling, information extraction, and other machine learning applications to text." It includes tools for document classification, sequence tagging, topic modeling, and numerical optimization.
