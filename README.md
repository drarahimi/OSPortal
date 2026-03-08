# OSPortal: Outstanding Scholars Project Explorer 🎓

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge)

**OSPortal** is a comprehensive, client-side web application designed to help students and faculty efficiently explore, track, and manage academic research opportunities. Created by **Dr. Afshin Rahimi** at the University of Windsor, this tool processes CSV data dynamically to provide an interactive dashboard with advanced filtering, analytics, and personal application tracking capabilities.

---

## ✨ Key Features

- 📊 **Dynamic Data Ingestion**: Seamlessly parses the `Available Projects.csv` data upon load. Includes a fallback drag-and-drop interface if auto-load fails.
- 🎨 **Modern & Responsive UI**: Built with Tailwind CSS, featuring a glassmorphism header, smooth transitions, and a layout that adapts flawlessly to both desktop and mobile devices.
- 🌓 **Dark/Light Mode Theme**: Full theme support with a toggle switch. Respects the user's system preferences and saves their choice locally.
- 🔍 **Advanced Search & Filtering**:
  - Filter by *Faculty*, *Department*, *Remote/Online* availability, and *Community Partnerships*.
  - Powerful keyword search across project titles, descriptions, and supervisors.
  - Dynamic sorting (Newest, Oldest, Title A-Z, End Date).
- 🧙‍♂️ **Match Me Assistant**: An interactive 3-step wizard that helps students discover tailored projects based on their faculty, remote work preferences, and specific skill sets.
- 📋 **Multiple Project Views**:
  - **Grid View**: A clean, easy-to-read card layout.
  - **Timeline View**: Chronological layout organizing projects based on their end dates.
  - **Kanban Board (Application Tracker)**: A built-in CRM where students can manage applications by moving projects through custom stages (*⭐ Shortlisted, ✉️ Emailed, 🗣️ Interviewing, ✅ Accepted*).
- 📈 **Interactive Insights Panel**: Visual analytics powered by Chart.js. Displays Projects by Faculty, Top Departments, Delivery Format, Top Competencies, Top Supervisors, and a Word Cloud of project titles. *Clicking on chart elements automatically filters the project list!*
- 📄 **PDF Flyer Generation**: Automatically generate and download a clean, formatted PDF flyer (complete with an auto-generated QR code) for any specific project to print or share.
- 🔗 **Deep Linking**: Easily copy and share unique URL links that open directly to specific project modals.
- 💾 **Local Data Persistence**: Your Kanban board tracking states and theme preferences are automatically saved in your browser's local storage.

---

## 🛠️ Technology Stack

This project is entirely client-side, requiring no backend database or server infrastructure, making it highly portable and easy to host.

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Styling**: [Tailwind CSS](https://tailwindcss.com/) (Loaded via CDN)
- **Data Parsing**: [PapaParse](https://www.papaparse.com/)
- **Data Visualization**: [Chart.js](https://www.chartjs.org/) & [chartjs-chart-wordcloud](https://github.com/sgratzl/chartjs-chart-wordcloud)
- **PDF Generation**: [html2pdf.js](https://ekoopmans.github.io/html2pdf.js/)
- **QR Codes**: [qrcode.js](https://davidshimjs.github.io/qrcodejs/)
- **Icons**: [Phosphor Icons](https://phosphoricons.com/)

---

## 📂 Data Format

The application expects the `Available Projects.csv` file to contain the following key column headers. (The parser is robust and will gracefully handle missing fields):

* `Project_ID_Number`
* `Faculty_Member_Name`
* `Project_Title`
* `Project_End_Date`
* `Faculty`
* `Department_School_of_Research`
* `Project_Description`
* `Student_Opportunities_and_Tasks`
* `Anticipated_Competencies`
* `Research_Completed_Online` (Expects "Yes" or "No")
* `Community_Partnerships`
* `Faculty_Contact_Email`

---

## 💡 Usage Guide

1. **Explore & Filter**: Use the left sidebar to filter by Faculty or Department, or type keywords into the search bar to instantly narrow down the grid.
2. **Match Me**: Click the "Match Me" button in the top navigation bar and answer three quick questions to get personalized recommendations.
3. **Application Tracking**: Click on any project card to open its details modal. Use the dropdown at the bottom to set your application status to "Shortlisted", "Emailed", etc.
4. **View Kanban Board**: Switch to the **Kanban View** using the toggle at the top right to see your personal application pipeline visually.
5. **Generate a Flyer**: Inside any project modal, click "Generate Flyer (PDF)" to download a formatted, printable version of the project description.
6. **Export Tracker**: Click the "Export Tracker" button to download a CSV file of all the projects you have currently saved or applied to.

---

## 🤝 Contributing

Contributions are welcome and appreciated! To contribute:

1. Fork the repository.
2. Create a new feature branch (`git checkout -b feature/amazing-feature`).
3. Commit your changes (`git commit -m 'Add some amazing feature'`).
4. Push to the branch (`git push origin feature/amazing-feature`).
5. Open a Pull Request.

---

## 👨‍🏫 Acknowledgements

* Designed and developed by **Dr. Afshin Rahimi**, Department of Mechanical, Automotive and Materials Engineering, **University of Windsor**.
* Created to enhance the **Outstanding Scholars** program experience, making research opportunities highly accessible and organized for the academic community.

---

## 📝 License

This project is licensed under the [MIT License](LICENSE).