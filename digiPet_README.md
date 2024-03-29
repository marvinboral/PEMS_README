<p align="center">
  <a href="" rel="noopener">
 <img width=200px height=200px src="https://rod.2-d.jp/files/medias/MOB_2/20190802161503.png" alt="Project Logo"></a>
</p>

<h3 align="center">DigiPet</h3>

<div align="center">

  [![Status](https://img.shields.io/badge/status-active-success.svg)]() 
  [![GitHub Issues](https://img.shields.io/github/issues/kylelobo/The-Documentation-Compendium.svg)](https://github.com/marvinboral/digiPet)
  [![GitHub Pull Requests](https://img.shields.io/github/issues-pr/kylelobo/The-Documentation-Compendium.svg)](https://github.com/marvinboral/digiPet/pulls)
  [![License](https://img.shields.io/badge/license-MIT-blue.svg)](/LICENSE)

</div>

---

<p align="center"> digiPet
    <br> 
</p>

## 📝 Table of Contents
- [Project Introduction](#project_intro)
- [Project Goal](#project_goal)
- [Getting Started](#getting_started)
  - [Installation Steps](#installation-steps)
  - [Installation of Visual Studio Community](#installation-of-visual-studio-community)
  - [Running the Project in Visual Studio](#running-the-project-in-visual-studio)
  - [Additional Notes](#additional-notes)
- [File Structure](#file_structure)
- [Deployment](#deployment)
- [Built Using](#built_using)
- [Contributing](../CONTRIBUTING.md)
- [Authors](#authors)
- [Acknowledgments](#acknowledgement)

# 🧐 Project Introduction <a name = "project_intro"></a>
This assignment is `digiPet` which aims to demonstrate our competency with various controls based on what we have learned in Mobile Application Development. 

## Project Goal <a name = "project_goal"></a>
The goal of this project is to create a digital pet that contains the following features.

The pet should:

- maintain its state between app launches
  - start in some happy state
  - over time transition to some less happy state
  - regain happiness when "treated"
- respond to gestures for example
  - petting/swiping
  - patting/tapping
  - walking/dragging
- keep track of toys/inventory/points/whatever
- produce feedback for the user when events occur
  - vibration
  - sound
  - colours
  - animation

**In Scope** for this project, means that these are the items that I was able to implement.
- petState
- petState transitions to some less happy state or `worse` if there is no interaction done within a specified amount of time. clingy much
- regain normal state when interacting like patting or feeding
- sounds via expo-av

**Out of Scope** - items that I didn't have the chance to implement or include in this project because of `reasons`, but mainly due to insufficient time for a lot of stuff. Maybe for the final project. hmmm
- inventory
- haptics
- orientation
- expo-sqlite or database

# 🏁 Getting Started <a name = "getting_started"></a>
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See [deployment](#deployment) for notes on how to deploy the project on a live system.

## Prerequisites
What things do you need to install the software and how to install them

- Visual Studio 2022
- Node.js
- Expo Go
- Android Studio 
   
## Installation Steps

### Installation of Visual Studio Community
- Visit  [this link](https://visualstudio.microsoft.com/vs/community/) to download and install Visual Studio Community from the official Visual Studio website.

### Installation of Node.js
- Visit [thislink](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) for the guide and installation of Node.js

### Installation of Expo Go
- Visit the following links for the detailed steps of installing Expo Go in your system
  - [Installation Guide](https://docs.expo.dev/get-started/installation/) - Installation
  - [How to install in your Device](https://docs.expo.dev/get-started/expo-go/) - Guide to installing to your mobile device
  - [Create and run a project](https://docs.expo.dev/get-started/create-a-project/) - creating and running a project

### Cloning Repo in Visual Studio Steps
- Follow these steps to clone a repository in Visual Studio:
  1. Open Visual Studio.
  2. Go to the "Team Explorer" tab.
  3. Click on the "Manage Connections" icon (usually looks like a plug).
  4. Click on "Clone" under the "Local Git Repositories" section.
  5. Enter the URL of the repository you want to clone.
     ```
     https://github.com/marvinboral/digiPet.git
     ```
  7. Choose a local path for the repository.
  8. Click "Clone" to start the cloning process.

## Running the Project in Visual Studio

Once you have cloned the repository and configured the SQL Server, follow these steps to run the project in Visual Studio:

1. Open Visual Studio.
2. Open the project solution file (.sln) from the cloned repository usually named as PEMS.sln.
3. In View tab, click terminal it will show the developer powershell on the bottom of your screen.
4. Navigate to the file location of the project folder using: `cd`.
5. Navigate to the digiPet: `cd digiPet`
8. Run npm install in the same directory location to install the dependencies: `npm install`
      
11. Build the solution by selecting "Build" > "Build Solution" from the menu.
12. Press F5 or select "Debug" > "Start Debugging" to run the project.

## Additional Notes
- If you encounter any issues during installation or configuration, refer to the official documentation provided by Microsoft, Visual Studio Community, or Expo Go.

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


## 🎈 Usage <a name="usage"></a>
Add notes about how to use the system. (TO DO)

## 🚀 Deployment <a name = "deployment"></a>
TO DO

## ⛏️ Built Using <a name = "built_using"></a>
- [MS SQL 2019](https://www.microsoft.com/en-us/sql-server/sql-server-2019) - Database
- [Windows Server 2019](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019#Overview) - Server Framework and Environment
- [.NET 6](https://learn.microsoft.com/en-us/dotnet/core/whats-new/dotnet-6) - Web Framework
- [Javascript](https://www.javascript.com/) - Front-End Web Development
- [Microsoft C#](https://learn.microsoft.com/en-us/dotnet/csharp/) - Back-End Development

## ✍️ Authors <a name = "authors"></a>
- [@kylelobo](https://github.com/kylelobo) - readme.md template

### Contributors ###
Stefan Joseph - Team Leader
Marvin Boral - Project Manager
Mark Alexander - Quality Assurance Lead
Grazielle Agcaoili - Lead Programmer
Martin Rizada - System Design Lead
Razario Honiwell - UI/UX Lead

## 🎉 Acknowledgements <a name = "acknowledgement"></a>
- Hat tip to anyone whose code was used
- Inspiration
- References
