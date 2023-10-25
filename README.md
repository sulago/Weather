# Weather
This code is an example of using the `Weather` interface and several classes implementing this interface to get weather data in different cities. Let's look at how it works and why the `FirstAPIWeatherAdapter` and `SecondAPIWeatherAdapter' classes were created.

1. The 'Weather` interface:
   - This interface defines methods for obtaining various weather data, such as temperature, maximum and minimum temperature, perceived temperature, humidity, and weather description.

2. The `Location` class:
   - This class represents a city and is used to determine the city for which to get weather data.

3. Classes `FirstAPIWeather` and `SecondAPIWeather`:
   - These classes implement the `Weather` interface and provide weather data for specific cities (Almaty, Atyrau, Astana).
   - `FirstAPIWeather` returns the temperature in Celsius, while `SecondAPIWeather' returns the temperature in Fahrenheit.

4. Classes `FirstAPIWeatherAdapter` and `SecondAPIWeatherAdapter`:
   - These classes serve as adapters for the `FirstAPIWeather` and `SecondAPIWeather` classes to provide weather data output in a specific format.
   - `FirstAPIWeatherAdapter` converts temperature from Celsius to Fahrenheit and outputs weather data according to this format.
   - `SecondAPIWeatherAdapter` converts temperature from degrees Fahrenheit to Celsius and also outputs weather data.

5. `MainClassToWeather`:
   - In the `main` method, `Location` instances are created for different cities, then `FirstAPIWeather` and `SecondAPIWeather` objects are created for these cities.
   - Then the adapters `FirstAPIWeatherAdapter` and `SecondAPIWeatherAdapter` are created and used to output weather data in various formats.

This code allows you to get weather data for different cities from two different sources (presumably, the first source returns the temperature in Celsius, and the second in degrees Fahrenheit) and output them in a user-friendly format. The `FirstAPIWeatherAdapter` and `SecondAPIWeatherAdapter` adapters provide a consistent representation of weather data, regardless of the units in which temperature data is provided.
