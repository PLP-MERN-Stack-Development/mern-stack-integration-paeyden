#   Project - MyBlog
This project is a full-stack MERN (MongoDB, Express.js, React.js, Node.js) application built to demonstrate seamless integration between the front-end and back-end. The application allows users to create, view, update, and delete blog posts, manage categories, and includes optional advanced features like authentication, image uploads, and comments.

The project follows clean architecture principles with a well-defined folder structure, reusable components, and clear separation of concerns between client and server.

# 📁 Project Structure
 <pre><code>txt 
  mern-blog/
│
├── client/                 # React front-end (Vite)
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/          # Page views (Home, Post, Create, etc.)
│   │   ├── hooks/          # Custom React hooks
│   │   ├── services/       # API service for back-end communication
│   │   └── App.jsx         # Root React component
│   ├── .env.example
│   └── package.json
│
├── server/                 # Express.js back-end
│   ├── models/             # Mongoose models (Post, Category, User)
│   ├── routes/             # Express routes for posts, categories, auth, etc.
│   ├── middleware/         # Validation and error-handling middleware
│   ├── controllers/        # Logic for API endpoints
│   ├── config/             # MongoDB connection setup
│   ├── .env.example
│   └── server.js           # Entry point
│
└── README.md

 </code></pre>


## ⚙️ Setup Instructions
### Prerequisites


Make sure you have installed:

- Node.js (v18+)
- MongoDB



## 1️⃣ Clone the repository
<pre><code> 
 bash
 git clone <your-repo-url>
 cd mern-blog

</code></pre>
## 2️⃣ Set up the Server
<pre><code> bash
 cd server
npm install

</code></pre>


- Create a .env file in the server directory:

<pre><code>
 ini
 PORT=yourportnumber
MONGO_URI=mongodb://localhost:27017/mern_blog
JWT_SECRET=your_jwt_secret
</code></pre>


<pre><code>bash
 #run the server
 npm run dev
</code></pre>

## 3️⃣ Set up the Client
<pre><code>bash
 cd ../client
npm install

</code></pre>


Create a .env file in the client directory:

<pre><code>
 VITE_API_URL=yourapiurl

</code></pre>


<pre><code>bash
 #runtheclient
 npm run dev
</code></pre>


The client will typically start on http://localhost:5173
 and the server on http://localhost:5000
.

# 🧩 Features Implemented
###  🛠 Back-End

- RESTful API built with Express.js

- Mongoose models for Post and Category

- Input validation using express-validator

- Error handling middleware

- CORS and JSON body parsing middleware

- Optional JWT authentication

### 💻 Front-End

- Built with React (Vite)

- React Router for page navigation

- Reusable components for posts, forms, and layout

- Custom hooks for API calls and data fetching

- Optimistic UI updates and loading/error states

- Responsive UI design

### 🧠 Advanced Features (Optional)

- Authentication (Login/Register)

- Pagination and search



# 🌐 API Documentation
### 🔹 Posts
| Method | Endpoint           | Description         |
|--------|--------------------|---------------------|
| GET    | /api/posts         | Get all blog posts  |
| POST   | /api/posts         | Create a new post   |
| PUT    | /api/posts/:id     | Update a post       |
| DELETE | /api/posts/:id     | Delete a post       |

### 🔹 Categories
| Method | Endpoint           | Description         |
|--------|--------------------|---------------------|
| GET    | /api/categories    | Get all categories  |
| POST   | /api/categories    | Create new category |
| GET    | /api/categories/:id| Get post by category|

# 🧪 Expected Outcome

- Functional blog system with CRUD operations

- Proper communication between React front-end and Node.js API

- MongoDB database integration

- Clear code organization and modular design

- Responsive and intuitive user experience

# 📸 Screenshots 

### 🏠 Home Page
![Home Page](./assets/blog2.png)

### 📝 Edit Post Form
![Edit Post](./assets/blog1.png)

# 📜 License

- This project is for educational purposes as part of the Week 4 MERN Stack Integration Assignment.








