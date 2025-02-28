# ReStork

ReStork is an automation tool for Stork

## Prerequisites

- Node.js (v14 or higher)
- npm (v6 or higher)

## Installation

1. **Clone the repository:**
    ```sh
    git clone https://github.com/Rhvetican/ReStork.git
    cd ReStork
    ```

2. **Install the dependencies:**
    ```sh
    npm install
    ```

3. **Create a `config.json` file in the root directory with the following structure:**
    ```json
    {
      "cognito": [
        {
          "region": "ap-northeast-1",
          "clientId": "5msns4n49hmg3dftp2tp1t2iuh",
          "userPoolId": "ap-northeast-1_M22I44OpC",
          "username": "",  // Add your username here
          "password": ""   // Add your password here
        }
        // Add more accounts by copying the above object and pasting it below, then filling in the details
      ],
      "stork": {
        "intervalSeconds": 15
      },
      "threads": {
        "maxWorkers": 1
      }
    }
    ```

4. **(Optional) Create a `proxies.txt` file in the root directory and add your proxy addresses, one per line.**

## Usage

To start the bot, run the following command:
```sh
node index.js
