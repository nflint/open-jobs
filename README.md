
## About Todo Jobs

Todojobs is a web application that allows to you record and keep track of your job applications. You can now ditch excel and use use todojobs which is easier and faster to use. Categorize and seamlessly manage your job applications.

![Todojobs Image](https://raw.githubusercontent.com/Babadinho/todo-jobs/main/client/src/public/images/hero.png)

## Features

- **Categorize your applications**: You can categorize your applications by creating different categories and adding your job applications to any corresponding category. You can also edit or delete your categories.
- **Manage application status**: You can manage your application status. You can change to Rejected, Assessment, Interview or set it to closed. It is automatically set to close when the end date reaches.
- **Manage job application**: You can delete or edit your job applications with easy. You can add notes to your job applications. Job applications with notes display the note count.
- **Robust job filter**: Filter between job applications using the category, status, and the job board or website. The search feature also adds and extra way to narrow down what you are looking for.

## Live Link

[https://todo-jobs-eta.vercel.app](https://todo-jobs-eta.vercel.app)

## Local Development Setup

### Prerequisites
- Node.js and npm installed
- MongoDB instance (local or Atlas)
- Git

### Installation Steps

1. **Clone the Repository**
```bash
git clone https://github.com/Babadinho/todo-jobs.git
cd todo-jobs
```

2. **Backend Setup**
```bash
# Install server dependencies
npm install

# Create .env file in root directory
touch .env
```

Add the following environment variables to `.env`:
```env
WEBSITE_DB=<your_mongodb_connection_string>
CLIENT_URL=http://localhost:3000
PORT=8000
JWT_SECRET=<your_jwt_secret>
```

3. **Frontend Setup**
```bash
# Navigate to client directory
cd client

# Install client dependencies
npm install

# Create .env file in client directory
touch .env
```

Add the following to client `.env`:
```env
REACT_APP_API=http://localhost:8000/api
```

4. **Running the Application**

In the root directory (backend):
```bash
npm start
# This will start the backend server on port 8000
```

In the client directory (frontend):
```bash
npm run dev
# This will start the frontend development server on port 3000
```

The application should now be running at:
- Frontend: http://localhost:3000
- Backend: http://localhost:8000

### Troubleshooting

If you encounter any issues during setup:
1. Make sure MongoDB is running if using local instance
2. Check that ports 3000 and 8000 are available
3. If you get module not found errors, try deleting node_modules and package-lock.json and run npm install again

