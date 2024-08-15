
Weather-App

This is a simple weather application built using SwiftUI. The app demonstrates the use of basic SwiftUI components, state management with @State and @Binding, and how to create a dynamic and responsive user interface.

Features

	•	Dynamic Background: The background color changes between day and night modes when the “Change Day Time” button is pressed.
	•	City Display: Shows the current city (“Cupertino, CA”).
	•	Main Weather Status: Displays the current weather condition with an icon and temperature.
	•	Weekly Forecast: Shows a simple five-day weather forecast with icons and temperatures.

Project Structure

	•	ContentView: The main view containing the overall layout of the app, including the city name, current weather status, weekly forecast, and the button to toggle between day and night modes.
	•	WeatherDayView: A custom view that displays a single day’s weather information, including the day of the week, weather icon, and temperature.
	•	BackgroundView: A custom view that handles the background gradient, changing colors based on the day or night mode.
	•	CityTextView: A custom view that displays the city name.
	•	MainWeatherStatusView: A custom view that displays the main weather icon and temperature.

UI Components

ContentView

	•	State Management: Uses @State to manage the isNight boolean, which toggles the interface between day and night modes.
	•	ZStack: Layers the background, main content, and button to create the app’s layout.

WeatherDayView

	•	Properties: Accepts dayOfWeek, imageName, and temp as parameters to display each day’s weather information.
	•	Image Rendering: Uses .symbolRenderingMode(.multicolor) to render SF Symbols in their original multicolor design.

BackgroundView

	•	@Binding: Uses @Binding to dynamically change the background gradient based on the isNight state from the parent view.

CityTextView and MainWeatherStatusView

	•	Custom Styling: Both views use Text and Image components with custom fonts, sizes, and colors to present the city name and main weather status.

SwiftUI Practices

	•	State Management: Demonstrates state management using @State and @Binding.
	•	Responsive Layout: Utilizes SwiftUI’s flexible layout system to create a responsive design that adapts to different screen sizes.
	•	Modern SwiftUI: Implements the latest SwiftUI features like .ignoresSafeArea() and .symbolRenderingMode(.multicolor) for better UI design and functionality.
Demo
https://github.com/user-attachments/assets/a4672a43-8c06-423d-ae40-ffbe1f0f701f
