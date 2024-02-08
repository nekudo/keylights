# keylights

Simple bash script to control my Elgato Key Light Air

Depends on: avahi-resolve, curl, awk, jq

## Usage

`./keylights -h <hostname> <action>`

### Examples

#### Turn light on/off

Using hostname resolution:

```bash
./keylights -h=elgato-key-light-air-12ab.local on
./keylights -h=elgato-key-light-air-12ab.local off
./keylights -h=elgato-key-light-air-12ab.local toggle
```

Using IP address:

```bash
./keylights -h=192.168.0.10 on
./keylights -h=192.168.0.10 off
./keylights -h=192.168.0.10 toggle
```

#### Turn brightness up/down

Using hostname resolution:

```bash
./keylights -h=elgato-key-light-air-12ab.local b+
./keylights -h=elgato-key-light-air-12ab.local b-
```

Using IP address:

```bash
./keylights -h=192.168.0.10 b+
./keylights -h=192.168.0.10 b-
```

#### Turn temperature up/down

Using hostname resolution:

```bash
./keylights -h=elgato-key-light-air-12ab.local t+
./keylights -h=elgato-key-light-air-12ab.local t-
```

Using IP address:

```bash
./keylights -h=192.168.0.10 t+
./keylights -h=192.168.0.10 t-
```

### Hint

Find hostnames of your devices using the following command:

`avahi-browse -r -t _elg._tcp`
