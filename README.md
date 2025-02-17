# In Class Problem Set 3
# Oliwia Majtyka, Michael Ojo

I used ComboBoxDemo.java a few years ago.  It used to compile cleanly.  Even though the code has not changed, it now  will not compile without throwing warnings.

Doing everything from a command prompt or Git Bash (no IDEs allowed), your mission is to debug the code and find out why it stopped compiling cleanly.  When you have figured it out,  note what you changed and why it stopped working in the README.md file.


**Changes to code**
We added a generic type <String> because JComboBox is a raw type. References to generic type JComboBox<E> should be parameterized. 


**What caused it to stop working?**
The reason older Java versions allowed JComboBox to be declared without specifying a generic type and newer versions show warnings is due to generics enforcement and raw type warnings introduced in later Java versions. Adding generic type ensures that only String values are allowed and avoids potential runtime errors.
