# Node-red Emotiv BCI

Node-RED Emotiv BCI is a programming tool which is a companion to BCI app that will allow people to interface Emotiv tech to create endless BCI intergrations.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites
![alt text](https://www.emotiv.com/wp-content/uploads/2018/05/cortex-overview-diagram.png)

Emotiv BCI Node-red requires Node-RED version 0.14 or more recent.
You need to install the cortex and Emotiv BCI app
https://emotiv.github.io/cortex-docs/#installing-cortex

### Installing

1.1 Download Nodejs:
```
https://nodejs.org/en/download/
```

1.2 Check your version of Node.js, We recommend the use of Node.js LTS 8.x. Users of Node.js 6.x and 4.x should ensure they have the latest updates. Node-RED no longer supports Node.js 0.12.x or 0.10.x.

Open Terminal in Mac/Linux or cmd in Windows
```
 	node -v
```

1.3 Installing as a global module adds the command node-red to your system path:
```
	sudo npm install -g --unsafe-perm node-red
```

On Windows:

```
	npm install -g --unsafe-perm node-red
```

## Running the tests
1.1 Install node module
```
	npm install
```

1.2 Move to your folder and run terminal/cmd:
```
	npm link
```

1.3 run node red
```
	node-red
```

1.4 Go to http://127.0.0.1:1880/ Start playing

## 

## Features

See the [Emotiv BCI Nodes.md](Emotiv BCI Nodes.md) file for details of each node
