<h1>Red Bus Automation Solution </h1>

<h2>Objective</h2>
The objective of this project is to automate the process of searching buses on RedBus
between Mumbai → Pune, applying filters (Primo and Evening), and handling lazy loading to ensure all bus results are captured until the "End of list" message appears.<br>
<br>This automation script demonstrates:</br>
<br>Browser automation using Selenium WebDriver.</br>
<br>Handling dynamic web elements and auto-suggestions.</br>
<br>Implementing explicit waits for stability.</br>
<br>Dealing with lazy loading using scroll actions.</br>

<h2>Tech Stack</h2>
<br>Programming Language: Java (JDK 11)</br>
<br>Automation Framework: Selenium WebDriver</br>
<br>Build Tool: Maven </br>
<br>Browser: Google Chrome</br>
<br>Driver: ChromeDriver (compatible with Chrome browser version)</br>

<h2>Challenges Tackled</h2>
<h3>Dynamic Auto-Suggestions</h3>
Challenge: Auto-suggestions for "From" and "To" locations appeared asynchronously.<br>
Solution: Used explicit waits to ensure suggestions were visible before selecting.
<h3>Click Interception Errors</h3>
Challenge: Elements like Primo or Evening filters were sometimes overlapped by popups or banners.<br>
Solution: Applied wait until clickable + slight scroll into view.
<h3>Lazy Loading of Bus List</h3>
Challenge: The bus list loaded dynamically as the user scrolled.<br>
Solution: Implemented a scroll loop with JavaScriptExecutor until "End of list" was found.
<h3>Stability Across Multiple Runs</h3>
Challenge: Inconsistent behavior due to network speed and dynamic DOM changes.<br>
Solution: Added retry logic + explicit waits to improve reliability

<h2>How It Works</h2>
Launch Browser & Open Website-Chrome browser is launched and navigates to RedBus<br>
Select Source & Destination-Source location: Mumbai.<br>
Destination location: Pune<br>
Auto-suggestions are handled dynamically.<br>
Search for Buses<br>
Apply Filters-Primo and Evening<br>
Handle Lazy Loading<br>

<h2>Setup Instructions</h2>
Install Java JDK (11 or above)<br>
Install Maven <br>
Install Google Chrome Browse<br>
<h3>Steps to Run</h3>
Clone the repository or copy the project files(https://github.com/manasi7830/RedBusAutomationAssignment.git).<br>
Install dependencies<br>
Run RedBusAutomationAssignment.java
