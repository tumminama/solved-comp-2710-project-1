Download Link: https://assignmentchef.com/product/solved-comp-2710-project-1
<br>









<ul>

 <li>To learn how to implement the concept of “Flow of Control” in C++</li>

 <li>To write a very simple C++ program</li>

</ul>

<strong><em><u>Descrip.on:</u> </em></strong>

You have just purchased a stereo system that cost $1000 on the following credit plan: no down payment, an interest rate of 18% per year (and hence 1.5% per month), and monthly payments of $50. The monthly payment of $50 is used to pay the interest, and whatever is leP is used to pay part of the remaining debt. Hence, the first month you pay 1.5% of $1000 in interest. That is $15 in interest. The remaining $35 is deducted from your debt, which leaves you with a debt of $965.00. The next month you pay interest of 1.5% of $965.00, which is $14.48. Hence, you can deduct $35.52 (which is $50–$14.48) from the amount you owe.

Write a program that will tell you how many months it will take you to pay off this loan in par[cular and any loan in general. Your program also needs to calculate the total amount of interest paid over the life of any loan. Use a loop to calculate the amount of interest and the size of the debt aPer each month. Your program must output the monthly amount of interest paid and remaining debt. Use a variable to count the number of loop itera[ons and hence the number of months un[l the debt is zero. You may want to use other variables as well. The last payment may be less than the monthly payment, therefore should be calculated based on the amount leP in balance (instead of monthly payment). And do not forget the interest. If you owe $50, then your monthly payment of $50 will not pay off your debt, although it will come close. One month’s interest on $50 is only 75 cents.

Here is a sample dialog (where the user input is depicted as <strong>Bold</strong>, but you do not need to display user input in bold.) Both number formats: 1234.56 and 1,234.56 are accepted:




Loan Amount: <strong>1000</strong>

Interest Rate (% per year): <strong>18</strong>

Monthly Payments: <strong>50 </strong>**********************************************************

Amortization Table

**********************************************************

Month Balance   Payment         Rate Interest   Principal

<ul>

 <li>$1000.00 N/A         N/A   N/A       N/A</li>

 <li>$965.00 $50.00      50 $15.00     $35.00 2      $929.47   $50.00        1.50 $14.47     $35.53 3 $893.42   $50.00 1.50 $13.94     $36.06</li>

 <li>$856.82 $50.00      50 $13.40     $36.60</li>

 <li>$819.67 $50.00      50 $12.85     $37.15</li>

 <li>$781.97 $50.00      50 $12.30     $37.70</li>

 <li>$743.70 $50.00      50 $11.73     $38.27</li>

 <li>$704.85 $50.00      50 $11.16     $38.84</li>

 <li>$665.42 $50.00      50 $10.57     $39.43</li>

 <li>$625.40 $50.00      50 $9.98     $40.02</li>

 <li>$584.79 $50.00      50 $9.38     $40.62</li>

 <li>$543.56 $50.00      50 $8.77     $41.23</li>

 <li>$501.71 $50.00      50 $8.15     $41.85</li>

 <li>$459.24 $50.00      50 $7.53     $42.47</li>

 <li>$416.13 $50.00      50 $6.89     $43.11</li>

 <li>$372.37 $50.00      50 $6.24     $43.76</li>

 <li>$327.95 $50.00      50 $5.59     $44.41</li>

 <li>$282.87 $50.00      50 $4.92     $45.08</li>

 <li>$237.11 $50.00      50 $4.24     $45.76</li>

 <li>$190.67 $50.00      50 $3.56     $46.44</li>

 <li>$143.53 $50.00      50 $2.86     $47.14 22      $95.68   $50.00   1.50 $2.15     $47.85</li>

</ul>

23   $47.12   $50.00   1.50 $1.44     $48.56 24      $0.00   $47.83    1.50 $0.71     $47.12

**********************************************************

It takes <strong>24</strong> months to pay off the loan.

Total interest paid is: <strong>$197.83</strong>

<strong>Your program’s output should match the style of the sample output (including a leE lined-up style). </strong>

In what follows, you find a second case used to test the correctness of your program.




Loan Amount: <strong>2000</strong>

Interest Rate (% per year): <strong>12</strong>

Monthly Payments: <strong>80</strong>




<table width="576">

 <tbody>

  <tr>

   <td width="576">********************************************************Amortization Table********************************************************Month Balance             Payment Rate Interest Principal0        $2,000.00   N/A   N/A   N/A     N/A1        $1,940.00   $80.00 1.00 $20.00   $60.002        $1,879.40   $80.00 1.00 $19.40   $60.603        $1,818.19   $80.00 1.00 $18.79   $61.214        $1,756.38   $80.00 1.00 $18.18   $61.825        $1,693.94   $80.00 1.00 $17.56   $62.446        $1,630.88   $80.00 1.00 $16.94   $63.067        $1,567.19   $80.00 1.00 $16.31   $63.698        $1,502.86   $80.00 1.00 $15.67   $64.339        $1,437.89   $80.00 1.00 $15.03   $64.97 10       $1,372.27   $80.00 1.00 $14.38   $65.6211      $1,305.99   $80.00 1.00 $13.72   $66.2812      $1,239.05   $80.00 1.00 $13.06   $66.9413      $1,171.44   $80.00 1.00 $12.39   $67.6114      $1,103.15   $80.00 1.00 $11.71   $68.2915      $1,034.19 $80.00 1.00 $11.03   $68.97 16 $964.53  $80.00 1.00 $10.34   $69.66 17 $894.17  $80.00 1.00 $9.65   $70.3518      $823.11     $80.00 1.00 $8.94   $71.0619      $751.35     $80.00 1.00 $8.23   $71.7720      $678.86     $80.00 1.00 $7.51   $72.4921      $605.65     $80.00 1.00 $6.79   $73.2122      $531.70     $80.00 1.00 $6.06   $73.9423      $457.02     $80.00 1.00 $5.32   $74.6824      $381.59     $80.00 1.00 $4.57   $75.4325      $305.41     $80.00 1.00 $3.82   $76.1826      $228.46     $80.00 1.00 $3.05   $76.9527      $150.75     $80.00 1.00 $2.28   $77.72 28       $72.25      $80.00 1.00 $1.51   $78.49 29       $0.00       $72.98 1.00 $0.72   $72.25********************************************************It takes <strong>29</strong> months to pay off the loan.Total interest paid is: <strong>$312.98</strong></td>

  </tr>

 </tbody>

</table>

<strong><em><u>Special Cases:</u> </em></strong>

<ol>

 <li>Please think about how to deal with the <strong>last payment</strong>, which is smaller than regular payment. For example, in the above table, the regular payments are $80.00 whereas the last payment is only 72.98.</li>

 <li>Your program needs to ensure that <strong>regular payments are larger than any monthly interest</strong>. For example, in the above amor[za[on table, your program must test if the regular monthly payment (i.e., $80.00) is larger than the monthly interest (e.g., $20.00 in the first month), otherwise your program should ask for a larger monthly payment.</li>

 <li>Your program should check if the <strong>loan amount and monthly payment are posiHve numbers</strong> and <strong>interest rate is a non-negaHve number. </strong>If encounters a 0, nega[ve number, or a char, your program should prompt the user to enter another input.</li>

 <li>If you do not address the above issues, your program may not terminate in some special cases and you will lose marks. See the example below:</li>

</ol>

<strong><em> </em></strong>

Loan Amount: <strong>2000</strong>

Interest Rate (% per year): <strong>49.2</strong>

Monthly Payments: <strong>80 </strong>

********************************************************

Amortization Table

********************************************************

Month Balance           Payment Rate Interest Principal

<ul>

 <li>$2,000.00 N/A   N/A   N/A     N/A</li>

 <li>$2,002.00 $80.00 4.10 $82.00   -$2.00</li>

 <li>$2,004.08 $80.00 4.10 $82.08   -$2.08</li>

 <li>$2,006.25 $80.00 4.10 $82.17   -$2.17</li>

 <li>$2,008.51 $80.00 4.10 $82.26   -$2.26</li>

 <li>$2,010.85 $80.00 4.10 $82.35   -$2.35</li>

 <li>$2,013.30 $80.00 4.10 $82.45   -$2.45</li>

 <li>$2,015.84 $80.00 4.10 $82.55   -$2.55</li>

 <li>$2,018.49 $80.00 4.10 $82.65   -$2.65</li>

 <li>$2,021.25 $80.00 4.10 $82.76   -$2.76 10      $2,024.12   $80.00 4.10 $82.87   -$2.87</li>

 <li>$2,027.11 $80.00 4.10 $82.99   -$2.99</li>

 <li>$2,030.22 $80.00 4.10 $83.11   -$3.11</li>

 <li>$2,033.46 $80.00 4.10 $83.24   -$3.24</li>

 <li>$2,036.84 $80.00 4.10 $83.37   -$3.37</li>

 <li>$2,040.35 $80.00 4.10 $83.51   -$3.51</li>

 <li>$2,044.00 $80.00 4.10 $83.65   -$3.65</li>

 <li>$2,047.80 $80.00 4.10 $83.80   -$3.80</li>

 <li>$2,051.76 $80.00 4.10 $83.96   -$3.96</li>

 <li>$2,055.89 $80.00 4.10 $84.12   -$4.12</li>

</ul>

…   …              …             …       …

<strong>  </strong>

<strong><em><u>Programming Environment:</u> </em></strong>

<ol>

 <li>Write a short program in C++. Compile and run it using AU server (no maeer what kind of text editor you use, please make sure your code could run on AU server, the only test bed we accept is AU server).</li>

 <li>You can use a compiler version that you are most comfortable with, but you need to specify it in the heading of your source code, e.g., -std=c++11 or -std=c++98.</li>

 <li>it is ideal to use the <strong>cout</strong> func[on, but pring is OK.</li>

</ol>

<strong><em><u>Requirements:</u> </em></strong>

<ol>

 <li>(5 points)<strong> Use comments to provide a heading at the top of your code</strong> containing your name, Auburn UserID, filename, and how to compile your code. Also describe any help or sources that you used (as per the syllabus).</li>

 <li>(5 points) Your source code file should be named as “<strong>cpp</strong>”. (e.g. project1_Liu_tzl0031.cpp)</li>

</ol>

Note: You will not lose any point if Canvas automa[cally changes your file name (e.g. project1_LastName_UserID-2.cpp) due to your resubmissions.

<ol start="3">

 <li>(40 points) No compila[on error and no warning messages.</li>

 <li>(10 points) Usability of your program (e.g., input and output).</li>

 <li>(40 points) Quality of your source code.</li>

</ol>

You will <strong>lose points</strong> if you: do not use the specific program file name, or do not have a comment block on <strong>EVERY</strong> program you hand in. You will lose <strong>at least 40 points</strong> if there are compila[on errors or warning messages when we compile your source code.

<ul>

 <li></li>

</ul>