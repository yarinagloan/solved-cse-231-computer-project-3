Download Link: https://assignmentchef.com/product/solved-cse-231-computer-project-3
<br>
<h2>Assignment Overview</h2>

<strong> </strong>

This assignment focuses on the design, implementation and testing of a Python program to compute tuition charges at MSU (see below).

<h2>Assignment Deliverable</h2>




The deliverable for this assignment is the following file:




proj03.py – the source code for your Python program




Be sure to use the specified file name and to submit it for grading via the <strong>Mimir</strong> <strong>system</strong> before the project deadline.




<h2>Assignment Background</h2>

<strong> </strong>

MSU has an on-line tuition calculator:




<u>http://ctlr.msu.edu/COStudentAccounts/TuitionCalculatorFall.aspx</u>




That calculator is based on information such as that posted at:




<u>http://ctlr.msu.edu/COStudentAccounts/Tuition_FeesResident_Undergrad_2019-20.aspx</u>




<h2>Assignment Specifications</h2>

<strong> </strong>

<ol>

 <li>You will develop a Python program which calculates the tuition for an undergraduate MSU student during Fall Semester 2019, based on parameters supplied by the user (such as the student’s residency status and class level).</li>

</ol>




<ol start="2">

 <li>Your program will permit mixed-case input strings. For example, the strings “yes”, “Yes”, “YES” and “yES” will all be processed by your program as equivalent user inputs.</li>

</ol>




<ol start="3">

 <li>The calculated tuition will be displayed with a dollar sign ($) and commas for the thousands. That is, a value of 12345.67 will be displayed as $12,345.67 by your program.  Also, even dollar amounts will have zeros for cents (for example, a value of 12 will be displayed as</li>

</ol>

$12.00).










<ol start="4">

 <li>The following tables give the necessary values.</li>

</ol>




<table width="623">

 <tbody>

  <tr>

   <td rowspan="2" width="90"><strong>College and year </strong></td>

   <td colspan="3" width="265"><strong>Resident </strong></td>

   <td colspan="3" width="267"><strong>Non-Resident &amp; International </strong></td>

  </tr>

  <tr>

   <td width="88">Per Credit (111)</td>

   <td width="89">Flat Rate (1218)</td>

   <td width="88">Flat + Credit (&gt;18)</td>

   <td width="90">Per Credit (1-11)</td>

   <td width="89">Flat Rate (1218)</td>

   <td width="88">Flat + Credit (&gt;18)</td>

  </tr>

  <tr>

   <td colspan="4" width="356">Core Units</td>

   <td colspan="3" width="267"></td>

  </tr>

  <tr>

   <td width="90">Freshman</td>

   <td width="88">$482</td>

   <td width="89">$7,230</td>

   <td width="88">Flat + credit</td>

   <td width="90">$1,325.50</td>

   <td width="89">$19,883</td>

   <td width="88">Flat + credit</td>

  </tr>

  <tr>

   <td width="90">Sophomore</td>

   <td width="88">$494</td>

   <td width="89">$7,410</td>

   <td width="88">Flat + credit</td>

   <td width="90">$1,325.50</td>

   <td width="89">$19,883</td>

   <td width="88">Flat + credit</td>

  </tr>

  <tr>

   <td width="90">Junior</td>

   <td width="88">$555</td>

   <td width="89">$8,325</td>

   <td width="88">Flat + credit</td>

   <td width="90">$1,366.75</td>

   <td width="89">$20,501</td>

   <td width="88">Flat + credit</td>

  </tr>

  <tr>

   <td width="90">Senior</td>

   <td width="88">$555</td>

   <td width="89">$8,325</td>

   <td width="88">Flat + credit</td>

   <td width="90">$1,366.75</td>

   <td width="89">$20,501</td>

   <td width="88">Flat + credit</td>

  </tr>

  <tr>

   <td colspan="4" width="356">Eli Broad College of Business &amp; College of Engineering</td>

   <td colspan="3" width="267"></td>

  </tr>

  <tr>

   <td width="90">Freshman</td>

   <td width="88">$482</td>

   <td width="89">$7,230</td>

   <td width="88">Flat + credit</td>

   <td width="90">$1,325.50</td>

   <td width="89">$19,883</td>

   <td width="88">Flat + credit</td>

  </tr>

  <tr>

   <td width="90">Sophomore</td>

   <td width="88">$494</td>

   <td width="89">$7,410</td>

   <td width="88">Flat + credit</td>

   <td width="90">$1,325.50</td>

   <td width="89">$19,883</td>

   <td width="88">Flat + credit</td>

  </tr>

  <tr>

   <td width="90">Junior</td>

   <td width="88">$573</td>

   <td width="89">$8,595</td>

   <td width="88">Flat + credit</td>

   <td width="90">$1,385.75</td>

   <td width="89">$20,786</td>

   <td width="88">Flat + credit</td>

  </tr>

  <tr>

   <td width="90">Senior</td>

   <td width="88">$573</td>

   <td width="89">$8,595</td>

   <td width="88">Flat + credit</td>

   <td width="90">$1,385.75</td>

   <td width="89">$20,786</td>

   <td width="88">Flat + credit</td>

  </tr>

 </tbody>

