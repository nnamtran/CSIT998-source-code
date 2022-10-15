# CSIT998-source-code

### Install instruction:
- Clone client folder into desktop
- Open CSIT998-source-code folder in favorite code editor (e.g. VSCODE)
- Open terminal
- `cd client`
- run command: `npm install` - to install all necessary dependencies
- run command: `npm run start:frontend` - to run Expo Client
- Scan the output barcode to open the mobile app - Make sure to have Expo Go installed on your phone

### Install machine learning model instruction:
- After run comman: `npm run start:frontend` from client folder
- In terminal look for expo IP address (e.g. exp://127.0.0.16:19000)
- Copy expo IP address
- In /client/app/AICamera.js, line 54: `let host = '127.0.0.16';` -> Make sure to change host ip address is the same with expo IP address
- In AI.py, line 70,
```
if __name__ == "__main__":
    app.run(host='127.0.0.16', port=5000)
```
- Make sure to change host ip address is the same with expo IP address
- Open terminal and run command: `python3 AI.py`, then machine learning function will be available
