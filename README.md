# Python Flathunter-Helper

## Setup


### Prerequisites
To set up from scratch: 
```
apt install python3
git clone https://github.com/GerRudi/flathunter.git
apt install python3-pip
cp config.yaml.dist config.yaml
nano config.yaml
-> Do your edits to config file
apt install python3-setuptools
apt install python3-wheel

```



### Requirements
Install requirements from ```requirements.txt``` to run execute flathunter properly.
```
pip3 install -r requirements.txt
```

## Usage
```
usage: python3 flathunter.py [-h] [--config CONFIG]

Searches for flats on Immobilienscout24.de and wg-gesucht.de and sends results
to Telegram User

optional arguments:
  -h, --help            show this help message and exit
  --config CONFIG, -c CONFIG
                        Config file to use. If not set, try to use
                        '~git-clone-dir/config.yaml'

```

### Configuration

#### Bot registration
A new bot can registered with the telegram chat with the [BotFather](https://telegram.me/BotFather).

#### Chat-Ids
To get the chat id (receiver ID), the [REST-Api](https://core.telegram.org/bots/api) of telegram can be used to fetch the received messages of the Bot.
```
$ curl https://api.telegram.org/bot[BOT-TOKEN]/getUpdates
```

#### Google API
To use the distance calculation feature a [Google API-Key](https://developers.google.com/maps/documentation/javascript/get-api-key) is needed.


## Contributers
- [@NodyHub](https://github.com/NodyHub)
- Bene
- [@tschuehly](https://github.com/tschuehly)
- [@Cugu](https://github.com/Cugu)


