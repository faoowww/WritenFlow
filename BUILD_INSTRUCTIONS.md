# WriteFlow - Download and Installation Guide

WriteFlow is a comprehensive rich text editor and writing application with offline capabilities.

## Option 1: Download Source Code (Recommended for Developers)

### Prerequisites
- Node.js 18 or higher
- PostgreSQL database (optional - app includes fallback to local storage)

### Installation Steps

1. **Download the source code**
   - Download all project files to your local machine
   - Extract to a folder called `writeflow`

2. **Install dependencies**
   ```bash
   cd writeflow
   npm install
   ```

3. **Set up database (Optional)**
   ```bash
   # If you want persistent storage across sessions
   # Set up PostgreSQL and create a database
   # Add DATABASE_URL to your environment variables
   export DATABASE_URL="postgresql://username:password@localhost:5432/writeflow"
   ```

4. **Run the application**
   ```bash
   npm run dev
   ```

5. **Access the app**
   - Open your browser to `http://localhost:5000`
   - The app will work offline once loaded

## Option 2: Portable Desktop App (Coming Soon)

We're working on creating downloadable desktop versions using Electron:
- Windows (.exe)
- macOS (.dmg) 
- Linux (.AppImage)

## Option 3: Progressive Web App (PWA)

The app can be installed as a PWA on your device:

1. Visit the app in Chrome/Edge
2. Click the install button in the address bar
3. The app will be available offline on your desktop/phone

## Features When Downloaded

✅ **Rich Text Editor** - Full Microsoft Word-like editing
✅ **Document Management** - Create, save, organize documents  
✅ **Writing Tools** - Story outlines, scene tracking
✅ **Customizable Themes** - Multiple UI themes and backgrounds
✅ **Offline Support** - Works without internet connection
✅ **Auto-save** - Never lose your work
✅ **Export Options** - Save as HTML, Markdown, Plain Text

## Troubleshooting

- **Port 5000 in use**: Change the port in `server/index.ts`
- **Database connection**: App falls back to local storage if no database
- **Build issues**: Ensure Node.js 18+ is installed

## Support

For technical support or feature requests, please contact the development team.