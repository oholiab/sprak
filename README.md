Sprak
=====
> Utility code for the Sprak programming language from the game [else
> Heart.Break()](http://store.steampowered.com/app/400110/Else_HeartBreak/)

Come again?
-----------
In the game 'else Heart.BreaK()' one of the core mechanics of the game is
interacting with computers and items in the game using the fictional Sprak
programming language

I'm on my second playthrough of the game and thought I'd put some of my
overenginneerd solutions in a git repository.

Files
-----
At the moment there's only one file - `sebOS.sprak`

This is a program which comes with a paired floppy disk. Whichever host machine
you're running it on, create a floppy with the following code:

```
var c = Connect("<your_host>")
c.StoreServer(Name())
```

Then on any machine you come across, with the disk in hand, issue:

```
BootFromFloppy()
```

and it will register itself in your host machine's memory so that you can
enumerate and connect to various machines.
