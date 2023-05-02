Download Link: https://assignmentchef.com/product/solved-comp9044-test-7-three-vowel-echo
<br>
Write a Perl program three_vowel_echo.pl that prints its command-line argument to standard output, similar to echo command in Shell, except arguments should be printed only if they contain 3 consecutive vowels.

Your program can assume vowels are there are 5 vowel {‘a’, ‘e’, ‘i’, ‘o’, ‘u’} and their upper-case equivalents {‘A’, ‘E’, ‘I’, ‘O’, ‘U’} Your answer must be Perl only. You can not use other languages such as Shell, Python or C.

You may not run external programs, e.g. via system or backquotes.

$ <strong>./three_vowel_echo.pl Pompeii Rome Aeolian Florence</strong>

Pompeii Aeolian

$ <strong>./three_vowel_echo.pl</strong>

$ <strong>./three_vowel_echo.pl an anxious bedouin beauty booed an ancient zoologist</strong> anxious bedouin beauty booed

$ <strong>./three_vowel_echo.pl abstemiously adenocarcinomatous Hawaiian Eoanthropus</strong> abstemiously Hawaiian Eoanthropus

Wh               thi k                           i          ki                                       t                       i      l        t         t d t     t

When you think your program is working you can autotest to run some simple automated tests:

$ <strong>2041 autotest three_vowel_echo</strong>

When you are finished working on this exercise you must submit your work by running give:

$ <strong>give cs2041 test07_three_vowel_echo three_vowel_echo.pl</strong>

Write a Perl program middle_lines.pl which prints the middle line(s) in a file.

If the file contains an odd number of lines it should print one line.

If the file contains an even number of lines it should print two lines.

If the file contains no lines it should print nothing.

You can assume one and only one file is given as argument and that it exists and it is readable.

For example:

<table width="961">

 <tbody>

  <tr>

   <td width="961">$ <strong>cat odd.txt</strong> line 0 line 1 line 2 line 3 line 4$ <strong>./middle_lines.pl odd.txt</strong> line 2$ <strong>cat even.txt</strong> line 0 line 1 line 2 line 3 line 4 line 5$ <strong>./middle_lines.pl even.txt</strong> line 2 line 3$ <strong>./middle_lines.pl /dev/null</strong></td>

  </tr>

 </tbody>

</table>

Your answer must be Perl only. You can not use other languages such as Shell, Python or C.

You may not run external programs, e.g. via system or backquotes.

When you think your program is working you can autotest to run some simple automated tests:

$ <strong>2041 autotest middle_lines</strong>

When you are finished working on this exercise you must submit your work by running give:

$ <strong>give cs2041 test07_middle_lines middle_lines.pl</strong>

  :

<h1>Print the Line(s) from Stdin With the Largest Number</h1>

Write a Perl program largest_numbered_line.pl that read lines from standardinput until end-of-input. It should then print the line(s) which contained the largest number.

You can assume numbers do not contain white space, commas or other extra characters.

You can assume numbers are only in decimal format.

You can assume numbers are not in scientific/exponential format.

Lines may contain multiple numbers and they may contain any number of any character between the numbers.

If the largest number occurs on multiple lines you should print all of the lines in the order they occurred.

If no line contains a number, your program should print nothing.

<table width="961">

 <tbody>

  <tr>

   <td width="961">$ <strong>./largest_numbered_line.pl</strong><strong>I spent $ 15.50 for </strong><strong>3.3 kg apples yesterday. </strong><strong>2000 is a leap year. </strong><em>Ctrl-D                      </em>2000 is a leap year.</td>

  </tr>

  <tr>

   <td width="961">$ <strong>./largest_numbered_line.pl</strong> <strong>two2 four4 eight8 sixteen16 </strong><strong>1 sixteen-and-half 16.5  1 </strong><strong>11 12 13 </strong><em>Ctrl-D                      </em>1 sixteen-and-half 16.5  1</td>

  </tr>

  <tr>

   <td width="961">$ <strong>./largest_numbered_line.pl</strong> <strong>the quick brown f42ox</strong><strong>4 9 42 2 4 1 2 3 4 42.0 no forty two last 42</strong><em>Ctrl-D                      </em>the quick brown f42ox4 9 42 2 4 1 2 3 4 42.0 last 42</td>

  </tr>

  <tr>

   <td width="961">$ <strong>./largest_numbered_line.pl</strong> <strong>a 0.01 b .5 c -0.9 </strong><em>Ctrl-D    </em> b .5</td>

  </tr>

  <tr>

   <td width="961">$ <strong>./largest_numbered_line.pl</strong> <strong>a -.5 b -5 c –90– </strong><em>Ctrl-D                      </em>a -.5</td>

  </tr>

  <tr>

   <td width="961">$ <strong>./largest_numbered_line.pl</strong> <strong>I love programming in Perl but I like Python better. </strong><em>Ctrl-D                      </em></td>

  </tr>

 </tbody>

</table>

Your answer must be Perl only. You can not use other languages such as Shell, Python or C.

You may not run external programs, e.g. via system or backquotes.

When you think your program is working you can autotest to run some simple automated tests:

$ <strong>2041 autotest largest_numbered_line</strong>

When you are finished working on this exercise you must submit your work by running give:

$ <strong>give cs2041 test07_largest_numbered_line largest_numbered_line.pl</strong>