# Stop-Watch App

A simple and interactive Stop-Watch application built with React. This app allows you to start, stop, and reset a digital stopwatch, displaying the elapsed time in a formatted manner.

![Stopwatch App Screenshot](./.github/screen.png)

## Features

- **Start**: Begin the stopwatch and start measuring elapsed time.
- **Stop**: Pause the stopwatch and hold the current elapsed time.
- **Reset**: Reset the stopwatch to zero.

## Code Overview

### Components

#### `DigitalClock`

This is the main component of the application. It includes the following states and functions:

- **States**
  - `isRunning`: A boolean indicating whether the stopwatch is running.
  - `elapsedTime`: A number representing the elapsed time in milliseconds.

- **Refs**
  - `intervalIdRef`: A reference to the interval ID for clearing the interval.
  - `startTimeRef`: A reference to the start time for calculating elapsed time.

- **Functions**
  - `start()`: Starts the stopwatch and sets the start time.
  - `stop()`: Stops the stopwatch.
  - `reset()`: Resets the stopwatch and clears elapsed time.
  - `formatTime()`: Formats the elapsed time into a string `MM:SS:MS`.
  - `padZero(number)`: Pads single digit numbers with a leading zero.

### UI Elements

- **Display**: Shows the formatted elapsed time.
- **Start Button**: Starts the stopwatch.
- **Stop Button**: Stops the stopwatch.
- **Reset Button**: Resets the stopwatch.