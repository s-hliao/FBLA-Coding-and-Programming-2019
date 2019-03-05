# FBLA-Coding-and-Programming-2019
General Project Documentation Henry Liao submission for WA FBLA 2018-19, Coding and Programming

DESCRIPTION: Manages ebook distribution and ID codes of books for members of a class. Programmed with C# in Microsoft Visual Studio 2015 Windows Forms.

INSTALLATION: To run, download the "release.zip" zip folder and extract it. Inside, simply running the FBLA Application executable (the first one) will allow for the application to run. Do not delete or move any of the contents of the folder outside of the folder. Do not modify filepaths.
Simply deleting the json file will erase all previous storage of the program, but the program will still be able to serialize and deserialize by recreating the file, albeit without previous data. Note that Microsoft Excel and Outlook are necessary to run this program correctly.

To view source code, all .cs files in the solution zip folder are commented.The classes upon which the program is founded upon are Account, Book, and LibrarySys.

Usage: At the login, there are three options: to create an account, reset the adminKey, or login. The admin key is used in the creation of an admin account when creating an account. Creating an account is fairly straightforward(there are no constraints except for password length and that ID is less than 9 digits). From the login, the program is split into two forms, the administrator and student forms. Students have only four options: to check out codes with given accession numbers, to view and return books, to view their account settings snd edit their passwords, and to visit the interactive Help. Administrators are able to also check out books,change password, and change account passwords. However, they are also able to generate comprehensive excel reports on the Accession numbers that students have previously used as well as their currently checked-out books. They may also add and manage the characteristics of books added to the system (such as accession number and number of copies). Administrators also have greater control over theirs and student's profiles, being able to also change grade levels as well as change student IDs and passwords. They also have the capability to generate formatted emails for recipients based on accession numbers, either in the library system or in student's checkout lists.

All of these actions are specified as buttons on the home page of students and admins (right after login), and they open dialog boxes to perform the action based on usee input.

If return is specified for emails, then the program will sesrch for the student ID in accounts, whereas if checkout is specified, the program will search in the library system.

Books, when returned, will gain a new accession number (the lowest possible one that has not been used yet) and can be changed by administrators. Multiple windows can be opened at once for the simultaneous usage, which is useful for seeing the accession numbers as an administrator and using them at the same time to send messages.
A listed interactive faq is also available on account homescreens right after login.
All data is stored continuously in the JSON file, serializing after every change and deserializing at the beginning of the program.
When finished with the program, return to Login and exit. All windows launched from the home page right after login may be closed by closing out, but to return to login there is a button.
All accounts can view the interactive help page, and administrators can reset the entire system using the admin key.

The sign-in for the administrator account Henry Liao is:

ID: 1019205
Password: Prisoner24601

The sign-in for student Vidyut Baskar is:

ID: 10
Password: Grinding

PROJECT GUIDELINES:

Coding & Programming Category: Prejudged Projects & Presentation Type: Individual Overview Two (2) parts: a prejudged project and a presentation. Competitors must complete both parts for award eligibility.

Topic: Develop a computer program to manage the issuance of e-books to a class of students. Give the class and e-book a name. The program must complete a minimum of the following tasks: Track student name and grade in school with ability to enter/view/edit. Track the redemption codes for each individual copy of the e-book with ability to enter/view/edit codes. Track the issuance of e-books for a student--a redemption code may be used only once and paired with the student. Generate or print weekly report to show to whom books are assigned. Data must be stored persistently. Storage may be in a relational database, a document-oriented NoSQL database, flat text files, flat JSON or XML files. The user interface must be a GUI with a minimum of five different control types including such things as drop-down lists, text fields, check boxes, emails, or other relevant control types. All data entry must be validated with appropriate user notifications and error messages including the use of required fields.


Specific Guidelines: The program must run on Windows 7 or higher. Solution must run standalone with no programming errors. Data must be free of viruses/malware. Any entry with contaminated data will not be judged. The program should be shown to the judges.
