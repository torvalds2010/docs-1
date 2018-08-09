# API

The Underwater GPS system comes with an easy-to-use software API. This API uses a HTTP-based scheme to interact with the system. Through the API you can among others:

* Read acoustic and global position data

* Read GPS and IMU raw data

* Read and set POIs

* Set configuration settings

See [demo.waterlinked.com/swagger](http://demo.waterlinked.com/swagger) for more information.

## How to install requirements before using API

When starting to use the Water Linked software API you need to make sure you have all the requriments installed. First install [Python 2.7](https://www.python.org/downloads/release/python-2715/) and [pip](https://pip.pypa.io/en/stable/installing/). Next you need to download/clone the repository which is found on [Github](https://github.com/waterlinked/examples). Then you open a terminal in the dictionary where you saved the files and install the required Python packages using this command:

```
pip install -r requirements.txt
```
Once this is done you are ready to start interfacing the API.

Example code which use the api can be found [here](https://github.com/waterlinked/examples).

## Providing depth to system when using Locator-A1/S1

Make sure you have completed the installation of the requirments found above. Then open a terminal window in the dictionary where the files are saved and run the command:
```
python python externaldepth.py -d DEPTH_OF_LOCATOR -t TEMP_OF_WATER -u URL_OF_KIT -r REPETATION_RATE
```

* DEPTH_OF_LOCATOR: Is the current depth of the Locator.
* TEMP_OF_WATER: Is the temperature of the water where the Locator is operating in.
* URL_OF_KIT: Is the url of the kit. Usually: "http://192.168.2.94"
* REPETATION_RATE: If you want to repate the sending of depth it is the delay between each sending in seconds.
