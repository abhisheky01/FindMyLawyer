# Find My Lawyer

**Find My Lawyer** is a web application where users can log in, post their legal problems and preferred appointment dates. The admin then assigns an advocate to the user. The advocate reviews the problem, provides solutions, and sets a consultation fee, which the user can then pay.

This project is built using **Spring Boot**, **React**, and **MySQL**.

## Features

- **User Registration & Login**: Users can create an account and log in to the system.
- **Problem Posting**: Users can post their legal issues and set an appointment date.
- **Admin Panel**: Admins can assign advocates to users, manage user and advocate data, and monitor transactions.
- **Advocate Interface**: Advocates can view assigned problems, provide solutions, and set consultation fees.
- **Payment Gateway**: Users can pay the consultation fees after receiving solutions from advocates.
- **Visitor Counter**: The application tracks the number of visitors.
- **Responsive UI**: The application features a responsive UI with animations for an enhanced user experience.

## Tech Stack

- **Backend**: Spring Boot
- **Frontend**: React.js
- **Database**: MySQL
- **Security**: JWT for authentication and authorization

## Project Structure

```bash
    
FindMyLawyer/
├── src/
│ ├── main/
│ │ ├── java/com/findmylawyer/
│ │ │ ├── controller/
│ │ │ ├── dto/
│ │ │ ├── dao/
│ │ │ ├── service/
│ │ │ ├── exception/
│ │ │ ├── security/
│ │ │ ├── model/
│ │ │ ├── util/
│ ├── resources/
│ │ ├── application.properties
│ ├── test/
├── frontend/
│ ├── src/
│ │ ├── components/
│ │ ├── pages/
│ │ ├── services/
│ ├── public/
│ ├── package.json
├── pom.xml
└── README.md
```

## Installation

### Prerequisites

- **Java 17** or higher
- **Node.js** (for the React frontend)
- **MySQL** database

### Backend Setup

1. **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/find-my-lawyer.git
    cd find-my-lawyer
    ```

2. **Configure the database:**

   Update the `src/main/resources/application.properties` file with your MySQL database credentials.

    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/find_my_lawyer_db
    spring.datasource.username=your-username
    spring.datasource.password=your-password
    ```

3. **Build and run the backend:**

    ```bash
    ./mvnw clean install
    ./mvnw spring-boot:run
    ```

### Frontend Setup

1. **Navigate to the `frontend` directory:**

    ```bash
    cd frontend
    ```

2. **Install the dependencies:**

    ```bash
    npm install
    ```

3. **Run the React application:**

    ```bash
    npm start
    ```

4. **Access the application** by navigating to `http://localhost:3000`.

## Usage

### Admin Panel

- Admins can log in using their credentials.
- Navigate to the Admin Dashboard to manage users, advocates, and appointments.
- Assign advocates to users based on the problems posted.

### Advocate Interface

- Advocates can log in and view assigned cases.
- Provide legal solutions and set the consultation fee for each case.

### User Interface

- Users can log in, post problems, and pay fees after receiving solutions.

## Registration & Authentication

- Users can register directly through the application.
- Advocates are registered only by the admin.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Special thanks to the developers and contributors who helped build this project.

