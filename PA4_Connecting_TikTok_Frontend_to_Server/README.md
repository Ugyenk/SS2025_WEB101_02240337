# TikTok Clone App

A TikTok-like app built with Next.js frontend and Express.js backend. Users can upload videos, follow each other, and interact with content.

## What it does
- Sign up and log in to your account
- Upload videos with captions
- Watch videos in a feed
- Like and comment on videos
- Follow other users
- See personalized "Following" feed
- Browse user profiles

## Built with
- **Next.js** - Frontend framework
- **Express.js** - Backend server
- **JWT** - User authentication
- **Axios** - API requests
- **React Context** - State management

## Quick Setup

1. **Install packages**
   ```bash
   npm install axios jwt-decode react-hot-toast
   ```

2. **Set environment variables**
   Create `.env.local`:
   ```
   NEXT_PUBLIC_API_URL=http://localhost:8000/api
   ```

3. **Start the app**
   ```bash
   npm run dev
   ```

## Main Features

### Authentication
- Sign up with email and password
- Log in and stay logged in
- Protected pages (need to be logged in)

### Videos
- Upload videos with captions
- Watch videos in a scrollable feed
- Like and unlike videos
- Add comments

### Social Features
- Follow and unfollow users
- See videos from people you follow
- Browse and discover new users
- Visit user profiles

## How to Test

1. **Create accounts**: Make 2-3 different user accounts
2. **Upload videos**: Add some videos with different accounts
3. **Follow users**: Follow some accounts and check your "Following" feed
4. **Interact**: Like videos, leave comments, visit profiles

## Project Structure
```
src/
├── app/              # Pages (upload, profile, etc.)
├── components/       # UI components
├── contexts/         # Authentication state
├── services/         # API calls
└── lib/             # Configuration
```

## Common Issues
- **Can't connect to server**: Make sure your backend is running
- **Login not working**: Check if JWT tokens are being saved
- **CORS errors**: Backend needs to allow requests from your frontend
- **Videos not uploading**: Check file size and format limits

## Key Files
- `authContext.jsx` - Handles login/logout
- `api-config.js` - Sets up API connections
- `VideoFeed.jsx` - Shows the main video feed
- `VideoCard.jsx` - Individual video display
- `AuthForms.jsx` - Login and signup forms

Perfect for learning how to connect a React frontend to a backend API with authentication and social features!