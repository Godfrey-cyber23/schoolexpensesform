# School Expenses Tracker 📚💰

A responsive web application for tracking school expenses with Google Sheets backend.

![Dashboard Preview](https://img.shields.io/badge/Status-Complete-success) ![Mobile Responsive](https://img.shields.io/badge/Mobile-Responsive-blue) ![Google Sheets](https://img.shields.io/badge/Backend-Google%20Sheets-green)

## ✨ Features

- **📱 Mobile-First Design** - Fully responsive for all screen sizes
- **📊 Real-time Dashboard** - View expenses with interactive statistics
- **➕ Smart Form Entry** - Dynamic category selection with auto-calculation
- **📝 Google Sheets Integration** - Store data securely in Google Sheets
- **🔍 Search & Filter** - Quickly find records by student or term
- **📤 Export Functionality** - Download data as CSV/Excel
- **🏷️ Flag Important Records** - Mark important expenses
- **🖨️ Receipt Generation** - Print/save payment receipts
- **🔄 Full CRUD Operations** - Create, Read, Update, Delete records

## 🚀 Quick Start

### Prerequisites
- Google Account
- Modern web browser
- Text editor (VS Code recommended)

### Setup Instructions

#### 1. **Create Google Sheet**
- Go to [Google Sheets](https://docs.google.com/spreadsheets)
- Create a new blank spreadsheet
- Name it "School Expenses Tracker"

#### 2. **Set Up Google Apps Script**
1. Open your Google Sheet
2. Click **Extensions → Apps Script**
3. Delete default code and paste the [backend code](#backend-code)
4. Click **Save** (💾 icon)
5. Run `setupSheet()` function once (click **Run** button)

#### 3. **Deploy as Web App**
1. Click **Deploy → New deployment**
2. Select **Web app** (click gear icon ⚙️)
3. Configure:
   - **Description**: Expense Tracker v1
   - **Execute as**: Me
   - **Who has access**: Anyone
4. Click **Deploy**
5. **Copy the Web App URL**

#### 4. **Configure HTML Files**
1. Open `index.html` and `form.html`
2. Find this line:
   ```javascript
   const API = "YOUR_API_URL_HERE";
   ```
3. Replace with your **actual Web App URL**
4. Save both files

## 📁 File Structure

```
school-expenses-tracker/
│
├── index.html          # Main dashboard
├── form.html           # Expense entry form
│
├── README.md           # This documentation
│
└── assets/             # (Optional) For images/styles
    ├── styles.css
    └── script.js
```

## 🔧 Backend Code

```javascript
// Google Apps Script Code
// Complete code available in the repository
// This handles all CRUD operations with Google Sheets
```

## 🎯 Usage Guide

### Adding a New Expense
1. Open `index.html` in browser
2. Click **"Add Record"** button
3. Fill student details
4. Select expense categories
5. Enter amounts
6. Click **"Save Record"**

### Managing Expenses
- **Edit**: Click "Edit" button on any record
- **Delete**: Click "Delete" button
- **Flag**: Click star icon to mark important
- **View**: Click any row to see receipt details

### Exporting Data
1. Select term filter (optional)
2. Click **"Download Excel"** button
3. CSV file will download automatically

## 📱 Mobile Features

- **Compact controls** fit in one row on phones
- **Touch-friendly** buttons and inputs
- **Horizontal scrolling** for data tables
- **Responsive grids** adapt to screen size
- **Optimized spacing** for small screens

## 🛠️ Technical Details

### Built With
- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Backend**: Google Apps Script
- **Database**: Google Sheets
- **Deployment**: Netlify/GitHub Pages (optional)

### Browser Support
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+
- Mobile browsers

## 🔒 Security Notes

- API URL should be kept private
- Never share your Apps Script deployment link publicly
- Use "Anyone" access only for personal/testing use
- For production, implement proper authentication

## 🚨 Troubleshooting

### Common Issues & Solutions

| Issue | Solution |
|-------|----------|
| **CORS errors** | Host files on web server, don't open locally |
| **"Script not deployed"** | Ensure "Who has access" is set to "Anyone" |
| **Data not saving** | Check API URL is correct in both HTML files |
| **Loading forever** | Open browser console (F12) for error details |
| **Sheet not found** | Run `setupSheet()` function in Apps Script |

### Testing API Directly
```bash
# Replace with your URL
curl "https://script.google.com/macros/s/YOUR_ID/exec?method=GET"
```

## 📈 Features Roadmap

- [ ] User authentication
- [ ] Multi-user support
- [ ] Data visualization charts
- [ ] Email notifications
- [ ] Budget planning
- [ ] Recurring expenses
- [ ] PDF report generation
- [ ] Dark mode

## 🤝 Contributing

1. Fork the repository
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Google Apps Script documentation
- Free hosting services (Netlify, GitHub Pages)
- Open source community

## 📞 Support

For support or questions:
1. Check [Troubleshooting](#troubleshooting) section
2. Review the code comments
3. Create an issue in the repository

---

## 📋 Deployment Checklist

### Before Deployment
- [ ] Google Sheet created
- [ ] Apps Script code deployed
- [ ] API URL copied
- [ ] HTML files updated with API URL
- [ ] Tested locally with web server

### After Deployment
- [ ] Dashboard loads data
- [ ] Form submits successfully
- [ ] Edit/Delete functions work
- [ ] Export generates CSV
- [ ] Mobile responsiveness verified

---

## 🎯 Quick Reference

| Action | File | Function |
|--------|------|----------|
| Add record | form.html | `submitForm()` |
| View dashboard | index.html | `loadData()` |
| Export data | index.html | `exportData()` |
| Toggle flag | index.html | `toggleFlag()` |
| Search | index.html | `filterTable()` |

---

**Happy Tracking!** 🎓💰

---
*Built with ❤️ for schools and educational institutions*