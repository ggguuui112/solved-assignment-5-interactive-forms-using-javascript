Download Link: https://assignmentchef.com/product/solved-assignment-5-interactive-forms-using-javascript
<br>
This assignment will show you how to make the HTML form your created last week interactive by adding in

JavaScript. It will calculate the correct gross pay for each valid employee entered into our form. A template (see other file link in this assignment) containing both HTML and JavaScript will be provided that will show you how to use JavaScript to test your form elements for valid data input. Instead of using a database (we’ll cover that in the last week), we will use a two dimensional array that associates a unique employee number with the full name of the employee.

<strong>Name</strong> – Employee Name (stored in our array)

<strong>Clock</strong> – Unique Employee Number to identify an employee (stored in our JavaScript array) <strong>Wage</strong> – Pay per hour

<strong>Hours</strong> – Hours worked in a given week

<strong>OT</strong> – Overtime Hours (total hours – 40.0) … 40 hours is a normal work week

<strong>Overtime Pay Factor</strong> – 1.5 (time and half) or 2.0 (double time)

<strong>Gross Pay</strong> – Normal Pay (wage * normal hours) + overtime pay (overtime hours * wage * overtime pay factor)

Employee Payroll information to test our Gross Pay Calculator (note:  gross pay based on overtime pay at time and a half – 1.5):

<strong>Name          Clock Wage Hours OT Gross Pay</strong>

<table width="413">

 <tbody>

  <tr>

   <td width="312">Connie Cobol 098401 10.60 51.0</td>

   <td width="101">11.0 598.90</td>

  </tr>

  <tr>

   <td width="312">Mary Apl        526488 9.75    42.5</td>

   <td width="101">2.5 426.56</td>

  </tr>

  <tr>

   <td width="312">Frank Fortran 765349 10.50 37.0</td>

   <td width="101">0.0 388.50</td>

  </tr>

  <tr>

   <td width="312">Jeff Ada           034645 12.25 45.0</td>

   <td width="101">5.0 581.88</td>

  </tr>

  <tr>

   <td width="312">Anton Pascal 127615 8.35     0.0</td>

   <td width="101">0.0 0.00</td>

  </tr>

 </tbody>

</table>

The JavaScript code will test the various HTML form elements once a “Calculate” button is clicked to show the employee name and associated gross pay for a given week, in particular:

Test an array to determine the existence of a given employee number.

Ensure that all fields contain a value (not empty)

Ensure that specific fields contain a numeric value

The overtime rate used is either 1.5 (time and a half) or 2.0 (double time)

<h1>Assignment Options</h1>

Like each week, there is a minimum assignment, and a challenge assignment, resulting in a different set of possible points. In either case, please use the template provided. The template will work out of the box, but only checking the clock and wage form fields … ignoring the others. Paste it into the HTML Real Time Editor and watch it run.

DO NOT start this assignment from scratch, go easy on yourself and use my template. Add a little bit of code at a time, test it in real time, then and more code, test, and so on. DO NOT just add all the code at once …

JavaScript can be very difficult to debug given our freely available tool suite.

<strong> Minimum Assignment (80 point maximum)</strong> – Use the template provided and use the standard set of fields already provided. Simply add the missing code (its easy, you just mimic code in areas clearly marked in the template).   Carefully follow the directions and you will have no problems. DO NOT add additional code not specified in the template.

<strong> Challenge Assignment (100 point maximum)</strong> – Add another field to your form called “Service” that shows the number of years an employee worked for the company. Like the other fields, ensure that the service value gets entered into the form field and is a numeric value.

<em>Want to challenge yourself even more???</em>

Add five other fields to your HTML form … perhaps the same five form elements you added if you did the challenge from the homework assignment last week. Note that with form elements like <em>radio</em> or <em>pick lists</em>, you don’t have to worry about validating their values with JavaScript as you are limited to what you can select. You could however decide to make them mandatory or not mandatory. No extra points for doing this additional challenge, but try it if you have the bandwidth.

<h1>Submitting the Assignment</h1>

The template you are updating this week is an<strong> HTML file</strong> that contains <strong>JavaScript code</strong>. Verify that your program works (see <strong>Use Cases</strong> below) in either the <em>HTML Real Time Editor</em>, or by saving and opening the HTML file on your computer with your favorite <em>web browser</em>.

