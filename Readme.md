

# **AI-Powered Chat Application (MERN Stack + OpenAI API)**  

## 🚀 **Overview**  
This is a full-stack AI-powered chat application built using the **MERN stack** (MongoDB, Express, React, Node.js) and the **ChatGPT API**. The app allows users to send messages and receive AI-generated responses.  

## 🏗 **Tech Stack**  
- **Frontend:** React, Axios  
- **Backend:** Node.js, Express, Axios  
- **Database:** MongoDB Atlas (Cloud)  
- **API Integration:** OpenAI GPT-3.5  

---

## 📁 **Project Structure**  
```
📦 chatgpt-web-app
 ┣ 📂 backend
 ┃ ┣ 📂 routes
 ┃ ┃ ┗ 📜 chat.js
 ┃ ┣ 📜 server.js
 ┃ ┣ 📜 .env
 ┃ ┗ 📜 package.json
 ┣ 📂 frontend
 ┃ ┣ 📂 src
 ┃ ┃ ┣ 📂 components
 ┃ ┃ ┃ ┗ 📜 Chat.js
 ┃ ┃ ┣ 📜 App.js
 ┃ ┃ ┣ 📜 index.js
 ┃ ┃ ┗ 📜 styles.css
 ┃ ┣ 📜 package.json
 ┃ ┣ 📜 .env
 ┃ ┗ 📜 README.md
 ┣ 📜 README.md
 ┗ 📜 .gitignore
```

---

## ⚙️ **Installation & Setup**  

### **1️⃣ Clone the Repository**  
```bash
git clone https://github.com/your-username/chatgpt-web-app.git
cd chatgpt-web-app
```

### **2️⃣ Backend Setup**  
```bash
cd backend
npm install
```
Create a `.env` file in the **backend** folder and add your OpenAI API key and MongoDB Atlas connection string:  
```
OPENAI_API_KEY=your_openai_api_key
MONGO_URI=your_mongodb_connection_string
PORT=5000
```
Start the backend server:  
```bash
npm run dev  # Using nodemon
```

### **3️⃣ Frontend Setup**  
```bash
cd ../frontend
npm install
```
Start the React app:  
```bash
npm start
```

---

## 📌 **Usage**  
1. Open **http://localhost:3000** in your browser.  
2. Type a message in the chat input and press "Send".  
3. The AI (ChatGPT) will respond to your message.  
4. The conversation history will be displayed in the chat window.  

---

## 🚀 **Features**  
✅ Real-time AI-powered chat responses  
✅ REST API built with Express.js  
✅ MongoDB Atlas integration for data storage  
✅ Fully responsive React frontend  
✅ Secure API key storage using `.env`  

---

## 🛠 **Troubleshooting & Common Issues**  

### ❌ **CORS Policy Error**
- Add CORS middleware in `backend/server.js`:  
  ```javascript
  const cors = require('cors');
  app.use(cors());
  ```

### ❌ **ChatGPT API Rate Limit Exceeded (Error 429)**
- Check usage at: [OpenAI Usage Dashboard](https://platform.openai.com/account/usage).  
- Reduce request frequency in `frontend/src/components/Chat.js`:  
  ```javascript
  await new Promise(resolve => setTimeout(resolve, 1000)); // 1-second delay
  ```

### ❌ **MongoDB Connection Issues**
- Ensure your **MongoDB Atlas URI** in `.env` is correct.  
- Verify IP Access in MongoDB Atlas: **Network Access > Add IP Address > Allow All (0.0.0.0/0)**.  

---

## 🎯 **Future Enhancements**  
🔹 User Authentication (Login & Signup)  
🔹 Store chat history in MongoDB  
🔹 Voice-to-text support  
🔹 Deploy on **Heroku (Backend)** & **Vercel (Frontend)**  

---

## 📝 **Contributing**  
Pull requests are welcome! Feel free to contribute by improving UI, adding new features, or optimizing performance.  

1. Fork the repo  
2. Create a new branch (`git checkout -b feature-name`)  
3. Commit changes (`git commit -m "Added new feature"`)  
4. Push to the branch (`git push origin feature-name`)  
5. Open a **Pull Request**  

---

## 📜 **License**  
This project is licensed under the **MIT License**.  

---

### 🌟 **Star this repo if you found it useful!** ⭐  
Let me know if you need any modifications! 🚀
