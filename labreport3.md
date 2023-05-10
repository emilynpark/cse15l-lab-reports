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
the string "looms" regardless of case(therefore, all lines with words such as "LOOMS", "Looms", and "looMS") would be matched. Its output is useful for locating lines within the file containing a precise word/phrase that the user would like to look for.
<br>Source for this usage of `-i`: https://www.thegeekstuff.com/2009/03/15-practical-unix-grep-command-examples/</br>

<br>A second example of using `-i`:</br>
```
Emilys-MacBook-Pro-3:docsearch emilypark$ grep -i "ACCORD" technical/plos/journal.pbio.0020010.txt
        others to develop services that are more in accord with 2003 than 1993. One lesson Roger
```
This example shows an instance of displaying all the lines within the file `journal.pbio.0020010.txt` in the directory `technical/plos` that match the string "ACCORD" regardless of case. Its output is useful for locating lines within the file containing a precise word/phrase that the user would like to look for.
<br>Source for this usage of `-i`: https://www.thegeekstuff.com/2009/03/15-practical-unix-grep-command-examples/</br>

* `-A`
<br>`-A` is a command-line option of grep. Its purpose is to display the matched string/pattern, along with the specified number of lines following it.</br>
<br>One example of using `-A`:</br>
```
Emilys-MacBook-Pro-3:docsearch emilypark$ grep -A 3 -i "conclusion" technical/biomed/rr167.txt
        Conclusion
        Our studies demonstrate a correlation between protegrin
        sensitivity/resistance and protegrin binding in 
        P. aeruginosa and 
```
This example shows an instance of displaying the string "conclusion"(regardless of case as the `-i` command is also used), alongside the 3 lines following it, in the file rr167.txt located in the `technical/biomed` directory. This is useful when a user wants to view a certain number of lines following a given word or phrase in a line.
<br>Source for this usage of `-A`: https://www.thegeekstuff.com/2009/03/15-practical-unix-grep-command-examples/</br>

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
This example shows an instance of displaying the line with the string "Background", alongside the 5 lines following it, in the file `1468-6708-3-7.txt` located in the directory `technical/biomed`. In contrast to the first example, the case matters as the `-i` command isn't being used here. This is useful when a user wants to view a certain number of lines following a given word or phrase in a line.
<br>Source for this usage of `-A`: https://www.geeksforgeeks.org/grep-command-in-unixlinux/

* `-B`
<br>`-B` is a command-line option of grep. Its purpose is to display the matched string/pattern, along with the specified number of lines preceding it.</br>
<br>One example of using `-B`:</br>
```
Emilys-MacBook-Pro-3:docsearch emilypark$ grep -B 2 -i "SPONSORED" technical/biomed/1468-6708-3-10.txt
        The Antihypertensive and Lipid Lowering Treatment to
        Prevent Heart Attack Trial (ALLHAT) is a randomized,
        two-component clinical trial sponsored by the National
```
This example shows an instance of displaying the 
<br>A second example of using `-B`:</br>
```
Emilys-MacBook-Pro-3:docsearch emilypark$ grep -B 1 "mammals" technical/biomed/1471-213X-1-1.txt
        the inhibitory neurotransmitter γ-amino butyric acid (GABA)
        from glutamate. In mammals, the two isoforms of this
```
