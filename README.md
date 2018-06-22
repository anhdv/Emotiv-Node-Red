# Emotiv BCI Node-RED toolkit

## About Node-RED toolkit  

Node-RED toolkit for Emotiv BCI is a custom library of nodes for Node-RED node based programming framework which will allow you to interface with Emotiv technology and create brain-computer interface applications and integrations with ease.
Build thing without a single line of code - learn more about Node-RED in official documentation [here](https://nodered.org/docs/).

## Getting Started

This instruction manual will allow you to set up and run the project on your local machine for development and testing purposes. If you would like to deploy to a live environment  refer to [Node-RED Documentation](https://nodered.org/docs/hardware/raspberrypi) for a variety of different set up’s.

### Prerequisites
![alt text](https://www.emotiv.com/wp-content/uploads/2018/05/cortex-overview-diagram.png)

Emotiv BCI Node-red requires Node-RED version 0.14 or more later. You also need to install the Emotiv [Cortex UI](https://www.emotiv.com/developer/) and [Emotiv BCI](https://www.emotiv.com/emotivbci/) app to train and process your mental commands.

### Installing Node-RED

1. Download and install [Node JS](https://nodejs.org/en/download/)

2. Check your version of Node.js, We recommend the use of Node.js LTS 8.x. Users of Node.js 6.x and 4.x should ensure they have the latest updates. Node-RED no longer supports Node.js 0.12.x or 0.10.x.

3. Open Terminal in Mac/Linux or cmd in Windows
```
 	node -v
```

4. Installing as a global module adds the command node-red to your system path:
```
	sudo npm install -g --unsafe-perm node-red
```

	On Windows:

```
	npm install -g --unsafe-perm node-red
```

## Running Emotiv BCI Node-RED toolkit
1. Install our nodes
```
	npm install node-red-emotiv
```

2. Install node module
```
	npm install
```

3. Move to your folder
```
	cd ../YourFolder/
```

4. Link your folder
```
	npm link
```

5. Run node red
```
	node-red
```

6. Go to http://127.0.0.1:1880/ Start playing

## 

## Features

For detail description of each node features and functionality see [Emotiv BCI Nodes.md](EmotivBCINodes.md)
