
# Donatehere-donation and fundraiser platform

DonateHere is a full-stack fundraising platform that allows users to create, manage, and share donation campaigns with ease. Designed with a focus on transparency and simplicity, the platform provides a smooth user experience for both donors and fundraisers. Users can set up fundraisers, upload details, track progress, and receive support, while the admin panel ensures authenticity through a verification process.

Built using modern web technologies and deployed on Render, DonateHere demonstrates practical skills in full-stack development, user-centric design, and cloud deployment.


## Features

- 3-Step Fundraiser Creation – A simple, guided process to set up fundraisers with essential details, images, and goals.

- Secure Payments via Stripe – Enables safe and seamless card transactions for donors.

- Role-Based Access (User, Admin, Super Admin) – Ensures controlled access and smooth management across all user types.

- Analytics Dashboard – Admins and Super Admins can track platform statistics, fundraiser performance, and overall activity.

- Recent Activity Tracking – Admins and Super Admins can monitor the latest actions taken across the platform.

- Fundraiser Requests Panel – A dedicated review section for Admins to verify or reject new fundraiser submissions.

- Admin Management (Super Admin) – Super Admins can promote or demote users to Admin roles with a single click.

- Published Fundraisers Control – Super Admins can remove suspicious or fraudulent fundraisers instantly.

- Verified Fundraisers Page – Super Admins can publish fundraisers that have been reviewed and approved by Admins.




## 🛠️ Tech Stack

### **Frontend**
- **React.js (v19)** – Component-based UI framework  
- **Vite** – Fast development environment and optimized builds  
- **Tailwind CSS (v4)** – Utility-first CSS for responsive styling  
- **React Router DOM (v7)** – Client-side routing  
- **Axios** – API communication  
- **React Toastify** – Toast notifications  
- **Framer Motion** – Smooth UI animations  
- **GSAP** – Advanced motion animations  
- **Lucide React** – Icon library  
- **Three.js** – 3D visuals & effects  
- **Chart.js + react-chartjs-2** – Analytics and charts  
- **Stripe JS + React Stripe** – Frontend payment integration  

---

### **Backend**
- **Node.js** – JavaScript runtime  
- **Express.js (v5)** – Backend framework for APIs  
- **Mongoose (v8)** – MongoDB ODM  
- **Stripe (v18)** – Secure payment integration  
- **Cloudinary** – Image hosting & management  
- **Multer + Streamifier** – File uploads & buffer handling  
- **Nodemailer** – Email notifications  
- **bcryptjs** – Password hashing  
- **JSON Web Token (JWT)** – Role-based authentication  
- **CORS** – Cross-origin access control  
- **Body-Parser** – Request parsing  
- **dotenv** – Environment variables  

---

### **Development & Deployment**
- **Nodemon** – Auto-restart for backend during development  
- **Render** – Deployment for frontend & backend



## 🚀 Installation & Setup

Get **DonateHere** running locally by following these steps.

---

### 🔗 Clone the Project

```bash
git clone https://github.com/Akshay448591/DonateHere-Mini-Project-.git
cd DonateHere-Mini-Project-
```
### 🗂 Project Structure
```bash
Backend
│
├─ config
│   └─ cloudinary.js
├─ controllers
│   ├─ adminController.js
│   ├─ authController.js
│   ├─ fundraiserController.js
│   └─ userController.js
├─ middleware
│   ├─ authMiddleware.js
│   └─ upload.js
├─ models
│   ├─ Fundraiser.js
│   └─ User.js
├─ routes
│   ├─ admin.js
│   ├─ auth.js
│   ├─ fundraisers.js
│   ├─ payments.js
│   └─ users.js
├─ .gitignore
├─ package.json
├─ package-lock.json
└─ server.js
```
```bash
Frontend
│
├─ public
├─ src
│   ├─ assets
│   │   └─ react.svg
│   ├─ components
│   │   ├─ Categories.jsx
│   │   ├─ FAQ.jsx
│   │   ├─ Footer.jsx
│   │   ├─ Hero.jsx
│   │   ├─ HowitWorks.jsx
│   │   ├─ Navbar.jsx
│   │   ├─ ProtectedRoute.jsx
│   │   ├─ SectionBreaker.jsx
│   │   ├─ SmallGifts.jsx
│   │   ├─ Steps.jsx
│   │   └─ TrendingFundraisers.jsx
│   ├─ pages
│   │   ├─ AdminDashboardFundraisers.jsx
│   │   ├─ CategoryPage.jsx
│   │   ├─ CreateFundraiserStep1.jsx
│   │   ├─ CreateFundraiserStep2.jsx
│   │   ├─ CreateFundraiserStep3.jsx
│   │   ├─ DashboardAnalytics.jsx
│   │   ├─ DashboardPage.jsx
│   │   ├─ FundraiserDashboard.jsx
│   │   ├─ FundraiserPage.jsx
│   │   ├─ LandingPage.jsx
│   │   ├─ LoginPage.jsx
│   │   ├─ ProfilePage.jsx
│   │   ├─ PublishedFundraisers.jsx
│   │   ├─ SignupPage.jsx
│   │   ├─ SuperAdminDashboardFundraisers.jsx
│   │   ├─ SuperAdminHandleAdmins.jsx
│   │   └─ SuperAdminPublishedFundraisers.jsx
│   ├─ App.jsx
│   ├─ App.css
│   ├─ Axios.jsx
│   ├─ index.css
│   └─ main.jsx
├─ .gitignore
├─ README.md
├─ eslint.config.js
├─ index.html
├─ package.json
├─ package-lock.json
└─ vite.config.js
```
### ⚙️ Backend Setup
1.Navigate to the backend folder:
```bash 
cd Backend
```
2.Install dependencies:
```bash
npm install
```
3.Create a .env file based on .env.example:
```bash
MONGO_URI=your_mongo_uri_here
JWT_SECRET=your_jwt_secret_here
PORT=5000
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
FRONTEND_URL=http://localhost:5173
STRIPE_SECRET_KEY=your_stripe_secret_key
```
4.Start the backend server:
```bash
npm run dev
```

### ⚙️ Frontend Setup
1.Navigate to the frontend folder:
```bash
cd ../Frontend
```
2.Install dependencies:
```bash
npm install
```
3.Create a .env file based on .env.example:
```bash
VITE_STRIPE_PUBLISHABLE_KEY=your_stripe_publishable_key_here
```
4.Start the frontend server:
```bash
npm run dev
```
5.Open the app in your browser at:
```bash
http://localhost:5173
```
### 📝 Notes
1.Use Postman or similar tools to test backend APIs.

2.For production, update .env with production credentials.

3.Ensure MongoDB Atlas, Cloudinary, and Stripe accounts are properly configured.
## License
This project is licensed under the **MIT License**.  

You are free to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the project, provided that you include the original copyright notice and this permission notice in all copies or substantial portions of the Software.  

For more details, see the
[MIT](https://choosealicense.com/licenses/mit/)


# ⭐ Give this a Star


