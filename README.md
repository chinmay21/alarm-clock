# ⏰ Alarm Clock

A simple command-line **Alarm Clock** built with Python. The program allows you to set an alarm for a specific time and plays an MP3 sound when the alarm time is reached.

## Features

* Set an alarm using `HH:MM:SS` format.
* Uses the computer's current system time.
* Checks the time every second.
* Plays an MP3 file when the alarm goes off.
* Uses `pygame` for audio playback.
* Simple command-line interface.

## Technologies Used

* **Python**
* **Pygame**
* **datetime** — for working with the current time and alarm time.
* **time** — for controlling the interval between time checks.

## Project Structure

```text
alarm-clock/
│
├── alarm_clock.py
├── my_music.mp3
└── README.md
```

> **Note:** The `my_music.mp3` file should be placed in the same directory as `alarm_clock.py`.

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/chinmay21/alarm-clock.git
```

### 2. Navigate to the Project Directory

```bash
cd alarm-clock
```

### 3. Install Pygame

Install the required Python package using pip:

```bash
pip install pygame
```

## Usage

Run the program:

```bash
python alarm_clock.py
```

You will be asked to enter the alarm time:

```text
Enter the alarm time (HH:MM:SS): 07:30:00
```

The program will then continuously check the current time:

```text
Alarm set for 07:30:00
07:29:56
07:29:57
07:29:58
07:29:59
07:30:00
Wake Up!
```

When the current time reaches the specified alarm time, the program plays the configured MP3 file.

## Time Format

The alarm must be entered using the following format:

```text
HH:MM:SS
```

The program uses the **24-hour clock**.

### Examples

```text
06:30:00
```

```text
14:45:30
```

```text
23:59:00
```

## Important Notes

* Make sure `pygame` is installed before running the program.
* The alarm time must follow the `HH:MM:SS` format.
* The program uses your computer's local system time.
* `my_music.mp3` must be present in the project directory.
* You can replace `my_music.mp3` with your own MP3 file.
* If you change the music file name, update the `sound_file` variable in the Python code.

## How It Works

1. The user enters an alarm time.
2. The program converts the entered time into a Python `datetime.time` object.
3. The program continuously retrieves the current system time.
4. The current time is compared with the alarm time.
5. When the current time reaches the alarm time, `pygame` initializes the audio system.
6. The selected MP3 file is played.
7. The program waits until the music finishes and then exits.

## Future Improvements

Possible improvements for future versions include:

* Add a graphical user interface (GUI).
* Allow users to select an audio file.
* Support multiple alarms.
* Add a snooze feature.
* Add an option to stop the alarm manually.
* Add input validation for incorrect time formats.
* Add a countdown/timer mode.
* Allow users to save recurring alarms.
* Add custom alarm labels.

## Author

**Chinmay Dhaundiyal**

* GitHub: [chinmay21](https://github.com/chinmay21)
* Repository: [Alarm Clock](https://github.com/chinmay21/alarm-clock)

## License

This project is open source and available for learning and personal use.
