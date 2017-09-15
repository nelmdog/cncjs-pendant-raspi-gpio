# cncjs-pendant-raspi-gpio
Simple Raspberry Pi GPIO Pendant control for CNCjs.

## Installation
#### NPM Install
```
npm install cncjs-pendant-raspi-gpio
```
#### Manual Install
```
wget https://github.com/cncjs/cncjs-pendant-raspi-gpio/archive/master.zip
unzip cncjs-pendant-raspi-gpio*.zip
cd cncjs-pendant-raspi-gpio*
npm install cncjs-pendant-raspi-gpio
```

## Usage
Run `bin/cncjs-pendant-raspi-gpio` to start. Pass --help to `cncjs-pendant-raspi-gpio` for more options.

Eamples:

```
bin/cncjs-pendant-keyboard --help
node bin/cncjs-pendant-raspi-gpio  --port /dev/ttyUSB0
```

#### Button Presses
 1. G-Code: M9
 2. G-Code: M8
 3. G-Code: M7
 4. G-Code: $X "Unlock"
 5. G-Code: $X "Unlock"
 6. blank
 7. blank
 8. G-Code: $H "Home"

#### Press & Hold
 - 3 Sec: sudo poweroff "Shutdown"