# Wi-Fi geolocation tool and library
Locate user by using global Wi-Fi database (no GPS required). Supported backends:
 * Yandex Maps API;
 * Google Geolocation API.

# License
GNU General Public License version 3. You can find it here: [COPYING](COPYING). External libraries can use another licenses, compatible with GNU GPLv3.

# Requirements
 * GNU/Linux (any modern distribution);
 * installed and enabled Network Manager;
 * Python 2.7 or 3.x;
 * python-networkmanager;
 * python-lxml;
 * python-requests.

# Installation
No installation required. Just clone repository and set your own API keys:
 1. Clone this repository:
 ```bash
 git clone https://github.com/xvitaly/wloc.git wloc
 ```
 2. Get API keys from [Yandex](https://tech.yandex.ru/maps/keys/get/) or/and [Google](https://developers.google.com/maps/documentation/geolocation/get-api-key).
 3. Open `wloc/settings.py` file in any text editor and set received API keys.
 4. Run:
 ```bash
 ./wloc.py -y -g
 ```

# Available options
```
usage: wloc.py [-h] [--yandex] [--google]
```

Optional arguments:
 * `-h` or `--help` - Show help message and exit;
 * `-y` or `--yandex` - Use Yandex Geolocation API;
 * `-g` or  `--google` - Use Google Geolocation API.
