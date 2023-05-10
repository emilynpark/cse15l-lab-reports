# Lab Report 3

I am choosing to focus on the command `grep`.

Four interesting command-line options of `grep`:

* `-n`
<br>`-n` is a command-line option of grep. Its purpose is to precede each line matching/containing a given pattern/string with a line number.</br>
<br>One example of using `-n`:</br>

```
Emilys-MacBook-Pro-3:docsearch emilypark$ grep -n "Boarding" technical/911report/chapter-1.txt
12:Boarding the Flights
```

This example shows an instance of displaying the line number of all lines within the file `chapter-1.txt`(accessed within the `technical/911report` directory) matching/containing the string "Boarding." Its output is useful in showing that line 12, which contains the string "Boarding the Flights," is a match.
<br>Source for this usage of `-n`: https://www.thegeekstuff.com/2009/03/15-practical-unix-grep-command-examples/</br>

<br>A second example of using `-n`:</br>

```
Emilys-MacBook-Pro-3:docsearch emilypark$ grep -n "Abbreviations" technical/biomed/1468-6708-3-3.txt
284:        Abbreviations
```
This example shows another instance of displaying the line number of all lines within the file `1468-6708-3-3.txt`(accessed within the directory of `technical/biomed`) matching/containing the string "Abbreviations." Its output is useful in showing the number of the line that contains the word "Abbreviations" is 284.
<br>Source for this usage of `-n`: https://www.geeksforgeeks.org/grep-command-in-unixlinux/</br>

* `-i`
<br>`-i` is a command-line option of grep. Its purpose is to locate all lines within a file that match the given string/pattern, regardless of if its uppercase or lowercase.</br>
<br>One example of using `-i`:</br>
```
Emilys-MacBook-Pro-3:docsearch emilypark$ grep -i "looms" technical/911report/chapter-7.txt
            THE ATTACK LOOMS
```
This example shows an instance of displaying all lines within the file `chapter-7.txt` in the directory `technical/911report` that match
the line `looms` regardless of case(therefore, all lines with words such as "LOOMS", "Looms", and "looMS") would be matched.
<br>Source for this usage of `-i`: https://www.thegeekstuff.com/2009/03/15-practical-unix-grep-command-examples/</br>

<br>A second example of using `-i`:</br>
```
Emilys-MacBook-Pro-3:docsearch emilypark$ grep -i "ACCORD" technical/plos/journal.pbio.0020010.txt
        others to develop services that are more in accord with 2003 than 1993. One lesson Roger
```


* `-A`
<br>`-A` is a command-line option of grep. Its purpose is to display the specified number of lines following the matched string/pattern.</br>
<br>One example of using `-A`:</br>
```
Emilys-MacBook-Pro-3:docsearch emilypark$ grep -A 3 -i "conclusion" technical/biomed/rr167.txt
        Conclusion
        Our studies demonstrate a correlation between protegrin
        sensitivity/resistance and protegrin binding in 
        P. aeruginosa and 
```
This example shows an instance of displaying the 3 lines following the line with the string "conclusion"(regardless of case as the `-i` command is also used) in the file rr167.txt located in the `technical/biomed` directory. This is useful when a user wants to view a certain number of lines following a given word or phrase in a line.
<br>Source for this usage of `-A`: https://www.geeksforgeeks.org/grep-command-in-unixlinux/</br>

<br>A second example of using `-A`:</br>
```
Emilys-MacBook-Pro-3:docsearch emilypark$ grep -A 5 "Background" technical/biomed/1468-6708-3-7.txt
        Background
        With the publication of the Antihypertensive and
        Lipid-Lowering Treatment to prevent Heart Attack Trial
        (ALLHAT), the role of peripheral alpha-1 antagonists in the
        treatment of hypertension has become controversial. The
        doxazosin arm of ALLHAT was stopped early, due to a
```
