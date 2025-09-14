# filesharingmmc
Share ourfiles with multiple systems with accesskey and password
---

📁 Documents Sharing Platform

A sleek and secure **web-based document sharing platform** built with **HTML, CSS, JavaScript, and Google Apps Script backend**.
It allows users to **upload documents with a password and access key**, then **share and retrieve them securely** using those credentials.
The interface features a **3D animated starfield background** using **Three.js** for a modern aesthetic.

---

✨ Features

* 📤 **Upload documents** with:

  * File name
  * Password protection
  * Unique access key
* 📥 **Retrieve documents** securely by entering:

  * Access key
  * Password
* ⚡ **Real-time upload progress bar**
* 🚫 **Duplicate access key detection** with automatic suggestions
* 🌌 **3D animated background** using Three.js
* ☁️ **Google Apps Script backend + Google Sheets CSV** storage integration

---

🛠 Tech Stack

* **Frontend:**

  * HTML5, CSS3, Vanilla JavaScript
  * Three.js for animated background
* **Backend:**

  * Google Apps Script Web App (for storing file data to Google Drive)
  * Google Sheets (for storing file metadata)

---

⚙️ Setup Instructions
1. Deploy the Google Apps Script

1. Go to [Google Apps Script](https://script.google.com/).
2. Create a new project and paste your backend script logic to:

   * Accept POST requests from the upload form.
   * Store files in Google Drive.
   * Append file metadata (name, access key, password, link) into a Google Sheet.
3. Deploy as a **Web App** and set access to **https://filesharingmmc.netlify.app/**.
4. Copy the https://filesharingmmc.netlify.app/  and replace the value of:

 

2. Publish your Google Sheet as CSV

1. Link the Google Sheet to your Apps Script project.
2. Publish the sheet to the web as CSV (File → Share → Publish to Web).
3. Copy the CSV URL and replace the value of:

   ```js
   const sheetCSVURL = "YOUR_SHEET_CSV_URL_HERE";
   ```

---
 🚀 Usage

1. **Open the website.**
2. **Upload a file** by filling in:

   * File Name
   * Password
   * Access Key
   * Selecting a File
3. Click **Upload File** and wait for the upload to complete.
4. Share the **Access Key and Password** with the recipient.
5. Recipients can enter the details under **"Access the shared files"** to download the file.

---

🖼 UI Preview

* Clean glassmorphic cards with gradient background
* Progress bar feedback
* Starfield animation using Three.js

---

📌 Notes

* All uploaded files and metadata are stored in your own Google account.
* Each Access Key must be **unique** (the system will suggest a new one if duplicate is found).
* This is a **client-side-only UI**; all actual file storage is handled by your Google Apps Script backend.

---

 📄 License

This project is licensed under the [MIT License](LICENSE).

---



