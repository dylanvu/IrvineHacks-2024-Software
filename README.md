# IrvineHacks-2024-Software

## Inspiration

## What it does

## How we built it

## Challenges we ran into

## Accomplishments that we're proud of

## What we learned

## What's next for Amelia

# Resources Used
* Pi Serial UART Communication: https://www.electronicwings.com/raspberry-pi/raspberry-pi-uart-communication-using-python-and-c
* If you get serial permission denied: https://askubuntu.com/questions/210177/serial-port-terminal-cannot-open-dev-ttys0-permission-denied
    * First, connect the ground betwee nthe pi and the arduino
    * Then, run `sudo chmod 666 /dev/ttyS0`
    * Remember to match the baud rates: `stty -F /dev/ttyS0 <baud_rate>`
* Installing python versions, using pyenv: https://github.com/pyenv/pyenv
    * Use `pyenv global <version>` to swap versions

# Installation and Deployment
* Our code works with Python version 3.8.0
* Note: `pyaudio` must be installed. It is a platform/OS dependent package.
    * Windows
        * You will get an error in `Pyaudio`
        * Run `pip install pipwin`
        * Run `pipwin install pyaudio`
    * Raspberry Pi
        * Basically, follow this: https://medium.com/@niveditha.itengineer/learn-how-to-setup-portaudio-and-pyaudio-in-ubuntu-to-play-with-speech-recognition-8d2fff660e94
        * Run `sudo apt-get install python-pyaudio python3-pyaudio`
        * Run `sudo apt-get install libasound-dev`
        * Run `pip install pyaudio`