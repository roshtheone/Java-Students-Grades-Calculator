# Java-Students-Grades-Calculator
Explanation:
This Java program allows users to enter a student ID, view their grades, calculate their future GPA, and includes functionality to lock the account after four failed attempts to enter a valid student ID. It also displays fun messages using emojis when the account gets deactivated. The program uses two HashMap structures to store student data, including names and grades, and interacts with users through the console.

Key Components:
Imports:

Scanner: Used for reading user input.
HashMap: Used to store key-value pairs for student information (ID and name) and their grades.
Main Method:

The main method starts the program. It:
Initializes student data by calling initializeStudentData().
Prompts the user to input their student ID.
Allows up to four attempts to enter a valid student ID.
If a valid ID is entered, the program displays the student's name, transcript, and calculates their future GPA.
If the user fails to enter the correct ID in four tries, the account is deactivated with a final message full of emojis.
Account Deactivation Logic:

A while loop is used to allow the user a maximum of four attempts to enter a valid Student ID.
If the entered ID is correct, the student's transcript and future GPA are displayed.
If the user fails four times, the program deactivates the account and ends with an "account blocked" message.
Methods:

initializeStudentData():
Stores mock student data in two HashMap structures:
studentInfo stores the student ID and their corresponding name.
studentGrades stores the student ID and an array of grades for different courses.
displayTranscript(String studentId):
This method fetches the student's grades (based on their ID) and prints their transcript for the following courses:
#ITSC 1213
#MAT 2164
#ITSC 2175
#ITSC 4353

​
 
Account Deactivation Flow:
If the user enters an invalid Student ID, they are informed and told how many attempts remain.
After 4 wrong attempts, the program deactivates the account permanently and prints a message with emojis like "❌ Account deactivated!" and "🚫 The user has passed away metaphorically. 😇 Rest in peace, dear account. 🕊️."
