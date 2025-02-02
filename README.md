# School Trip Management System

This project is a simple web-based application for managing school trips. It allows users to add new trips and view the list of all trips saved in a text file.

## Features
- **Add New Trip**: Users can fill out a form to enter details of a new trip (Destination, Start Date, End Date, Number of People, Budget).
- **View All Trips**: Displays a list of all trips stored in a text file.

## Technology Stack
- **JSP (JavaServer Pages)** for dynamic web content.
- **Servlets** (Embedded in JSP) for server-side logic.
- **HTML/CSS** for front-end user interface.
- **Java I/O** for saving trip data in a text file.

## How It Works
1. **Add New Trip**: The form in `tripForm.jsp` allows the user to enter trip details. When the form is submitted, the data is saved to a file `trips.txt` located in the `data` directory.
2. **View All Trips**: The `viewTrips.jsp` page reads the data from `trips.txt` and displays it in a table.

## Project Structure
- `tripForm.jsp`: Contains the form for adding new trips.
- `saveTrip.jsp`: Handles saving the trip data to a file.
- `viewTrips.jsp`: Displays the list of all trips stored in the `trips.txt` file.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/bettonhezron/School-Trip-Manager.git
2. Open the project with VS Code:
After cloning, open the project directory (School-Trip-Manager) in VS Code.
You can make any changes as needed. Ensure your project structure is correct, and add any additional code if necessary.
3. Install Tomcat if you don't have Tomcat installed.

Follow the instructions for your operating system to set up Tomcat.
4. Deploy the Project to Tomcat:
Navigate to your Tomcat installation directory. Inside the webapps folder, create a new folder named schooltripmanager.
Copy the entire project folder (the contents of School-Trip-Manager) into the schooltripmanager folder inside webapps. The folder structure should look like this:

webapps/
  schooltripmanager/
    WEB-INF/
      web.xml
    tripForm.jsp
    saveTrip.jsp
    viewTrips.jsp
    data/
      trips.txt
      
The data directory is used to store the trip data in the trips.txt file.
5. Start Tomcat: After deploying the project, you need to start Tomcat.
6. Access the Application:  Open your web browser and go to:  http://localhost:8080/schooltripmanager/ This will open the homepage of your School Trip Manager application.
7. Interact with the Application:Add a New Trip:
Navigate to http://localhost:8080/schooltripmanager/tripForm.jsp to fill in and submit a new trip.
View All Trips:
Navigate to http://localhost:8080/schooltripmanager/viewTrips.jsp to see the list of all trips saved in the trips.txt file.
