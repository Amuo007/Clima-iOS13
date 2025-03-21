# Clima ☁️

A beautiful, dark-mode enabled weather app that allows you to check current weather conditions based on your location or by searching for a city manually.

![Clima App Screenshot](screenshots/clima-screenshot.png)

## Features

- 🌗 Dark-mode enabled for comfortable viewing day or night
- 📱 Responsive design that works on various iOS devices
- 🔍 Search functionality to find weather in any city
- 📍 GPS integration to show weather at your current location
- 🌈 Beautiful UI with condition-specific weather icons
- 🌡️ Current temperature display in Celsius
- 🌎 City name display

## Technologies Used

- Swift 5
- UIKit
- CoreLocation for GPS functionality
- URLSession for API networking
- MVC Architecture
- JSON parsing with Codable protocols
- Grand Central Dispatch for thread management
- Vector assets for crisp UI elements
- Delegate pattern for communication between components

## Getting Started

### Prerequisites

- Xcode 11.0 or later
- iOS 13.0 or later
- Swift 5.0 or later

### Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/Clima.git
```

2. Open the project in Xcode
```bash
cd Clima
open Clima.xcodeproj
```

3. Build and run the project on your simulator or iOS device

## App Structure

```
Clima/
├── Controller/
│   └── WeatherViewController.swift
├── View/
│   └── Main.storyboard
├── Model/
│   └── (Weather data models)
├── Assets.xcassets/
├── Supporting Files/
└── Info.plist
```

## Weather Condition Codes

The app uses the following SF Symbols to display different weather conditions:

```swift
switch conditionID {
    case 200...232:
        return "cloud.bolt"
    case 300...321:
        return "cloud.drizzle"
    case 500...531:
        return "cloud.rain"
    case 600...622:
        return "cloud.snow"
    case 701...781:
        return "cloud.fog"
    case 800:
        return "sun.max"
    case 801...804:
        return "cloud.bolt"
    default:
        return "cloud"
}
```

## Learning Outcomes

Through this project, I learned:
- How to create dark-mode enabled interfaces
- Using delegate pattern and protocols in Swift
- Making HTTP requests and handling JSON responses
- Using GPS data from the device
- Swift closures and completion handlers
- Extensions and computed properties
- Managing threads with Grand Central Dispatch
- Proper error handling with the guard keyword

## Future Improvements

- Add weather forecast for upcoming days
- Implement unit switching between Celsius and Fahrenheit
- Add more detailed weather information (humidity, wind speed, etc.)
- Implement weather alerts and notifications
- Add custom themes beyond dark/light mode

## Acknowledgements

- [App Brewery](https://www.appbrewery.co/) for the initial project guidance
- [OpenWeather API](https://openweathermap.org/api) for weather data
- SF Symbols by Apple for weather condition icons

## License

This project is licensed under the MIT License - see the LICENSE file for details.

---

*This project was developed as part of [The App Brewery's Complete iOS App Development Bootcamp](https://www.appbrewery.co/)*
