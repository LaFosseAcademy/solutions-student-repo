# C4 Level 1 and 2 Task

Practice working with C4 level 1 and 2 diagarms

### Organisation

### Duration

You have **1.5 hours** to make as much progress on this task as possible.

Make sure to take breaks!

### Team

Solo task

## Brief: Weather-Watcher App

Create a C4 Level 1 and 2 Diagram for the following Scenario

*A small web service called Weather Watcher lets users query the current weather for a city and receive a push notification when the temperature crosses a user defined threshold.*

- User interacts with a Mobile App (or web client) to request the current weather and to set a temperature‑alert threshold.
- The app calls the Weather‑Watcher API (your system) to:
  1. GET /weather?city=… – forwards the request to an external Weather API (e.g., OpenWeatherMap) and returns the result to the user.
  2. POST /alert – stores the user’s threshold and registers the device with a Push Notification Service.
- The Weather Watcher API periodically (e.g., every 5min) pulls the latest weather data from the external Weather API.
- When the fetched temperature exceeds any stored threshold, the service pushes a notification to the user via the Push Notification Service.


