# 💬 Mini WhatsApp

A clean and responsive full-stack chat application built using **Node.js, Express, MongoDB, and EJS**. This app features full CRUD functionality (Create, Read, Update, Delete) with a WhatsApp Web-inspired UI layout.

---

## 🚀 Features

* 📩 **Live Message Feed:** Displays active chats with sender, receiver, content, and real-time formatted timestamps.
* ➕ **Create Conversation:** Instantly post new messages through dedicated forms.
* ✏️ **Edit Message:** Update chat content dynamically using RESTful PUT routes.
* 🗑️ **Delete Chat:** Cleanly remove conversations using `method-override` DELETE requests.
* 🎨 **Modern WhatsApp UI:** Features modern CSS cards, color themes, responsive layouts, and styled action buttons.

---

## 🛠️ Tech Stack

* **Backend:** Node.js, Express.js
* **Database:** MongoDB, Mongoose ODM
* **Templating Engine:** EJS (Embedded JavaScript)
* **Styling:** Custom CSS3 (Flexbox, CSS Variables)
* **Middleware:** `method-override`, `express.urlencoded`, `express.static`

---

## 📂 Project Structure

```text
mini-whatsapp/
│-- models/
│   └── chat.js          # Mongoose Chat Schema & Model
│-- public/
│   └── style.css        # Modern WhatsApp-themed CSS
│-- views/
│   │-- index.ejs        # All chats display feed
│   │-- new.ejs          # New message creation form
│   └── edit.ejs         # Edit chat content form
│-- init.js              # Database seed data script
│-- index.js             # Express application server & routes
└── package.json

---

## 📦 Installation & Setup

1. **Clone the repository:**
git clone https://github.com/Rajesh07-art/mini-whatsapp.git
cd mini-whatsapp


2. **Install dependencies:**
mongodb://127.0.0.1:27017/whatsapp


3. **Seed initial data (Optional):**
node init.js


4. **Start the Express server:**
node index.js


5. **View in Browser:**
Open http://localhost:8080/chats


## 🛣️ API / REST Routes

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| **GET** | `/chats` | Fetch and display all existing chats |
| **GET** | `/chats/new` | Render form to create a new message |
| **POST** | `/chats` | Save a new chat to the database |
| **GET** | `/chats/:id/edit` | Render form to edit an existing message |
| **PUT** | `/chats/:id` | Update chat message content in MongoDB |
| **DELETE** | `/chats/:id` | Remove a chat from the database |