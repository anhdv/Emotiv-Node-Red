# Node-red Emotiv BCI Nodes

There are the details of each Emotiv Node.

## Nodes details

### Login node
This node is using for log in Emotiv account.

#### IO
Input: no need input
Output: array of authorization token. Eg: [authToken]

#### Node Properties
| Properties    | Type          | Mandatory |
| ------------- | ------------- | --------- |
| EmotivID      | String        | Yes       |
| Password      | String        | Yes       |

![alt text](https://www.emotiv.com/wp-content/uploads/2018/05/cortex-overview-diagram.png)

### Profile Name node
This node will check the profile name is existed in list profile.

#### IO
Required input node: Login node

Input: array of authorization token. Eg: [authToken]
Output: array of authorization token and profile name. Eg: [authToken,profileName]

#### Node Properties
| Properties    | Type          | Mandatory |
| ------------- | ------------- | --------- |
| Profile name  | String        | Yes       |

![alt text](https://www.emotiv.com/wp-content/uploads/2018/05/cortex-overview-diagram.png)

### Mental Commands node
This node will output value of trained mental command which is selected in node

#### IO
Required input node: Profile Name node

Input: array of authorization token and profile name. Eg: [authToken,profileName]
Output: Interger [0-100]

#### Node Properties
| Properties    | Type          | Mandatory |
| ------------- | ------------- | --------- |
| Command       | String        | Yes       |
| Sensitivity   | Int           | No        |

![alt text](https://www.emotiv.com/wp-content/uploads/2018/05/cortex-overview-diagram.png)

### Facial Expressions input node
This node will output value of trained facial expression which is selected in node

#### IO
Required input node: Profile Name node

Input: array of authorization token and profile name. Eg: [authToken,profileName]
Output: Interger [0-100]

#### Node Properties
| Properties    | Type          | Mandatory |
| ------------- | ------------- | --------- |
| Action        | String        | Yes       |
| Sensitivity   | Int           | No        |

![alt text](https://www.emotiv.com/wp-content/uploads/2018/05/cortex-overview-diagram.png)

### Performance Metric input node
This node will hook up emotions and cognitive states to particular outputs in node

#### IO
Required input node: Login node

Input: array of authorization token. Eg: [authToken]
Output: Interger [0-100]

#### Node Properties
| Properties    | Type          | Mandatory |
| ------------- | ------------- | --------- |
| Action        | String        | Yes       |

![alt text](https://www.emotiv.com/wp-content/uploads/2018/05/cortex-overview-diagram.png)

### Frequency Band input node
This node will hook up higher resolution mental states to particular outputs in node

#### IO
Required input node: Login node

Input: array of authorization token. Eg: [authToken]
Output: Interger

#### Node Properties
| Properties    | Type          | Mandatory |
| ------------- | ------------- | --------- |
| Band          | String        | Yes       |

![alt text](https://www.emotiv.com/wp-content/uploads/2018/05/cortex-overview-diagram.png)

### Motion sensors input node
This node will hook up higher resolution mental states to particular outputs in node

#### IO
Required input node: Login node

Input: array of authorization token. Eg: [authToken]
Output: Interger

#### Node Properties
| Properties    | Type          | Mandatory |
| ------------- | ------------- | --------- |
| Sensor        | String        | Yes       |

![alt text](https://www.emotiv.com/wp-content/uploads/2018/05/cortex-overview-diagram.png)