<strong> IMPORTANT SUBMISSION NOTE:  </strong>Just like last week, you will have to place your JavaScript file which will have an *.htm or *.html type file extension into a zip file to submit it since BlackBoard will not allow you to upload a native HTML file.

DO WATCH the “<strong>Forms and JavaScript</strong>” video I posted in this week’s lecture notes.   It shows you exactly what you need to do with this assignment and gives you a real time demo on how the calculator actually works.   Additionally, use cases are show in the next section below to help you understand what needs to be tested.

DO VERIFY that everything works.  If you click the <em>Calculate button</em> and nothing happens, you likely have an error in one of your statements that you added.  <strong>Add only a few statements at a time</strong> and click the Calculate button frequently to ensure that either an alert box is displaying for an invalid field entry or the gross pay is being calculated and displayed.

DO NOT add all the statements at once, otherwise if there is any error, you have no idea which set of statements is causing it … at that point you’ll have to comment out or delete statements, clicking the Calculate button, until you can figure out which statements are invalid.  For example, you spelled the field name incorrectly, or you forgot an end curly brace to correspond to an open curly brace in an if statement. Unfortunately, JavaScript isn’t like compiling a program and getting a listing of errors up front.

<strong>How to Submit the Assignment:</strong> Once satisfied, just attach the HTML file when you submit the

assignment. If you use the <strong>HTML Real Time Editor</strong>, simply copy and paste your final code from it into an HTML file (has an *.html or *.htm file extension) and submit that file. This file format will allow me to download your assignment submission to verify it is correct.

<strong>Submission Note:</strong>  You will likely have to <u>put </u>y<u>our file into a zip file to submit it</u> into BlackBoard Learn given its recently added “security” feature, as it no longer accepts native files containing HTML and/or JavaScript.

<strong>Important Note:</strong>  if you notice your program works fine in the <em>HTML Square Free Editor</em> … but does not work with your <em>web browser</em> … make sure your web browser is not <em>disabling</em> JavaScript. Some browsers may disable JavaScript automatically if specific security settings are set too high.

A good web site that provides instructions on how to check your specific web browser to determine if JavaScript is enabled can be found at: <u><a href="http://www.enable-javascript.com/">http</a><a href="http://www.enable-javascript.com/">://</a><a href="http://www.enable-javascript.com/">www.enable-</a></u><a href="http://www.enable-javascript.com/">j</a><u><a href="http://www.enable-javascript.com/">avascript.com</a></u>

<h1>Use Cases</h1>

The sequence of screen shots below show how the form is designed to work. The first screen shot shows how the form should work if everything is correctly entered. In this case, the clock number has been defined in the two dimensional array, all fields have been filled out, the OT Pay factor is either 1.5 and 2.0, and each field is a number.

The <strong>key</strong> to making all the “magic” happen is to click the <strong>Calculate button</strong>. At that point, the JavaScript code will activate to ensure that all fields are filled in correctly, and if so, display the Employee Name associated with the clock number, and calculate their gross pay.

<strong>Note: </strong>The template will work out of the box with no changes on your part. Checking is already done on the Clock and Wage fields. Your job is to add the missing code to the template to verify the values entered into the Hours, OT, and OT Pay Factor fields.

The example above uses an overtime pay factor of 1.5, for time and half, which would pay all overtime hours at a wage of time and half. In this case, the 11 overtime hours would be paid at a wage rate of $15.90 (which is 1.5 multiplied by 10.60). If you type in an overtime pay factor of 2.0, for double time, it would pay all overtime hours at twice the hourly wage, which is $21.20 (calculated as 2.0 multiplied by 10.60). The OT Pay Factor field will only accept a value of 1.5 or 2.0

<table>

 <tbody>

  <tr>

   <td width="11"></td>

  </tr>

  <tr>

   <td></td>

   <td></td>

  </tr>

 </tbody>

</table>

There is also some error checking involved. When implemented, all input fields must contain a value. Processing will start from the top and work its way down. If any field is left blank, an alert box message will show the user the first field it encountered that was missing a value.

Additionally, the clock number will be checked against a list of valid clock numbers and the rest of the fields will be checked for numeric values.




<table style="height: 108px;" width="1163">

 <tbody>

  <tr>

   <td width="11"></td>

  </tr>

  <tr>

   <td></td>

   <td></td>

  </tr>

 </tbody>

</table>