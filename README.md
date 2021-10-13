![Build Status](https://img.shields.io/travis/remi-boivin/spy-robot-web-interface.svg?style=for-the-badge)
![Issues](https://img.shields.io/github/issues/remi-boivin/spy-robot-web-interface.svg?style=for-the-badge)
![pull request](https://img.shields.io/github/issues-pr-raw/remi-boivin/spy-robot-web-interface?color=red&style=for-the-badge)
![Licence](https://img.shields.io/github/license/remi-boivin/spy-robot-web-interface.svg?style=for-the-badge)
![maintainability](https://img.shields.io/codeclimate/maintainability/remi-boivin/spy-robot-web-interface.svg?style=for-the-badge)
![sponsors](https://img.shields.io/github/sponsors/remi-boivin.svg?style=for-the-badge)
# Spy-robot
## _The best opensource spy robot_

Spy-robot is an exploration robot built on python. The mission of the robot is to explore safelly dangerous places (fire zone, disaster zone, war zone ...). He can succesfully rescue peoples, inspect damages structure, transport equipment (dugs, food, survival kit ...) and more.

## Features

- Streaming video through socket

## Tech

Dillinger uses a number of open source projects to work properly:

- [Opencv](https://opencv.org/) Image and video processing library.
- [Raspberry pi](https://www.raspberrypi.com/) - Open source Nano computer
- [Arduino](https://www.arduino.cc/) - microprocessor for communicating with electronics.

## Installation

Spy-robot requires [Python](https://python.org/) v3.7+ to run.

Install the dependencies and start the server.

```sh
cd spy-robot-web-interface
docker build -t server sever/ 
docker network create --subnet=XXX.XXX.XXX.0/24 spybot
docker run --net spybot --ip XXX.XXX.XXX.XXX--device=/dev/video0 server
```

> :warning: **Please replace XXX with your ip subne and place same values in client.py** !

Start the client

```sh
cd spy-robot-web-interface
python3 client/client.py
```

# Road Map
This is a no-excusive list of features we will implement in the next version

- Depth camera estimation
- Estimation speed of the robot
- Facial recognition
- Sound streaming

For more please read the [Issues](https://github.com/remi-boivin/spy-robot-web-interface/issues/)

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

For more informations please read [CONTRIBUTING.md](https://github.com/remi-boivin/spy-robot-web-interface/blob/master/CONTRIBUTING.md)

> :warning: **Please respect** [code of conduct](https://github.com/remi-boivin/spy-robot-web-interface/blob/master/CODE_OF_CONDUCT.md) ! If someone don't play fair. Please tell us and we'll discuss with him. 

**Free Software, Hell Yeah!**