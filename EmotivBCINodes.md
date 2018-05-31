# Node-red Emotiv BCI Nodes

There are the details of each Emotiv Node.

## Nodes details

### Login node
This node is using for log in Emotiv account.
![alt text](https://github.com/anhdv/Emotiv-Node-Red/blob/master/Image/a1.png)

#### IO
Input: no need input
Output: array of authorization token. Eg: [authToken]

#### Node Properties
| Properties    | Type          | Mandatory |
| ------------- | ------------- | --------- |
| EmotivID      | String        | Yes       |
| Password      | String        | Yes       |

![alt text](https://github.com/anhdv/Emotiv-Node-Red/blob/master/Image/a2.png)

### Profile Name node
This node will check the profile name is existed in list profile.
![alt text](https://github.com/anhdv/Emotiv-Node-Red/blob/master/Image/b1.png)

#### IO
Required input node: Login node

Input: array of authorization token. Eg: [authToken]
Output: array of authorization token and profile name. Eg: [authToken,profileName]

#### Node Properties
| Properties    | Type          | Mandatory |
| ------------- | ------------- | --------- |
| Profile name  | String        | Yes       |

![alt text](https://github.com/anhdv/Emotiv-Node-Red/blob/master/Image/b2.png)

### Mental Commands node
This node will output value of trained mental command which is selected in node
![alt text](https://github.com/anhdv/Emotiv-Node-Red/blob/master/Image/c1.png)

#### IO
Required input node: Profile Name node

Input: array of authorization token and profile name. Eg: [authToken,profileName]
Output: Interger [0-100]

#### Node Properties
| Properties    | Type          | Mandatory |
| ------------- | ------------- | --------- |
| Command       | String        | Yes       |
| Sensitivity   | Int           | No        |

![alt text](https://github.com/anhdv/Emotiv-Node-Red/blob/master/Image/c2.png)

### Facial Expressions input node
This node will output value of trained facial expression which is selected in node
![alt text](https://github.com/anhdv/Emotiv-Node-Red/blob/master/Image/d1.png)

#### IO
Required input node: Profile Name node

Input: array of authorization token and profile name. Eg: [authToken,profileName]
Output: Interger [0-100]

#### Node Properties
| Properties    | Type          | Mandatory |
| ------------- | ------------- | --------- |
| Action        | String        | Yes       |
| Sensitivity   | Int           | No        |

![alt text](https://github.com/anhdv/Emotiv-Node-Red/blob/master/Image/d2.png)

### Performance Metric input node
This node will hook up emotions and cognitive states to particular outputs in node
![alt text](https://github.com/anhdv/Emotiv-Node-Red/blob/master/Image/e1.png)

#### IO
Required input node: Login node

Input: array of authorization token. Eg: [authToken]
Output: Interger [0-100]

#### Node Properties
| Properties    | Type          | Mandatory |
| ------------- | ------------- | --------- |
| Action        | String        | Yes       |

![alt text](https://github.com/anhdv/Emotiv-Node-Red/blob/master/Image/e2.png)

### Frequency Band input node
This node will hook up higher resolution mental states to particular outputs in node
![alt text](https://github.com/anhdv/Emotiv-Node-Red/blob/master/Image/f1.png)

#### IO
Required input node: Login node

Input: array of authorization token. Eg: [authToken]
Output: Interger

#### Node Properties
| Properties    | Type          | Mandatory |
| ------------- | ------------- | --------- |
| Band          | String        | Yes       |

![alt text](https://github.com/anhdv/Emotiv-Node-Red/blob/master/Image/f2.png)

### Motion sensors input node
This node will hook up higher resolution mental states to particular outputs in node
![alt text](https://github.com/anhdv/Emotiv-Node-Red/blob/master/Image/g1.png)

#### IO
Required input node: Login node

Input: array of authorization token. Eg: [authToken]
Output: Interger

#### Node Properties
| Properties    | Type          | Mandatory |
| ------------- | ------------- | --------- |
| Sensor        | String        | Yes       |

![alt text](https://github.com/anhdv/Emotiv-Node-Red/blob/master/Image/g2.png)