Let's break down the rotation equations for the hour, minute, and second hands of an 
analog clock in a more detailed and beginner-friendly way:

1. **Hour Hand (h):** The hour hand on a clock moves slower than the minute and second 
hands. It completes one full rotation (360 degrees) in 12 hours. This means that each 
hour corresponds to a rotation of 30 degrees (360 degrees / 12 hours). Additionally, 
for every minute that passes, the hour hand moves a little bit further. Since there are 
60 minutes in an hour, each minute adds 0.5 degrees to the hour hand's rotation (30 
degrees / 60 minutes).

   So, the total rotation of the hour hand for 'h' hours and 'm' minutes is calculated 
   using this formula:
   Rotation of hour hand = (30 * h) + (m * 0.5) degrees.

   For example, if it's 3:15 (3 hours and 15 minutes):
   Rotation of hour hand = (30 * 3) + (15 * 0.5) = 90 + 7.5 = 97.5 degrees.

2. **Minute Hand (m):** The minute hand moves faster than the hour hand. It completes 
one full rotation (360 degrees) in 60 minutes. This means that each minute corresponds 
to a rotation of 6 degrees (360 degrees / 60 minutes).

   So, the total rotation of the minute hand for 'm' minutes is calculated using this 
   formula:
   Rotation of minute hand = 6 * m degrees.

   For example, if it's 25 minutes past the hour:
   Rotation of minute hand = 6 * 25 = 150 degrees.

3. **Second Hand (s):** The second hand moves even faster than the minute hand. It 
completes one full rotation (360 degrees) in 60 seconds. This means that each second 
corresponds to a rotation of 6 degrees (360 degrees / 60 seconds).

   So, the total rotation of the second hand for 's' seconds is calculated using this 
   formula:
   Rotation of second hand = 6 * s degrees.

   For example, if it's 10 seconds past the minute:
   Rotation of second hand = 6 * 10 = 60 degrees.

These equations help us understand how the hands of an analog clock move relative to 
each other based on the passage of time. The hour hand moves slowly, the minute hand 
moves faster, and the second hand moves the fastest, each contributing to the overall 
timekeeping function of the clock.

# Explanation of project

Analog Clock Project
This project is a simple analog clock created using HTML, CSS, and JavaScript. The 
clock displays the current time and updates every second to show the accurate time.

Project Structure
HTML (index.html): This file contains the basic structure of the web page. It includes 
a <div> with the id clockContainer, which serves as the container for the clock hands 
(hour, minute, second).

CSS (style.css): The CSS file defines the styles for the clock elements. The 
#clockContainer is styled to be a square container with a background image of a clock 
face. The #hour, #minute, and #second elements are positioned absolutely within the 
container and styled as black rectangles representing the hour, minute, and second 
hands of the clock.

JavaScript (index.js):The index.js file contains the JavaScript code that powers the 
functionality of the analog clock. Here's a breakdown of its key components:

setInterval(() => { ... }, 1000);: This function is used to update the clock every 
second (1000 milliseconds). Inside the function, the current time is obtained using new 
Date() and stored in the variables htime (hours), mtime (minutes), and stime (seconds).
Calculating Rotation Angles:
hrotation, mrotation, srotation: These variables calculate the rotation angles for the 
hour, minute, and second hands based on the current time. The hour hand moves 30 
degrees per hour (360 degrees/12 hours) plus half a degree for every minute (30 degrees/
60 minutes), the minute hand moves 6 degrees per minute (360 degrees/60 minutes), and 
the second hand moves 6 degrees per second (360 degrees/60 seconds).
Applying Transformations:
hour.style.transform = rotate(${hrotation}deg);: Applies the calculated rotation angle 
to the hour hand using the transform property with the rotate() function.
minute.style.transform = rotate(${mrotation}deg);: Applies the calculated rotation 
angle to the minute hand.
second.style.transform = rotate(${srotation}deg);: Applies the calculated rotation 
angle to the second hand.
These transformations cause the clock hands to rotate dynamically, reflecting the 
current time.

Credits:
This project was created by following a tutorial by Code With Harry on YouTube.

# What i have learnd
HTML Structure: I learned how to structure an HTML document to create a basic web page, 
including the use of <meta> tags for character encoding and viewport settings, and 
linking external CSS and JavaScript files.

CSS Styling: I gained experience in using CSS to style HTML elements, including setting 
up a container with a background image and positioning elements using position: 
relative and position: absolute.

JavaScript Logic: I learned how to use JavaScript to add interactivity to my web page, 
such as updating the clock hands based on the current time using the setInterval 
function and calculating rotation angles for the hands.

Positioning in CSS: I explored different positioning techniques in CSS, including 
position: relative for positioning elements relative to their normal position, and 
position: absolute for absolute positioning within a container.

Transformations in CSS: I gained an understanding of how to use CSS transform property 
to apply transformations like rotation (rotate()) to elements, allowing me to create 
dynamic visual effects.

Project Workflow: I experienced the process of creating a project from scratch, 
including setting up the project structure, writing HTML, CSS, and JavaScript code, and 
testing the project locally before deploying it.