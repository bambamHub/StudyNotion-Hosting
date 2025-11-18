StudyNotion Ed-Tech Project
<p align="center">🧠 StudyNotion – MERN EdTech Platform</p>
<p align="center"> <img width="1919" height="869" alt="image" src="https://github.com/user-attachments/assets/713c1a82-1d59-4ae4-ba2b-9c515f954172" />
 </p> 
<p align="center">A modern and scalable EdTech platform built using the MERN stack.</p> <p align="center"> <img src="https://img.shields.io/badge/Frontend-React.js-61dafb?style=for-the-badge&logo=react&logoColor=white" /> <img src="https://img.shields.io/badge/Backend-Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" /> <img src="https://img.shields.io/badge/Database-MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" /> <img src="https://img.shields.io/badge/Authentication-JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white" /> </p>
📚 Overview

StudyNotion is a full-featured EdTech platform where students can learn, purchase courses, track progress, and watch videos, while instructors can create courses, upload content, and manage students.

This project uses:

React + Redux Toolkit for UI

Node.js + Express for API

MongoDB + Mongoose for database

Razorpay for secure payments

Cloudinary for content upload

OTP-based authentication + Nodemailer

🚀 Features
👨‍🎓 Student Features

Sign up & Login with OTP

Purchase courses using Razorpay

Watch videos securely

Track course progress

Review and rate courses

Edit profile & change password

👨‍🏫 Instructor Features

Create & manage courses

Upload lecture videos to Cloudinary

Add sections & subsections

Instructor dashboard analytics

🛡️ Backend & Admin Features

JWT Authentication with cookies

Secure password hashing (bcrypt)

OTP verification via email

Payment signature verification

Scheduled tasks (node-schedule)

Error handling & middleware security

📁 Folder Structure
studynotion
│── backend
│   ├── controllers
│   ├── models
│   ├── routes
│   ├── middleware
│   ├── utils
│   ├── index.js
│   └── package.json

│── frontend
│   ├── src
│   │   ├── components
│   │   ├── pages
│   │   ├── redux
│   │   ├── utils
│   │   └── App.js
│   ├── public
│   └── package.json

🔧 Environment Variables

Create a .env file inside the backend folder:

PORT=4000
MONGODB_URL=your_mongo_url
JWT_SECRET=your_jwt_secret
CLOUDINARY_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_key
CLOUDINARY_API_SECRET=your_cloudinary_secret
MAIL_HOST=smtp.gmail.com
MAIL_USER=your_email
MAIL_PASS=your_password
RAZORPAY_KEY=your_razorpay_key
RAZORPAY_SECRET=your_razorpay_secret

🛠️ Installation & Setup
1. Clone the repo
git clone https://github.com/your-username/studynotion.git
cd studynotion

2. Install backend dependencies
cd backend
npm install

3. Install frontend dependencies
cd ../frontend
npm install

▶️ Run the App
Start backend
cd backend
npm run dev

Start frontend
cd frontend
npm start

Start both together (from frontend)
npm run dev

📸 Screenshots
Home Page
![Home Page](https://github.com/user-attachments/assets/705b9060-7f88-4b22-9451-e1b7f45f7acb)

Course Page
![Course Page](https://github.com/user-attachments/assets/1717cb28-cf85-440f-9378-02e61972357a)

Video Player
![Video Player](https://github.com/user-attachments/assets/286902f5-519f-4d3d-8a0c-d71a7fe83b5b)

Student Dashboard
![Student Dashboard](https://github.com/user-attachments/assets/32ece1bc-2c3d-4648-9a47-9665c9137020)

Instructor Dashboard
![Instructor Dashboard](https://github.com/user-attachments/assets/704853de-ec70-438f-8fa4-e07ef3e21b2d)


💳 Payment Flow (Razorpay)

User selects a course

Razorpay order created

Payment successful → Backend verifies signature

Course unlocked for the student

🔗 API Endpoints
Auth

POST /auth/signup

POST /auth/login

POST /auth/send-otp

Courses

POST /course/create

GET /course/all

GET /course/:id

POST /course/add-section

POST /course/add-subsection

Payments

POST /payment/capture

POST /payment/verify

🤝 Contributing

Contributions are always welcome!
Submit a PR or open an issue.

📝 License

This project is licensed under the ISC License.

👨‍💻 Author

Bambam Gupta
Creator of StudyNotion – MERN EdTech Platform

