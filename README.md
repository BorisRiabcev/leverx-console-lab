## LeverX Java Lab (Autumn 2021)
# leverx-console-lab
Practice in Java in Terminal
***
For doing this hometask I used the second hometask TicTacToe. This program is the game TicTacToe with 2 game mods: play with other human and play with computer 

***
In folder leverx-console-lab i have a folder Java. In folder Java I have a folder src. Main.java and Game.java are located in package com.riabcev.tasks

In folder leverx-console-lab/Java i am going to create a folder bin for .class files  

next command do it:
>mkdir Java/bin
***
For getting .class files is necessary to do next command on terminal:

>javac -sourcepath Java/src -d Java/bin Java/src/com/riabcev/tasks/Main.java
***

For execute our .class files I write the next command in my terminal window:

>java -classpath Java/bin com.riabcev.tasks.Main

After this command you can play TicTacToe in Terminal
***
Now let's try to create JAR file
#### Next command will create a JAR file without manifest-file:

>jar cf Main.jar -C Java/bin .
***

## And finally execute JAR file
### it was created without manifest-file, but this file was created automatically
#### But there is no any information about the main class, which contains main method
##### For execute this JAR file is necessary to indicate main class
##### This command will execute this JAR file:

> java -cp Main.jar com.riabcev.tasks.Main
***
After this you can play TicTacToe in Terminal again  
Have fun!
