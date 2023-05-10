# Lab Report 3

I am choosing to focus on the command `grep`.

Four interesting

* `-n`
<br>`-n` is a command-line option of grep. Its purpose is to precede each line matching a given pattern/string with a line number.</br>
<br>One example of using `-n`:</br>

```
Emilys-MacBook-Pro-3:docsearch emilypark$ grep -n "Boarding" technical/911report/chapter-1.txt
12:Boarding the Flights
```

This example shows an instance of displaying the line number of all lines within the file `chapter-1.txt`(accessed with the directory
of `technical/911report/chapter-1.txt`) matching the string "Boarding." Its output shows that line 12, which contains the string "Boarding the Flights," is a match.
<br>Source for this usage of `-n`: https://www.thegeekstuff.com/2009/03/15-practical-unix-grep-command-examples/</br>

<br>A second example of using `n`:</br>


of locating entries within a given file system.
* `-i`
<br>`-i` is a command-line option of grep. Its purpose is to locate all lines within a file that match the given string/pattern, regardless of 
if its uppercase or lowercase.</br>
<br>One example of using `-i`:</br>
```
Emilys-MacBook-Pro-3:docsearch emilypark$ grep -i "Manipulated" technical/911report/chapter-1.txt
  On the morning of 9/11, there were only 37 passengers on United 93-33 in addition to the 4 hijackers. This was below the norm for Tuesday mornings during the summer of 2001. But there is no evidence that the hijackers manipulated passenger levels or purchased additional seats to facilitate their operation.
```
