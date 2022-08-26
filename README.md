[![PyPI version](https://badge.fury.io/py/fordpass.svg)](https://badge.fury.io/py/fordpass)

# fordpass-python

This is a basic Python wrapper around the FordPass APIs. The wrapper provides methods to return vehicle status as well as some basic commands, e.g. start/stop, lock/unlock.

Original:
* It's more or less a straight port of @d4v3y0rk's NPM module [d4v3y0rk/ffpass](https://github.com/d4v3y0rk/ffpass-module) - props to him for his work figuring out the relevant API requests needed.

Additions:
* Based on the work of [clarkd/fordpass-python](https://github.com/clarkd/fordpass-python)
* Merged with the work of [NicKoehler/fordpass-python](https://github.com/NicKoehler/fordpass-python) to get the auth up to speed with the changed by Ford
* Used data from the iOS widget from [tonesto7/fordpass-scriptable](https://github.com/tonesto7/fordpass-scriptable) for the urls and some information about the variables used in the vehicle status and service logs calls
* Added charge logs retrieval

## Features

* Automatically auth & re-fetches tokens once expired
* Get status of the vehicle (this returns a ton of info about the car: lat/long, oil, battery, fuel, odometer, tire pressures, open windows and a bunch of other stuff that may/may not apply to your car, e.g. charge level, diesel filters.)
* Start the engine (if supported)
* Stop the engine (if supported)
* Lock the doors
* Unlock the doors
* Get charge logs
* Get vehicle status information
* Get service logs

## Install
Note: this version is not in PyPi, you will have to install it yourself.

Install the original version using pip:

```
pip install fordpass
```

## Demo

The demo is not functional at this time.
