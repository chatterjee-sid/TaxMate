# TaxMate
This project is the model for an Income Tax Calculator, whose main aim is to tell the user, which tax regime is beneficial for him or her. For this, this site also shows an approximate tax calculation (Approximate because of miscellaneous reasons). This project uses a total of 7 web-pages, 1 CSV file and 1 JavaScript file. The web-pages formed are as follows:

1. Home / Index (page1.html)
2. About (about_us.html)
3. Contact (contact_us.html)
4. Rules (rules.html)
5. Income Calculator (page2.html)
6. Deductions Calculator (page3.html)
7. Results (page4.html)

All 7 pages share similar headers and footers, so it was possible to have common headers and footers for all the pages, and link them using the JavaScript file. Though, this developer did not realise that something like that was possible, before the project was completed.While only an external JavaScript file is used, all types of CSS (i.e. inline, internal, and external)
are used, depending on common and unique properties of elements throughout the 7 webpages.

## Description

### Page Base
The image (a logo) was created using AI. However, the main purpose of doing so was simply to demonstrate how to use an image in HTML. The 4 links on Navigation bar, i.e. Home, About Us, Contact Us and Rules, were arranged in this order using **flexbox** property. Each of them links to the respective page. The headline “TaxMate” also links to the home page of the site.

Similarly, we used **flexbox** property with **direction column** and keeping **min-height** of the body to be 98% of the screen height or **98vh** (viewport height) (It was showing a scroll-bar at 100%, which was not desired), allowing the **flex** to be true for the *main* tag only. In this way, the footer was always located only at the end of the page or the end of the screen.

### Home/Index Page
This page is used to take input from the user, regarding his/her name and age group. This page is also used to display the meaning of Income Tax and its importance.

The layout of the table was obtained by applying **border** style on *td* tags rather than the *table* tag.

In case, the user does not select any age group, a message pops on the browser, telling the user that he or she must select an age group, and thus, not allowing the user to proceed ahead, without selecting any age group. While it is fine, if the user does not input his or her name, we still confirm it from the user if he or she really does not wish to use his or her name. In this case, we use the name “User” to refer to the user later.

### About
This page simply explains the purpose of the site

### Contact
This page displays the contact details of the developer

### Rules
This page displays the benchmarks on which all tax calculations are performed. It explains the tax slab distribution, and tax on each slab, based on age group and regime. It also shows the limit up to which deduction for a particular section can be deducted.

### Income Calculator
The user is provided with various options from where he can calculate his or her gross income. The user inputs the values which are then stored in **localStorage**.

A tooltip also appears when you hover on the ྦྷ symbol, giving you more information on the income.

### Deductions Calculator
Similar operations are conducted on this page, just like those on the “Income Calculator” page, however limits on deductions are also considered in this case.

### Results
Storing all necessary information on localStorage, we use the stored data and perform required calculations. The numbers which come out are then wriƩen in the table with the help of a function which is called right when the page loads.

Comparing the results, the page also suggests the user to opt for the regime which is more beneficial to him or her.

Another buƩon is provided at the end of the results table, which brings him or her back to the home page, in case he or she wishes to recalculate the tax on puƫng different inputs.

## Issues Unresolved
In case, the user uses a device with low resolution, like a smartphone, then values inside a table will appear tiny for them. While the user can tackle that issue by zooming, but that still leaves a negative remark.
