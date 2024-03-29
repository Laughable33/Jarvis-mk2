# Jarvis

A Personal Assistant for Linux, MacOS and Windows

Jarvis is a simple personal assistant for Linux, MacOS and Windows which works on the command line. He can talk to you if you enable his voice. He can tell you the weather, he can find restaurants and other places near you. He can do some great stuff for you.

## Getting Started With Installation

In order to install Jarvis, follow these steps:
1. Clone [this repository](https://github.com/Laughable33/Jarvis.git) with `git clone https://github.com/sukeesh/Jarvis.git`
2. Run the command `python installer` (or `python3 installer` if that doesn't work) from the terminal.

Run **Jarvis** from anywhere by command `jarvis`, or `./jarvis` from within the project directory to start up Jarvis!

You can start by typing `help` within the Jarvis command line to check what Jarvis can do for you.

### Frequently encountered issues
**Question**: When I run Jarvis, it shows an error relating to module not found<br>
**Platform**: Windows<br>
**Solution 1**: Uninstall and/or install the module package<br>
Example:<br>
Error: `ImportError: DLL load failed while importing win32api: The specified module could not be found.`<br>
Solution:<br>
`pip uninstall pywin32`<br>
`pip install pywin32` or `conda instapll pywin32`<br>
**Solution 2**: add the package to your environment variables system PATH.<br>

**Question**: After cloning the repo in terminal it gives an error when running python3 installer saying please install virtual environemnt
**Solution**: 
- Install virtual env using this command "python3 -m pip install virtualenv"
- OR: On Linux use package manager (e.g. Ubuntu sudo apt install python3-venv)
- Restart Installer

## Optional Dependencies

- Any pyttsx3 text-to-speech engine (``sapi5, nsss or espeak``) for Jarvis to talk out loud (e.g. Ubuntu do ``sudo apt install espeak``)
- Portaudio + python-devel packages for voice control
- ``notify-send`` on Linux if you want to receive *nice* and desktop-notification instead of *ugly* pop up windows (e.g. Ubuntu do ``sudo apt install libnotify-bin``)
- ``ffmpeg`` if you want ``music`` to download songs as .mp3 instead of .webm

## Docker

Run with docker (docker needs to be installed and running):

```
[sudo] make build_docker
[sudo] make run_docker
```
## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