</table>







<table width="624">

 <tbody>

  <tr>

   <td width="211"></td>

   <td width="207"><strong>Special Fees (per semester) </strong></td>

   <td width="206"></td>

  </tr>

  <tr>

   <td width="211"><strong> </strong></td>

   <td width="207"><strong>Part-Time (4 credits or fewer) </strong></td>

   <td width="206"><strong>Full-Time </strong></td>

  </tr>

  <tr>

   <td width="211">Business – juniors and seniors</td>

   <td width="207">$113</td>

   <td width="206">$226</td>

  </tr>

  <tr>

   <td width="211">Engineering – admitted</td>

   <td width="207">$402</td>

   <td width="206">$670</td>

  </tr>

  <tr>

   <td width="211">Health – juniors and seniors</td>

   <td width="207">$50</td>

   <td width="206">$100</td>

  </tr>

  <tr>

   <td width="211">Sciences – juniors and seniors</td>

   <td width="207">$50</td>

   <td width="206">$100</td>

  </tr>

  <tr>

   <td width="211">CMSE – juniors and seniors</td>

   <td width="207">$402</td>

   <td width="206">$670</td>

  </tr>

  <tr>

   <td width="211">International</td>

   <td width="207">$375</td>

   <td width="206">$750</td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<table width="637">

 <tbody>

  <tr>

   <td colspan="2" width="460"><strong>Student-Voted Taxes (per semester) </strong></td>

   <td width="177"></td>

  </tr>

  <tr>

   <td width="340">ASMSU Tax – all undergraduate students</td>

   <td width="120"></td>

   <td width="177">$21</td>

  </tr>

  <tr>

   <td width="340">FM Radio Tax – all students</td>

   <td width="120"></td>

   <td width="177">$3</td>

  </tr>

  <tr>

   <td width="340">State News Tax – all students with 6 or more credits</td>

   <td width="120"></td>

   <td width="177">$5</td>

  </tr>

  <tr>

   <td width="340">James Madison College Student Senate Tax – all students in James Madison College</td>

   <td width="120"></td>

   <td width="177">$7.50</td>

  </tr>

 </tbody>

</table>







<ol start="5">

 <li>“flat + credit”: Students taking more than 18 credits calculate their tuition by starting with the flat fee and adding on the specified per-credit for each credit greater than 18. For example, a student taking 20 credits pays the flat rate plus 2*(per-credit).  The “per-credit” value is the value in the “per-credit (1-11) column.</li>

</ol>




<ol start="6">

 <li><strong>Input Specification and Ordering</strong>: To facilitate grading the input must be in the following order:

  <ol>

   <li>Resident (yes/no):</li>

   <li>If not resident, International (yes/no):</li>

   <li>Enter Level as freshman, sophomore, junior, senior:</li>

   <li>If level is junior or senior, ask for College.</li>

  </ol></li>

</ol>

College—business, engineering, health, sciences, none:

<ol>

 <li>If level is junior or senior ask if major is CMSE (“Computational Mathematics and Engineering”) (yes/no)</li>

 <li>If level is freshman or sophomore, ask if admitted to College of Engineering (yes/no):</li>

 <li>If college not business, engineering, health or sciences, ask if James Madison</li>

</ol>

College (yes/no)

<ol>

 <li>Credits</li>

 <li>Ask if the user wants to do another calculation.</li>

</ol>




<h2>Assignment Notes</h2>




<ol>

 <li>To clarify the project specifications, sample output is provided at the end of this document.</li>

</ol>




<ol start="2">

 <li>Your program must accept user inputs in the order specified.</li>

</ol>




<ol start="3">

 <li>Python 3 provides formatting for the dollar output. A comma (,) causes commas to be properly placed in numbers.  Note that the ordering matters so that comma is placed immediately after the colon and before other formatting marks, e.g. {:,.2f}  Experiment in the shell.</li>

</ol>




<ol start="4">

 <li>The string method lower() can be used to convert all letters in a string to lower case. This is particularly useful for input, that is you can handle “yEs”, “yeS”, “YEs”, etc by converting the input to lower case and checking against “yes”.</li>

