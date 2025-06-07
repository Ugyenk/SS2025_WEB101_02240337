# File Upload 

A React app where users can upload files by dragging and dropping them, with a progress bar to show how it's going.

## What it does
- Upload files by clicking or dragging
- Shows a progress bar while uploading
- Checks if files are the right type and size
- Can handle multiple files at once
- Works on phones and computers

## Built with
- **Next.js** - The main framework
- **React** - For the user interface
- **Tailwind CSS** - Makes it look good
- **React Dropzone** - Handles drag and drop

## Setup

1. **Make the project**
   ```bash
   npx create-next-app my-upload-app
   cd my-upload-app
   ```

2. **Install packages**
   ```bash
   npm install react-hook-form formidable axios react-dropzone
   ```

3. **Run it**
   ```bash
   npm run dev
   ```

## File rules
- Accepts: Images (JPEG, PNG, GIF), PDFs, and text files
- Max size: 5MB per file
- Max files: 10 at once

## How it works
- **Drag and drop**: Drop files right onto the upload box
- **Progress tracking**: Watch the bar fill up as files upload
- **Smart validation**: Tells you if something's wrong with your files
- **Mobile ready**: Touch-friendly on mobile devices

## Upload process
1. Choose files (click the box or drag files onto it)
2. Add a note about your files (optional)
3. Hit "Upload Files"
4. Watch the progress bar
5. Done!

## Safety stuff
- Checks files twice (on your device and the server)
- Gives each file a unique name
- Keeps uploaded files secure

## Common issues
- **Upload failed?** Your file might be too big or the wrong type
- **Taking forever?** Try uploading fewer files
- **Getting errors?** The error message will tell you what's wrong

Great for learning file uploads or starting a bigger project!