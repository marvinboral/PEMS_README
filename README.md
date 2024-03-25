<p align="center">
  <a href="" rel="noopener">
 <img width=200px height=200px src="https://i.imgur.com/kYtfvCA.png" alt="Project Logo"></a>
</p>

<h3 align="center">Peer Evaluation Management</h3>

<div align="center">

  [![Status](https://img.shields.io/badge/status-active-success.svg)]() 
  [![GitHub Issues](https://img.shields.io/github/issues/kylelobo/The-Documentation-Compendium.svg)](https://github.com/MartinRizada/PEMS/issues)
  [![GitHub Pull Requests](https://img.shields.io/github/issues-pr/kylelobo/The-Documentation-Compendium.svg)](https://github.com/MartinRizada/PEMS/pulls)
  [![License](https://img.shields.io/badge/license-MIT-blue.svg)](/LICENSE)

</div>

---

<p align="center"> The project is a Database Management System (DBMS) that will facilitate the student evaluation process.  The main goal is to enhance efficiency and accuracy.
    <br> 
</p>

## 📝 Table of Contents
- [Project Introduction](#project_intro)
- [Project Scope](#project_scope)
- [Team Introduction](#team_intro)
- [Getting Started](#getting_started)
  - [Installation Steps](#installation-steps)
    - [Downloading MS SQL Server 2019 Standard Edition](#downloading-ms-sql-server-2019-standard-edition)
    - [Installation of SQL Server](#installation-of-sql-server)
    - [Installing SQL Server Management Studio (SSMS)](#installing-sql-server-management-studio-ssms)
  - [Installation of Visual Studio Community](#installation-of-visual-studio-community)
    - [Configuring SQL Server](#configuring-sql-server)
    - [Restoring the Database Steps](#restoring-the-database-steps)
    - [Cloning Repo in Visual Studio Steps](#cloning-repo-in-visual-studio-steps)
  - [Running the Project in Visual Studio](#running-the-project-in-visual-studio)
  - [Additional Notes](#additional-notes)
- [File Structure](#file_structure)
- [Deployment](#deployment)
- [Usage](#usage)
- [Built Using](#built_using)
- [TODO](../TODO.md)
- [Contributing](../CONTRIBUTING.md)
- [Authors](#authors)
- [Acknowledgments](#acknowledgement)

# 🧐 Project Introduction <a name = "project_intro"></a>
Our project name is Peer Evaluation Management System or PEMS which is an evaluation database management system for our System Analysis and Design course which is also known as the CIT 2775/76 Program. Currently, the client is gathering student information from Canvas and manually transposing it into an Excel spreadsheet, he must manually calculate the ratings of each student and the ratings they receive from their teammates, he must categorize them as well as provide his evaluation/rating to the students. This process takes excessive time and requires constant precision, which can be difficult to do when he has over 40 students’ feedback and ratings to calculate and record.

The client is looking to create a database tied to a website that will allow students to log into their profiles and provide numerical and written feedback on each team member. The program needs to automatically calculate the scores entered by the students so that he can have grand totals for each student. The client also wants to be able to provide feedback to each student, view their feedback, view the ratings of other students, and generate a categorized report of the ratings by student or team.

**Purpose of Project:**
The project will facilitate the student evaluation process to enhance efficiency and accuracy, and provide insights through automated data collection, calculation, and presentation. The system that is being built in this project will be aligned to only two courses (CIT2275/6) and will not be integrated into Canvas. It will encompass two user types: **instructors** and **students**.

**Business Need:**
The project has been initiated to address the business need to streamline the current evaluation process. The existing manual data collection and calculation methods are time-consuming and inefficient, especially given the high number of student evaluations required. The need is to modernize and automate this process to improve efficiency and accuracy.

## Project Scope <a name = "project_scope"></a>
The project will facilitate the student evaluation process to enhance efficiency and accuracy, and provide insights through automated data collection, calculation, and presentation. The system being built in this project will be aligned to only two courses (CIT2275/6) and will not be integrated into Canvas. It will encompass two user types: instructors and students.

**In Scope**
- Data Collection
- Calculation
- Data Presentation
- Security
- Data Backup & Restoration

**Out of Scope**
- Course Alignment
- System Integration
- Excluded System features such as notifications and MFA (Multi-Factor Authentication)

## Team Introduction <a name = "team_intro"></a>
<p align="center">
  <a href="" rel="noopener">
 <img width=400px height=400px src="https://i.imgur.com/T9ElGBK.png" alt="Team Logo"></a>
</p>

**Team Name**: GR3MS Tech Solutions <br>
**Official Email Address**: <a href> GR3MSTechSolutions@lethbridgecollege.onmicrosoft.com </a> <br><br>
**Team Members** 
- Stefan Joseph, Team Leader
- Marvin Boral, Project Manager
- Grazielle Agcaoili, Lead Programmer
- Martin Rizada, System Design Lead
- Razario Honiwell, UIX Lead Designer
- Mark Alexander, Lead Quality Assurance Tester
  
**Client**: Mr. Timothy Frantz, CIT Instructor at Lethbridge College

# 🏁 Getting Started <a name = "getting_started"></a>
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See [deployment](#deployment) for notes on how to deploy the project on a live system.

## Prerequisites
What things do you need to install the software and how to install them.

- Visual Studio 2022
- NET Core 6 Framework
- C#
- Microsoft SQL 2019
   
## Installation Steps

### Downloading MS SQL Server 2019 Standard Edition
- Visit [this link](https://azureforeducation.microsoft.com/devtools) to download the 2019 MS SQL Standard Edition.

### Installation of SQL Server
- Follow the installation instructions provided by Microsoft for installing the SQL Server.
- Check the Database Engine
- Set the Instance Name to: `PEMS_SERVER`

### Installing SQL Server Management Studio (SSMS)
- After installing SQL Server, download and install SQL Server Management Studio from the official Microsoft website.

### Installation of Visual Studio Community
- Visit  [this link](https://visualstudio.microsoft.com/vs/community/) to download and install Visual Studio Community from the official Visual Studio website.

## Configuring SQL Server

### Restoring the Database Steps
- Follow these steps to restore a database:
  1. Open SQL Server Management Studio.
  2. Connect to your SQL Server instance.
  3. Right-click on `Databases` and select `Restore Files and Filegroups` 
  4. Choose the appropriate backup source (e.g., disk or URL).
  5. Select the most recent backup file
  6. Specify the destination database name: `PEMS`.
  7. Click "OK" to start the restoration process.

### Cloning Repo in Visual Studio Steps
- Follow these steps to clone a repository in Visual Studio:
  1. Open Visual Studio.
  2. Go to the "Team Explorer" tab.
  3. Click on the "Manage Connections" icon (usually looks like a plug).
  4. Click on "Clone" under the "Local Git Repositories" section.
  5. Enter the URL of the repository you want to clone.
  6. Choose a local path for the repository.
  7. Click "Clone" to start the cloning process.

## Running the Project in Visual Studio

Once you have cloned the repository and configured the SQL Server, follow these steps to run the project in Visual Studio:

1. Open Visual Studio.
2. Open the project solution file (.sln) from the cloned repository usually named as PEMS.sln.
3. In View tab, click terminal it will show the developer powershell on the bottom of your screen.
4. Navigate to the file location of the project folder using: `cd`.
5. Navigate to the PEMS: `cd PEMS`
6. Navigate to the ClientApp directory: `cd ClientApp`
7. It should be like this: `C:\Users\yourname\source\repos\ProjectPEMS\PEMS\ClientApp`
8. Run npm install in the same directory location to install the dependencies: `npm install`
9. Change the database connection string based on SQL Server Name and Database name in the following location
    - appsettings.json
    - PEMSContext.cs 
      
11. Build the solution by selecting "Build" > "Build Solution" from the menu.
12. Press F5 or select "Debug" > "Start Debugging" to run the project.

## Additional Notes
- Make sure to have the necessary permissions and credentials to perform the above actions.
- If you encounter any issues during installation or configuration, refer to the official documentation provided by Microsoft or Visual Studio Community.

#  File Structure <a name = "file_structure"></a>

This project is organized into several directories and files. 

## 📁  ClientApp/src

Main directory

### 📁 Components
- `AdminNav.js`: Navigation component for admin users.
- `EvaluationForm.js`: Form component for evaluations.
- `EvaluationForStudent.js`: Evaluation viewing component for students.
- `Footer.js`: Footer component displayed on all pages.
- `InstructorNav.js`: Navigation component for instructors.
- `StudentEvaluationReport.js`: Component to display evaluation reports to students.
- `StudentNav.js`: Navigation component for students.

## 📁 Modals

Modals are used to create pop-up windows in the application interface.  Modals are mainly used for CRUD functions on the administrator page. 

### List of Add Modal Components

- `AddCriteriaModal.js`: Modal to add evaluation criteria.
- `AddEvaluationModal.js`: Modal to add evaluations.
- `AddInstructorModal.js`: Modal to add instructors.
- `AddStudentModal.js`: Modal to add students.
-  `AddTeamModal.js`: Modal to add teams.

### Edit Modals

These modals are used for editing existing information.

- `EditCriteriaModal.js`: Modal to edit criteria information and details.
- `EditEvaluationModal.js`: Modal to edit evaluation details and information.
- `EditInstructorModal.js`: Modal used by admins or higher authority users, allowing them the ability to edit instructor details and information within the application interface easily and efficiently without needing direct access to the database or backend system directly, ensuring security protocols are maintained while providing flexibility in user management tasks.
- `EditSectionModal.js`: This modal allows authorized users (instructor/adminsitrator) with privileges sufficient enough, access into sections’ data where they can make necessary adjustments, corrections or updates as required ensuring that data integrity is maintained at all times while also allowing adaptability and modifications as needed aligning with organizational needs and requirements.
- `EditStudentModal.js`: A specialized modal designed specifically with features enabling easy editing of student’s data by instructor/administrator ensuring that student records are always up-to-date reflecting their current status, achievements, progress among other relevant details crucial in monitoring and evaluating student performance over time.
- `EditTeamModal.js`: This modal provides functionalities tailored towards making team data adjustments where necessary such as removing team members and updating the team name.

## 📁 Pages
This directory contains the main pages of PEMS:

- `AccountPage.js`: The account page.
- `AdminDashboard.js`: The admin dashboard page.
- `EvaluationPage.js`: The evaluation page.
- `InstructorReport.js`: The instructor report page.
- `LoginPage.js`: The login page.
- `StudentDashboard.js`: The student dashboard page.

## 📁 Styles

This directory contains the styles for the applications and has several sub-directories. 

### 📁 Components

This sub-directory contains the main components of the application. Each component has a corresponding CSS file for styling:

- `AdminNav.css`: Styles for the AdminNav component.
- `EvaluationForm.css`: Styles for the EvaluationForm component.
- `Footer.css`: Styles for the Footer component.
- `InstructorNav.css`: Styles for the InstructorNav component.
- `StudentNav.css`: Styles for the StudentNav component.

### 📁 Modals

This sub-directory contains the modals used in the application. Each modal has a corresponding CSS file for styling:

- `AddCriteriaModal.css`: Styles for the AddCriteriaModal.
- `AddEvaluationModal.css`: Styles for the AddEvaluationModal.
- `AddInstructorModal.css`: Styles for the AddInstructorModal.
- `AddStudentModal.css`: Styles for the AddStudentModal.
- `AddTeamModal.css`: Styles for the AddTeamModal.
- `EditCriteriaModal.css`: Styles for the EditCriteriaModal.
- `EditEvaluationModal.css`: Styles for the EditEvaluationModal.
- `EditInstructorModal.css`: Styles for the EditInstructorModal.
- `EditSectionModal.css`: Styles for the EditSectionModal.
- `EditStudentModal.css`: Styles for the EditStudentModal.

### 📁 Pages

This sub-directory contains the css styles for the following pages. 

- `AdminDashboard.css`: Styles for the AdminDashboard page.
- `InstructorReport.css`: Styles for the InstructorReport page.
- `LoginPage.css`: Styles for the LoginPage.
- `StudentDashboard.css`: Styles for the StudentDashboard page.

## Main Files

This directory contains the main files of PEMS.

- `App.js`: This is the main JavaScript file that holds the base component of the React app.
- `AppRoutes.js`: This file defines routes to various pages/views within the app.
- `custom.css`: This is a custom stylesheet for additional styles.
- `index.js`: This is the entry point JavaScript file for the React app, where ReactDOM renders the App component.
- `setupProxy.js`: This is a configuration file to set up a proxy to the backend API server


## 🔧 Running the tests <a name = "tests"></a>
Explain how to run the automated tests for this system.

### Break down into end to end tests
Explain what these tests test and why

```
Give an example
```

### And coding style tests
Explain what these tests test and why

```
Give an example
```

## 🎈 Usage <a name="usage"></a>
Add notes about how to use the system.

## 🚀 Deployment <a name = "deployment"></a>
Add additional notes about how to deploy this on a live system.

## ⛏️ Built Using <a name = "built_using"></a>
- [MongoDB](https://www.mongodb.com/) - Database
- [Express](https://expressjs.com/) - Server Framework
- [VueJs](https://vuejs.org/) - Web Framework
- [NodeJs](https://nodejs.org/en/) - Server Environment

## ✍️ Authors <a name = "authors"></a>
- [@kylelobo](https://github.com/kylelobo) - Idea & Initial work

See also the list of [contributors](https://github.com/kylelobo/The-Documentation-Compendium/contributors) who participated in this project.

## 🎉 Acknowledgements <a name = "acknowledgement"></a>
- Hat tip to anyone whose code was used
- Inspiration
- References
