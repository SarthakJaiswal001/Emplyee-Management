# User Management Web App

This is a user management web application built with Prisma, Next.js, TypeScript, and Docker. It facilitates basic CRUD (Create, Read, Update, Delete) operations on user data.

## Features

- **Create**: Add new users with relevant details.
- **Read**: View a list of all users and their information.
- **Update**: Modify existing user information.
- **Delete**: Remove users from the system.

## Prerequisites

Ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v14 or higher)
- [Docker](https://www.docker.com/) and [Docker Compose](https://docs.docker.com/compose/install/) (for containerization)

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/user-management-app.git
   cd user-management-app
2. **Install Dependencies**
   ```bash
   cd frontend
   npm install
   cd ../backend
   npm install

3. **Setup environment variables**
   Create a `.env` file in the `backend` directory and configure it with your PostgreSQL database credentials. For example:
   ```bash
   DATABASE_URL="postgresql://username:password@localhost:5432/database_name"

   Username and password are both postgres in my case.

4. **Start PostgreSQL with Docker**
   ```bash
   docker-compose up -d PostgreSQL
5. **Run Database Migration**
   ```bash
   cd backend
   npx prisma migrate dev

6. **Build the Frontend**
   ```bash
   cd ../frontend
   npm run build

7. **Build the backend**
   ```bash
   cd ../backend
   npm run build

## Usage
1. **Start the Container**
   ```bash
   docker-compose up -d

2. **Access the application**
  - Frontend: Open your browser and visit `http://localhost:3000`
  - Backend API: Access API endpoints through `http://localhost:4000`

## Contributing
I welcome contributions! To contribute to this project, follow these steps:

1. Fork this repository.
2. Create a branch: `git checkout -b feature-name`.
3. Make your changes and commit: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin feature-name`.
5. Submit a pull request.


