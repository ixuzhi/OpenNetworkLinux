Open Network Linux
==================

Check out the main/offical website at http://opennetlinux.org .

Open Network Linux (ONL) is a Linux distribution for bare metal switches.  ONL
builds an ONIE-compatible installer and a switch image which contains a complete
Debian distribution with added drivers and configuration for running on bare metal
switches.

Software License
-----------------

Licenses for the software are described under the [LICENSE](LICENSE) file.  Download or use of the software implies consent.

Documentation
-------------

* [docs/Building.md](docs/Building.md)
    Instructions for building ONL from scratch.

Please see the docs directory for additional information.

![alt text] (https://scan.coverity.com/projects/8655/badge.svg "Coverity Scan Build Status")

Credentials
-----------

For security reason, the password loging method is disabled by default, but you can still login to the system via the console cable.


## compile onl for amd64
```
make docker

docker/tools/onlbuilder
source setup.env
make -C packages/base/amd64/onlp/builds/onlp clean
make -C packages/base/amd64/onlp/builds/onlp
make onlp-dev

make -C packages/base/amd64/onlp/builds
```
