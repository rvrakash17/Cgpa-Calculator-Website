# CGPA Calculator Website

A web-based application for calculating the CGPA (Cumulative Grade Point Average) and GPA (Grade Point Average) for up to 8 semesters. This tool allows students to input their semester GPAs and calculates the overall CGPA, providing motivational feedback based on the calculated CGPA.

## Features

- **Multi-Semester GPA Input:** Allows users to input GPAs for up to 8 semesters.
- **CGPA Calculation:** Calculates the average of the entered GPAs to determine the CGPA.
- **Motivational Feedback:** Displays motivational messages based on the CGPA result.
- **Responsive Design:** Optimized for both desktop and mobile devices.

## Technologies Used

- **HTML:** Structure of the webpage.
- **CSS:** Styling and layout of the webpage.
- **JavaScript:** Functionality for CGPA calculation and dynamic feedback.
- **Bootstrap:** For responsive design and modal functionality (if used).

## Setup and Installation

To run this project locally, follow these steps:

1. **Clone the Repository:**
   ```sh
   git clone https://www.github.com/rvrakash17/Cgpa-Calculator-Website.git
   cd Cgpa-Calculator-Website
   ```

2. **Open the Project:**
   Open the `index.html` file in a web browser to view the application.

3. **Dependencies:**
   Ensure you have an internet connection to load external resources like fonts and CSS frameworks from CDNs.

## Usage

1. **Enter GPA Values:**
   - Open the `index.html` file in your browser.
   - Input your GPAs for each semester into the provided input fields.

2. **Submit:**
   - Click the "Submit" button to calculate your CGPA.
   - A modal will appear displaying your calculated CGPA and a motivational message based on the result.

## Code Explanation

### HTML

- **Structure:** Defines the layout of the page, including input fields for each semester GPA and a button to trigger the calculation.
- **Modal:** Displays the result and motivational message.

### CSS

- **Styling:** Styles the layout and components of the page to ensure a visually appealing and responsive design.

### JavaScript

- **Functionality:** Handles the calculation of CGPA and updates the result and feedback based on the calculated value.
  ```javascript
  function myfunction() {
    var s1 = document.getElementById("I").value * 1;
    var s2 = document.getElementById("II").value * 1;
    var s3 = document.getElementById("III").value * 1;
    var s4 = document.getElementById("IIII").value * 1;
    var s5 = document.getElementById("IIIII").value * 1;
    var s6 = document.getElementById("IIIIII").value * 1;
    var s7 = document.getElementById("IIIIIII").value * 1;
    var s8 = document.getElementById("IIIIIIII").value * 1;
    
    var t = (s1 + s2 + s3 + s4 + s5 + s6 + s7 + s8) / 8;
    var gpa = t.toFixed(2);
    
    document.getElementById("result").innerHTML = "YOUR CGPA IS: " + gpa;
    
    if (gpa < 7.00) {
      document.getElementById("output").innerHTML = "Failure is simply the opportunity to begin again. This time more intelligently....😇";
    } else if (gpa >= 7.00 && gpa < 8.00) {
      document.getElementById("output").innerHTML = "Push yourself to do more. Work hard, train hard, and be the best that you can be.";
    } else if (gpa >= 8.00 && gpa < 9.00) {
      document.getElementById("output").innerHTML = "Success is not final, failure is not fatal; it is the courage to continue that counts.";
    } else {
      document.getElementById("output").innerHTML = "YOUR TODAY’S SUCCESS IS THE BEGINNING OF TOMORROW’S ACHIEVEMENT. CONGRATULATIONS!";
    }
  }
  ```
  
## Author
- Akash R
