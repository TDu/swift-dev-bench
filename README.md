## Description

Build a test server of Swift OpenStack Object Storage locally, using Docker.

## Installation

Needs Docker and Dockercompose installed locally then run :

    doco create
    doco build

Install the swift client on the local machine:

    sudo apt-get install python-swiftclient


## Use

To start the docker container

    doco start

To test that it is working

    swift  -A http://172.30.0.1:12345/auth/v1.0 -U test:tester -K testing stat
