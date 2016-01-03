# Custom program to consume OwnTracks data

Proof of concept of [OwnTracks](http://owntracks.org/).

## Pre requisites

1. Register on https://hosted.owntracks.org/

2. Download and configure mobile application

## Test

1. Download ca-bundle.pem

```console
$ wget https://www.startssl.com/certs/ca-bundle.pem
```

2. Define environment variables for authentication

```console
$ export OWNTRACKS_USERNAME=username
$ export OWNTRACKS_DEVICE=Android
$ export OWNTRACKS_TOKEN=secret
```

3. Run test program

```console
$ python3 -m venv .venv
$ source .venv/bin/activate
$ pip install paho-mqtt
$ python test.py
```

## References

- http://owntracks.org/booklet/tech/program/
- http://owntracks.org/booklet/tech/proghosted/#programming-for-hosted
