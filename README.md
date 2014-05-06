##Terminal
Terminal is what your computer looked like before your desktop was created. The desktop we all know is a GUI, which stands for "Graphical User Interface". The terminal screen can seem intimidating, so in order to make computers more user friendly, the desktop was created, and all of its icons.


Let's go ahead an open terminal. You're going to be in your root directory, which basically is the very base of your entire computer. To make sure we're actually there, let's go ahead and check. We're going to type `pwd`. `pwd` stands for "Print Working Directory" A directory is the exact same thing as a folder. If you enter `pwd` you should see something like `/Users/victoriafriedman` but with your name.


##Let's use command line to save the Princess from the castle tower where she is being held prisoner! 


We're going to need to enter the territory ruled by the castle, and because this is fairy-tale land, we're going to need to create that territory.

To make the territory, we'll need to create a directory called `territory`. We do that by using the command `mkdir`. This command stands for "make directory". You need to follow the command by the name of the directory, so here we type `mkdir territory`

Spaces separate values of commands, so the space is really important here. You can even use it to create more than one directory at once, `mkdir territory evil_swamp` makes two directories: `territory` and `evil_swamp`. If we used a space in `evil_swamp` instead of the underscore, it would have created three directories. 

So let's make sure the territory directory exists. `ls` is the command that lists the contents of a directory. Note that we created territory in our root directory, so you will see a lot of other files and directories listed along with `territory`. Think of `ls` as binoculars for you to use to check out his surroundings.

Now you need to travel forth into the territory. To travel about our directories, we use `cd`. So to go into the territory, we enter `cd territory`. 

So now what? we're in this big land. Since this is our fairy tale, let's create a tavern where we can ask for help. Yepp, this means we'll have to make another directory. `mkdir tavern`.

We have to enter the tavern in order to ask for directions to the castle. We don't want to be rude and just stand outside and shout, so let's `cd tavern`.

Let's create a wise man who can answer our questions. We're going to create a file now, and enter his directions into the file. `Touch` is the command to create a file. We'll enter `touch wiseman.txt`.
`ls` will prove the wiseman has been created.

Now we need to open the text file we created, `open wiseman.txt`.

Let's enter directions into the text file. "The princess is in the castle by the lake, just through the spiny forest" Save those changes to your file.

Now we need the wiseman to actually tell us those directions. `say -f wiseman.txt`
The `-f` is a flag that passes an option to the say command. If you want the wiseman to have a different voice, you can enter a few options, Bruce, Vicki, Alex, Fred, Kathy, or Victoria. You do that by entering `say -f wiseman.txt -v Bruce` The order really matters here, it wouldn't read the file name if you put it after Bruce.

We thank the wiseman, and head out on our way. So first we have to leave the tavern and head back out into the territory. The `territory` directory is the parent directory of `tavern`. It is the directory that holds `tavern`. You can also call `tavern` a child of `territory`. In order to move into a parent directory, we type `cd ..` The `..` basically means take me back one level. Why don't we check our location with `pwd` just to be sure.

So now we know we need to go through the Spiney Forest, which first means in it, and then out of it. Let's create our Spiney Forest `mkdir spiney_forest` and then move into it `cd spiney_forest` But OH NO. We encounter a DRAGON! Let's create him and then see what he has to say. `touch dragon.txt` 

Let's open the text file `open dragon.txt` and type, "I can breath fire, so beware. Put me in my cage if you dare." And then let him speak `say -f dragon.txt` 

Let's create the dragon's cage `mkdir dragon_cage`. And now let's move the dragon into his cage. I bet he didn't think it would be this simple: `mv dragon.txt cage`. If we check the contents of spiney_forest `ls`, we'll only see the cage. If we `cd dragon_cage` and then `ls` we'll see the dragon is put in his place!

Back in the spiney_forest, we start to get a little hungry. So we come across an apple. Let's make the apple, `touch apple.txt`. This apple isn't like other fairy-tales, this one is ok to eat. And actually, we can even use our own magic powers to duplicate it.  `cp` is the command to copy something. You can easy copy something to another directory, maybe if we wanted to give the dragon and apple `cp apple.txt cage`. OR let's say we wanted to duplicate apple and rename it apple2, so we know we have two of them. `cp apple.txt ./apple2.txt`. To rename something, you just change the name along with exactly where you want it to go. The `./` indicates the current directory.

Because the dragon wanted to kill us, we should really take away his apple. We use `rm` to remove things. To remove the apple from the dragon's cage, we'd type `rm cage/apple.txt` We have to list the cage directory name so it knows where to go. `rm` won't delete entire directories automatically. There are special flags for that. Let's go ahead and use this newfound powers to get rid of the dragon for good!

`rm -r cage` The `-r` is a flag that means recurisve. It will call remove on everything in `cage` until only the directory is left, and then remove that too. You'll want to be careful with using the `-r` flag, especially if you're in your root directory. Imagine deleting everything on your computer!!

So now, all we need to do is get to the castle!! Let's create it first, `mkdir castle`. And then go in to it, `cd castle`. And now we need to get in the tower, `mkdir tower` and go in the tower to find the Princess `cd tower`. Now let's create our beautiful princess `touch princess.txt`. Open `princess.txt`. 

And type "Oh you're my hero!!! I don't know how I'll ever repay you!!! I love you!!!"

And let's give her a girl's voice `say -f princess.txt -v Victoria`

Congratulations! You saved the Princess!!




