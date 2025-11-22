# Technology College Freshers Portal

This is a simple console-based Python application that simulates a basic student portal, allowing users to check their attendance, view marks, and submit a leave request.

# Features

The portal offers four main functionalities accessed via a numbered menu:

  - View Attendance: Displays current attendance percentages for all subjects and allows viewing total present/absent days.

  - View Marks: Displays the marks obtained in all subjects for the current semester.

  - Leave Process: Guides the student through submitting a leave request.

       Requires verification against the stored Procter Name.

       Calculates the number of academic weekdays between the start and end date (excluding weekends).

       Approval Criteria: Leave is only approved if the student's attendance percentage is 75% or higher in all subjects.

   - Exit / Re-login: Allows the user to exit the portal or attempt a new login session.

# Data Structure

All student data is stored locally in the student_record dictionary at the top of the file:

- Roll Number            01, 102, etc.

- Field- name- marks- present_day- absent_day- procter

- Description

     Student's name (used for login validation).

     Subject-wise marks.

     Total days present per subject.

     Total days absent per subject.

     The assigned procter's name (used for leave request verification).

     To test the application, use one of the following valid login combinations:

Name- student1, student2

Roll Number- 101, 102

Procter Name -ramraj,sitaram

# How to Run

   - Requirements: Ensure you have Python installed (Python 3.x recommended).
   - Execution: Save the code as student_portal.py and run it from your terminal:
                 python student_portal.py


# Critical Usage Warning (Input Safety)

This program was specifically developed without standard Python error handling mechanisms (try/except) for robust input validation.

This means you MUST enter a number when the program asks for:
     
 - Menu Choices (1, 2, 3, or 4)

 - CAPTCHA (the 4-digit number displayed)
      
 - Back to Menu Option (e.g., key <1>)

 - Attendance Option (e.g., key <44>)

If you enter any letters, symbols, or text when a number is expected, the program will crash immediately.

Similarly, the date inputs for the leave process must strictly follow the YYYY-MM-DD format (e.g., 2025-11-22), or the program will crash.
