Parkrun Helper Organizer - Separated Database Files
Overview
This project has been restructured to separate the data storage from the main HTML file. This ensures that your volunteer data and helper database won't be lost when updating the HTML interface.

File Structure
parkrun-organizer/
├── index.html           # Main application interface (updated)
├── parkrun-data.js      # Data storage and management module
├── parkrun-config.js    # Configuration, roles, and translations
├── backup-utility.html  # Backup and restore tool
└── README.md           # This file
Files Description
1. index.html
The main application interface that now references external JavaScript files instead of containing embedded data. This file can be updated without affecting your stored data.

2. parkrun-data.js
Handles all data storage and retrieval operations:

Manages volunteer assignments by week
Stores helper information (names and IDs)
Handles localStorage operations
Provides data export/import functionality
3. parkrun-config.js
Contains all configuration data:

List of volunteer roles
Translations for English and German
Helper functions for accessing translations
4. backup-utility.html
A standalone tool for backing up and restoring your data:

Export all data as a JSON file
Import data from a previously exported backup
View statistics about your data
Setup Instructions
Save all files in the same directory
Create a folder (e.g., parkrun-organizer)
Save all four files in this folder
Open the application
Open index.html in your web browser
The application will automatically load the external JavaScript files
Existing data migration
If you have existing data from the old version, it will be automatically loaded
The data structure remains the same, so no migration is needed
Usage
Regular Use
Open index.html in your browser
Select a week from the dropdown
Assign helpers to volunteer roles
Export team information via email
Backup Your Data
Open backup-utility.html in your browser
Click "Download Backup" to save your data as a JSON file
Store this file safely for future restoration
Restore Data
Open backup-utility.html in your browser
Click "Choose Backup File" and select your backup JSON file
Review the file information
Click "Import Data" to restore (this will replace existing data)
Updating the Application
When you need to update the HTML interface:

Before updating: Create a backup using backup-utility.html
Replace only the index.html file with the new version
Keep parkrun-data.js and parkrun-config.js unchanged
Your data will be preserved
Data Storage
Data is stored in your browser's localStorage:

parkrunHelperData: Weekly volunteer assignments
parkrunHelpers: Helper database
parkrunLanguage: Language preference
Browser Compatibility
Works with all modern browsers (Chrome, Firefox, Safari, Edge)
Data is stored locally in each browser
Data is not shared between different browsers or devices
Tips
Regular Backups: Use the backup utility weekly or before major updates
Multiple Browsers: If you use multiple browsers, export/import data to sync
Sharing Data: Export your data and share the JSON file with other organizers
Troubleshooting
Data not loading?

Ensure all JavaScript files are in the same directory as index.html
Check browser console for errors (F12 → Console tab)
Try clearing browser cache and reloading
Lost data after update?

Check if old index.html had embedded data
Use browser developer tools to inspect localStorage
Restore from a backup if available
Import not working?

Ensure the backup file is a valid JSON file
Check that the file contains both parkrunData and helpersDatabase
Try creating a fresh backup and comparing the structure
