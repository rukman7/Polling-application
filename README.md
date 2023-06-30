# Polling Application

Welcome to the Polling Application! This web application allows users to create and share polls, giving participants the opportunity to vote on various topics. The project was developed to refresh Python web app knowledge and gain a better understanding of React basics. The choice of a polling application was chosen as it encompasses various tools, libraries, and common web development designs I wanted to learn and refresh. Flask was selected as the web framework for its flexibility and ability to add additional functionality as needed.

## Features

The Polling Application offers the following features:

1. **User Registration:** Users can create an account to access the full features of the polling application. Registration requires providing basic information such as name, email, and password.

2. **Poll Creation:** Authenticated users can create their own polls by providing a question and a set of options. Each option represents a possible choice for the participants. The poll creator can customize the number of options and assign a label to each option.

3. **Poll Sharing:** Each poll is assigned a unique URL that can be shared with others, allowing them to participate in the poll. The URL can be easily copied and sent to friends, colleagues, or shared on social media platforms.

4. **Single Vote:** To ensure fair and accurate results, each participant can cast only one vote per poll. Once a vote is submitted, the participant cannot change their vote for that specific poll.

5. **Progress Bar:** The application displays the percentage of votes for each poll option, allowing participants to see the current distribution of votes. This feature provides visual feedback on the popularity of each choice.

6. **User Dashboard:** Users have access to a personalized dashboard where they can view and manage their created polls. The dashboard provides an overview of all the polls created by the user, allowing easy tracking and management.

## Technologies Used

The Polling Application utilizes the following technologies:

### Backend

- **Python:** The core programming language used for backend development.
- **Flask:** A lightweight web framework used for routing and handling HTTP requests. Flask provides a minimalistic yet powerful foundation for building web applications.
  - **Key libraries used:**
    - Flask SQL Alchemy: A Flask extension that simplifies working with SQL databases. It provides an easy-to-use interface for interacting with the database.
    - Flask Migrate: A Flask extension that handles database migrations. It allows seamless database schema changes during the development process.
    - Flask Admin: A Flask extension that generates administrative interfaces for managing the application's data. It provides a user-friendly interface for managing polls and user data.
    - Flask blueprints: A Flask extension that enables the creation of modular and reusable application components. Blueprints help structure the codebase and promote code organization.

- **Celery:** Celery is a distributed task queue system that allows running background jobs asynchronously. It is used in the Polling Application to handle time-consuming tasks such as sending notifications or processing large amounts of data without affecting the application's responsiveness.

- **SQLAlchemy:** SQLAlchemy is an Object-Relational Mapping (ORM) library for Python. It provides a high-level interface for working with databases, allowing developers to interact with the database using Python objects and methods. The Polling Application uses SQLAlchemy to interact with the underlying SQLite database.

- **SQLite:** SQLite is a lightweight and serverless relational database management system. It is used as the database backend for storing poll data in the Polling Application. SQLite is chosen for its simplicity and ease of use, making it suitable for smaller-scale applications.

### Frontend

- **React:** React is a popular JavaScript library for building user interfaces. It provides a component-based architecture and a virtual DOM, enabling developers to create dynamic and interactive web UIs. React is used in the Polling Application to build the frontend components and handle user interactions.

- **Bootstrap:** Bootstrap is a widely used CSS framework that provides pre-styled components and a responsive design system. It simplifies the process of creating visually appealing and mobile-friendly web interfaces. The Polling Application leverages Bootstrap to ensure a consistent and user-friendly look and feel.

- **HTML5/CSS3:** HTML5 and CSS3 are standard web technologies used for structuring and styling web pages. HTML5 provides the structure and semantic elements, while CSS3 is responsible for the visual presentation and layout of the web components. The Polling Application utilizes these technologies to create well-organized and visually appealing UI components.

### Deployment

- **GitHub:** GitHub is a version control and project management platform widely used by developers. It provides a centralized repository for hosting the Polling Application's source code, enabling collaboration and version control. GitHub also offers features such as issue tracking, pull requests, and code reviews, which streamline the development process.

- **Heroku:** Heroku is a cloud platform that simplifies the deployment and hosting of web applications. It provides an easy way to deploy Flask applications and ensures scalability and reliability. The Polling Application can be deployed to Heroku, allowing users to access and use the application from anywhere.

### Other Tools

- **Visual Studio Code:** Visual Studio Code is a popular source code editor that provides a rich set of features for web development. It offers syntax highlighting, debugging capabilities, and extensions that enhance the development experience. Visual Studio Code is used for frontend development in the Polling Application.

- **PyCharm:** PyCharm is a powerful integrated development environment (IDE) specifically designed for Python development. It offers advanced features such as code completion, debugging, and project management. PyCharm is used for backend development in the Polling Application, providing a comprehensive and efficient development environment.

- **SQL Toad:** SQL Toad is a tool used for designing and visualizing database schemas. It offers a user-friendly interface for creating and modifying database structures, allowing developers to design the database schema for the Polling Application efficiently.

## Installation

To get started with the Polling Application, follow these steps:

1. Clone the project repository:

   ```shell
   git clone https://github.com/rukman7/Polling-application.git
   ```

2. Install the required dependencies:

   ```shell
   pip install -r requirements.txt
   ```

3. Set the FLASK_APP and FLASK_DEBUG environment variables:

   ```shell
   export FLASK_APP=votr.py
   export FLASK_DEBUG=1
   ```

4. Finally start the application:

   ```shell
   flask run
   ```
   
   The application should now be up and running. Click on the URL provided at the command line to visit the application. 

## Screenshots

![create a poll](/static/images/create_polls.png)

![view polls](/static/images/view_polls.png)