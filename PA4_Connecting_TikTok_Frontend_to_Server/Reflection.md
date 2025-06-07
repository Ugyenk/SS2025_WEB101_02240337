# TikTok Clone Reflection

## What I Built
A TikTok-like app connecting a Next.js frontend to an Express.js backend. Users can sign up, upload videos, follow each other, and interact with content.

## Key Technologies
- **Next.js** - Frontend framework
- **Express.js** - Backend server
- **JWT** - User authentication
- **React Context** - Global state management
- **Axios** - API requests

## What I Learned

### Full-Stack Integration
Learned how frontend and backend talk to each other:
- Setting up API connections
- Sending data between client and server
- Managing user sessions across both sides

### Authentication Systems
JWT tokens are trickier than expected:
- Storing tokens securely in the browser
- Keeping users logged in after page refresh
- Protecting pages that need login

### State Management
Managing data across the whole app:
- Used React Context for user login state
- Handled loading and error states properly
- Made sure UI updates when data changes

### API Design Patterns
Created organized code for API calls:
- Separate files for different types of requests (users, videos)
- Centralized error handling
- Consistent response formats

## Biggest Challenges

### CORS Errors
**Problem**: Frontend couldn't talk to backend - kept getting blocked.
**Solution**: Had to configure the server to allow requests from my frontend.
**Learned**: Browsers block cross-origin requests by default for security.

### Users Getting Logged Out
**Problem**: Every page refresh would log users out.
**Solution**: Store login tokens in localStorage and check them on startup.
**Learned**: Browser memory gets wiped on refresh - need persistent storage.

### Messy Error Handling
**Problem**: Some errors crashed the app, others were invisible to users.
**Solution**: Created one place to handle all API errors and show user-friendly messages.
**Learned**: Users need to know what went wrong in terms they understand.

### Complex Component Communication
**Problem**: Passing data between components got confusing.
**Solution**: Used React Context for global data and clear patterns for local data.
**Learned**: Good data flow makes debugging much easier.

### File Uploads Acting Up
**Problem**: Video uploads would fail or hang forever.
**Solution**: Added proper file validation and progress indicators.
**Learned**: File uploads need special handling and user feedback.

## Key Insights

### Architecture Matters
Well-organized code makes everything easier. When I needed to add features or fix bugs, having clear separation between different parts saved tons of time.

### User Experience Is King
Technical stuff working isn't enough - users need to know what's happening:
- Loading spinners during uploads
- Clear error messages they can act on
- Smooth transitions between states

### Security From Day One
Can't add security as an afterthought:
- Validate data on both frontend and backend
- Protect sensitive pages
- Handle tokens carefully

### Test With Real Scenarios
Created multiple fake accounts to test following, uploading, and interacting. Real usage patterns revealed issues I never would have found otherwise.

## What I'd Do Different
- Add proper loading states from the beginning
- Write tests for the tricky authentication logic
- Design the API structure more carefully upfront
- Implement better caching for faster performance

## Final Thoughts
This project showed me how all the pieces of a modern web app fit together. Frontend and backend aren't separate things - they're partners that need to work smoothly together.

The biggest lesson: building features is only half the job. Making them reliable, secure, and user-friendly is where the real work happens. Every technical decision should make the user's experience better, not just solve a coding problem.