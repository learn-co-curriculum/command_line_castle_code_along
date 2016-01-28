
##Use the command line to save the princess!

###The saga begins
A beautiful princess has been taken prisoner in the castle tower, and it's your mission to save her. Are you up for the task?

###Get oriented with pwd
<img src="http://images.rapgenius.com/c3289a78cba7c49e8b0111629e9d727c.528x704x1.jpg" height="300" align="right" hspace="20"> To start, open terminal. You'll begin in your home directory, which is the topmost `directory` for the computer's current user. A directory is another name for a folder. To make sure you're actually there, type `pwd`. `pwd` stands for "Present Working Directory" or, more simply, "Tell me where I am!" You should see something like `/Users/victoriafriedman` but with your user name. Now you need to enter the territory ruled by the castle, and because this is fairy tale land, we're going to need to create that territory.

###Make directories with mkdir
Create a directory called `territory`. To do this, you'll use the command `mkdir`. This command is self-explanatory. It means "make directory". You need to follow the command with the name of the directory, so here we type `mkdir territory`.

Spaces separate values of commands, so the space is really important here. You can even use it to create more than one directory at once. `mkdir territory evil_swamp` makes two directories: `territory` and `evil_swamp`. If we used a space in `evil_swamp` instead of the underscore, it would have created three directories. So be sure to use the underscore if you want to use two words to name one directory. 

###Check your contents with ls
Now check to make sure the territory directory exists. `ls` is the command that lists the contents of a directory. Note that we created territory in our root directory, so you will see a lot of other files and directories listed along with `territory`. Think of `ls` as binoculars for you to use to check out your surroundings.

###Change into a directory with cd
<img src="http://upload.wikimedia.org/wikipedia/commons/5/56/Tavern_Scene-1658-David_Teniers_II.jpg" width="300" align="right" hspace="20">Now you need to travel forth into the territory. To travel about our directories, use `cd`. So to go into the territory, enter `cd territory`.

So now what? Since this is our fairy tale, create a tavern where we can ask for help. Yep, this means you'll have to make another directory with `mkdir tavern`. You have to enter the tavern in order to ask for directions to the castle. You don't want to be rude and just stand outside shouting, so `cd tavern`.

###Create a file with touch
Create a wise man who can answer our questions. We're going to create a file now, and enter his directions into that file. `touch` is the command to create a file. We'll enter `touch wiseman.txt`. Enter `ls` to prove the wiseman has been created.

###Open a file with open
Now you need to open the text file you created, `open wiseman.txt`. Enter these directions into the text file: "The princess is in the castle by the lake, just through the spiny forest" Don't forget to save your changes!

###Get out of a directory with cd ..
You thank the wiseman and head out on your way. First you have to leave the tavern and head back out into the territory. The `territory` directory is the parent directory of `tavern`. It holds `tavern` inside it like a baby. In other words, `tavern` is a child of `territory`. In order to move into a parent directory, type `cd ..` The `..` basically means, "Take me back one level."" Check your location with `pwd` just to be sure.

So now you know you need to go through the Spiney Forest, which first means in it, and then out of it. Create your Spiney Forest with `mkdir spiney_forest` and then move into it `cd spiney_forest`. But OH NO! You encounter a DRAGON! Create him and then see what he has to say with `touch dragon.txt`. Open the text file with `open dragon.txt` and type, "I can breath fire, so beware. Put me in my cage if you dare."

###Moving around with mv
<img src="http://th01.deviantart.net/fs70/200H/i/2014/129/8/b/hungry_dragon_by_mourri-d7hp8fg.jpg" width="300" align="right" hspace="20"> Create the dragon's cage `mkdir dragon_cage`. And now move the dragon into his cage. I bet he didn't think it would be this simple: `mv dragon.txt dragon_cage`. The first argument `dragon.txt`, is the file you're moving and the second argument, `dragon_cage`, is the location you want to move it to. Check the contents of spiney_forest with `ls`. You should only see the cage. If you `cd dragon_cage` and then `ls` you'll see the dragon is put in his place!

###Copy copy copy with cp
Back in the spiney_forest, you start to get a little hungry. Thankfully you come across an apple. Make the apple with `touch apple.txt`. This apple is golden and delicious and you're hungry from more apples. You can use your own magic powers to duplicate it. `cp` is the command to copy something. You can easily copy something to another directory similarly to how you use the mv. If you wanted to give the dragon an apple, enter `cp apple.txt dragon_cage`. Or say you wanted to duplicate apple and rename it apple2, enter `cp apple.txt ./apple2.txt`. To rename something when you copy it, you just change the name in the last argument when you indicate where you want it to go. The `./` indicates the current directory.

###Remove a file with rm
Because the dragon wanted to kill you, you should take away his apple to punish him. Use `rm` to remove things. To remove the apple from the dragon's cage, type `rm dragon_cage/apple.txt`. You have to list the cage directory name so it knows where to go. `rm` won't delete entire directories automatically. There are special flags for that. Go ahead and use this newfound power to get rid of the dragon for good!

###Remove a directory with rm -r
`rm -r dragon_cage` The `-r` is a flag that means recursive. A recursive action is one that gets repeated. In this case, the command will call remove on everything inside `dragon_cage` until only the directory is left, and then it'll remove that, too. You'll want to be careful with using the `-r` flag, especially if you're in your root directory. Imagine deleting everything on your computer!

<img src="http://th08.deviantart.net/fs48/PRE/f/2009/216/f/6/Saved_Princess___DO_NOT_FAVE_by_peach_club.png" width="250" align="left" hspace="20">So now, all you need to do is get to the castle! Create it first with `mkdir castle`. Then go into it with `cd castle`. Now you need to create the tower with `mkdir tower` and go into it to find the Princess with `cd tower`. Now create the beautiful princess with `touch princess.txt`. Open `princess.txt`. 

The princess is so grateful for you saving her! Enter "Oh you're my hero!!! I don't know how I'll ever repay you!!! I love you!!!" into the text file and save. Give her a girl's voice and listen as she thanks you for rescuing her with. You saved the day!





<p data-visibility='hidden'>View <a href='https://learn.co/lessons/command_line_castle_code_along' title='Use the command line to save the princess!'>Use the command line to save the princess!</a> on Learn.co and start learning to code for free.</p>
