# keylights

Simple bash script to control my Elgato Key Light Air

Depends on: avahi-resolve, curl, awk, jq

## Usage:

`./keylights -h <hostname> <action>`

### Examples

#### Turn light on/off
```
./keylights -h=elgato-key-light-air-12ab.local on
./keylights -h=elgato-key-light-air-12ab.local off
```

#### Turn brightness up/down

```
./keylights -h=elgato-key-light-air-12ab.local b+
./keylights -h=elgato-key-light-air-12ab.local b-
```

#### Turn temperature up/down

```
./keylights -h=elgato-key-light-air-12ab.local t+
./keylights -h=elgato-key-light-air-12ab.local t-
```

### Hint

Find hostnames of your devices using the following command:

`avahi-browse -r -t _elg._tcp`
