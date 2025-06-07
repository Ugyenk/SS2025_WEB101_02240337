# TikTok Clone Project

A simple TikTok-like web app built with modern web technologies. Features video feeds, user authentication, and mobile-friendly design.

## What It Does

- Browse videos in a TikTok-style feed
- Navigate between different sections (For You, Following, Explore, etc.)
- Login and register with form validation
- Upload videos (mockup interface)
- Works on both phones and computers

## Built With

- **Next.js** - For creating pages and routing
- **React** - For interactive components
- **Tailwind CSS** - For styling and responsive design
- **React Hook Form** - For handling forms

## Getting Started

### What You Need
- Node.js installed on your computer
- Basic knowledge of terminal/command line

### Setup Steps

1. **Download the project**
   ```bash
   git clone https://github.com/your-username/tiktok-clone.git
   cd tiktok-clone
   ```

2. **Create the app**
   ```bash
   npx create-next-app@latest
   ```
   Choose these options:
   - TypeScript: No
   - Tailwind CSS: Yes
   - App Router: Yes

3. **Install extra packages**
   ```bash
   npm install react-icons react-hook-form
   ```

4. **Start the app**
   ```bash
   npm run dev
   ```

5. **Open in browser**
   Go to `http://localhost:3000`

## How It's Organized

```
src/
├── app/                    # All pages
│   ├── page.js            # Home page
│   ├── login/             # Login page
│   ├── signup/            # Register page
│   └── profile/           # User profile
├── components/            # Reusable parts
│   ├── layout/           # Page layout
│   └── ui/               # UI components
```

## Main Features

### Pages
- **Home**: Main video feed
- **Login/Signup**: User registration with validation
- **Profile**: User profile page
- **Upload**: Video upload interface
- **Following**: Videos from people you follow

### Components
- **Video Cards**: Individual video displays
- **Navigation**: Sidebar menu like TikTok
- **Forms**: Login and registration with error checking

## Form Validation

The forms check for:
- Valid email addresses
- Password length (at least 8 characters)
- Matching password confirmation
- Required fields filled out

## Testing

Try these things to test the app:
- Submit forms without filling them out
- Enter invalid email addresses
- Use passwords that don't match
- Navigate between different pages
- Resize browser window to test mobile view

## What I Learned

- How to build multi-page websites with Next.js
- Creating reusable components with React
- Making forms work properly with validation
- Designing for mobile and desktop
- Using modern CSS with Tailwind

## Future Ideas

- Connect to a real database
- Add actual video uploading
- User accounts and profiles
- Like and comment features
- Video streaming

## Resources

- [Next.js Guide](https://nextjs.org/learn)
- [React Basics](https://react.dev/learn)
- [Tailwind CSS](https://tailwindcss.com/docs)

## Need Help?

If you run into problems:
1. Make sure Node.js is installed
2. Check that all packages installed correctly
3. Look at the browser console for errors
4. Google error messages - they're usually helpful!