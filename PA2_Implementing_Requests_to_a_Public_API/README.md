# Weather API App

A simple weather app that shows how to use different types of API requests. Get weather data, save your favorite locations, and manage them all in one place.

## What It Does

- **Get Weather**: Look up current weather for any city
- **Save Locations**: Keep a list of your favorite places
- **Edit Locations**: Update saved location details
- **Delete Locations**: Remove places you don't need anymore

## What You'll Learn

- How to make API requests (GET, POST, PUT, DELETE)
- Working with real weather data
- Saving information in your browser
- Handling errors when things go wrong

## Getting Started

### What You Need
- A web browser
- Free weather API key (takes 2 minutes to get)

### Setup Steps

1. **Download the files**
   - Save `index.html` and `script.js` to a folder

2. **Get a weather API key**
   - Go to [OpenWeatherMap.org](https://openweathermap.org/api)
   - Sign up for free
   - Copy your API key

3. **Add your API key**
   - Open `script.js` in a text editor
   - Find this line: `YOUR_OPENWEATHERMAP_API_KEY`
   - Replace it with your actual API key

4. **Open the app**
   - Double-click `index.html` to open in your browser
   - That's it!

## How to Use

### Check Weather (GET Request)
1. Click the "Weather Data" tab
2. Type a city name like "London" or "Tokyo"
3. Click "Get Weather"
4. See temperature, humidity, and weather description

### Save a Location (POST Request)
1. Click the "Save Location" tab
2. Fill in:
   - Name (like "Home" or "Work")
   - City name
   - Country
   - Notes (optional)
3. Click "Save Location"

### Manage Locations (PUT/DELETE Requests)
1. Click the "Manage Locations" tab
2. Click "Load Saved Locations"
3. For each saved place:
   - Click "Edit" to change details
   - Click "Delete" to remove it

## What's Happening Behind the Scenes

The app uses four different types of API requests:

- **GET**: Asks for weather information
- **POST**: Sends new location data to save
- **PUT**: Updates existing location information
- **DELETE**: Removes saved locations

## Testing Ideas

Try these to see how it works:
- Search for your hometown weather
- Save a few favorite cities
- Edit a saved location's notes
- Delete a location you don't need
- Try typing a fake city name (see the error message)

## Common Problems

**Weather not showing up?**
- Check your API key is correct
- Make sure you're connected to the internet
- Try a different city name

**API key not working?**
- Wait a few minutes after signing up (keys take time to activate)
- Make sure there are no extra spaces when copying the key

## What I Built This With

- **HTML** - The page structure
- **CSS** - Making it look nice
- **JavaScript** - All the interactive parts
- **Weather API** - Real weather data
- **Browser Storage** - Remembering your saved locations

## Cool Features

- Works on phones and computers
- Shows loading messages while getting data
- Remembers your locations between visits
- Handles errors gracefully
- Clean, easy-to-use interface

## Next Steps

Want to make it better? Try adding:
- Weather forecasts (not just current weather)
- Location search with suggestions
- Different weather themes
- Export your saved locations

## Need Help?

If something's not working:
1. Check the browser console for error messages
2. Make sure your API key is set up correctly
3. Try refreshing the page
4. Test with a simple city name like "London"

This project is perfect for learning how websites talk to other services on the internet!