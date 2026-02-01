# 📝 Markdown Note App

Modern Markdown note-taking web app with folders, dark/light mode, live preview, and export to PDF/MD.

## Screenshots

![Screenshot 1](https://github.com/SyedShaheerHussain/markdown-note-app/blob/1fec7c8a1ac827d106eb4096a2b8a7c7975caaf7/markdown-note-app/sceenshots/Screenshot%20(51).png)

![Screenshot 2](https://github.com/SyedShaheerHussain/markdown-note-app/blob/1fec7c8a1ac827d106eb4096a2b8a7c7975caaf7/markdown-note-app/sceenshots/Screenshot%20(52).png)

## **Introduction**

A modern, professional, and fully-featured **Markdown note-taking web app** that supports **folders, dark/light mode, live preview, exporting notes to PDF/Markdown**, and local storage. Designed for developers, students, and anyone who wants a clean, productive note-taking experience.

## **Languages & Technologies Used**

### **Languages**

* JavaScript (ES6+)
* HTML5
* CSS3

### **Technologies / Libraries / Tools**

* Node.js 🌐 (for server-side markdown-to-HTML/PDF conversion)
* Express.js (Server API)
* Markdown-It (for Markdown to HTML conversion)
* HTML DOM APIs (frontend)
* CSS Variables (for dark/light theme switching)
* LocalStorage (for saving notes locally)

## **Learning Outcomes / What I Learned**

* How to structure a full-stack **frontend + backend web app**
* Handling **theme toggling** and **CSS variables**
* Implementing **folder-based note systems**
* Exporting content as **Markdown and PDF**
* Using **internal scrolls vs page scroll** properly
* Best practices in **flexbox/grid layouts** for modern GUIs
* Communicating between **frontend and backend via fetch API**

## **Discussion / Flow**

### **Flow of the Application**

```text
User → Folder → Note → Editor → Live Preview → Save / Export

```

1. User creates/selects a **folder**
2. Adds or edits a **note**
3. **Markdown editor** displays input on the left
4. **Live preview** renders on the right
5. User can **save locally**, **download Markdown**, or **export PDF**

## **Example Use Case**

* Developer wants to **take daily notes** for projects.
* Student wants **organized notes with folder structure**.
* Writer wants **markdown writing experience with preview**.

## **Installation & Setup**

### **Server Setup**

1. Open terminal in the **server folder**
2. Run:

```bash
npm install

```

3. Then run the server:

```bash

node index.js

```

### 4. Server output example:

```text
Server running on http://localhost:3000

```

### 🕴 **Client Setup**

1. Navigate to **client folder**
2. Open `index.html` **by double-clicking** (do not open via browser file URL only)
3. App should now run locally and connect to backend

>[!note]
> ⚠️ Opening `index.html` without running the server will break **Markdown to HTML/PDF export** functionality.

## 📃 **Objectives**

* Provide a **full-featured markdown editor** for notes
* Organize notes in **folders**
* Support **dark and light modes** for accessibility
* Allow **live preview** of markdown
* Export notes as **PDF or Markdown**
* Enable **local storage saving** for offline usage

## 🗝 **Key Concepts**

* **Markdown syntax** and conversion to HTML
* **Client-server communication** via Fetch API
* **CSS Variables** for dynamic theming
* **Flexbox & Grid layouts** for responsive UI
* **LocalStorage** for persistent data

## 💻 **GUI / Project Structure**

### **Project Folder Structure**

```
MarkdownNoteApp/
├── client/
│   ├── index.html
│   ├── style.css
│   └── app.js
├── server/
│   ├── index.js
│   └── package.json
├── README.md

```

### 🖥 **User Interface**

* **Sidebar:** Folder list + theme toggle + create folder button
* **Main Content:**

  * Note title input (small)
  * Editor (large, scrollable)
  * Preview (large, scrollable)
  * Action buttons: Save, Download MD, Export PDF

## 🔄 **Features**

* 🌙 **Dark/Light Mode** toggle
* 📁 **Folder system** for organizing notes
* 📝 **Markdown Editor** with live preview
* 💾 **Save notes locally**
* 📄 **Export Markdown files**
* 📑 **Export full notebook PDF**
* 🖱️ **Scrollable editor & preview** independent of window
* ✅ **Responsive layout** (modern professional style)

## ✔ **Functions / How It Works**

* **Create Folder:** Prompt user → add folder → save to localStorage
* **Select Folder:** Load note data → populate editor & preview
* **Edit Note:** Live markdown rendering via server
* **Save Note:** Save note content in localStorage
* **Download Markdown:** Blob → download `.md`
* **Export PDF:** Send markdown → convert to HTML → PDF → download
* **Toggle Theme:** Switch CSS variables between dark/light

## 🏢 **Working Code Example**

```js

// Save note example
function saveNote() {
  if (!currentFolder) return alert("Select folder first");
  data[currentFolder] = [{ title: titleInput.value, content: editor.value }];
  localStorage.setItem("notes", JSON.stringify(data));
}

```

## 💯 **Important Notes / Disclaimer**

>[!disclaimer]
> * This is a **learning and demo project**
> * Server must run to enable **export and live preview** features
> * Opening `index.html` alone only works for editing notes, not exporting
> * Scroll and theme fixes have been implemented professionally

## 🔭 **Objectives Achieved**

* Fully functional **Markdown note web app**
* Persistent storage with **localStorage**
* **Dynamic theme** switching working correctly
* **Modern GUI** with proper alignment and scrolling
* **Export functionality** integrated with Node server

## 🤼 **Target Audience**

* Students 🧑‍🎓
* Developers 👩‍💻
* Writers ✍️
* Productivity enthusiasts 🚀

## 🔍 **Future Enhancements**

* Multiple notes per folder
* Search functionality
* Drag & drop folders
* React/Tailwind frontend for better UX
* Desktop version with Electron

## 📝 **Implementation & Value**

* Helps **organize notes efficiently**
* Improves **productivity with markdown**
* Teaches **frontend + backend integration**
* Demonstrates **theme management and responsive design**

## 📜 **License**

>[!important]
> MIT License – Free to use, modify, and distribute 💡

## **Summary**

This Markdown Note App is a **professional, modern, and full-featured note-taking tool** built with JavaScript, Node.js, HTML, and CSS. It covers **everything from theming, folder structure, live preview, export features, GUI layout, and internal scroll handling**. Perfect for beginners learning full-stack web development, or anyone looking for a **clean, local markdown note system**.

_**© 2026 @SyedShaheerHussain**_
