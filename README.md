# ⏰ Alarm Clock

A simple command-line **Alarm Clock** built with Python. The program allows you to set an alarm for a specific time and plays an MP3 sound when the alarm time is reached.

## Features

* Set an alarm using `HH:MM:SS` format.
* Continuously checks the current system time.
* Plays an MP3 audio file when the alarm goes off.
* Uses `pygame` for audio playback.
* Simple command-line interface.

## Technologies Used

* **Python**
* **Pygame**
* `datetime` — for retrieving the current time.
* `time` — for controlling the checking interval.

## Project Structure

```text
alarm-clock/
│
├── alarm_clock.py
├── my_music.mp3
└── README.md
```

> Make sure your audio file is named `my_music.mp3` and is located in the same directory as the Python file.

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/chinmay21/alarm-clock.git
```

### 2. Navigate into the project

```bash
cd alarm-clock
```

### 3. Install Pygame

```bash
pip install pygame
```

## Usage

Run the Python program:

```bash
python alarm_clock.py
```

You will be prompted to enter an alarm time:

```text
Enter the alarm time (HH:MM:SS): 06:30:00
```

The program will continuously monitor the current time:

```text
Alarm set for 06:30:00
06:29:57
06:29:58
06:29:59
06:30:00
Wake Up!
```

Once the specified time is reached, the program plays the configured MP3 file.

## Important Notes

* Enter the alarm time using **24-hour format**.
* The required format is:

```text
HH:MM:SS
```

* The alarm uses your computer's local system time.
* The MP3 file must exist in the project directory.
* You can replace `my_music.mp3` with another audio file by changing the `sound_file` variable.

## Future Improvements

Some possible improvements for this project include:

* Add a graphical user interface (GUI).
* Allow users to select their own music file.
* Add support for multiple alarms.
* Add an option to stop or snooze the alarm.
* Validate incorrect time input.
* Add a countdown/timer mode.
* Allow alarms to be saved and reused.

## License

This project is open source and available for learning and personal use.