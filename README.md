
## Connect sensor

https://www.modmypi.com/blog/am2302-temphumidity-sensor

https://pinout.xyz/#

## Dependencies

SSH to the Pi Zero and install dependencies:

```sh
sudo apt-get upgrade
sudo apt-get install git build-essential python-dev python-pip
```

## Code

```sh
cd /home/pi
git clone https://github.com/adafruit/Adafruit_Python_DHT.git
cd Adafruit_Python_DHT
sudo python setup.py install
```

## Run

Assuming that an AM2303 is connected to GPIO pin 4:

```sh
sudo ./AdafruitDHT.py 2302 4
```