# labo-4-research-smartmirror

## Installation (Server only OR Rasberry Pi)

Download and install the latest *Node.js* version:
- `curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -`
- `sudo apt install -y nodejs` \

### Server Only

The smartmirror is automatically set to server only mode. \
1. Download the files and navigate to the folder in terminal
2. Install and run the app with: `npm install && node serveronly` 


### Raspberry Pi

1. Download the files and navigate to the folder in terminal
2. Navigate to config.js and change these lines:

```javascript
var config = {
	address: "localhost",	// default is "0.0.0.0"
	port: 8080,		// default
    ipWhitelist: ["127.0.0.1", "::ffff:127.0.0.1", "::1"], // default is ["127.0.0.1", "::ffff:127.0.0.1", "::1", "::ffff:172.17.0.1"]
	...
};
```
3. Save config.js
4. Install and run the app with: `npm install && npm start` 
