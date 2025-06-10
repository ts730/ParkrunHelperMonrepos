# Parkrun Helper Organizer 🏃‍♀️🏃‍♂️

A bilingual web application for organizing Parkrun volunteer helpers and managing weekly schedules.

## 📋 Overview

The Parkrun Helper Organizer is a simple, user-friendly tool designed to help Parkrun event directors and organizers manage their volunteer teams efficiently. The application allows you to assign volunteers to different roles for each Saturday's event, track missing positions, and export schedules via email.

## ✨ Features

### Core Functionality
- **📅 Weekly Schedule Management** - Select and manage volunteers for each Saturday
- **👥 Helper Database** - Add, edit, and remove volunteer helpers with their Parkrun IDs
- **🎯 Role Assignment** - Assign helpers to specific Parkrun volunteer roles
- **📊 Team Overview** - Visual summary of filled and missing positions
- **📧 Email Export** - Generate and send volunteer schedules via email
- **⚠️ Missing Position Alerts** - Instantly see which roles still need volunteers

### User Experience
- **🌐 Bilingual Support** - Full English and German localization
- **📱 Responsive Design** - Works seamlessly on desktop, tablet, and mobile devices
- **💾 Local Storage** - All data is saved locally in your browser
- **🎨 Clean Interface** - Modern, intuitive design with Parkrun's color scheme
- **⚡ Fast Performance** - Lightweight single-page application

### Volunteer Roles Supported
- Run Director
- Timekeeper
- Course Setup
- Token Dispenser
- Barcode Scanner
- Marshal
- Tail Walker
- Parkwalker
- Photographer
- New Runner Briefing
- Close Down
- Catering

## 🚀 Getting Started

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/parkrun-helper-organizer.git
   cd parkrun-helper-organizer
   ```

2. **Open the application:**
   - Simply open `index.html` in your web browser
   - No server setup required!

### Alternative Setup Methods

**Option 1: Direct Download**
- Download the `index.html` file
- Open it in any modern web browser

**Option 2: Web Server (Optional)**
- If you prefer running on a local server:
  ```bash
  # Using Python 3
  python -m http.server 8000
  
  # Using Node.js
  npx serve .
  ```

## 📖 Usage Guide

### 1. Language Selection
- Choose between English (EN) and German (DE) using the language switcher in the top right
- Your language preference is automatically saved

### 2. Managing Helpers
1. Click **"Manage Helpers"** button
2. Add new helpers with their name and Parkrun ID
3. Delete helpers as needed
4. All helpers are stored locally and persist between sessions

### 3. Scheduling Volunteers
1. Select the desired Saturday from the week dropdown
2. For each role, choose a helper from the dropdown menu
3. Use the clear button (🗑️) to remove a helper from a role
4. Changes are automatically saved

### 4. Monitoring Team Status
- **Missing Positions Alert**: See which roles still need volunteers
- **Team Overview**: Click "View Team" for a comprehensive status summary
- **Visual Indicators**: Green checkmarks for filled positions, red warnings for missing ones

### 5. Exporting Schedules
- Click **"Export to Email"** to generate a mailto link
- The email will contain a formatted table with all volunteer assignments
- Send directly to your team or event participants

### 6. Data Management
- **Clear Week**: Remove all assignments for the selected week
- **Persistent Storage**: All data is automatically saved in your browser
- **No Account Required**: Everything works offline after the initial load

## 🛠️ Technical Details

### Technology Stack
- **HTML5** - Structure and semantic markup
- **CSS3** - Styling with modern features (Grid, Flexbox, CSS Variables)
- **Vanilla JavaScript** - No external dependencies
- **Local Storage API** - Client-side data persistence

### Browser Compatibility
- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

### Key Features
- **Responsive Design**: Mobile-first approach with breakpoints at 480px
- **Accessibility**: Semantic HTML, proper ARIA labels, keyboard navigation
- **Performance**: Lightweight (~15KB total), fast loading, smooth animations
- **Offline Capable**: Works without internet connection after initial load

## 🎨 Customization

### Color Scheme
The application uses Parkrun's official colors:
- **Primary Blue**: `#003D71`
- **Orange Accent**: `#FF6900`
- **White/Light Gray**: Backgrounds and contrast

### Modifying Volunteer Roles
To add or modify volunteer roles, edit the `volunteerRoles` array in the JavaScript section:

```javascript
const volunteerRoles = [
    'Run Director',
    'Timekeeper',
    // Add your custom roles here
    'Your Custom Role',
];
```

### Adding Translations
To add a new language, extend the `translations` object:

```javascript
const translations = {
    en: { /* English translations */ },
    de: { /* German translations */ },
    fr: { /* Add French translations */ },
};
```

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### Reporting Issues
- Use the GitHub Issues tab to report bugs
- Include browser version, steps to reproduce, and expected vs actual behavior

### Suggesting Features
- Check existing issues before creating new ones
- Provide detailed use cases and benefits

### Code Contributions
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Translation Contributions
- Native speakers welcome to improve or add translations
- Ensure consistency with Parkrun terminology

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙋‍♀️ Support

### Getting Help
- Check the [Issues](https://github.com/yourusername/parkrun-helper-organizer/issues) page for common problems
- Create a new issue for bugs or feature requests

### Parkrun Resources
- [Official Parkrun Website](https://www.parkrun.com/)
- [Parkrun Volunteer Handbook](https://www.parkrun.com/volunteer/)

## 🏆 Acknowledgments

- **Parkrun Community** - For inspiring this project
- **Volunteer Coordinators** - For feedback and testing
- **Contributors** - Thank you for your improvements and translations

## 📊 Project Status

- ✅ **Stable**: Ready for production use
- 🔄 **Actively Maintained**: Regular updates and bug fixes
- 📈 **Growing**: New features added based on community feedback

---

**Made with ❤️ for the Parkrun community**

*This is an unofficial tool created by volunteers for volunteers. Not affiliated with Parkrun Global.*
