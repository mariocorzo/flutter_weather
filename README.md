# Weather App with Flutter and BLoC

This Flutter application displays weather information using the BLoC (Business Logic Component) pattern. It demonstrates the use of the `flutter_bloc` package to manage state and includes features such as weather search, settings management, and weather details display.

---

## Features

- **Weather Search**: Search for weather by city using a floating action button.
- **Dynamic Weather Display**: Displays weather conditions based on the selected city.
- **Settings Page**: Access application settings via an AppBar icon.
- **State Management**: Implements the BLoC pattern with `flutter_bloc` to manage application state.
- **Responsive UI**: Automatically updates UI based on state changes (e.g., loading, success, failure).

---

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/mariocorzo/flutter_weather
   cd flutter_weather
   ```

2. **Install dependencies**:
   ```bash
   flutter pub get
   ```

3. **Run the app**:
   ```bash
   flutter run
   ```

---

## Folder Structure

The application uses a modular structure to organize code efficiently:

- **`search`**: Handles city search functionality.
- **`settings`**: Contains settings page and related logic.
- **`weather`**: Includes weather state management (`WeatherCubit` and `WeatherState`) and weather-related widgets.

---

## Key Components

- **`WeatherPage`**: The main page of the application. It integrates weather state management, search functionality, and navigation to the settings page.
- **`WeatherCubit`**: Manages weather-related state, such as fetching weather data and refreshing it.
- **`WeatherState`**: Represents the current state of the weather data (e.g., initial, loading, success, failure).

---

## Usage

### Search for Weather

1. Click the **search** button (floating action button).
2. Enter the city name in the search page.
3. View the weather details for the selected city.

### Adjust Settings

1. Click the **settings** icon in the AppBar.
2. Modify settings as needed.

### Refresh Weather

1. Pull to refresh the weather data (enabled in the `WeatherPopulated` widget).

---

## Requirements

- Flutter SDK version: `>=3.0.0`
- Dependencies:
    - `flutter_bloc`: State management using BLoC
    - `flutter_material`: Core material design widgets

---

## Future Improvements

- Add more detailed weather data (e.g., hourly forecast, wind speed, humidity).
- Enhance the settings page to support more user preferences.
- Implement unit tests for critical components.

--- 

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.