</ol>




<ol start="5">

 <li>The Python None is a useful default initialization for variables that may not be assigned a value. For example, not everyone is asked for their college so initializing college to None can be handy because None evaluates as False in a Boolean expression.</li>

</ol>

college = None    if college:

print(“this will not print if college has the value None”)




<ol start="6">

 <li>Notes on handling input errors:

  <ul>

   <li>For “yes/no” questions, assign all answers that are <strong>not</strong> “yes” to be “no” .</li>

   <li>For the question about college that has an option of “none”, assign any answer to be “none” (or None, if you wish) for any response that is <strong>not</strong> one of the specified colleges.</li>

   <li>For level, if the answer is <strong>not</strong> one of the specified responses (“freshman”, etc.), you must print an error message “Invalid input. Try again.” and re-prompt until you get a specified response.</li>

   <li>For credits, input must be an integer greater than zero. Print an error message “Invalid input. Try again.” and re-prompt until you get an integer greater than zero.  Hint:</li>

  </ul></li>

</ol>

the string isdigit() method useful here.




<ol start="7">

 <li>Common error to avoid. You might like to use a Boolean expression such as this:</li>

</ol>

level == ‘freshman’ or ‘sophomore’ or ‘junior’ or ‘senior’

Unfortunately, that expression always evaluates to True because any non-empty string is

True so it is effectively: level == ‘freshman’ or True or True or True

Instead use the following

(level == ‘freshman’) or (level == ‘sophomore’) \ or (level == ‘junior’) or (level == ‘senior’)







<ol start="8">

 <li>You are responsible for following the coding standard items 1-6</li>

</ol>




<ol start="9">

 <li>You are not allowed to use advanced data structures such as list, dictionaries, classes, etc. However, you are allowed to read ahead and use try-except and functions.</li>

</ol>




<ul>

 <li>“Hard-coded answers” will receive a zero score for the project. That is, if you design your code to handle the specific test cases rather than the general problem, you will not get credit.</li>

</ul>




<h2>Sample Output</h2>




<h3>TEST 1</h3>




2019 MSU Undergraduate Tuition Calculator.




Resident (yes/no): yes

Enter Level as freshman, sophomore, junior, senior: freshman

Are you admitted to the College of Engineering (yes/no): no

Are you in the James Madison College (yes/no): no

Credits: 12

Tuition is $7,259.00.

Do you want to do another calculation (yes/no): no




<h3>TEST 2</h3>




2019 MSU Undergraduate Tuition Calculator.




Resident (yes/no): yes

Enter Level as freshman, sophomore, junior, senior: Junior Enter college as business, engineering, health, sciences, or none: business

Is your major CMSE (“Computational Mathematics and Engineering”)

(yes/no): No

Credits: 17

Tuition is $8,850.00.

Do you want to do another calculation (yes/no): no




<h3>TEST 3</h3>




2019 MSU Undergraduate Tuition Calculator.




Resident (yes/no): yEs

Enter Level as freshman, sophomore, junior, senior: Senior Enter college as business, engineering, health, sciences, or none: engineering

Is your major CMSE (“Computational Mathematics and Engineering”)

(yes/no): no

Credits: 5

Tuition is $3,559.00.

Do you want to do another calculation (yes/no): Yes

Resident (yes/no): nO

International (yes/no): yes

Enter Level as freshman, sophomore, junior, senior: sophomore

Are you admitted to the College of Engineering (yes/no): yes

Credits: 20

Tuition is $23,983.00.

Do you want to do another calculation (yes/no): no







<h3>TEST 4</h3>




2019 MSU Undergraduate Tuition Calculator.




Resident (yes/no): yes

Enter Level as freshman, sophomore, junior, senior: xxx

Invalid input. Try again.

Enter Level as freshman, sophomore, junior, senior: yyy

Invalid input. Try again.

Enter Level as freshman, sophomore, junior, senior: junior Enter college as business, engineering, health, sciences, or none: abcd

Is your major CMSE (“Computational Mathematics and Engineering”)

(yes/no): yes

Are you in the James Madison College (yes/no): no

Credits: 0

Invalid input. Try again.

Credits: ab

Invalid input. Try again.

Credits: 3.5

Invalid input. Try again.

Credits: 11

Tuition is $6,804.00.

Do you want to do another calculation (yes/no): no




<strong>Grading Rubric </strong>




Computer Project #3

Scoring Summary




General Requirements:

(4 pts)         Coding Standard 1-6

(descriptive comments, mnemonic identifiers, format, etc…)







Implementations:




(4 pts) Test 1

(4 pts) Test 2

(4 pts) Test 3

(4 pts) Test 4


