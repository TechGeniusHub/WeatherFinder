# WeatherFinder
Demo: [here](https://weather-finder-2024.vercel.app/) 
The Weather Finder application is a React-based web app that allows users to get instant weather updates for any city. The app provides real-time weather data, including current conditions, temperature, humidity, and a 5-day weather forecast. Users can enter a city name, and the app will fetch data from the WeatherAPI to display accurate weather information.

## Features:
- **Search for City:** Users can enter a city name to fetch the weather data.
- **Current Weather:** Displays the current temperature, humidity, and weather condition for the entered city.
- **5-Day Forecast:** Shows the weather forecast for the next five days, including the maximum, minimum, and average temperatures.
- **User-friendly Interface:** A clean and modern design for easy navigation and understanding of the weather data.

## Components:
1. **App.js:**
   - The main component that manages the overall state of the weather data and renders either the search bar or the weather display based on whether the data has been fetched.
   - Utilizes the `Searchbar` component to handle city searches and the `WeatherDisplay` component to show the fetched weather data.
   
2. **Searchbar.js:**
   - A form component that allows the user to input a city name.
   - Handles the API request to fetch weather data for the entered city using the WeatherAPI.
   - Includes dynamic styling for the submit button, changing its appearance on hover and click events.

3. **WeatherDisplay.js:**
   - Displays the weather information for the current day as well as a 5-day forecast.
   - Presents data such as the city name, temperature, humidity, and weather conditions.
   - Includes styling for each section and condition icons for a better visual experience.

4. **formatDate.js:**
   - A utility function that formats date strings into a human-readable format with the day of the week, date, and time.
   - Used to display dates in the forecast section and make the app's UI more intuitive.

## Data Flow:

![Data Flow Diagram](https://github.com/user-attachments/assets/a050f16b-862a-4487-a1c1-7fd3138fb9b9)

## Technologies Used:
- **React:** The primary JavaScript framework for building the UI.
- **Axios:** A promise-based HTTP client used to make API requests to WeatherAPI.
- **WeatherAPI:** A third-party API that provides weather data, including current weather, historical data, and forecasts.
- **CSS:** Styling the components to ensure a responsive and visually appealing interface.

## API Integration:
The app makes requests to the WeatherAPI to fetch weather data. Here are the endpoints used:
- **Current Weather:** `https://api.weatherapi.com/v1/current.json?key=<API_KEY>&q=<city_name>`
- **Historical Weather:** `https://api.weatherapi.com/v1/history.json?key=<API_KEY>&q=<city_name>&dt=<date>`
- **Forecast:** `https://api.weatherapi.com/v1/forecast.json?key=<API_KEY>&q=<city_name>&days=5`

## Output:

![Output 1](https://github.com/user-attachments/assets/1cab3c73-9bfc-4dbe-8938-8e9d95d0c2f1)

![Output 2](https://github.com/user-attachments/assets/9c3f7364-d1f4-4a29-b29b-eb9655184bd6)
